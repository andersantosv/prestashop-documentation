Class LanguageCore
=====================





* Class name: LanguageCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Language.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L27)


Contents
--------


### Properties

* [$_LANGUAGES](#property-$_LANGUAGES)
* [$_cache_language_installation](#property-$_cache_language_installation)
* [$_checkedLangs](#property-$_checkedLangs)
* [$active](#property-$active)
* [$countActiveLanguages](#property-$countActiveLanguages)
* [$date_format_full](#property-$date_format_full)
* [$date_format_lite](#property-$date_format_lite)
* [$definition](#property-$definition)
* [$id](#property-$id)
* [$is_rtl](#property-$is_rtl)
* [$iso_code](#property-$iso_code)
* [$language_code](#property-$language_code)
* [$name](#property-$name)
* [$translationsFilesAndVars](#property-$translationsFilesAndVars)
* [$webserviceParameters](#property-$webserviceParameters)
* [$cache_objects](#property-$cache_objects)
* [$db](#property-$db)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$force_id](#property-$force_id)
* [$get_shop_from_context](#property-$get_shop_from_context)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$id_shop_list](#property-$id_shop_list)
* [$identifier](#property-$identifier)
* [$image_dir](#property-$image_dir)
* [$image_format](#property-$image_format)
* [$loaded_classes](#property-$loaded_classes)
* [$table](#property-$table)
* [$tables](#property-$tables)
* [$update_fields](#property-$update_fields)

### Methods

* [__construct](#method-__construct)
* [_copyNoneFlag](#method-_copyNoneFlag)
* [_generateFiles](#method-_generateFiles)
* [_getThemesList](#method-_getThemesList)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [associateTo](#method-associateTo)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [checkAndAddLanguage](#method-checkAndAddLanguage)
* [checkFiles](#method-checkFiles)
* [checkFilesWithIsoCode](#method-checkFilesWithIsoCode)
* [clearCache](#method-clearCache)
* [copyLanguageData](#method-copyLanguageData)
* [countActiveLanguages](#method-countActiveLanguages)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [disableCache](#method-disableCache)
* [displayFieldName](#method-displayFieldName)
* [downloadAndInstallLanguagePack](#method-downloadAndInstallLanguagePack)
* [duplicateObject](#method-duplicateObject)
* [duplicateShops](#method-duplicateShops)
* [enableCache](#method-enableCache)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAssociatedShops](#method-getAssociatedShops)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getFilesList](#method-getFilesList)
* [getIdByIso](#method-getIdByIso)
* [getIsoById](#method-getIsoById)
* [getIsoIds](#method-getIsoIds)
* [getLanguage](#method-getLanguage)
* [getLanguageByIETFCode](#method-getLanguageByIETFCode)
* [getLanguageCodeByIso](#method-getLanguageCodeByIso)
* [getLanguagePackListContent](#method-getLanguagePackListContent)
* [getLanguages](#method-getLanguages)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isInstalled](#method-isInstalled)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiLanguageActivated](#method-isMultiLanguageActivated)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [loadLanguages](#method-loadLanguages)
* [loadUpdateSQL](#method-loadUpdateSQL)
* [makeTranslationFields](#method-makeTranslationFields)
* [moveToIso](#method-moveToIso)
* [recurseDeleteDir](#method-recurseDeleteDir)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateModulesTranslations](#method-updateModulesTranslations)
* [updateMultishopTable](#method-updateMultishopTable)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)




Properties
----------


### <a name="property-$_LANGUAGES"></a>$_LANGUAGES

```php
protected mixed $_LANGUAGES
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Language.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L72).


### <a name="property-$_cache_language_installation"></a>$_cache_language_installation

```php
protected mixed $_cache_language_installation = null
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Language.php line 802](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L802).


### <a name="property-$_checkedLangs"></a>$_checkedLangs

```php
protected array $_checkedLangs
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Language.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L71).


### <a name="property-$active"></a>$active

```php
public boolean $active = true
```





* Visibility: **public**
* Source: [classes/Language.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L50).


### <a name="property-$countActiveLanguages"></a>$countActiveLanguages

```php
protected mixed $countActiveLanguages = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Language.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L73).


### <a name="property-$date_format_full"></a>$date_format_full

```php
public string $date_format_full = 'Y-m-d H:i:s'
```





* Visibility: **public**
* Source: [classes/Language.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L44).


### <a name="property-$date_format_lite"></a>$date_format_lite

```php
public string $date_format_lite = 'Y-m-d'
```





* Visibility: **public**
* Source: [classes/Language.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L41).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'lang', 'primary' => 'id_lang', 'fields' => array('name' => array('type' => self::TYPE_STRING, 'validate' => 'isGenericName', 'required' => true, 'size' => 32), 'iso_code' => array('type' => self::TYPE_STRING, 'validate' => 'isLanguageIsoCode', 'required' => true, 'size' => 2), 'language_code' => array('type' => self::TYPE_STRING, 'validate' => 'isLanguageCode', 'size' => 5), 'active' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'is_rtl' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'date_format_lite' => array('type' => self::TYPE_STRING, 'validate' => 'isPhpDateFormat', 'required' => true, 'size' => 32), 'date_format_full' => array('type' => self::TYPE_STRING, 'validate' => 'isPhpDateFormat', 'required' => true, 'size' => 32)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Language.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L55).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/Language.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L29).


### <a name="property-$is_rtl"></a>$is_rtl

```php
public boolean $is_rtl = false
```





* Visibility: **public**
* Source: [classes/Language.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L47).


### <a name="property-$iso_code"></a>$iso_code

```php
public string $iso_code
```





* Visibility: **public**
* Source: [classes/Language.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L35).


### <a name="property-$language_code"></a>$language_code

```php
public string $language_code
```





* Visibility: **public**
* Source: [classes/Language.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L38).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Language.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L32).


### <a name="property-$translationsFilesAndVars"></a>$translationsFilesAndVars

```php
protected mixed $translationsFilesAndVars = array('fields' => '_FIELDS', 'errors' => '_ERRORS', 'admin' => '_LANGADM', 'pdf' => '_LANGPDF', 'tabs' => 'tabs')
```





* Visibility: **protected**
* Source: [classes/Language.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L80).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectNodeName' => 'language', 'objectsNodeName' => 'languages')
```





* Visibility: **protected**
* Source: [classes/Language.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L75).


### <a name="property-$cache_objects"></a>$cache_objects

```php
protected boolean $cache_objects = true
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L153).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 143](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L143).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L133).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L106).


### <a name="property-$force_id"></a>$force_id

```php
public \boolean, $force_id = false
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L148).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L64).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L58).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L60).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L120).


### <a name="property-$loaded_classes"></a>$loaded_classes

```php
protected mixed $loaded_classes = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 128](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L128).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 138](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L138).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed LanguageCore::__construct($id, $id_lang)
```





* Visibility: **public**
* Source: [classes/Language.php line 88](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L88)


#### Arguments
* $id **mixed**
* $id_lang **mixed**



### <a name="method-_copyNoneFlag"></a>_copyNoneFlag

```php
mixed LanguageCore::_copyNoneFlag($id)
```





* Visibility: **protected**
* This method is **static**.
* Source: [classes/Language.php line 797](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L797)


#### Arguments
* $id **mixed**



### <a name="method-_generateFiles"></a>_generateFiles

```php
mixed LanguageCore::_generateFiles($newIso)
```

Generate translations files



* Visibility: **protected**
* Source: [classes/Language.php line 110](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L110)


#### Arguments
* $newIso **mixed**



### <a name="method-_getThemesList"></a>_getThemesList

```php
\array([theme LanguageCore::_getThemesList()
```

Return an array of theme



* Visibility: **protected**
* Source: [classes/Language.php line 184](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L184)




### <a name="method-add"></a>add

```php
mixed LanguageCore::add($autodate, $nullValues, $only_add)
```





* Visibility: **public**
* Source: [classes/Language.php line 199](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L199)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**
* $only_add **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1244](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1244)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1302](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1302)


#### Arguments
* $id_shops **integer|array**



### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1231](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1231)


#### Arguments
* $all **mixed**



### <a name="method-checkAndAddLanguage"></a>checkAndAddLanguage

```php
mixed LanguageCore::checkAndAddLanguage($iso_code, $lang_pack, $only_add, $params_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 729](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L729)


#### Arguments
* $iso_code **mixed**
* $lang_pack **mixed**
* $only_add **mixed**
* $params_lang **mixed**



### <a name="method-checkFiles"></a>checkFiles

```php
mixed LanguageCore::checkFiles()
```





* Visibility: **public**
* Source: [classes/Language.php line 224](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L224)




### <a name="method-checkFilesWithIsoCode"></a>checkFilesWithIsoCode

```php
mixed LanguageCore::checkFilesWithIsoCode(mixed $iso_code)
```

This functions checks if every files exists for the language $iso_code.

Concerned files are those located in translations/$iso_code/
and translations/mails/$iso_code .

* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 238](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L238)


#### Arguments
* $iso_code **mixed**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1258](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1258)


#### Arguments
* $all **mixed**



### <a name="method-copyLanguageData"></a>copyLanguageData

```php
mixed LanguageCore::copyLanguageData($from, $to)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 676](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L676)


#### Arguments
* $from **mixed**
* $to **mixed**



### <a name="method-countActiveLanguages"></a>countActiveLanguages

```php
mixed LanguageCore::countActiveLanguages($id_shop)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 815](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L815)


#### Arguments
* $id_shop **mixed**



### <a name="method-delete"></a>delete

```php
mixed LanguageCore::delete()
```





* Visibility: **public**
* Source: [classes/Language.php line 484](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L484)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1433](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1433)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
mixed LanguageCore::deleteSelection($selection)
```





* Visibility: **public**
* Source: [classes/Language.php line 557](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L557)


#### Arguments
* $selection **mixed**



### <a name="method-disableCache"></a>disableCache

```php
mixed ObjectModelCore::disableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1719](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1719)




### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1014](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1014)


#### Arguments
* $field **mixed**
* $class **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-downloadAndInstallLanguagePack"></a>downloadAndInstallLanguagePack

```php
mixed LanguageCore::downloadAndInstallLanguagePack($iso, $version, $params, $install)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 829](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L829)


#### Arguments
* $iso **mixed**
* $version **mixed**
* $params **mixed**
* $install **mixed**



### <a name="method-duplicateObject"></a>duplicateObject

```php
\new ObjectModelCore::duplicateObject()
```

Duplicate current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 549](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L549)




### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1346](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1346)


#### Arguments
* $id **mixed**



### <a name="method-enableCache"></a>enableCache

```php
mixed ObjectModelCore::enableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1714](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1714)




### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1470](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1470)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 348](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L348)


#### Arguments
* $type **integer** - FORMAT_COMMON or FORMAT_LANG or FORMAT_SHOP
* $id_lang **integer** - If this parameter is given, only take lang fields



### <a name="method-formatValue"></a>formatValue

```php
mixed ObjectModelCore::formatValue(mixed $value, integer $type, $with_quotes, $purify)
```

Format a data



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 395](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L395)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**
* $purify **mixed**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1331](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1331)




### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1576](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1576)


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
* Source: [classes/ObjectModel.php line 1683](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1683)


#### Arguments
* $field_name **mixed**
* $id_lang **null**



### <a name="method-getFields"></a>getFields

```php
array LanguageCore::getFields()
```





* Visibility: **public**
* Source: [classes/Language.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L97)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 313](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L313)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1223](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1223)


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
* Source: [classes/ObjectModel.php line 299](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L299)




### <a name="method-getFilesList"></a>getFilesList

```php
mixed LanguageCore::getFilesList($iso_from, $theme_from, $iso_to, $theme_to, $select, $check, $modules)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 250](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L250)


#### Arguments
* $iso_from **mixed**
* $theme_from **mixed**
* $iso_to **mixed**
* $theme_to **mixed**
* $select **mixed**
* $check **mixed**
* $modules **mixed**



### <a name="method-getIdByIso"></a>getIdByIso

```php
integer LanguageCore::getIdByIso(string $iso_code)
```

Return id from iso code



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 619](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L619)


#### Arguments
* $iso_code **string** - Iso code



### <a name="method-getIsoById"></a>getIsoById

```php
string LanguageCore::getIsoById(integer $id_lang)
```

Return iso code from id



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 606](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L606)


#### Arguments
* $id_lang **integer** - Language ID



### <a name="method-getIsoIds"></a>getIsoIds

```php
array LanguageCore::getIsoIds($active)
```

Return array (id_lang, iso_code)



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 671](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L671)


#### Arguments
* $active **mixed**



### <a name="method-getLanguage"></a>getLanguage

```php
mixed LanguageCore::getLanguage($id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 593](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L593)


#### Arguments
* $id_lang **mixed**



### <a name="method-getLanguageByIETFCode"></a>getLanguageByIETFCode

```php
mixed LanguageCore::getLanguageByIETFCode($code)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 635](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L635)


#### Arguments
* $code **mixed**



### <a name="method-getLanguageCodeByIso"></a>getLanguageCodeByIso

```php
mixed LanguageCore::getLanguageCodeByIso($iso_code)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 627](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L627)


#### Arguments
* $iso_code **mixed**



### <a name="method-getLanguagePackListContent"></a>getLanguagePackListContent

```php
mixed LanguageCore::getLanguagePackListContent($iso, $tar)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 928](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L928)


#### Arguments
* $iso **mixed**
* $tar **mixed**



### <a name="method-getLanguages"></a>getLanguages

```php
array LanguageCore::getLanguages(boolean $active, $id_shop)
```

Return available languages



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 578](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L578)


#### Arguments
* $active **boolean** - Select only active languages
* $id_shop **mixed**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 804](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L804)


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
* Source: [classes/ObjectModel.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L161)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1164](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1164)


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
* Source: [classes/ObjectModel.php line 1086](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1086)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1371)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1508](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1508)


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
* Source: [classes/ObjectModel.php line 1527](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1527)


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
* Source: [classes/ObjectModel.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1273)


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
* Source: [classes/ObjectModel.php line 1488](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1488)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isInstalled"></a>isInstalled

```php
mixed LanguageCore::isInstalled($iso_code)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 803](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L803)


#### Arguments
* $iso_code **mixed**



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1388](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1388)




### <a name="method-isMultiLanguageActivated"></a>isMultiLanguageActivated

```php
boolean LanguageCore::isMultiLanguageActivated($id_shop)
```

Check if more on than one language is activated



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 923](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L923)


#### Arguments
* $id_shop **mixed**



### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1383](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1383)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1378](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1378)




### <a name="method-loadLanguages"></a>loadLanguages

```php
mixed LanguageCore::loadLanguages()
```

Load all languages in memory for caching



* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 704](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L704)




### <a name="method-loadUpdateSQL"></a>loadUpdateSQL

```php
boolean LanguageCore::loadUpdateSQL()
```

loadUpdateSQL will create default lang values when you create a new lang, based on default id lang



* Visibility: **public**
* Source: [classes/Language.php line 397](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L397)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 820](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L820)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-moveToIso"></a>moveToIso

```php
mixed LanguageCore::moveToIso($newIso)
```

Move translations files after editing language iso code



* Visibility: **public**
* Source: [classes/Language.php line 142](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L142)


#### Arguments
* $newIso **mixed**



### <a name="method-recurseDeleteDir"></a>recurseDeleteDir

```php
mixed LanguageCore::recurseDeleteDir($dir)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 464](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L464)


#### Arguments
* $dir **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 446](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L446)


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
* Source: [classes/ObjectModel.php line 1614](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1614)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1709](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1709)


#### Arguments
* $fields **array**



### <a name="method-toggleStatus"></a>toggleStatus

```php
mixed LanguageCore::toggleStatus()
```





* Visibility: **public**
* Source: [classes/Language.php line 216](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L216)




### <a name="method-update"></a>update

```php
mixed LanguageCore::update($nullValues)
```





* Visibility: **public**
* Source: [classes/Language.php line 721](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L721)


#### Arguments
* $nullValues **mixed**



### <a name="method-updateModulesTranslations"></a>updateModulesTranslations

```php
mixed LanguageCore::updateModulesTranslations(array $modules_list)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Language.php line 940](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/Language.php#L940)


#### Arguments
* $modules_list **array**



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1403](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1403)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1032](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1032)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1038](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1038)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang, $skip, $human_errors)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 931](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L931)


#### Arguments
* $field **string** - Field name
* $value **mixed** - Field value
* $id_lang **integer**
* $skip **mixed**
* $human_errors **mixed**



### <a name="method-validateFields"></a>validateFields

```php
boolean|string ObjectModelCore::validateFields(boolean $die, boolean $error_return)
```

Check for fields validity before database interaction



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 858](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L858)


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
* Source: [classes/ObjectModel.php line 887](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L887)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1200](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.13/classes/ObjectModel.php#L1200)


#### Arguments
* $htmlentities **mixed**


