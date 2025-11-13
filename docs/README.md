# Mage2Plenty Connector Documentation

Technical documentation for the Mage2Plenty connector - a bi-directional integration between Magento 2 and PlentyMarkets.

## Features

- [Stock Synchronization](../../../modules/module-plenty-stock-profile/docs/stock-synchronization.md) - How inventory sync works between systems
- [Order Management](../../../modules/module-plenty-order-profile/docs/ORDER_MANAGEMENT.md) - Bi-directional order synchronization

## Quick Links

- **Main Project**: `/packages/metapackages/mage2plenty-suite`
- **Modules**: `/packages/modules/module-plenty-*`
- **Configuration**: See individual feature documentation

## Module Overview

The connector consists of 40+ interconnected modules, key ones include:

- `module-plenty-stock-profile` - Stock synchronization
- `module-plenty-order-profile` - Order management
- `module-plenty-item-profile` - Product synchronization
- `module-plenty-customer-profile` - Customer synchronization
- `module-plenty-client` - PlentyMarkets API client

## Getting Started

1. Review the [project overview](../../../CLAUDE.md)
2. Check feature-specific documentation
3. Configure profiles in Magento Admin
