## Changelog




# mage2plenty-suite [1.15.1] 20 Aug 2025

### softcommerce/module-plenty-order-profile [1.13.1]
- **Fix**: improve error messages for warehouse mapping issues

### softcommerce/module-plenty-stock-profile [1.7.6]
- **Fix**: resolve one-to-many warehouse mapping for multi-warehouse shipments


# mage2plenty-suite [1.15.0] 08 Aug 2025

### softcommerce/module-plenty-client [1.5.0]
- **Feature**: Add commands to create referrers

### softcommerce/module-plenty-customer-client [1.3.0]
- **Feature**: Improve customer data collection command

### softcommerce/module-plenty-item-client [1.4.0]
- **Feature**: Improve item data collection command

### softcommerce/module-plenty-log [1.3.0]
- **Feature**: Improve log collection and processing commands

### softcommerce/module-plenty-order-client [1.6.0]
- **Feature**: Improve order data collection command

### softcommerce/module-plenty-order-profile [1.13.0]
- **Feature**: Add commands to delete orders and payments

### softcommerce/module-plenty-stock-client [1.3.0]
- **Feature**: Improve stock data collection command


# mage2plenty-suite [1.14.1] 14 Jul 2025

### softcommerce/module-plenty-attribute [1.5.3]
- ## softcommerce/module-plenty-attribute [1.5.2] - **Enhancement**: Added a setup script to remove attribute entries from the `plenty_attribute_entity` table after migrating manufacturers to a dedicated table
- ## softcommerce/module-plenty-attribute [1.5.1] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-attribute [1.5.0] - **Feature**: Add attributes for manufacturer model to facilitate GPSR data for Product Safety Regulation [#40]
- ## softcommerce/module-plenty-attribute [1.4.2] - **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-attribute-rest-api [1.2.10]
- ## softcommerce/module-plenty-attribute-rest-api [1.2.9] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-attribute-rest-api [1.2.8] - **Compatibility**: Added REST API collect functionality for compatability with GH feature: #40 [https://github.com/softcommerceltd/mage2plenty-os/issues/40]

### softcommerce/module-plenty-category [1.3.1]
- ## softcommerce/module-plenty-category [1.3.0] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-category [1.2.11] - **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-category-profile [1.4.1]
- ## softcommerce/module-plenty-category-profile [1.4.0] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-category-profile [1.3.13] - **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-category-profile-schedule [1.2.7]
- ## softcommerce/module-plenty-category-profile-schedule [1.2.6] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-category-rest-api [1.2.6]
- ## softcommerce/module-plenty-category-rest-api [1.2.5] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-client [1.4.5]
- ## softcommerce/module-plenty-client [1.4.4] - **Enhancement**: Improved the client token refresh logic to check if the refresh token has expired before using it. This prevents unnecessary login attempts and makes the token handling more robust. [#72]
- ## softcommerce/module-plenty-client [1.4.3] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-client [1.4.2] - **Enhancement**: Added an option to clear client repository runtime cached data - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-client-rest-api [1.3.3]
- ## softcommerce/module-plenty-client-rest-api [1.3.2] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-client-rest-api [1.3.1] - **Fix**: SoftCommerce\PlentyClientRestApi\Model\Response\ConfigDataBuilder::buildItemArrayResponse(): Argument #1 ($item) must be of type array, string given #36

### softcommerce/module-plenty-customer [1.3.5]
- ## softcommerce/module-plenty-customer [1.3.4] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-customer [1.3.3] - **Fix**: Fix Unique Constraints in Database Schema for Plenty Address Relations [#55]
- ## softcommerce/module-plenty-customer [1.3.2] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-customer-client [1.2.10]
- ## softcommerce/module-plenty-customer-client [1.2.9] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-customer-client [1.2.8] - **Enhancement**: Minor changes to codebase `SoftCommerce\PlentyCustomerClient\Model\AddressOptionTypeManagement`

### softcommerce/module-plenty-customer-profile [1.1.5]
- ## softcommerce/module-plenty-customer-profile [1.1.4] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-customer-profile [1.1.3] - **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-customer-rest-api [1.2.8]
- ## softcommerce/module-plenty-customer-rest-api [1.2.7] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item [1.6.2]
- ## softcommerce/module-plenty-item [1.6.1] - **Enhancement** Add isShippingType() Method to Plenty Item Modules [#69]
- ## softcommerce/module-plenty-item [1.6.0] - **Feature**: Allow Export of “Not Visible Individually” Products to PlentyMarkets [#66] - **Enhancement**: Add Pagination to Product Chooser Modal in Product Export Listing [#65]
- ## softcommerce/module-plenty-item [1.5.1] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-item [1.5.0] - **Feature**: Introduce a feature to delete local item storage from admin UI [#23]
- ## softcommerce/module-plenty-item [1.4.8] - **Enhancement**: Added new methods to `SoftCommerce\PlentyItem\Model\Service\SaveProductItemVariationIdMappingInterface`

### softcommerce/module-plenty-item-client [1.3.1]
- ## softcommerce/module-plenty-item-client [1.3.0] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-item-client [1.2.10] - **Enhancement**: Remove `stock_warehouse_dimension, stock_warehouse_location and stock_warehouse_location_details` configs from client data collection process

