# Stock Synchronization

This document describes how stock synchronization works between PlentyMarkets and Magento 2 in the Mage2Plenty connector.

## Overview

The stock synchronization system maps PlentyMarkets warehouses to Magento Multi-Source Inventory (MSI) sources, enabling bi-directional stock updates while maintaining source-level tracking through the order lifecycle.

## Key Concepts

### Warehouse to Source Mapping
- **PlentyMarkets**: Uses warehouses to manage inventory
- **Magento**: Uses MSI with stocks and sources
- **Connector**: Maps each PM warehouse to a Magento source code

### Inventory Reservations
The connector tracks which source an item is reserved from by storing the source code in the `inventory_reservation.metadata` field. This ensures shipments use the correct warehouse.

## Stock Import Flow (PM → Magento)

### 1. Data Collection
Stock data from PlentyMarkets is stored in `plenty_stock_inventory` table with:
- Variation ID (PM product ID)
- Warehouse ID
- Physical stock quantity
- Reserved stock quantity
- Net stock (physical - reserved)

### 2. Pre-Processing
- **SKU Assignment**: Maps PM variation IDs to Magento SKUs
- **Source Validation**: Ensures warehouse has a mapped source
- **Reservation Cleanup**: Removes outdated reservations

### 3. Stock Update Generation
Two generators create update requests:

#### Physical Stock Generator
```php
// Updates source item quantity
$sourceItem = [
    'sku' => $sku,
    'source_code' => $sourceCode,
    'quantity' => $qtyRequest,
    'status' => $qtyRequest > 0
];
```

#### Reservation Generator (Optional)
```php
// Creates inventory reservations for reserved stock
$reservation = [
    'sku' => $sku,
    'quantity' => -$reservedQty,
    'stock_id' => $stockId,
    'metadata' => ['source_code' => $sourceCode]
];
```

### 4. Processing
- Physical stock updates are saved to MSI source items
- Reservations are created with source tracking metadata

## Order Export Flow (Magento → PM)

### Source Code Assignment
When orders are exported, the connector:
1. Retrieves source code from reservation metadata
2. Maps source code to PM warehouse ID
3. Assigns warehouse to order items in PlentyMarkets

```php
// ReservationSourceCodeAssignment processor
$sourceCode = $reservation['source_code'];
$warehouseId = $stockConfig->getWarehouseIdBySourceCode($sourceCode);
$item->setWarehouseId($warehouseId);
```

## Order Import Flow (PM → Magento)

### Shipment Generation
When importing shipments:
1. Gets warehouse ID from PM order item
2. Maps to Magento source code
3. Validates against original reservation
4. Creates shipment with correct source

```php
// Shipment generator logic
$warehouseId = $clientOrderItem->getWarehouseId();
$sourceCode = $stockConfig->getSourceCodeByWarehouseId($warehouseId);

// Validate against reservation
if ($sourceCodeReservation !== $sourceCode) {
    // Log warning about source mismatch
}
```

## Configuration

### Stock Profile Settings
- **Main Warehouse**: Default warehouse for unmapped sources
- **Warehouse Mapping**: Configure warehouse → source relationships
- **Reservation Mode**: Enable/disable reservation synchronization
- **Source Selection**: Algorithm for multi-source allocation

### Key Configuration Paths
```
/stock_config/main_warehouse_id
/stock_config/stock_source_mapping
/stock_config/is_active_reservation
/stock_config/source_selection_algorithm
```

## Important Classes

### Stock Import
- `StockImportService`: Main import orchestrator
- `StockPhysical` (Generator/Processor): Handles quantity updates
- `StockReservation` (Generator/Processor): Manages reservations
- `StockConfigInterface`: Provides mapping configuration

### Order Integration
- `ReservationSourceAssignment`: Plugin to track source in reservations
- `SalesEventToArrayConverterPlugin`: Adds source to reservation metadata
- `ReservationSourceCodeAssignment`: Updates reservations during order export
- `Shipment` (Generator): Creates shipments with source validation

## Troubleshooting

### Common Issues

1. **"Could not find applicable source code"**
   - Check warehouse mapping in stock profile configuration
   - Ensure source exists in Magento MSI

2. **"Source code does not match the one assigned initially"**
   - Indicates warehouse changed in PM after order placement
   - Review order history for manual warehouse changes

3. **Stock not updating**
   - Verify stock profile is active
   - Check `plenty_stock_inventory` table for pending items
   - Review system logs for processing errors

### Debug Commands
```bash
# Process stock import manually
bin/magento plenty:stock:import --profile-id=X

# Check reservation source assignments
bin/magento plenty:stock:reservation:cleanup

# Validate warehouse mappings
bin/magento plenty:client:collect-config --profile-id=X
```