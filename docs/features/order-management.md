# Order Management

This document describes the bi-directional order synchronization between Magento 2 and PlentyMarkets.

## Overview

The order management system handles:
- **Order Export**: Magento orders → PlentyMarkets
- **Order Import**: PlentyMarkets orders → Magento (for marketplace orders)
- **Status Synchronization**: Keeps order states in sync
- **Document Management**: Invoices, shipments, credit memos

## Order Export Flow (Magento → PM)

### 1. Order Collection
Orders are collected based on:
- Order status (configurable)
- Store view mapping
- Time range (last modified)

### 2. Pre-Processing
- **Customer Validation**: Ensures customer/guest exists in PM
- **Address Validation**: Validates and maps addresses
- **Payment Method Mapping**: Maps Magento payment methods to PM MOP IDs

### 3. Order Generation

#### Main Order Data
```php
// Order generator creates base order
$request = [
    'typeId' => ORDER_TYPE_SALE,
    'ownerId' => $userId,
    'plentyId' => $clientId,
    'referrerId' => $referrerId,
    'statusId' => $mappedStatusId
];
```

#### Order Items
Each visible order item is processed:
- Simple products: Direct mapping
- Configurable products: Child items with parent info
- Bundle products: Component items tracked

Key item data:
```php
$item = [
    'typeId' => TYPE_VARIATION,
    'quantity' => $qty,
    'orderItemName' => $name,
    'variationId' => $plentyVariationId,
    'warehouseId' => $warehouseFromReservation,
    'amounts' => [
        'priceOriginalGross' => $price,
        'surcharge' => $discount,
        'tax' => $taxPercent
    ]
];
```

#### Warehouse Assignment
The warehouse is determined from inventory reservations:
1. Retrieves source code from reservation metadata
2. Maps source code to PM warehouse ID
3. Assigns warehouse to each order item

### 4. Payment Processing
If payment processing is enabled:
```php
$payment = [
    'amount' => $amountPaid,
    'mopId' => $paymentMethodId,
    'currency' => $baseCurrency,
    'type' => TYPE_CREDIT,
    'status' => APPROVED/AWAITING_APPROVAL,
    'properties' => [
        'orderReference' => $incrementId,
        'transactionId' => $transactionId
    ]
];
```

### 5. Post-Processing
- Updates order status in Magento
- Saves PM order ID to Magento order
- Creates order history records
- Triggers stock collection if configured

## Order Import Flow (PM → Magento)

### 1. Order Collection
Retrieves orders from PM based on:
- Order type (marketplace orders)
- Status filters
- Referrer ID (marketplace channel)

### 2. Customer Creation
Creates or retrieves customer:
- Guest checkout for marketplace orders (default)
- Customer account creation (optional)
- Email validation and generation

### 3. Quote Generation

#### Quote Creation
```php
// Quote generator creates cart
$quote->setStoreId($storeId);
$quote->setCustomer($customer);
$quote->setInventoryProcessed(false);
```

#### Quote Items
Maps PM items to Magento products:
- Uses variation ID → SKU mapping
- Sets custom prices from PM
- Handles product options

#### Shipping & Payment
- Maps PM shipping profile to Magento method
- Sets payment method based on marketplace
- Applies shipping costs

### 4. Order Creation
```php
// Order processor submits quote
$order = $quoteManagement->submit($quote, [
    'plenty_order_id' => $clientOrderId,
    'plenty_order_status' => 'complete'
]);
```

### 5. Document Import

#### Shipment Creation
When PM order has delivery documents:
1. Retrieves warehouse from PM order item
2. Maps to Magento source code
3. Validates against original reservation
4. Creates shipment with source tracking

```php
// Shipment generator logic
$shipmentItem = [
    'orderItemId' => $itemId,
    'qty' => $qty,
    'sourceCode' => $mappedSourceCode
];
```

#### Invoice Import
- Creates invoices for PM invoices
- Maps payment status
- Updates totals

## Configuration

### Order Export Settings
```
/order_config/is_active_export
/order_config/order_status_filter
/order_config/payment_method_mapping
/order_config/shipping_method_mapping
/order_config/plenty_status_mapping
```

### Order Import Settings
```
/order_config/is_active_import
/order_config/order_type_filter
/order_config/create_customer_account
/order_config/shipping_process_config
```

### Key Mappings
1. **Payment Methods**: Magento code → PM MOP ID
2. **Order Status**: Magento status → PM status ID
3. **Shipping Methods**: Carrier mapping
4. **Order Properties**: Custom field mappings

## Status Synchronization

### Export Status Flow
```
Magento Status → PM Status ID
pending → 3 (Waiting for payment)
processing → 5 (Cleared for shipping)
complete → 7 (Shipped)
canceled → 8 (Canceled)
```

### Import Status Flow
```
PM Status → Magento Action
5.x → Create shipment
6.x → Create invoice
7.x → Mark complete
8.x → Cancel order
```

## Important Classes

### Order Export
- `OrderExportService`: Main export orchestrator
- `Order` (Generator): Creates order request
- `Order/Items/Item`: Processes order items
- `Payment` (Generator): Handles payment data
- `ReservationSourceCodeAssignment`: Assigns warehouse from reservations

### Order Import
- `OrderImportService`: Main import orchestrator
- `Quote` (Generator): Creates quote from PM order
- `Order` (Processor): Converts quote to order
- `Shipment` (Generator): Creates shipments with source validation
- `Invoice` (Processor): Processes invoice documents

## Troubleshooting

### Common Export Issues

1. **"Could not retrieve payment method ID"**
   - Check payment method mapping in configuration
   - Ensure PM MOP ID exists

2. **"Could not find source code for warehouse"**
   - Verify stock profile configuration
   - Check reservation has source code metadata

3. **Order not exporting**
   - Check order status is in export filter
   - Verify store view mapping
   - Review order locks

### Common Import Issues

1. **"Product not found"**
   - Ensure variation ID mapping exists
   - Check product is enabled in store

2. **"Invalid shipping method"**
   - Map PM shipping profile to Magento method
   - Verify carrier is enabled

3. **Shipment source mismatch**
   - Review warehouse changes in PM
   - Check reservation metadata

### Debug Commands
```bash
# Export orders manually
bin/magento plenty:order:export --profile-id=X

# Import orders
bin/magento plenty:order:import --profile-id=X

# Check order mappings
bin/magento plenty:order:map-relation --profile-id=X

# Delete test orders in PM
bin/magento plenty:order:delete --profile-id=X --order-id=Y
```