### softcommerce/module-plenty-item-profile [1.13.2]
- ## softcommerce/module-plenty-item-profile [1.13.1] - **Fix**: Resolved an issue where the image import process would stop prematurely if the `namesData` array was empty. The logic has been adjusted to ensure the process continues, allowing for more flexible image handling. [#71]
- ## softcommerce/module-plenty-item-profile [1.13.0] - **Feature**: Allow Export of “Not Visible Individually” Products to PlentyMarkets [#66]
- ## softcommerce/module-plenty-item-profile [1.12.0] - **Feature**: New CLI Command to Clear Product Mappings [#61] - **Fix**: Override Configurable Attribute Values on Product Export [#60]
- ## softcommerce/module-plenty-item-profile [1.11.3] - **Compatibility**: Proper Cache Invalidation for Varnish After Product Import [#59]
- ## softcommerce/module-plenty-item-profile [1.11.2] - **Enhancement**: Validation error found :: attribute values do not match the other variations [#57]
- ## softcommerce/module-plenty-item-profile [1.11.1] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-item-profile [1.11.0] - **Enhancement**: Optimize Image Handling to Prevent Unnecessary Downloads During Item and Variation Collection [#51]
- ## softcommerce/module-plenty-item-profile [1.10.0] - **Enhancement**: Added an enhancement to accurately align the import of image sort orders with the data in the PlentyONE system. This change ensures that images maintain the correct sequence and display order based on PlentyONE’s configuration. [#44] - **Enhancement**: Introduced an enhancement to correctly remove outdated super attributes from configurable products. Previously, old configuration attributes remained in the system even after being deleted in PlentyONE, causing inconsistencies. This update ensures that any attributes removed in PlentyONE are now properly deleted and no longer remain in the system. [#43] - **Fix**: Applied a fix for TypeError: str_replace(): Argument #3 ($subject) must be of type array|string, null given in softcommerce/module-plenty-item-profile/Ui/Component/Form/PlentyAttributeOptions.php:50
- ## softcommerce/module-plenty-item-profile [1.9.3] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-item-profile [1.9.2] - **Fix**: TypeError: SoftCommerce\PlentyItemProfile\Model\ItemExportService\Processor\Item::retrieveSkuByItemId() must be of type array, string given [#30]
- ## softcommerce/module-plenty-item-profile [1.9.1] - **Compatibility**: Applied compatibility for profile common configuration paths [#27]
- ## softcommerce/module-plenty-item-profile [1.9.0] - **Feature**: Introduce a feature to map product SKUs to Item and Variation IDs [#24] - **Feature**: Introduce a feature to schedule item collect process from the admin UI [#22] - **Fix**: Add a fix for duplicate client images deletion functionality [#18]
- ## softcommerce/module-plenty-item-profile [1.8.3] - **Enhancement**: An option to configure media image export type. E.g. Images can be exported by providing either a direct URL or a base64 encoded image data. [#21] - **Enhancement**: Allow mapping properties with type scope global to attributes with type scope website/store [#20] - **Fix**: Fix massaction responsible for deleting client items externally [#19] - **Enhancement**: Add an option to resolve duplicate client images [#18]
- ## softcommerce/module-plenty-item-profile [1.8.2] - **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-item-profile-schedule [1.3.2]
- ## softcommerce/module-plenty-item-profile-schedule [1.3.1] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item-rest-api [1.3.2]
- ## softcommerce/module-plenty-item-rest-api [1.3.1] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-log [1.2.9]
- ## softcommerce/module-plenty-log [1.2.8] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order [1.5.3]
- ## softcommerce/module-plenty-order [1.5.2] - **Feature**: Added support for order comments, allowing comments to be stored and retrieved with order data. [#70]
- ## softcommerce/module-plenty-order [1.5.1] - **Enhancement**: Apply Descending Sort Order to getOrdersById Interface Collection [#56]
- ## softcommerce/module-plenty-order [1.5.0] - **Feature**: Added functionality to refresh sales order grid using CLI [#45]
- ## softcommerce/module-plenty-order [1.4.2] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order-client [1.5.1]
- ## softcommerce/module-plenty-order-client [1.5.0] - **Feature**: Compatibility with shipping tracking functionality [#52]
- ## softcommerce/module-plenty-order-client [1.4.2] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-order-client [1.4.1] - **Enhancement**: Remove `stock_warehouse_dimension, stock_warehouse_location and stock_warehouse_location_details` configs from client data collection process

### softcommerce/module-plenty-order-profile [1.12.1]
- ## softcommerce/module-plenty-order-profile [1.12.0]
- ## softcommerce/module-plenty-order-profile [1.11.1] - **Fix** Support Multiple Tracking Numbers in Order Shipping Import [#68] - **Enhancement** Ensure Sales Order Grid Reindexing for Orders Skipped by Export [#67]
- ## softcommerce/module-plenty-order-profile [1.11.0] - **Feature**: Option to Exclude Warehouse Assignment on Order Line Items [#62]
- ## softcommerce/module-plenty-order-profile [1.10.2] - **Fix** Ensure Customer Address Relation Is Always Assigned [#58]
- ## softcommerce/module-plenty-order-profile [1.10.1] - **Enhancement** Added the ability to conditionally add product options to order line items based on defined rules.
- ## softcommerce/module-plenty-order-profile [1.10.0] - **Feature**: Add Support for Exporting Shipment Tracking Information from Magento to Plenty [#52] - **Feature**: Implement Channel-Based Restrictions for Order Export Functionality [#50]
- ## softcommerce/module-plenty-order-profile [1.9.2] - **Enhancement**: A fix has been implemented to correct VAT rate exports for order items. Previously, bundle items without a VAT reference in the Magento sales order table were mistakenly exported with a 0% VAT rate, and this update ensures the correct rate is now exported. [#49]
- ## softcommerce/module-plenty-order-profile [1.9.1] - **Enhancement**: Optimized stock source assignment: Orders with default stock sources now reference item configuration for reservation checks, reducing resource overhead. [#48]
- ## softcommerce/module-plenty-order-profile [1.9.0] - **Feature**: Added new feature to map PlentyONE and Magento orders using CLI [#46]
- ## softcommerce/module-plenty-order-profile [1.8.2] - **Enhancement**: Applied a fix to resolved an issue affecting orders from third-party sales channels. These orders were getting stuck in the scheduling queue repeatedly because their status wasn’t updating properly after processing. This caused the system to attempt processing them over and over without success. The fix ensures that the status updates correctly, preventing orders from being stuck and allowing them to move through the system smoothly
- ## softcommerce/module-plenty-order-profile [1.8.1] -- **Fix**: SourceItemRepository::getQtyPhysical(): Argument #2 ($sourceCode) must be of type string, null given, called in /../softcommerce/module-plenty-order-profile/Model/OrderImportService/Generator/Shipment.php on line 247 [#42]
- ## softcommerce/module-plenty-order-profile [1.8.0] - **Feature**: Added an option to export product options for orders #41 - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-order-profile [1.7.6] - **Enhancement**: Improvements to shipment creation for out of stock items [#39]
- ## softcommerce/module-plenty-order-profile [1.7.5] - **Enhancement**: Added an option to control the export of order shipping profiles [#35]
- ## softcommerce/module-plenty-order-profile [1.7.4] - **Enhancement**: Added a functionality to handle cancelled order status synchronisation [#34]
- ## softcommerce/module-plenty-order-profile [1.7.3] - **Enhancement**: Generate unique ID for guest customers that is required for PM contact number [#28] - **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-order-profile-schedule [1.3.2]
- ## softcommerce/module-plenty-order-profile-schedule [1.3.1] - **Enhancement**: Efficient Order Export Using Status Filters [#63]
- ## softcommerce/module-plenty-order-profile-schedule [1.3.0] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta
- ## softcommerce/module-plenty-order-profile-schedule [1.2.15] - **Enhancement**: Added an interception plugin to handle order cancellation synchronisation [#34]
- ## softcommerce/module-plenty-order-profile-schedule [1.2.14] - **Enhancement**: Added order cancel event to handle cancelled order status synchronisation [#34]

