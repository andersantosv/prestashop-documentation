Class CMSCore
=====================





* Class name: CMSCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/CMS.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L28)


Contents
--------


### Properties

* [$active](#property-$active)
* [$content](#property-$content)
* [$definition](#property-$definition)
* [$id_cms_category](#property-$id_cms_category)
* [$link_rewrite](#property-$link_rewrite)
* [$meta_description](#property-$meta_description)
* [$meta_keywords](#property-$meta_keywords)
* [$meta_title](#property-$meta_title)
* [$position](#property-$position)
* [$webserviceParameters](#property-$webserviceParameters)
* [$def](#property-$def)
* [$fieldsRequired](#property-$fieldsRequired)
* [$fieldsRequiredDatabase](#property-$fieldsRequiredDatabase)
* [$fieldsRequiredLang](#property-$fieldsRequiredLang)
* [$fieldsSize](#property-$fieldsSize)
* [$fieldsSizeLang](#property-$fieldsSizeLang)
* [$fieldsValidate](#property-$fieldsValidate)
* [$fieldsValidateLang](#property-$fieldsValidateLang)
* [$id](#property-$id)
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
* [associateTo](#method-associateTo)
* [cleanPositions](#method-cleanPositions)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getCMSPages](#method-getCMSPages)
* [getDefinition](#method-getDefinition)
* [getEntity](#method-getEntity)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getLastPosition](#method-getLastPosition)
* [getLinks](#method-getLinks)
* [getTranslationsFields](#method-getTranslationsFields)
* [getUrlRewriteInformations](#method-getUrlRewriteInformations)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToGroupShop](#method-isAssociatedToGroupShop)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [listCms](#method-listCms)
* [makeTranslationFields](#method-makeTranslationFields)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updatePosition](#method-updatePosition)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)




Properties
----------


### <a name="property-$active"></a>$active

```php
public mixed $active
```





* Visibility: **public**
* Source: [classes/CMS.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L38).


### <a name="property-$content"></a>$content

```php
public mixed $content
```





* Visibility: **public**
* Source: [classes/CMS.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L34).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'cms', 'primary' => 'id_cms', 'multilang' => true, 'fields' => array('id_cms_category' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'position' => array('type' => self::TYPE_INT), 'active' => array('type' => self::TYPE_BOOL), 'meta_description' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'size' => 255), 'meta_keywords' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'size' => 255), 'meta_title' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 128), 'link_rewrite' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isLinkRewrite', 'required' => true, 'size' => 128), 'content' => array('type' => self::TYPE_HTML, 'lang' => true, 'validate' => 'isString', 'size' => 3999999999999.0)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/CMS.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L43).


### <a name="property-$id_cms_category"></a>$id_cms_category

```php
public mixed $id_cms_category
```





* Visibility: **public**
* Source: [classes/CMS.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L36).


### <a name="property-$link_rewrite"></a>$link_rewrite

```php
public mixed $link_rewrite
```





* Visibility: **public**
* Source: [classes/CMS.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L35).


### <a name="property-$meta_description"></a>$meta_description

```php
public mixed $meta_description
```





* Visibility: **public**
* Source: [classes/CMS.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L32).


### <a name="property-$meta_keywords"></a>$meta_keywords

```php
public mixed $meta_keywords
```





* Visibility: **public**
* Source: [classes/CMS.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L33).


### <a name="property-$meta_title"></a>$meta_title

```php
public string $meta_title
```





* Visibility: **public**
* Source: [classes/CMS.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L31).


### <a name="property-$position"></a>$position

```php
public mixed $position
```





* Visibility: **public**
* Source: [classes/CMS.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L37).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectNodeName' => 'content', 'objectsNodeName' => 'content_management_system')
```





* Visibility: **protected**
* Source: [classes/CMS.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L61).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 122](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L122).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L72).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L57).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L87).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L77).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L92).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L82).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L97).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L48).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L51).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 53](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L53).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L67).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L108).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L111).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L62).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 102](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L102).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 150](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L150)


#### Arguments
* $id **integer** - Existing object id in order to load object (optional)
* $id_lang **integer** - Required if object is multilingual (optional)
* $id_shop **integer** - ID shop for objects with multishop on langs



### <a name="method-add"></a>add

```php
mixed CMSCore::add($autodate, $nullValues)
```





* Visibility: **public**
* Source: [classes/CMS.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L66)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 961](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L961)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops, string $type)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1009](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1009)


#### Arguments
* $id_shops **integer|array**
* $type **string**



### <a name="method-cleanPositions"></a>cleanPositions

```php
mixed CMSCore::cleanPositions($id_category)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L161)


#### Arguments
* $id_category **mixed**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 975](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L975)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
mixed CMSCore::delete()
```





* Visibility: **public**
* Source: [classes/CMS.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L79)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage()
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1079](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1079)




### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 553](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L553)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $className, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 740](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L740)


#### Arguments
* $field **mixed**
* $className **mixed**
* $htmlentities **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1049](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1049)


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
* Source: [classes/ObjectModel.php line 1113](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1113)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 272](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L272)


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
* Source: [classes/ObjectModel.php line 319](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L319)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**



### <a name="method-getCMSPages"></a>getCMSPages

```php
mixed CMSCore::getCMSPages($id_lang, $id_cms_category, $active)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L184)


#### Arguments
* $id_lang **mixed**
* $id_cms_category **mixed**
* $active **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
mixed ObjectModelCore::getDefinition($class, $field)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1209](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1209)


#### Arguments
* $class **mixed**
* $field **mixed**



### <a name="method-getEntity"></a>getEntity

```php
mixed ObjectModelCore::getEntity($entity)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1269](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1269)


#### Arguments
* $entity **mixed**



### <a name="method-getFields"></a>getFields

```php
array ObjectModelCore::getFields()
```

Prepare fields for ObjectModel class (add, update)
All fields are verified (pSQL, intval.

..)

* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 234](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L234)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L249)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 953](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L953)


#### Arguments
* $all **mixed**



### <a name="method-getLastPosition"></a>getLastPosition

```php
mixed CMSCore::getLastPosition($id_category)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 179](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L179)


#### Arguments
* $id_category **mixed**



### <a name="method-getLinks"></a>getLinks

```php
mixed CMSCore::getLinks($id_lang, $selection, $active, \Link $link)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L86)


#### Arguments
* $id_lang **mixed**
* $selection **mixed**
* $active **mixed**
* $link **[Link](class.LinkCore.md)**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fieldsArray)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 589](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L589)


#### Arguments
* $fieldsArray **mixed**



### <a name="method-getUrlRewriteInformations"></a>getUrlRewriteInformations

```php
mixed CMSCore::getUrlRewriteInformations($id_cms)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 199](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L199)


#### Arguments
* $id_cms **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $className)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L130)


#### Arguments
* $className **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 929](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L929)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWebserviceParameters"></a>getWebserviceParameters

```php
mixed ObjectModelCore::getWebserviceParameters($wsParamsAttributeName)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 799](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L799)


#### Arguments
* $wsParamsAttributeName **mixed**



### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1148](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1148)


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
* Source: [classes/ObjectModel.php line 1167](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1167)


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
* Source: [classes/ObjectModel.php line 1035](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1035)


#### Arguments
* $id_group_shop **integer**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 990](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L990)


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
* Source: [classes/ObjectModel.php line 1131](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1131)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1069](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1069)




### <a name="method-listCms"></a>listCms

```php
mixed CMSCore::listCms($id_lang, $id_block, $active)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/CMS.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L111)


#### Arguments
* $id_lang **mixed**
* $id_block **mixed**
* $active **mixed**



### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fieldsArray, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 605](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L605)


#### Arguments
* $fields **mixed**
* $fieldsArray **mixed**
* $id_language **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 360](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L360)


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
* Source: [classes/ObjectModel.php line 1224](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L1224)




### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 569](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L569)




### <a name="method-update"></a>update

```php
mixed CMSCore::update($nullValues)
```





* Visibility: **public**
* Source: [classes/CMS.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L72)


#### Arguments
* $nullValues **mixed**



### <a name="method-updatePosition"></a>updatePosition

```php
mixed CMSCore::updatePosition($way, $position)
```





* Visibility: **public**
* Source: [classes/CMS.php line 127](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/CMS.php#L127)


#### Arguments
* $way **mixed**
* $position **mixed**



### <a name="method-validateControler"></a>validateControler

```php
mixed ObjectModelCore::validateControler($htmlentities)
```

TODO: refactor rename all calls to this to validateController



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 753](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L753)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 759](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L759)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 704](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L704)


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
* Source: [classes/ObjectModel.php line 643](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L643)


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
* Source: [classes/ObjectModel.php line 669](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.3/classes/ObjectModel.php#L669)


#### Arguments
* $die **boolean**
* $error_return **boolean**


