Class OrderInvoiceCore
=====================





* Class name: OrderInvoiceCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/order/OrderInvoice.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L27)


Contents
--------

### Constants

* [DETAIL](#constant-DETAIL)
* [TAX_EXCL](#constant-TAX_EXCL)
* [TAX_INCL](#constant-TAX_INCL)

### Properties

* [$_total_paid_cache](#property-$_total_paid_cache)
* [$date_add](#property-$date_add)
* [$definition](#property-$definition)
* [$delivery_date](#property-$delivery_date)
* [$delivery_number](#property-$delivery_number)
* [$id_order](#property-$id_order)
* [$note](#property-$note)
* [$number](#property-$number)
* [$shipping_tax_computation_method](#property-$shipping_tax_computation_method)
* [$total_discount_tax_excl](#property-$total_discount_tax_excl)
* [$total_discount_tax_incl](#property-$total_discount_tax_incl)
* [$total_paid_tax_excl](#property-$total_paid_tax_excl)
* [$total_paid_tax_incl](#property-$total_paid_tax_incl)
* [$total_products](#property-$total_products)
* [$total_products_wt](#property-$total_products_wt)
* [$total_shipping_tax_excl](#property-$total_shipping_tax_excl)
* [$total_shipping_tax_incl](#property-$total_shipping_tax_incl)
* [$total_wrapping_tax_excl](#property-$total_wrapping_tax_excl)
* [$total_wrapping_tax_incl](#property-$total_wrapping_tax_incl)
* [$db](#property-$db)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id](#property-$id)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)
* [$webserviceParameters](#property-$webserviceParameters)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateObject](#method-duplicateObject)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAssociatedShops](#method-getAssociatedShops)
* [getByDateInterval](#method-getByDateInterval)
* [getByDeliveryDateInterval](#method-getByDeliveryDateInterval)
* [getByStatus](#method-getByStatus)
* [getCarrier](#method-getCarrier)
* [getCarrierId](#method-getCarrierId)
* [getDefinition](#method-getDefinition)
* [getEcoTaxTaxesBreakdown](#method-getEcoTaxTaxesBreakdown)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getGlobalRestPaid](#method-getGlobalRestPaid)
* [getInvoiceNumberFormatted](#method-getInvoiceNumberFormatted)
* [getOrderPaymentCollection](#method-getOrderPaymentCollection)
* [getProductTaxesBreakdown](#method-getProductTaxesBreakdown)
* [getProducts](#method-getProducts)
* [getProductsDetail](#method-getProductsDetail)
* [getRestPaid](#method-getRestPaid)
* [getShippingTaxesBreakdown](#method-getShippingTaxesBreakdown)
* [getSibling](#method-getSibling)
* [getSiblingTotal](#method-getSiblingTotal)
* [getTotalPaid](#method-getTotalPaid)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [getWrappingTaxesBreakdown](#method-getWrappingTaxesBreakdown)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [isPaid](#method-isPaid)
* [makeTranslationFields](#method-makeTranslationFields)
* [retrieveOneById](#method-retrieveOneById)
* [save](#method-save)
* [saveCarrierTaxCalculator](#method-saveCarrierTaxCalculator)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [setProductCurrentStock](#method-setProductCurrentStock)
* [setProductCustomizedDatas](#method-setProductCustomizedDatas)
* [setProductImageInformations](#method-setProductImageInformations)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateMultishopTable](#method-updateMultishopTable)
* [useOneAfterAnotherTaxComputationMethod](#method-useOneAfterAnotherTaxComputationMethod)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)


Constants
----------


### <a name="constant-DETAIL"></a>DETAIL

```php
const DETAIL = 2
```





* Source: [classes/order/OrderInvoice.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L31).


### <a name="constant-TAX_EXCL"></a>TAX_EXCL

```php
const TAX_EXCL = 0
```





* Source: [classes/order/OrderInvoice.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L29).


### <a name="constant-TAX_INCL"></a>TAX_INCL

```php
const TAX_INCL = 1
```





* Source: [classes/order/OrderInvoice.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L30).


Properties
----------


### <a name="property-$_total_paid_cache"></a>$_total_paid_cache

```php
protected array $_total_paid_cache = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/order/OrderInvoice.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L85).


### <a name="property-$date_add"></a>$date_add

```php
public \intger $date_add
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L82).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'order_invoice', 'primary' => 'id_order_invoice', 'fields' => array('id_order' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'number' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'delivery_number' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'delivery_date' => array('type' => self::TYPE_DATE, 'validate' => 'isDateFormat'), 'total_discount_tax_excl' => array('type' => self::TYPE_FLOAT), 'total_discount_tax_incl' => array('type' => self::TYPE_FLOAT), 'total_paid_tax_excl' => array('type' => self::TYPE_FLOAT), 'total_paid_tax_incl' => array('type' => self::TYPE_FLOAT), 'total_products' => array('type' => self::TYPE_FLOAT), 'total_products_wt' => array('type' => self::TYPE_FLOAT), 'total_shipping_tax_excl' => array('type' => self::TYPE_FLOAT), 'total_shipping_tax_incl' => array('type' => self::TYPE_FLOAT), 'shipping_tax_computation_method' => array('type' => self::TYPE_INT), 'total_wrapping_tax_excl' => array('type' => self::TYPE_FLOAT), 'total_wrapping_tax_incl' => array('type' => self::TYPE_FLOAT), 'note' => array('type' => self::TYPE_STRING, 'validate' => 'isCleanHtml', 'size' => 65000), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/order/OrderInvoice.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L90).


### <a name="property-$delivery_date"></a>$delivery_date

```php
public integer $delivery_date = '0000-00-00 00:00:00'
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L43).


### <a name="property-$delivery_number"></a>$delivery_number

```php
public integer $delivery_number
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L40).


### <a name="property-$id_order"></a>$id_order

```php
public integer $id_order
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L34).


### <a name="property-$note"></a>$note

```php
public string $note
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L79).


### <a name="property-$number"></a>$number

```php
public integer $number
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L37).


### <a name="property-$shipping_tax_computation_method"></a>$shipping_tax_computation_method

```php
public integer $shipping_tax_computation_method
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L70).


### <a name="property-$total_discount_tax_excl"></a>$total_discount_tax_excl

```php
public float $total_discount_tax_excl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L46).


### <a name="property-$total_discount_tax_incl"></a>$total_discount_tax_incl

```php
public float $total_discount_tax_incl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L49).


### <a name="property-$total_paid_tax_excl"></a>$total_paid_tax_excl

```php
public float $total_paid_tax_excl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L52).


### <a name="property-$total_paid_tax_incl"></a>$total_paid_tax_incl

```php
public float $total_paid_tax_incl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L55).


### <a name="property-$total_products"></a>$total_products

```php
public float $total_products
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L58).


### <a name="property-$total_products_wt"></a>$total_products_wt

```php
public float $total_products_wt
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L61).


### <a name="property-$total_shipping_tax_excl"></a>$total_shipping_tax_excl

```php
public float $total_shipping_tax_excl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L64).


### <a name="property-$total_shipping_tax_incl"></a>$total_shipping_tax_incl

```php
public float $total_shipping_tax_incl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L67).


### <a name="property-$total_wrapping_tax_excl"></a>$total_wrapping_tax_excl

```php
public float $total_wrapping_tax_excl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L73).


### <a name="property-$total_wrapping_tax_incl"></a>$total_wrapping_tax_incl

```php
public float $total_wrapping_tax_incl
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L76).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 140](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L140).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L130).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L80).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L65).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 95](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L95).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L85).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L100).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L90).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 105](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L105).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 63](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L63).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L54).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L57).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L59).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L61).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L75).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 116](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L116).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L119).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L70).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 110](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L110).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 135](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L135).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected array $webserviceParameters = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 113](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L113).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 168](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L168)


#### Arguments
* $id **integer** - Existing object id in order to load object (optional)
* $id_lang **integer** - Required if object is multilingual (optional)
* $id_shop **integer** - ID shop for objects with multishop on langs



### <a name="method-add"></a>add

```php
boolean ObjectModelCore::add(boolean $autodate, boolean $null_values)
```

Add current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 427](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L427)


#### Arguments
* $autodate **boolean**
* $null_values **boolean**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1182](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1182)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1229](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1229)


#### Arguments
* $id_shops **integer|array**



### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1169](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1169)




### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1196](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1196)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
boolean ObjectModelCore::delete()
```

Delete current object from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 688](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L688)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1360](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1360)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 734](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L734)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 958](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L958)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateObject"></a>duplicateObject

```php
\new ObjectModelCore::duplicateObject()
```

Duplicate current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 518](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L518)




### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1273)


#### Arguments
* $id **mixed**



### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1397](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1397)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 325](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L325)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 371](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L371)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1258](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1258)




### <a name="method-getByDateInterval"></a>getByDateInterval

```php
array OrderInvoiceCore::getByDateInterval($date_from, $date_to)
```

Returns all the order invoice that match the date interval



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 414](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L414)


#### Arguments
* $date_from **mixed**
* $date_to **mixed**



### <a name="method-getByDeliveryDateInterval"></a>getByDeliveryDateInterval

```php
array OrderInvoiceCore::getByDeliveryDateInterval($date_from, $date_to)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 462](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L462)


#### Arguments
* $date_from **mixed**
* $date_to **mixed**



### <a name="method-getByStatus"></a>getByStatus

```php
array OrderInvoiceCore::getByStatus($id_order_state)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 435](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L435)


#### Arguments
* $id_order_state **mixed**



### <a name="method-getCarrier"></a>getCarrier

```php
mixed OrderInvoiceCore::getCarrier($id_order_invoice)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 482](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L482)


#### Arguments
* $id_order_invoice **mixed**



### <a name="method-getCarrierId"></a>getCarrierId

```php
mixed OrderInvoiceCore::getCarrierId($id_order_invoice)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 496](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L496)


#### Arguments
* $id_order_invoice **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1503](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1503)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getEcoTaxTaxesBreakdown"></a>getEcoTaxTaxesBreakdown

```php
array OrderInvoiceCore::getEcoTaxTaxesBreakdown()
```

Returns the ecotax taxes breakdown



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 385](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L385)




### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1610](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1610)


#### Arguments
* $field_name **mixed**
* $id_lang **null**



### <a name="method-getFields"></a>getFields

```php
array ObjectModelCore::getFields()
```

Prepare fields for ObjectModel class (add, update)
All fields are verified (pSQL, intval.

..)

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 253](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L253)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 290](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L290)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1161](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1161)


#### Arguments
* $all **mixed**



### <a name="method-getFieldsShop"></a>getFieldsShop

```php
array ObjectModelCore::getFieldsShop()
```

Prepare fields for multishop
Fields are not validated here, we considere they are already validated in getFields() method, this
not the best solution but this is the only one possible for retro compatibility.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L276)




### <a name="method-getGlobalRestPaid"></a>getGlobalRestPaid

```php
mixed OrderInvoiceCore::getGlobalRestPaid()
```

Get global rest to paid
   This method will return something different of the method getRestPaid if
   there is an other invoice linked to the payments of the current invoice



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 614](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L614)




### <a name="method-getInvoiceNumberFormatted"></a>getInvoiceNumberFormatted

```php
string OrderInvoiceCore::getInvoiceNumberFormatted(integer $id_lang, $id_shop)
```

Get the formatted number of invoice



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 665](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L665)


#### Arguments
* $id_lang **integer** - for invoice_prefix
* $id_shop **mixed**



### <a name="method-getOrderPaymentCollection"></a>getOrderPaymentCollection

```php
\Collection OrderInvoiceCore::getOrderPaymentCollection()
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 654](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L654)




### <a name="method-getProductTaxesBreakdown"></a>getProductTaxesBreakdown

```php
array OrderInvoiceCore::getProductTaxesBreakdown()
```

Returns the correct product taxes breakdown.



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 255](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L255)




### <a name="method-getProducts"></a>getProducts

```php
array OrderInvoiceCore::getProducts($products, $selectedProducts, $selectedQty)
```

Get order products



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 131](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L131)


#### Arguments
* $products **mixed**
* $selectedProducts **mixed**
* $selectedQty **mixed**



### <a name="method-getProductsDetail"></a>getProductsDetail

```php
mixed OrderInvoiceCore::getProductsDetail()
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L114)




### <a name="method-getRestPaid"></a>getRestPaid

```php
float OrderInvoiceCore::getRestPaid()
```

Rest Paid



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 542](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L542)




### <a name="method-getShippingTaxesBreakdown"></a>getShippingTaxesBreakdown

```php
array OrderInvoiceCore::getShippingTaxesBreakdown($order)
```

Returns the shipping taxes breakdown



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 341](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L341)


#### Arguments
* $order **mixed**



### <a name="method-getSibling"></a>getSibling

```php
mixed OrderInvoiceCore::getSibling()
```

Return collection of order invoice object linked to the payments of the current order invoice object



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 553](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L553)




### <a name="method-getSiblingTotal"></a>getSiblingTotal

```php
mixed OrderInvoiceCore::getSiblingTotal(integer $mod)
```

Return total to paid of sibling invoices



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 584](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L584)


#### Arguments
* $mod **integer** - TAX_EXCL, TAX_INCL, DETAIL



### <a name="method-getTotalPaid"></a>getTotalPaid

```php
float OrderInvoiceCore::getTotalPaid()
```

Amounts of payments



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 523](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L523)




### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 769](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L769)


#### Arguments
* $fields_array **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $class)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L148)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1102](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1102)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed ObjectModelCore::getWebserviceParameters($ws_params_attribute_name)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1027](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1027)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-getWrappingTaxesBreakdown"></a>getWrappingTaxesBreakdown

```php
array OrderInvoiceCore::getWrappingTaxesBreakdown()
```

Returns the wrapping taxes breakdown



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 373](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L373)




### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1298](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1298)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1435](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1435)


#### Arguments
* $data **array**
* $id_lang **integer**



### <a name="method-hydrateCollection"></a>hydrateCollection

```php
array ObjectModelCore::hydrateCollection(string $class, array $datas, integer $id_lang)
```

Fill (hydrate) a list of objects in order to get a collection of these objects



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1454](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1454)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1211](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1211)


#### Arguments
* $id_shop **integer**



### <a name="method-isCurrentlyUsed"></a>isCurrentlyUsed

```php
boolean ObjectModelCore::isCurrentlyUsed(string $table, boolean $has_active_column)
```

This method is allow to know if a entity is currently used



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1415](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1415)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1315](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1315)




### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1310](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1310)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1305](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1305)




### <a name="method-isPaid"></a>isPaid

```php
boolean OrderInvoiceCore::isPaid()
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 645](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L645)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 785](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L785)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-retrieveOneById"></a>retrieveOneById

```php
\OrderInvoice OrderInvoiceCore::retrieveOneById($id)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/OrderInvoice.php line 510](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L510)


#### Arguments
* $id **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 415](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L415)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-saveCarrierTaxCalculator"></a>saveCarrierTaxCalculator

```php
mixed OrderInvoiceCore::saveCarrierTaxCalculator(array $taxes_amount)
```





* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 670](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L670)


#### Arguments
* $taxes_amount **array**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1541](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1541)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1636](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1636)


#### Arguments
* $fields **array**



### <a name="method-setProductCurrentStock"></a>setProductCurrentStock

```php
mixed OrderInvoiceCore::setProductCurrentStock($product)
```

This method allow to add stock information on a product detail



* Visibility: **protected**
* Source: [classes/order/OrderInvoice.php line 191](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L191)


#### Arguments
* $product **mixed**



### <a name="method-setProductCustomizedDatas"></a>setProductCustomizedDatas

```php
mixed OrderInvoiceCore::setProductCustomizedDatas($product, $customized_datas)
```





* Visibility: **protected**
* Source: [classes/order/OrderInvoice.php line 177](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L177)


#### Arguments
* $product **mixed**
* $customized_datas **mixed**



### <a name="method-setProductImageInformations"></a>setProductImageInformations

```php
mixed OrderInvoiceCore::setProductImageInformations($product)
```

This method allow to add image information on a product detail



* Visibility: **protected**
* Source: [classes/order/OrderInvoice.php line 206](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L206)


#### Arguments
* $product **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 750](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L750)




### <a name="method-update"></a>update

```php
boolean ObjectModelCore::update(boolean $null_values)
```

Update current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 574](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L574)


#### Arguments
* $null_values **boolean**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1330](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1330)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-useOneAfterAnotherTaxComputationMethod"></a>useOneAfterAnotherTaxComputationMethod

```php
boolean OrderInvoiceCore::useOneAfterAnotherTaxComputationMethod()
```

This method returns true if at least one order details uses the
One After Another tax computation method.



* Visibility: **public**
* Source: [classes/order/OrderInvoice.php line 236](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/order/OrderInvoice.php#L236)




### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 973](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L973)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 979](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L979)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 896](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L896)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string ObjectModelCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 823](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L823)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsLang"></a>validateFieldsLang

```php
boolean|string ObjectModelCore::validateFieldsLang(boolean $die, boolean $error_return)
```

Check for multilingual fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 852](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L852)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1138](https://github.com/PrestaShop/PrestaShop/blob/1.5.6.0/classes/ObjectModel.php#L1138)


#### Arguments
* $htmlentities **mixed**