### softcommerce/module-plenty-order-rest-api [1.4.1]
- ## softcommerce/module-plenty-order-rest-api [1.4.0] - **Feature**: Compatibility with shipping tracking functionality [#52]
- ## softcommerce/module-plenty-order-rest-api [1.3.1] - **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-profile [1.5.3]
- ## softcommerce/module-plenty-profile [1.5.2] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-profile [1.5.1] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-profile [1.5.0] - **Feature**: Profiles that share common configuration paths can now be saved simultaneously from any profile [#27]
- Added release auto generation

### softcommerce/module-plenty-property [1.3.9]
- ## softcommerce/module-plenty-property [1.3.8] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-property [1.3.7] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-property [1.3.6] - **Fix**: Argument #1 ($responseItem) must be of type array, string given in SoftCommerce\PlentyProperty\Profile\PropertyExportService\Processor\BatchProcessor::retrievePropertyId() [#31]
- ## softcommerce/module-plenty-property [1.3.5] - **Enhancement**: An option to override `isGlobal` condition in `SoftCommerce\PlentyProperty\Model\AttributeToPropertyTypeMappingInterface::getPropertyTypeByAttribute`
- ## softcommerce/module-plenty-property [1.3.4] - **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-property-rest-api [1.2.8]
- ## softcommerce/module-plenty-property-rest-api [1.2.7] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-rest-api [1.3.10]
- ## softcommerce/module-plenty-rest-api [1.3.9] - **Enhancement**: Enhance Batch Request Method to Allow Grouping Responses by Resource URI [#53]
- ## softcommerce/module-plenty-rest-api [1.3.8] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-rest-api [1.3.7] - **Fix**: Argument #1 ($item) must be of type array, string given in SoftCommerce\PlentyCustomerRestApi\Model\Response\AddressDataBuilder::buildItemResponse(): [#32]

### softcommerce/module-plenty-stock [1.4.3]
- ## softcommerce/module-plenty-stock [1.4.2] - **Enhancement**: Removed unused database schema declaration.
- ## softcommerce/module-plenty-stock [1.4.1] - **Enhancement**: Created new interface for item stock configuration that allows quick verification of stock management status. This enhancement optimizes the overall efficiency of stock management within our system. [#47]
- ## softcommerce/module-plenty-stock [1.4.0] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-stock [1.3.9] - **Enhancement**: Improvements to Order Item source selection algorithm [#38]
- ## softcommerce/module-plenty-stock [1.3.8] - **Fix**: Too few arguments to function SoftCommerce\PlentyStock\Model\GetOrderItemSourceSelection::generateInventoryRequest() 3 passed, exactly 4 [#33]
- ## softcommerce/module-plenty-stock [1.3.7] - **Enhancement**: Addressed minor performance improvements for `SoftCommerce\PlentyStock\Model\GetOrderItemSourceSelection::generateInventoryRequest()`

### softcommerce/module-plenty-stock-client [1.2.10]
- ## softcommerce/module-plenty-stock-client [1.2.9] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock-profile [1.7.4]
- ## softcommerce/module-plenty-stock-profile [1.7.3] - **Enhancement**: Minor codebase style improvements.
- ## softcommerce/module-plenty-stock-profile [1.7.2] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-stock-profile [1.7.1] - **Enhancement**: Improvements to Order Item source selection algorithm [#38]
- ## softcommerce/module-plenty-stock-profile [1.7.0] - **Compatibility**: Applied compatibility for profile common configuration paths [#27] - **Feature**: Introduce custom Source Selection Algorithm to achieve precise NET calculation by accounting for reservations [#26]

### softcommerce/module-plenty-stock-profile-schedule [1.3.1]
- ## softcommerce/module-plenty-stock-profile-schedule [1.3.0] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-plenty-stock-profile-schedule [1.2.10] - **Fix** CRITICAL: Message has been rejected: Profile ID is not set [#37]

### softcommerce/module-plenty-stock-rest-api [1.2.9]
- ## softcommerce/module-plenty-stock-rest-api [1.2.8] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-config [1.3.1]
- ## softcommerce/module-profile-config [1.3.0] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.
- ## softcommerce/module-profile-config [1.2.13] - **Fix**: Apply a fix where profile config scope writer saves value as array opposed to serialised data [#29]

### softcommerce/module-profile-history [1.2.10]
- ## softcommerce/module-profile-history [1.2.9] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-queue [1.1.3]
- ## softcommerce/module-profile-queue [1.1.2] - **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.


# Mage2PlentyOs [1.14.0] 10 Jul 2025

