Class CountryCore
=====================





* Class name: CountryCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Country.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L28)


Contents
--------


### Properties

* [$_idZones](#property-$_idZones)
* [$active](#property-$active)
* [$call_prefix](#property-$call_prefix)
* [$contains_states](#property-$contains_states)
* [$definition](#property-$definition)
* [$display_tax_label](#property-$display_tax_label)
* [$id](#property-$id)
* [$id_currency](#property-$id_currency)
* [$id_zone](#property-$id_zone)
* [$iso_code](#property-$iso_code)
* [$name](#property-$name)
* [$need_identification_number](#property-$need_identification_number)
* [$need_zip_code](#property-$need_zip_code)
* [$webserviceParameters](#property-$webserviceParameters)
* [$zip_code_format](#property-$zip_code_format)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$table](#property-$table)
* [$tables](#property-$tables)

### Methods

* [__construct](#method-__construct)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [affectZoneToSelection](#method-affectZoneToSelection)
* [associateTo](#method-associateTo)
* [clearCache](#method-clearCache)
* [containsStates](#method-containsStates)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getByIso](#method-getByIso)
* [getCountries](#method-getCountries)
* [getCountriesByZoneId](#method-getCountriesByZoneId)
* [getDefaultCountryId](#method-getDefaultCountryId)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getIdByName](#method-getIdByName)
* [getIdZone](#method-getIdZone)
* [getIsoById](#method-getIsoById)
* [getNameById](#method-getNameById)
* [getNeedZipCode](#method-getNeedZipCode)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [getZipCodeFormat](#method-getZipCodeFormat)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToGroupShop](#method-isAssociatedToGroupShop)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isNeedDni](#method-isNeedDni)
* [isNeedDniByCountryId](#method-isNeedDniByCountryId)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)




Properties
----------


### <a name="property-$_idZones"></a>$_idZones

```php
protected mixed $_idZones = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Country.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L65).


### <a name="property-$active"></a>$active

```php
public boolean $active = true
```





* Visibility: **public**
* Source: [classes/Country.php line 63](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L63).


### <a name="property-$call_prefix"></a>$call_prefix

```php
public integer $call_prefix
```





* Visibility: **public**
* Source: [classes/Country.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L42).


### <a name="property-$contains_states"></a>$contains_states

```php
public boolean $contains_states
```





* Visibility: **public**
* Source: [classes/Country.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L48).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'country', 'primary' => 'id_country', 'multilang' => true, 'fields' => array('id_zone' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_currency' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'call_prefix' => array('type' => self::TYPE_INT, 'validate' => 'isInt'), 'iso_code' => array('type' => self::TYPE_STRING, 'validate' => 'isLanguageIsoCode', 'required' => true, 'size' => 3), 'active' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'contains_states' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool', 'required' => true), 'need_identification_number' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool', 'required' => true), 'need_zip_code' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'zip_code_format' => array('type' => self::TYPE_STRING, 'validate' => 'isZipCodeFormat'), 'display_tax_label' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool', 'required' => true), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 64)), 'associations' => array('zone' => array('type' => self::HAS_ONE), 'currency' => array('type' => self::HAS_ONE)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Country.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L70).


### <a name="property-$display_tax_label"></a>$display_tax_label

```php
public boolean $display_tax_label = true
```





* Visibility: **public**
* Source: [classes/Country.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L60).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/Country.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L30).


### <a name="property-$id_currency"></a>$id_currency

```php
public integer $id_currency
```





* Visibility: **public**
* Source: [classes/Country.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L36).


### <a name="property-$id_zone"></a>$id_zone

```php
public integer $id_zone
```





* Visibility: **public**
* Source: [classes/Country.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L33).


### <a name="property-$iso_code"></a>$iso_code

```php
public string $iso_code
```





* Visibility: **public**
* Source: [classes/Country.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L39).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Country.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L45).


### <a name="property-$need_identification_number"></a>$need_identification_number

```php
public boolean $need_identification_number
```





* Visibility: **public**
* Source: [classes/Country.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L51).


### <a name="property-$need_zip_code"></a>$need_zip_code

```php
public boolean $need_zip_code
```





* Visibility: **public**
* Source: [classes/Country.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L54).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectsNodeName' => 'countries', 'fields' => array('id_zone' => array('xlink_resource' => 'zones'), 'id_currency' => array('xlink_resource' => 'currencies')))
```





* Visibility: **protected**
* Source: [classes/Country.php line 95](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L95).


### <a name="property-$zip_code_format"></a>$zip_code_format

```php
public string $zip_code_format
```





* Visibility: **public**
* Source: [classes/Country.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L57).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 122](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L122).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L72).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L57).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L87).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L77).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L92).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L82).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L97).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L51).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 53](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L53).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L67).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L108).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L111).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L62).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 102](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L102).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 150](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L150)


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
* Source: [classes/ObjectModel.php line 372](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L372)


#### Arguments
* $autodate **boolean**
* $null_values **boolean**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 925](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L925)


#### Arguments
* $fields **mixed**



### <a name="method-affectZoneToSelection"></a>affectZoneToSelection

```php
boolean CountryCore::affectZoneToSelection($ids_countries, $id_zone)
```





* Visibility: **public**
* Source: [classes/Country.php line 322](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L322)


#### Arguments
* $ids_countries **mixed**
* $id_zone **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops, string $type)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 973](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L973)


#### Arguments
* $id_shops **integer|array**
* $type **string**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 939](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L939)


#### Arguments
* $all **mixed**



### <a name="method-containsStates"></a>containsStates

```php
mixed CountryCore::containsStates($id_country)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 309](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L309)


#### Arguments
* $id_country **mixed**



### <a name="method-delete"></a>delete

```php
mixed CountryCore::delete()
```





* Visibility: **public**
* Source: [classes/Country.php line 103](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L103)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage()
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1047](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1047)




### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 559](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L559)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 757](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L757)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1017](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1017)


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
* Source: [classes/ObjectModel.php line 1081](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1081)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 272](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L272)


#### Arguments
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 319](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L319)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-getByIso"></a>getByIso

```php
integer CountryCore::getByIso(string $iso_code)
```

Get a country ID with its iso code



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 156](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L156)


#### Arguments
* $iso_code **string** - Country iso code



### <a name="method-getCountries"></a>getCountries

```php
array CountryCore::getCountries(integer $id_lang, boolean $active, $contain_states, \Shop $shop)
```

Return available countries



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L117)


#### Arguments
* $id_lang **integer** - Language ID
* $active **boolean** - return only active coutries
* $contain_states **mixed**
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-getCountriesByZoneId"></a>getCountriesByZoneId

```php
mixed CountryCore::getCountriesByZoneId($id_zone, $id_lang, \Shop $shop)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 278](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L278)


#### Arguments
* $id_zone **mixed**
* $id_lang **mixed**
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-getDefaultCountryId"></a>getDefaultCountryId

```php
integer CountryCore::getDefaultCountryId()
```

Returns the default country Id



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 272](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L272)




### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1184)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1261](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1261)


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
* Source: [classes/ObjectModel.php line 234](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L234)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L249)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 917](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L917)


#### Arguments
* $all **mixed**



### <a name="method-getIdByName"></a>getIdByName

```php
\intval CountryCore::getIdByName(integer $id_lang, string $country)
```

Get a country id with its name



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 230](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L230)


#### Arguments
* $id_lang **integer** - Language ID
* $country **string** - Country Name



### <a name="method-getIdZone"></a>getIdZone

```php
mixed CountryCore::getIdZone($id_country)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 168](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L168)


#### Arguments
* $id_country **mixed**



### <a name="method-getIsoById"></a>getIsoById

```php
string CountryCore::getIsoById(integer $id_country)
```

Get a country iso with its ID



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 212](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L212)


#### Arguments
* $id_country **integer** - Country ID



### <a name="method-getNameById"></a>getNameById

```php
string CountryCore::getNameById(integer $id_lang, integer $id_country)
```

Get a country name with its ID



* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 192](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L192)


#### Arguments
* $id_lang **integer** - Language ID
* $id_country **integer** - Country ID



### <a name="method-getNeedZipCode"></a>getNeedZipCode

```php
mixed CountryCore::getNeedZipCode($id_country)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 244](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L244)


#### Arguments
* $id_country **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 595](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L595)


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
* Source: [classes/ObjectModel.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L130)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 890](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L890)


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
* Source: [classes/ObjectModel.php line 816](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L816)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-getZipCodeFormat"></a>getZipCodeFormat

