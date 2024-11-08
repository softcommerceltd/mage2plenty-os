## Changelog

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