### softcommerce/module-plenty-client [1.4.4]
- **Enhancement**: Improved the client token refresh logic to check if the refresh token has expired before using it. This prevents unnecessary login attempts and makes the token handling more robust. [#72]

### softcommerce/module-plenty-item-profile [1.13.1]
- **Fix**: Resolved an issue where the image import process would stop prematurely if the `namesData` array was empty. The logic has been adjusted to ensure the process continues, allowing for more flexible image handling. [#71]

### softcommerce/module-plenty-order [1.5.2]
- **Feature**: Added support for order comments, allowing comments to be stored and retrieved with order data. [#70]

### softcommerce/module-plenty-order-profile [1.12.0]

# Mage2PlentyOs [1.13.1] 11 Jun 2025

### softcommerce/module-plenty-item [1.6.1]
- **Enhancement** Add isShippingType() Method to Plenty Item Modules [#69]

### softcommerce/module-plenty-order-profile [1.11.1]
- **Fix** Support Multiple Tracking Numbers in Order Shipping Import [#68]
- **Enhancement** Ensure Sales Order Grid Reindexing for Orders Skipped by Export [#67]

# Mage2PlentyOs [1.13.0] 28 May 2025

### softcommerce/module-core [1.6.1]
- **Enhancement**: Enhanced Configurable-Product Detection in Export/Import Interface [#64]

### softcommerce/module-plenty-item [1.6.0]
- **Feature**: Allow Export of “Not Visible Individually” Products to PlentyMarkets [#66]
- **Enhancement**: Add Pagination to Product Chooser Modal in Product Export Listing [#65]

### softcommerce/module-plenty-item-profile [1.13.0]
- **Feature**: Allow Export of “Not Visible Individually” Products to PlentyMarkets [#66]

# Mage2PlentyOs [1.12.1] 19 May 2025

### softcommerce/module-plenty-order-profile-schedule [1.3.1]
- **Enhancement**: Efficient Order Export Using Status Filters [#63]

# Mage2PlentyOs [1.12.0] 08 May 2025

### softcommerce/module-core [1.6.0]
- **Compatibility**: Added compatibility for Magento 2.4.8

# Mage2PlentyOs [1.11.0] 07 May 2025

### softcommerce/module-plenty-item-profile [1.12.0]
- **Feature**: New CLI Command to Clear Product Mappings [#61]
- **Fix**: Override Configurable Attribute Values on Product Export [#60]

### softcommerce/module-plenty-order-profile [1.11.0]
- **Feature**: Option to Exclude Warehouse Assignment on Order Line Items [#62]

# Mage2PlentyOs [1.10.5] 07 May 2025

### softcommerce/module-plenty-item-profile [1.11.3]
- **Compatibility**: Proper Cache Invalidation for Varnish After Product Import [#59]

# Mage2PlentyOs [1.10.4] 06 May 2025

### softcommerce/module-plenty-order-profile [1.10.2]
- **Fix** Ensure Customer Address Relation Is Always Assigned [#58]

# Mage2PlentyOs [1.10.3] 30 Apr 2025

### softcommerce/module-plenty-item-profile [1.11.2]
- **Enhancement**: Validation error found :: attribute values do not match the other variations [#57]

# Mage2PlentyOs [1.10.2] 29 Apr 2025

### softcommerce/module-plenty-client [1.4.3]
- **Enhancement**: Removed unused database schema declaration.

### softcommerce/module-plenty-customer [1.3.4]
- **Enhancement**: Removed unused database schema declaration.

### softcommerce/module-plenty-item-profile [1.11.1]
- **Enhancement**: Removed unused database schema declaration.

### softcommerce/module-plenty-profile [1.5.2]
- **Enhancement**: Removed unused database schema declaration.

### softcommerce/module-plenty-property [1.3.8]
- **Enhancement**: Removed unused database schema declaration.

### softcommerce/module-plenty-stock [1.4.2]
- **Enhancement**: Removed unused database schema declaration.

# Mage2PlentyOs [1.10.1] 09 Apr 2025

### softcommerce/module-plenty-order-profile [1.10.1]
- **Enhancement** Added the ability to conditionally add product options to order line items based on defined rules.

# Mage2PlentyOs [1.10.0] 01 Apr 2025

### softcommerce/module-core [1.5.9]
- **Enhancement**: Add Method to FileImageManagement Interface for Deleting Downloaded Images from pub/media/import Directory
- **Enhancement**: Add Weight Unit Source Options to Enable Configuration via UI Profiles

### softcommerce/module-plenty-customer [1.3.3]
- **Fix**: Fix Unique Constraints in Database Schema for Plenty Address Relations [#55]

### softcommerce/module-plenty-item-profile [1.11.0]
- **Enhancement**: Optimize Image Handling to Prevent Unnecessary Downloads During Item and Variation Collection [#51]

### softcommerce/module-plenty-order [1.5.1]
- **Enhancement**: Apply Descending Sort Order to getOrdersById Interface Collection [#56]

### softcommerce/module-plenty-order-client [1.5.0]
- **Feature**: Compatibility with shipping tracking functionality [#52]

### softcommerce/module-plenty-order-profile [1.10.0]
- **Feature**: Add Support for Exporting Shipment Tracking Information from Magento to Plenty [#52]
- **Feature**: Implement Channel-Based Restrictions for Order Export Functionality [#50]

### softcommerce/module-plenty-order-rest-api [1.4.0]
- **Feature**: Compatibility with shipping tracking functionality [#52]

### softcommerce/module-plenty-rest-api [1.3.9]
- **Enhancement**: Enhance Batch Request Method to Allow Grouping Responses by Resource URI [#53]

# Mage2PlentyOs [1.9.2] 26 Feb 2025

### softcommerce/module-plenty-order-profile [1.9.2]
- **Enhancement**: A fix has been implemented to correct VAT rate exports for order items. Previously, bundle items without a VAT reference in the Magento sales order table were mistakenly exported with a 0% VAT rate, and this update ensures the correct rate is now exported. [#49]

# Mage2PlentyOs [1.9.1] 18 Feb 2025

### softcommerce/module-plenty-order-profile [1.9.1]
- **Enhancement**: Optimized stock source assignment: Orders with default stock sources now reference item configuration for reservation checks, reducing resource overhead. [#48]

### softcommerce/module-plenty-stock [1.4.1]
- **Enhancement**: Created new interface for item stock configuration that allows quick verification of stock management status. This enhancement optimizes the overall efficiency of stock management within our system. [#47]

### softcommerce/module-plenty-stock-profile [1.7.3]
- **Enhancement**: Minor codebase style improvements.

# Mage2PlentyOs [1.9.0] 05 Feb 2025

### softcommerce/module-plenty-order [1.5.0]
- **Feature**: Added functionality to refresh sales order grid using CLI [#45]

### softcommerce/module-plenty-order-profile [1.9.0]
- **Feature**: Added new feature to map PlentyONE and Magento orders using CLI [#46]

# Mage2PlentyOs [1.8.3] 31 Jan 2025

### softcommerce/module-plenty-attribute [1.5.2]
- **Enhancement**: Added a setup script to remove attribute entries from the `plenty_attribute_entity` table after migrating manufacturers to a dedicated table

### softcommerce/module-plenty-item-profile [1.10.0]
- **Enhancement**: Added an enhancement to accurately align the import of image sort orders with the data in the PlentyONE system. This change ensures that images maintain the correct sequence and display order based on PlentyONE’s configuration. [#44]
- **Enhancement**: Introduced an enhancement to correctly remove outdated super attributes from configurable products. Previously, old configuration attributes remained in the system even after being deleted in PlentyONE, causing inconsistencies. This update ensures that any attributes removed in PlentyONE are now properly deleted and no longer remain in the system. [#43]
- **Fix**: Applied a fix for TypeError: str_replace(): Argument #3 ($subject) must be of type array|string, null given in softcommerce/module-plenty-item-profile/Ui/Component/Form/PlentyAttributeOptions.php:50

# Mage2PlentyOs [1.8.2] 23 Jan 2025

### softcommerce/module-plenty-order-profile [1.8.2]
- **Enhancement**: Applied a fix to resolved an issue affecting orders from third-party sales channels. These orders were getting stuck in the scheduling queue repeatedly because their status wasn’t updating properly after processing. This caused the system to attempt processing them over and over without success. The fix ensures that the status updates correctly, preventing orders from being stuck and allowing them to move through the system smoothly

# Mage2PlentyOs [1.8.1] 15 Jan 2025

### softcommerce/module-plenty-order-profile [1.8.1]
-- **Fix**: SourceItemRepository::getQtyPhysical(): Argument #2 ($sourceCode) must be of type string, null given, called in /../softcommerce/module-plenty-order-profile/Model/OrderImportService/Generator/Shipment.php on line 247 [#42]

# Mage2PlentyOs [1.8.0] 13 Jan 2025

### softcommerce/module-core [1.5.8]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-attribute [1.5.1]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-attribute-rest-api [1.2.9]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-category [1.3.0]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-category-profile [1.4.0]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-category-profile-schedule [1.2.6]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-category-rest-api [1.2.5]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-client [1.4.2]
- **Enhancement**: Added an option to clear client repository runtime cached data
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-client-rest-api [1.3.2]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-customer [1.3.2]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-customer-client [1.2.9]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-customer-profile [1.1.4]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-customer-rest-api [1.2.7]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item [1.5.1]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item-client [1.3.0]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item-profile [1.9.3]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item-profile-schedule [1.3.1]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-item-rest-api [1.3.1]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-log [1.2.8]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order [1.4.2]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order-client [1.4.2]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order-profile [1.8.0]
- **Feature**: Added an option to export product options for orders #41
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order-profile-schedule [1.3.0]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-order-rest-api [1.3.1]
- **Compatibility**: Added compatibility for PHP 8.4 and Magento 2.4.8-beta

### softcommerce/module-plenty-profile [1.5.1]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-property [1.3.7]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-property-rest-api [1.2.7]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-rest-api [1.3.8]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock [1.4.0]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock-client [1.2.9]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock-profile [1.7.2]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock-profile-schedule [1.3.0]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-plenty-stock-rest-api [1.2.8]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile [1.4.5]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-config [1.3.0]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-history [1.2.9]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-queue [1.1.2]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

### softcommerce/module-profile-schedule [1.3.7]
- **Enhancement**: Included `servicepoint` type to account for `pakshop` facility.

# Mage2PlentyOs [1.7.0] 12 Dec 2024

### softcommerce/module-plenty-attribute [1.5.0]
- **Feature**: Add attributes for manufacturer model to facilitate GPSR data for Product Safety Regulation [#40]

### softcommerce/module-plenty-attribute-rest-api [1.2.8]
- **Compatibility**: Added REST API collect functionality for compatability with GH feature: #40 [https://github.com/softcommerceltd/mage2plenty-os/issues/40]

# Mage2PlentyOs [1.6.2] 08 Nov 2024

### softcommerce/module-plenty-order-profile [1.7.6]
- **Enhancement**: Improvements to shipment creation for out of stock items [#39]

### softcommerce/module-plenty-stock [1.3.9]
- **Enhancement**: Improvements to Order Item source selection algorithm [#38]

### softcommerce/module-plenty-stock-profile [1.7.1]
- **Enhancement**: Improvements to Order Item source selection algorithm [#38]

# Mage2PlentyOs [1.6.10] 17 Oct 2024

### softcommerce/module-plenty-client-rest-api [1.3.1]
- **Fix**: SoftCommerce\PlentyClientRestApi\Model\Response\ConfigDataBuilder::buildItemArrayResponse(): Argument #1 ($item) must be of type array, string given #36

### softcommerce/module-plenty-stock-profile-schedule [1.2.10]
- **Fix** CRITICAL: Message has been rejected: Profile ID is not set [#37]

# Mage2PlentyOs [1.6.9] 15 Oct 2024

### softcommerce/module-plenty-order-profile [1.7.5]
- **Enhancement**: Added an option to control the export of order shipping profiles [#35]

### softcommerce/module-plenty-order-profile-schedule [1.2.15]
- **Enhancement**: Added an interception plugin to handle order cancellation synchronisation [#34]

# Mage2PlentyOs [1.6.8] 09 Oct 2024

### softcommerce/module-plenty-order-profile [1.7.4]
- **Enhancement**: Added a functionality to handle cancelled order status synchronisation [#34]

### softcommerce/module-plenty-order-profile-schedule [1.2.14]
- **Enhancement**: Added order cancel event to handle cancelled order status synchronisation [#34]

# Mage2PlentyOs [1.6.7] 01 Oct 2024

### softcommerce/module-plenty-customer-client [1.2.8]
- **Enhancement**: Minor changes to codebase `SoftCommerce\PlentyCustomerClient\Model\AddressOptionTypeManagement`

### softcommerce/module-plenty-item-client [1.2.10]
- **Enhancement**: Remove `stock_warehouse_dimension, stock_warehouse_location and stock_warehouse_location_details` configs from client data collection process

### softcommerce/module-plenty-order-client [1.4.1]
- **Enhancement**: Remove `stock_warehouse_dimension, stock_warehouse_location and stock_warehouse_location_details` configs from client data collection process

### softcommerce/module-plenty-stock [1.3.8]
- **Fix**: Too few arguments to function SoftCommerce\PlentyStock\Model\GetOrderItemSourceSelection::generateInventoryRequest() 3 passed, exactly 4 [#33]

# Mage2PlentyOs [1.6.6] 01 Oct 2024

### softcommerce/module-core [1.5.7]
- **Enhancement**: Added console log debugging in admin area for JS modules

### softcommerce/module-plenty-item-profile [1.9.2]
- **Fix**: TypeError: SoftCommerce\PlentyItemProfile\Model\ItemExportService\Processor\Item::retrieveSkuByItemId() must be of type array, string given [#30]

### softcommerce/module-plenty-property [1.3.6]
- **Fix**: Argument #1 ($responseItem) must be of type array, string given in SoftCommerce\PlentyProperty\Profile\PropertyExportService\Processor\BatchProcessor::retrievePropertyId() [#31]

### softcommerce/module-plenty-rest-api [1.3.7]
- **Fix**: Argument #1 ($item) must be of type array, string given in SoftCommerce\PlentyCustomerRestApi\Model\Response\AddressDataBuilder::buildItemResponse(): [#32]

### softcommerce/module-profile [1.4.4]
- **Enhancement**: Applied a fix to profile menu items on listing pages.

# Mage2PlentyOs [1.6.5] 27 Sep 2024

### softcommerce/module-core [1.5.6]
- **Enhancement**: Added an option to display installed metapackages for the bundled modules

### softcommerce/module-plenty-category-profile [1.3.13]
- **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-customer-profile [1.1.3]
- **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-item-profile [1.9.1]
- **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-order-profile [1.7.3]
- **Enhancement**: Generate unique ID for guest customers that is required for PM contact number [#28]
- **Compatibility**: Applied compatibility for profile common configuration paths [#27]

### softcommerce/module-plenty-profile [1.5.0]
- **Feature**: Profiles that share common configuration paths can now be saved simultaneously from any profile [#27]

### softcommerce/module-plenty-stock [1.3.7]
- **Enhancement**: Addressed minor performance improvements for `SoftCommerce\PlentyStock\Model\GetOrderItemSourceSelection::generateInventoryRequest()`

### softcommerce/module-plenty-stock-profile [1.7.0]
- **Compatibility**: Applied compatibility for profile common configuration paths [#27]
- **Feature**: Introduce custom Source Selection Algorithm to achieve precise NET calculation by accounting for reservations [#26]

### softcommerce/module-profile [1.4.3]
- **Enhancement**: Added profile config data to event dispatcher for save before/after events.

### softcommerce/module-profile-config [1.2.13]
- **Fix**: Apply a fix where profile config scope writer saves value as array opposed to serialised data [#29]

# Mage2PlentyOs [1.6.4] 25 Sep 2024

### softcommerce/module-plenty-item [1.5.0]
- **Feature**: Introduce a feature to delete local item storage from admin UI [#23]

### softcommerce/module-plenty-item-profile [1.9.0]
- **Feature**: Introduce a feature to map product SKUs to Item and Variation IDs [#24]
- **Feature**: Introduce a feature to schedule item collect process from the admin UI [#22]
- **Fix**: Add a fix for duplicate client images deletion functionality [#18]

### softcommerce/module-profile [1.4.2]
- **Enhancement**: Add an option to include a menu with item that depends on URL and confirmation message for profile actions button [#25]

# Mage2PlentyOs [1.6.3] 24 Sep 2024

### softcommerce/module-core [1.5.5]
- **Compatibility**: Add compatibility for Magento 2.4.7-p2

### softcommerce/module-plenty-item [1.4.8]
- **Enhancement**: Added new methods to `SoftCommerce\PlentyItem\Model\Service\SaveProductItemVariationIdMappingInterface`

### softcommerce/module-plenty-item-profile [1.8.3]
- **Enhancement**: An option to configure media image export type. E.g. Images can be exported by providing either a direct URL or a base64 encoded image data. [#21]
- **Enhancement**: Allow mapping properties with type scope global to attributes with type scope website/store [#20]
- **Fix**: Fix massaction responsible for deleting client items externally [#19]
- **Enhancement**: Add an option to resolve duplicate client images [#18]

### softcommerce/module-plenty-property [1.3.5]
- **Enhancement**: An option to override `isGlobal` condition in `SoftCommerce\PlentyProperty\Model\AttributeToPropertyTypeMappingInterface::getPropertyTypeByAttribute`

# Mage2PlentyOs [1.6.2] 21 Sep 2024

### softcommerce/module-core [1.5.4]
- **Fix**: Cannot use "String" in namespace as it is reserved since PHP 7 [#13]

### softcommerce/module-plenty-attribute [1.4.2]
- **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-category [1.2.11]
- **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-item-profile [1.8.2]
- **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

### softcommerce/module-plenty-property [1.3.4]
- **Feature**: Introduce compatibility with `softcommerce/magento-core` module [#17]

# Mage2PlentyOs [1.6.1] 17 Sep 2024

### softcommerce/module-plenty-client [1.4.1]
- **Enhancement**: Applied changes to allow installation of media channels dynamically opposed to static declaration of image types during install

### softcommerce/module-plenty-item-profile [1.8.1]
- **Enhancement**: Applied changes to allow import of media channels dynamically opposed to static declaration of image types

# Mage2PlentyOs [1.6.0] 13 Sep 2024

### softcommerce/module-core [1.5.3]
- **Enhancement**: Introduce tooltip renderer for UI columns [#12]
- **Enhancement**: Introduce flattening array interface [#11]

### softcommerce/module-plenty-attribute [1.4.1]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-category [1.2.10]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-category-profile [1.3.12]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-client [1.4.0]
- **Feature**: Added a functionality to create referrers for system attributes to be used for multiple channels [#4]

### softcommerce/module-plenty-client-rest-api [1.3.0]
- **Feature**: Added REST API routes for `referrer` [#2]

### softcommerce/module-plenty-customer [1.3.1]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-customer-client [1.2.7]
- **Compatibility**: Introduced compatibility with client referrer functionality [#2]

### softcommerce/module-plenty-customer-profile [1.1.2]
- **Compatibility**: Introduced compatibility with client referrer functionality [#11]

### softcommerce/module-plenty-item [1.4.7]
- **Enhancement**: Added status argument to SoftCommerce\PlentyItem\Api\ItemExportQueueManagementInterface::addToQueue function [#11]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-item-profile [1.8.0]
- **Feature**: Introduce support for controlling product image types by using referrer channels [#38]
- **Enhancement**: Add products to export queue when exporting manually from within the product view page. [#37]
- **Enhancement**: Disable export/import action button on product view pages for products not visible in site visibility [#36]
- **Enhancement**: Reduce the size of message data being saved into profile history for item import/export result messages by flattening array values [#35]

### softcommerce/module-plenty-order [1.4.1]
- **Compatibility**: Introduced compatibility with client referrer functionality [#8]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-order-client [1.4.0]
- **Feature**: Move order referrer interface over to `softcommerce/module-plenty-client` to make it accessible by all modules [#5] 

### softcommerce/module-plenty-order-profile [1.7.2]
- **Compatibility**: Introduced compatibility with client referrer functionality [#41]
- **Fix**: Could not import order. Order: ###, Reason: Payment Gateway is unreachable at the moment. Please use another payment option. [#40]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-order-profile-schedule [1.2.13]
- **Compatibility**: Introduced compatibility with client referrer functionality [#4]

### softcommerce/module-plenty-order-rest-api [1.3.0]
- **Feature**: Phase out ReferrerInterface in favour of \SoftCommerce\PlentyClientRestApi\Model\ReferrerInterface [#6]

### softcommerce/module-plenty-property [1.3.3]
- **Enhancement**: Manor changes that include modification to menu titles.

### softcommerce/module-plenty-stock-profile [1.6.0]
- **Feature**: Introduce inventory reservation UI listing to enable data manipulation for reservations [#18]
- **Enhancement**: Manor changes that include modification to menu titles.

# Mage2PlentyOs [1.5.9] 17 Aug 2024

### softcommerce/module-core [1.5.2]
- **Fix**: Applied a fix to \SoftCommerce\Core\Model\Store\WebsiteStorage::getStoreIdToWebsiteId method where argument data type for $storeId was changed from string to an integer [#10].

### softcommerce/module-plenty-attribute [1.4.0]
- **Feature**: Introduce new functionality to manage manufacture synchronisation [#5]

### softcommerce/module-plenty-attribute-rest-api [1.2.7]
- **Compatibility**: Compatibility with new functionality introduced in `SoftCommerce_PlentyAttribute` [#1]

### softcommerce/module-plenty-category-profile [1.3.11]
- **Compatibility**: Introduce support for Magento 2.4.7 [#8]

### softcommerce/module-plenty-item [1.4.6]
- **Compatibility**: Introduce support for Magento 2.4.7 [#9]

### softcommerce/module-plenty-item-profile [1.7.6]
- **Compatibility**: Compatibility with new functionality introduced in `SoftCommerce_PlentyAttribute` [#34]
- **Compatibility**: Introduce support for Magento 2.4.7 [#33]

### softcommerce/module-profile-config [1.2.12]
- **Compatibility**: Introduce support for Magento 2.4.7 [#4]

# Mage2PlentyOs [1.5.8] 28 May 2024

### softcommerce/module-core [1.5.1]
- **Feature**: Added service & processor interface wrapper for dependant modules that use data processing.

### softcommerce/module-plenty-item-profile [1.7.5]
- **Feature**: Add an option to collect + import items from within the product page view #32

### softcommerce/module-profile [1.4.1]
- **Enhancement**: Preserve an array key for context services in `SoftCommerce\Profile\Model\ServiceAbstract\Service::initServices` [#4]

# Mage2PlentyOs [1.5.7] 16 May 2024

### softcommerce/module-plenty-item-profile [1.7.4]
- **Fix**: Deprecated Functionality: Creation of dynamic property SoftCommerce\PlentyItemProfile\...\ItemStorage::$variationIdToItemId is deprecated [#31]

# Mage2PlentyOs [1.5.6] 25 Apr 2024

### softcommerce/module-plenty-attribute [1.3.2]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-attribute-rest-api [1.2.6]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-category-profile-schedule [1.2.5]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-category-rest-api [1.2.4]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-client [1.3.3]
- **Feature**: Introduce new config data collect management interface [#3]

### softcommerce/module-plenty-client-rest-api [1.2.7]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-customer [1.3.0]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-customer-client [1.2.6]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#1]

### softcommerce/module-plenty-customer-profile [1.1.1]
- **Enhancement**: Switch to using new client data collect interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface [#10]

### softcommerce/module-plenty-customer-rest-api [1.2.6]
- **Compatibility**: Compatibility with PHP 8.3

### softcommerce/module-plenty-item-client [1.2.9]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#1]

### softcommerce/module-plenty-item-profile [1.7.3]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#30]

### softcommerce/module-plenty-item-profile-schedule [1.3.0]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-item-rest-api [1.3.0]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-log [1.2.7]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-order-client [1.3.0]
- **Feature**: Create order item property type "product options" to enable exporting additional order item information [#4]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#3]
- **Feature**: Introduce new order property management to create and handle custom order item attributes [#2]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#1]

### softcommerce/module-plenty-order-profile [1.7.1]
- **Enhancement**: Include export of order item "additional_options" data for order export #39
- **Enhancement**: Include client configuration data collect pre-process to be able to collect data prio to order export [#38]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#37]
- **Fix**: Argument #1 ($countryCode) must be of type string, null given in SoftCommerce\PlentyOrderProfile\Model\OrderExportService\Generator\Order\Items\ItemAbstract::getCountryId() [#36]

### softcommerce/module-plenty-order-rest-api [1.2.9]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-property [1.3.2]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-property-rest-api [1.2.6]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-rest-api [1.3.6]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-stock-client [1.2.8]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#1]

### softcommerce/module-plenty-stock-profile [1.5.2]
- **Enhancement**: Switch to using new interface SoftCommerce\PlentyClient\Model\CollectClientConfigDataManagementInterface to collect client data configuration [#17]

### softcommerce/module-plenty-stock-profile-schedule [1.2.9]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-stock-rest-api [1.2.7]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-profile-history [1.2.8]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-profile-queue [1.1.1]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-profile-schedule [1.3.6]
- **Compatibility**: Introduced support for PHP 8.3

# Mage2PlentyOs [1.5.5] 22 Apr 2024

### softcommerce/module-plenty-category [1.2.9]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-client [1.3.2]
- **Feature**: Introduce new method to retrieve client data by locale. [#2]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-item [1.4.5]
- **Compatibility**: Introduced support for PHP 8.3
- **Enhancement**: Removed unused etc/config.xml that has no purpose. 

### softcommerce/module-plenty-item-client [1.2.8]
- **Compatibility**: Introduced support for PHP 8.3

### softcommerce/module-plenty-item-profile [1.7.2]
- **Feature**: Add attribute mapping for availability fields [#29]

### softcommerce/module-plenty-stock [1.3.6]
- **Compatibility**: Introduced support for PHP 8.3
- **Enhancement**: Added new methods `getReservedBundle` and `setReservedBundle` to `SoftCommerce\PlentyStock\Api\Data\InventoryInterface`

### softcommerce/module-plenty-stock-client [1.2.7]
- **Compatibility**: Introduced support for PHP 8.3
- **Enhancement**: Added new methods to `SoftCommerce\PlentyStockClient\Api\Data\WarehouseLocationInterface`

### softcommerce/module-plenty-stock-profile [1.5.1]
- **Enhancement**: Include stock calculation for reservation bundle [#16]

# Mage2PlentyOs [1.5.4] 25 Mar 2024

### softcommerce/module-plenty-item-profile [1.7.1]
- **Enhancement**: Added an option to allow/disallow child product name generation based on parent name and attributes [#28]

# Mage2PlentyOs [1.5.4] 25 Mar 2024

### softcommerce/module-plenty-item-profile [1.7.1]
- **Enhancement**: Added an option to allow/disallow child product name generation based on parent name and attributes [#28]

# Mage2PlentyOs [1.5.3] 21 Mar 2024

### softcommerce/module-core [1.5.0]
- **Compatibility**: Introduced compatibility with PHP type declaration [#9]
- **Compatibility**: Introduced support for PHP 8.3 [#8]
- **Feature**: Implement functionality to support UI form scope data [#7]

### softcommerce/module-plenty-category-profile [1.3.10]
- **Compatibility**: Introduced support for PHP 8.3 [#7]
- **Enhancement**: Improvements to UI form components for category configuration profile [#6]

### softcommerce/module-plenty-customer-profile [1.1.0]
- **Enhancement**: An option to retrieve a referrer ID by store cope [#9]
- **Compatibility**: Introduced support for PHP 8.3 [#8]
- **Enhancement**: Improvements to UI form components for customer profile configuration [#7]

### softcommerce/module-plenty-item-profile [1.7.0]
- **Compatibility**: Introduced support for PHP 8.3 [#27]
- **Enhancement**: Improvements to UI form components for item profile configuration [#26]

### softcommerce/module-plenty-order [1.4.0]
- **Compatibility**: Introduced support for PHP 8.3 [#7]
- **Enhancement**: Introduced compatibility with PHP type declaration [#6]

### softcommerce/module-plenty-order-profile [1.7.0]
- **Compatibility**: Introduced support for PHP 8.3 [#35]
- **Feature**: Introduced support for scoped configuration within profile UI form components [#34]

### softcommerce/module-plenty-order-profile-schedule [1.2.12]
- **Compatibility**: Introduced support for PHP 8.3 [#3]

### softcommerce/module-plenty-profile [1.4.0]
- **Enhancement**: Changes to profile configuration where referrer ID is now retrieved by store scope instead of website [#2]
- **Compatibility**: Introduced support for PHP 8.3 [#1]

### softcommerce/module-plenty-stock-profile [1.5.0]
- **Feature**: Introduced support for scoped configuration within profile UI form components [#15]
- **Compatibility**: Introduced support for PHP 8.3 [#14]

### softcommerce/module-profile [1.4.0]
- **Feature**: Introduced functionality to support UI form scoped data [#3]
- **Compatibility**: Introduced support for PHP 8.3 [#2]

### softcommerce/module-profile-config [1.2.11]
- **Compatibility**: Introduced support for PHP 8.3 [#2]