```php
mixed CountryCore::getZipCodeFormat($id_country)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 255](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L255)


#### Arguments
* $id_country **mixed**



### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1116](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1116)


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
* Source: [classes/ObjectModel.php line 1135](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1135)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-isAssociatedToGroupShop"></a>isAssociatedToGroupShop

```php
boolean ObjectModelCore::isAssociatedToGroupShop(integer $id_group_shop)
```

Check if current object is associated to a group shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1003](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1003)


#### Arguments
* $id_group_shop **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 954](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L954)


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
* Source: [classes/ObjectModel.php line 1099](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1099)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1037](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1037)




### <a name="method-isNeedDni"></a>isNeedDni

```php
mixed CountryCore::isNeedDni()
```





* Visibility: **public**
* Source: [classes/Country.php line 296](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L296)




### <a name="method-isNeedDniByCountryId"></a>isNeedDniByCountryId

```php
mixed CountryCore::isNeedDniByCountryId($id_country)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Country.php line 301](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/Country.php#L301)


#### Arguments
* $id_country **mixed**



### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 611](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L611)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 360](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L360)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1207](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L1207)




### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 575](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L575)




### <a name="method-update"></a>update

```php
boolean ObjectModelCore::update(boolean $null_values)
```

Update current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 446](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L446)


#### Arguments
* $null_values **boolean**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L772)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 778](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L778)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 710](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L710)


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
* Source: [classes/ObjectModel.php line 649](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L649)


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
* Source: [classes/ObjectModel.php line 675](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.5/classes/ObjectModel.php#L675)


#### Arguments
* $die **boolean**
* $error_return **boolean**


