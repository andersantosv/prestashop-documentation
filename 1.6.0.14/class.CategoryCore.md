Class CategoryCore
=====================





* Class name: CategoryCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Category.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L27)


Contents
--------


### Properties

* [$_links](#property-$_links)
* [$active](#property-$active)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$definition](#property-$definition)
* [$description](#property-$description)
* [$groupBox](#property-$groupBox)
* [$id](#property-$id)
* [$id_category](#property-$id_category)
* [$id_category_default](#property-$id_category_default)
* [$id_image](#property-$id_image)
* [$id_parent](#property-$id_parent)
* [$id_shop_default](#property-$id_shop_default)
* [$is_root_category](#property-$is_root_category)
* [$level_depth](#property-$level_depth)
* [$link_rewrite](#property-$link_rewrite)
* [$meta_description](#property-$meta_description)
* [$meta_keywords](#property-$meta_keywords)
* [$meta_title](#property-$meta_title)
* [$name](#property-$name)
* [$nleft](#property-$nleft)
* [$nright](#property-$nright)
* [$position](#property-$position)
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
* [_subTree](#method-_subTree)
* [add](#method-add)
* [addFieldsRequiredDatabase](#method-addFieldsRequiredDatabase)
* [addGroups](#method-addGroups)
* [addGroupsIfNoExist](#method-addGroupsIfNoExist)
* [addPosition](#method-addPosition)
* [addShop](#method-addShop)
* [addToShop](#method-addToShop)
* [associateTo](#method-associateTo)
* [cacheFieldsRequiredDatabase](#method-cacheFieldsRequiredDatabase)
* [calcLevelDepth](#method-calcLevelDepth)
* [categoryExists](#method-categoryExists)
* [checkAccess](#method-checkAccess)
* [checkBeforeMove](#method-checkBeforeMove)
* [cleanAssoProducts](#method-cleanAssoProducts)
* [cleanGroups](#method-cleanGroups)
* [cleanPositions](#method-cleanPositions)
* [clearCache](#method-clearCache)
* [delete](#method-delete)
* [deleteCategoriesFromShop](#method-deleteCategoriesFromShop)
* [deleteFromShop](#method-deleteFromShop)
* [deleteImage](#method-deleteImage)
* [deleteLite](#method-deleteLite)
* [deleteSelection](#method-deleteSelection)
* [disableCache](#method-disableCache)
* [displayFieldName](#method-displayFieldName)
* [duplicateObject](#method-duplicateObject)
* [duplicateProductCategories](#method-duplicateProductCategories)
* [duplicateShops](#method-duplicateShops)
* [enableCache](#method-enableCache)
* [existsInDatabase](#method-existsInDatabase)
* [existsInShop](#method-existsInShop)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAllChildren](#method-getAllChildren)
* [getAllParents](#method-getAllParents)
* [getAssociatedShops](#method-getAssociatedShops)
* [getCategories](#method-getCategories)
* [getCategoriesWithoutParent](#method-getCategoriesWithoutParent)
* [getCategoryInformations](#method-getCategoryInformations)
* [getChildren](#method-getChildren)
* [getChildrenWithNbSelectedSubCat](#method-getChildrenWithNbSelectedSubCat)
* [getChildrenWs](#method-getChildrenWs)
* [getDefinition](#method-getDefinition)
* [getDescriptionClean](#method-getDescriptionClean)
* [getDuplicatePosition](#method-getDuplicatePosition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getGroups](#method-getGroups)
* [getHomeCategories](#method-getHomeCategories)
* [getInterval](#method-getInterval)
* [getLastPosition](#method-getLastPosition)
* [getLink](#method-getLink)
* [getLinkRewrite](#method-getLinkRewrite)
* [getName](#method-getName)
* [getNestedCategories](#method-getNestedCategories)
* [getParentsCategories](#method-getParentsCategories)
* [getProducts](#method-getProducts)
* [getProductsWs](#method-getProductsWs)
* [getRootCategories](#method-getRootCategories)
* [getRootCategory](#method-getRootCategory)
* [getShopID](#method-getShopID)
* [getShopsByCategory](#method-getShopsByCategory)
* [getSimpleCategories](#method-getSimpleCategories)
* [getSubCategories](#method-getSubCategories)
* [getTopCategory](#method-getTopCategory)
* [getTranslationsFields](#method-getTranslationsFields)
* [getUrlRewriteInformations](#method-getUrlRewriteInformations)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [getWsNbProductsRecursive](#method-getWsNbProductsRecursive)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [inShop](#method-inShop)
* [inShopStatic](#method-inShopStatic)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isMultiShopField](#method-isMultiShopField)
* [isMultishop](#method-isMultishop)
* [isParentCategoryAvailable](#method-isParentCategoryAvailable)
* [isRootCategoryForAShop](#method-isRootCategoryForAShop)
* [makeTranslationFields](#method-makeTranslationFields)
* [recalculateLevelDepth](#method-recalculateLevelDepth)
* [recurseCategory](#method-recurseCategory)
* [recurseLiteCategTree](#method-recurseLiteCategTree)
* [recursiveDelete](#method-recursiveDelete)
* [regenerateEntireNtree](#method-regenerateEntireNtree)
* [save](#method-save)
* [searchByName](#method-searchByName)
* [searchByNameAndParentCategoryId](#method-searchByNameAndParentCategoryId)
* [searchByPath](#method-searchByPath)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [setNewGroupForHome](#method-setNewGroupForHome)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateFromShop](#method-updateFromShop)
* [updateGroup](#method-updateGroup)
* [updateMultishopTable](#method-updateMultishopTable)
* [updatePosition](#method-updatePosition)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)




Properties
----------


### <a name="property-$_links"></a>$_links

```php
protected mixed $_links = array()
```





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Category.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L87).


### <a name="property-$active"></a>$active

```php
public boolean $active = 1
```





* Visibility: **public**
* Source: [classes/Category.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L38).


### <a name="property-$date_add"></a>$date_add

```php
public string $date_add
```





* Visibility: **public**
* Source: [classes/Category.php line 74](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L74).


### <a name="property-$date_upd"></a>$date_upd

```php
public string $date_upd
```





* Visibility: **public**
* Source: [classes/Category.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L77).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'category', 'primary' => 'id_category', 'multilang' => true, 'multilang_shop' => true, 'fields' => array('nleft' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'nright' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'level_depth' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'active' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool', 'required' => true), 'id_parent' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'), 'id_shop_default' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'is_root_category' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'position' => array('type' => self::TYPE_INT), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isCatalogName', 'required' => true, 'size' => 128), 'link_rewrite' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isLinkRewrite', 'required' => true, 'size' => 128), 'description' => array('type' => self::TYPE_HTML, 'lang' => true, 'validate' => 'isCleanHtml'), 'meta_title' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'size' => 128), 'meta_description' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'size' => 255), 'meta_keywords' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'size' => 255)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/Category.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L92).


### <a name="property-$description"></a>$description

```php
public string $description
```





* Visibility: **public**
* Source: [classes/Category.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L44).


### <a name="property-$groupBox"></a>$groupBox

```php
public mixed $groupBox
```





* Visibility: **public**
* Source: [classes/Category.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L85).


### <a name="property-$id"></a>$id

```php
public mixed $id
```





* Visibility: **public**
* Source: [classes/Category.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L29).


### <a name="property-$id_category"></a>$id_category

```php
public integer $id_category
```





* Visibility: **public**
* Source: [classes/Category.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L32).


### <a name="property-$id_category_default"></a>$id_category_default

```php
public integer $id_category_default
```





* Visibility: **public**
* Source: [classes/Category.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L50).


### <a name="property-$id_image"></a>$id_image

```php
public string $id_image = 'default'
```





* Visibility: **public**
* Source: [classes/Category.php line 119](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L119).


### <a name="property-$id_parent"></a>$id_parent

```php
public integer $id_parent
```





* Visibility: **public**
* Source: [classes/Category.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L47).


### <a name="property-$id_shop_default"></a>$id_shop_default

```php
public integer $id_shop_default
```





* Visibility: **public**
* Source: [classes/Category.php line 83](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L83).


### <a name="property-$is_root_category"></a>$is_root_category

```php
public boolean $is_root_category
```





* Visibility: **public**
* Source: [classes/Category.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L80).


### <a name="property-$level_depth"></a>$level_depth

```php
public integer $level_depth
```





* Visibility: **public**
* Source: [classes/Category.php line 53](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L53).


### <a name="property-$link_rewrite"></a>$link_rewrite

```php
public string $link_rewrite
```





* Visibility: **public**
* Source: [classes/Category.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L62).


### <a name="property-$meta_description"></a>$meta_description

```php
public string $meta_description
```





* Visibility: **public**
* Source: [classes/Category.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L71).


### <a name="property-$meta_keywords"></a>$meta_keywords

```php
public string $meta_keywords
```





* Visibility: **public**
* Source: [classes/Category.php line 68](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L68).


### <a name="property-$meta_title"></a>$meta_title

```php
public string $meta_title
```





* Visibility: **public**
* Source: [classes/Category.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L65).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* Source: [classes/Category.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L35).


### <a name="property-$nleft"></a>$nleft

```php
public integer $nleft
```





* Visibility: **public**
* Source: [classes/Category.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L56).


### <a name="property-$nright"></a>$nright

```php
public integer $nright
```





* Visibility: **public**
* Source: [classes/Category.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L59).


### <a name="property-$position"></a>$position

```php
public integer $position
```





* Visibility: **public**
* Source: [classes/Category.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L41).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected mixed $webserviceParameters = array('objectsNodeName' => 'categories', 'hidden_fields' => array('nleft', 'nright', 'groupBox'), 'fields' => array('id_parent' => array('xlink_resource' => 'categories'), 'level_depth' => array('setter' => false), 'nb_products_recursive' => array('getter' => 'getWsNbProductsRecursive', 'setter' => false)), 'associations' => array('categories' => array('getter' => 'getChildrenWs', 'resource' => 'category'), 'products' => array('getter' => 'getProductsWs', 'resource' => 'product')))
```





* Visibility: **protected**
* Source: [classes/Category.php line 121](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L121).


### <a name="property-$cache_objects"></a>$cache_objects

```php
protected boolean $cache_objects = true
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L153).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 143](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L143).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L133).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L106).


### <a name="property-$force_id"></a>$force_id

```php
public \boolean, $force_id = false
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L148).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L64).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L58).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L60).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L120).


### <a name="property-$loaded_classes"></a>$loaded_classes

```php
protected mixed $loaded_classes = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 128](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L128).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 138](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L138).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed CategoryCore::__construct($id_category, $id_lang, $id_shop)
```





* Visibility: **public**
* Source: [classes/Category.php line 135](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L135)


#### Arguments
* $id_category **mixed**
* $id_lang **mixed**
* $id_shop **mixed**



### <a name="method-_subTree"></a>_subTree

```php
mixed CategoryCore::_subTree($categories, $id_category, $n)
```





* Visibility: **protected**
* This method is **static**.
* Source: [classes/Category.php line 407](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L407)


#### Arguments
* $categories **mixed**
* $id_category **mixed**
* $n **mixed**



### <a name="method-add"></a>add

```php
mixed CategoryCore::add($autodate, $null_values)
```





* Visibility: **public**
* Source: [classes/Category.php line 147](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L147)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1244](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1244)


#### Arguments
* $fields **mixed**



### <a name="method-addGroups"></a>addGroups

```php
mixed CategoryCore::addGroups($groups)
```





* Visibility: **public**
* Source: [classes/Category.php line 1106](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1106)


#### Arguments
* $groups **mixed**



### <a name="method-addGroupsIfNoExist"></a>addGroupsIfNoExist

```php
mixed CategoryCore::addGroupsIfNoExist($id_group)
```





* Visibility: **public**
* Source: [classes/Category.php line 1130](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1130)


#### Arguments
* $id_group **mixed**



### <a name="method-addPosition"></a>addPosition

```php
mixed CategoryCore::addPosition($position, $id_shop)
```





* Visibility: **public**
* Source: [classes/Category.php line 1519](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1519)


#### Arguments
* $position **mixed**
* $id_shop **mixed**



### <a name="method-addShop"></a>addShop

```php
boolean CategoryCore::addShop(integer $id_shop)
```

Add association between shop and categories



* Visibility: **public**
* Source: [classes/Category.php line 1441](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1441)


#### Arguments
* $id_shop **integer**



### <a name="method-addToShop"></a>addToShop

```php
boolean CategoryCore::addToShop(array $categories, $id_shop)
```

Add some categories to a shop



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1605](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1605)


#### Arguments
* $categories **array**
* $id_shop **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1302](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1302)


#### Arguments
* $id_shops **integer|array**



### <a name="method-cacheFieldsRequiredDatabase"></a>cacheFieldsRequiredDatabase

```php
mixed ObjectModelCore::cacheFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1231](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1231)


#### Arguments
* $all **mixed**



### <a name="method-calcLevelDepth"></a>calcLevelDepth

```php
integer CategoryCore::calcLevelDepth()
```

Get the depth level for the category



* Visibility: **public**
* Source: [classes/Category.php line 373](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L373)




### <a name="method-categoryExists"></a>categoryExists

```php
boolean CategoryCore::categoryExists(integer $id_category)
```

Specify if a category already in base



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1086](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1086)


#### Arguments
* $id_category **integer** - Category id



### <a name="method-checkAccess"></a>checkAccess

```php
boolean CategoryCore::checkAccess(mixed $id_customer)
```

checkAccess return true if id_customer is in a group allowed to see this category.



* Visibility: **public**
* Source: [classes/Category.php line 1145](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1145)


#### Arguments
* $id_customer **mixed**



### <a name="method-checkBeforeMove"></a>checkBeforeMove

```php
boolean CategoryCore::checkBeforeMove(integer $id_category, integer $id_parent)
```

Check if category can be moved in another one.

The category cannot be moved in a child category.

* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 896](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L896)


#### Arguments
* $id_category **integer** - current category
* $id_parent **integer** - Parent candidate



### <a name="method-cleanAssoProducts"></a>cleanAssoProducts

```php
mixed CategoryCore::cleanAssoProducts()
```





* Visibility: **public**
* Source: [classes/Category.php line 1101](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1101)




### <a name="method-cleanGroups"></a>cleanGroups

```php
mixed CategoryCore::cleanGroups()
```





* Visibility: **public**
* Source: [classes/Category.php line 1096](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1096)




### <a name="method-cleanPositions"></a>cleanPositions

```php
boolean CategoryCore::cleanPositions(mixed $id_category_parent)
```

cleanPositions keep order of category in $id_category_parent,
but remove duplicate position. Should not be used if positions
are clean at the beginning !



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1234](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1234)


#### Arguments
* $id_category_parent **mixed**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1258](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1258)


#### Arguments
* $all **mixed**



### <a name="method-delete"></a>delete

```php
mixed CategoryCore::delete()
```





* Visibility: **public**
* Source: [classes/Category.php line 314](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L314)




### <a name="method-deleteCategoriesFromShop"></a>deleteCategoriesFromShop

```php
boolean CategoryCore::deleteCategoriesFromShop($id_shop)
```

Delete every categories



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1595](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1595)


#### Arguments
* $id_shop **mixed**



### <a name="method-deleteFromShop"></a>deleteFromShop

```php
boolean CategoryCore::deleteFromShop(integer $id_shop)
```

Delete category from shop $id_shop



* Visibility: **public**
* Source: [classes/Category.php line 1583](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1583)


#### Arguments
* $id_shop **integer**



### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1433](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1433)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteLite"></a>deleteLite

```php
mixed CategoryCore::deleteLite()
```





* Visibility: **public**
* Source: [classes/Category.php line 308](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L308)




### <a name="method-deleteSelection"></a>deleteSelection

```php
mixed CategoryCore::deleteSelection($categories)
```

Delete several categories from database

return boolean Deletion result

* Visibility: **public**
* Source: [classes/Category.php line 354](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L354)


#### Arguments
* $categories **mixed**



### <a name="method-disableCache"></a>disableCache

```php
mixed ObjectModelCore::disableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1719](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1719)




### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1014](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1014)


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
* Source: [classes/ObjectModel.php line 549](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L549)




### <a name="method-duplicateProductCategories"></a>duplicateProductCategories

```php
boolean CategoryCore::duplicateProductCategories(integer $id_old, boolean $id_new)
```

Copy products from a category to another



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 865](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L865)


#### Arguments
* $id_old **integer** - Source category ID
* $id_new **boolean** - Destination category ID



### <a name="method-duplicateShops"></a>duplicateShops

```php
mixed ObjectModelCore::duplicateShops($id)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1346](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1346)


#### Arguments
* $id **mixed**



### <a name="method-enableCache"></a>enableCache

```php
mixed ObjectModelCore::enableCache()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1714](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1714)




### <a name="method-existsInDatabase"></a>existsInDatabase

```php
boolean ObjectModelCore::existsInDatabase(integer $id_entity, string $table)
```

Specify if an ObjectModel is already in database



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1470](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1470)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-existsInShop"></a>existsInShop

```php
mixed CategoryCore::existsInShop($id_shop)
```





* Visibility: **public**
* Source: [classes/Category.php line 1627](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1627)


#### Arguments
* $id_shop **mixed**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 348](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L348)


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
* Source: [classes/ObjectModel.php line 395](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L395)


#### Arguments
* $value **mixed**
* $type **integer**
* $with_quotes **mixed**
* $purify **mixed**



### <a name="method-getAllChildren"></a>getAllChildren

```php
\PrestaShopCollection CategoryCore::getAllChildren(integer $id_lang)
```

Return an array of all children of the current category



* Visibility: **public**
* Source: [classes/Category.php line 788](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L788)


#### Arguments
* $id_lang **integer**



### <a name="method-getAllParents"></a>getAllParents

```php
\PrestaShopCollection CategoryCore::getAllParents(integer $id_lang)
```

Return an array of all parents of the current category



* Visibility: **public**
* Source: [classes/Category.php line 805](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L805)


#### Arguments
* $id_lang **integer**



### <a name="method-getAssociatedShops"></a>getAssociatedShops

```php
array ObjectModelCore::getAssociatedShops()
```

Get the list of associated id_shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1331](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1331)




### <a name="method-getCategories"></a>getCategories

```php
array CategoryCore::getCategories(integer $id_lang, boolean $active, $order, $sql_filter, $sql_sort, $sql_limit)
```

Return available categories



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 459](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L459)


#### Arguments
* $id_lang **integer** - Language ID
* $active **boolean** - return only active categories
* $order **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getCategoriesWithoutParent"></a>getCategoriesWithoutParent

```php
mixed CategoryCore::getCategoriesWithoutParent()
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1475](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1475)




### <a name="method-getCategoryInformations"></a>getCategoryInformations

```php
Array CategoryCore::getCategoryInformations(Array $ids_category, integer $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1397](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1397)


#### Arguments
* $ids_category **Array**
* $id_lang **integer**



### <a name="method-getChildren"></a>getChildren

```php
array CategoryCore::getChildren(integer $id_parent, integer $id_lang, boolean $active, $id_shop)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 759](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L759)


#### Arguments
* $id_parent **integer**
* $id_lang **integer**
* $active **boolean**
* $id_shop **mixed**



### <a name="method-getChildrenWithNbSelectedSubCat"></a>getChildrenWithNbSelectedSubCat

```php
array CategoryCore::getChildrenWithNbSelectedSubCat(integer $id_parent, $selected_cat, integer $id_lang, \Shop $shop, $use_shop_context)
```

This method allow to return children categories with the number of sub children selected for a product



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 824](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L824)


#### Arguments
* $id_parent **integer**
* $selected_cat **mixed**
* $id_lang **integer**
* $shop **[Shop](class.ShopCore.md)**
* $use_shop_context **mixed**



### <a name="method-getChildrenWs"></a>getChildrenWs

```php
mixed CategoryCore::getChildrenWs()
```





* Visibility: **public**
* Source: [classes/Category.php line 1333](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1333)




### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1576](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1576)


#### Arguments
* $class **string** - Name of object
* $field **string** - Name of field if we want the definition of one field only



### <a name="method-getDescriptionClean"></a>getDescriptionClean

```php
mixed CategoryCore::getDescriptionClean($description)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 142](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L142)


#### Arguments
* $description **mixed**



### <a name="method-getDuplicatePosition"></a>getDuplicatePosition

```php
array CategoryCore::getDuplicatePosition()
```

Search for another category with the same parent and the same position



* Visibility: **public**
* Source: [classes/Category.php line 1360](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1360)




### <a name="method-getFieldByLang"></a>getFieldByLang

```php
mixed ObjectModelCore::getFieldByLang($field_name, null $id_lang)
```

Return the field value for the specified language if the field is multilang, else the field value.



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1683](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1683)


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
* Source: [classes/ObjectModel.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L276)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 313](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L313)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1223](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1223)


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
* Source: [classes/ObjectModel.php line 299](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L299)




### <a name="method-getGroups"></a>getGroups

```php
mixed CategoryCore::getGroups()
```





* Visibility: **public**
* Source: [classes/Category.php line 1113](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1113)




### <a name="method-getHomeCategories"></a>getHomeCategories

```php
array CategoryCore::getHomeCategories(integer $id_lang, boolean $active, $id_shop)
```

Return main categories



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 726](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L726)


#### Arguments
* $id_lang **integer** - Language ID
* $active **boolean** - return only active categories
* $id_shop **mixed**



### <a name="method-getInterval"></a>getInterval

```php
array CategoryCore::getInterval(integer $id)
```

Return nleft and nright fields for a given category



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1291](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1291)


#### Arguments
* $id **integer**



### <a name="method-getLastPosition"></a>getLastPosition

```php
integer CategoryCore::getLastPosition(integer $id_category_parent, integer $id_shop)
```

this function return the number of category + 1 having $id_category_parent as parent.



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1264](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1264)


#### Arguments
* $id_category_parent **integer** - the parent category
* $id_shop **integer**



### <a name="method-getLink"></a>getLink

```php
mixed CategoryCore::getLink(\Link $link, $id_lang)
```





* Visibility: **public**
* Source: [classes/Category.php line 927](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L927)


#### Arguments
* $link **[Link](class.LinkCore.md)**
* $id_lang **mixed**



### <a name="method-getLinkRewrite"></a>getLinkRewrite

```php
mixed CategoryCore::getLinkRewrite($id_category, $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 912](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L912)


#### Arguments
* $id_category **mixed**
* $id_lang **mixed**



### <a name="method-getName"></a>getName

```php
mixed CategoryCore::getName($id_lang)
```





* Visibility: **public**
* Source: [classes/Category.php line 939](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L939)


#### Arguments
* $id_lang **mixed**



### <a name="method-getNestedCategories"></a>getNestedCategories

```php
mixed CategoryCore::getNestedCategories($root_category, $id_lang, $active, $groups, $use_shop_restriction, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 485](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L485)


#### Arguments
* $root_category **mixed**
* $id_lang **mixed**
* $active **mixed**
* $groups **mixed**
* $use_shop_restriction **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getParentsCategories"></a>getParentsCategories

```php
array CategoryCore::getParentsCategories(integer $id_lang)
```

Get Each parent category of this category until the root category



* Visibility: **public**
* Source: [classes/Category.php line 1036](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1036)


#### Arguments
* $id_lang **integer** - Language ID



### <a name="method-getProducts"></a>getProducts

```php
mixed CategoryCore::getProducts(integer $id_lang, integer $p, integer $n, $order_by, $order_way, boolean $get_total, boolean $active, boolean $random, integer $random_number_products, boolean $check_access, \Context $context)
```

Return current category products



* Visibility: **public**
* Source: [classes/Category.php line 610](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L610)


#### Arguments
* $id_lang **integer** - Language ID
* $p **integer** - Page number
* $n **integer** - Number of products per page
* $order_by **mixed**
* $order_way **mixed**
* $get_total **boolean** - return the number of results instead of the results themself
* $active **boolean** - return only active products
* $random **boolean** - active a random filter for returned products
* $random_number_products **integer** - number of products to return if random is activated
* $check_access **boolean** - set to false to return all products (even if customer hasn&#039;t access)
* $context **[Context](class.ContextCore.md)**



### <a name="method-getProductsWs"></a>getProductsWs

```php
mixed CategoryCore::getProductsWs()
```





* Visibility: **public**
* Source: [classes/Category.php line 1345](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1345)




### <a name="method-getRootCategories"></a>getRootCategories

```php
mixed CategoryCore::getRootCategories($id_lang, $active)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1462](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1462)


#### Arguments
* $id_lang **mixed**
* $active **mixed**



### <a name="method-getRootCategory"></a>getRootCategory

```php
mixed CategoryCore::getRootCategory($id_lang, \Shop $shop)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 731](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L731)


#### Arguments
* $id_lang **mixed**
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-getShopID"></a>getShopID

```php
mixed CategoryCore::getShopID()
```





* Visibility: **public**
* Source: [classes/Category.php line 554](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L554)




### <a name="method-getShopsByCategory"></a>getShopsByCategory

```php
mixed CategoryCore::getShopsByCategory($id_category)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1549](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1549)


#### Arguments
* $id_category **mixed**



### <a name="method-getSimpleCategories"></a>getSimpleCategories

```php
mixed CategoryCore::getSimpleCategories($id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 541](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L541)


#### Arguments
* $id_lang **mixed**



### <a name="method-getSubCategories"></a>getSubCategories

```php
array CategoryCore::getSubCategories(integer $id_lang, boolean $active)
```

Return current category childs



* Visibility: **public**
* Source: [classes/Category.php line 566](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L566)


#### Arguments
* $id_lang **integer** - Language ID
* $active **boolean** - return only active categories



### <a name="method-getTopCategory"></a>getTopCategory

```php
\Category CategoryCore::getTopCategory(null $id_lang)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1503](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1503)


#### Arguments
* $id_lang **null**



### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 804](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L804)


#### Arguments
* $fields_array **mixed**



### <a name="method-getUrlRewriteInformations"></a>getUrlRewriteInformations

```php
mixed CategoryCore::getUrlRewriteInformations($id_category)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1273)


#### Arguments
* $id_category **mixed**



### <a name="method-getValidationRules"></a>getValidationRules

```php
array ObjectModelCore::getValidationRules(string $class)
```

Returns object validation rules (fields validity)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L161)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1164](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1164)


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
* Source: [classes/ObjectModel.php line 1086](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1086)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-getWsNbProductsRecursive"></a>getWsNbProductsRecursive

```php
mixed CategoryCore::getWsNbProductsRecursive()
```





* Visibility: **public**
* Source: [classes/Category.php line 1371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1371)




### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1371)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1508](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1508)


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
* Source: [classes/ObjectModel.php line 1527](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1527)


#### Arguments
* $class **string** - Class of objects to hydrate
* $datas **array** - List of data (multi-dimensional array)
* $id_lang **integer**



### <a name="method-inShop"></a>inShop

```php
boolean CategoryCore::inShop(\Shop $shop)
```

Check if current category is a child of shop root category



* Visibility: **public**
* Source: [classes/Category.php line 1312](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1312)


#### Arguments
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-inShopStatic"></a>inShopStatic

```php
mixed CategoryCore::inShopStatic($id_category, \Shop $shop)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1322](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1322)


#### Arguments
* $id_category **mixed**
* $shop **[Shop](class.ShopCore.md)**



### <a name="method-isAssociatedToShop"></a>isAssociatedToShop

```php
boolean ObjectModelCore::isAssociatedToShop(integer $id_shop)
```

Check if current object is associated to a shop



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1273)


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
* Source: [classes/ObjectModel.php line 1488](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1488)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1388](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1388)




### <a name="method-isMultiShopField"></a>isMultiShopField

```php
mixed ObjectModelCore::isMultiShopField($field)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1383](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1383)


#### Arguments
* $field **mixed**



### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1378](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1378)




### <a name="method-isParentCategoryAvailable"></a>isParentCategoryAvailable

```php
boolean CategoryCore::isParentCategoryAvailable($id_shop)
```





* Visibility: **public**
* Source: [classes/Category.php line 1424](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1424)


#### Arguments
* $id_shop **mixed**



### <a name="method-isRootCategoryForAShop"></a>isRootCategoryForAShop

```php
mixed CategoryCore::isRootCategoryForAShop()
```





* Visibility: **public**
* Source: [classes/Category.php line 1490](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1490)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 820](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L820)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-recalculateLevelDepth"></a>recalculateLevelDepth

```php
mixed CategoryCore::recalculateLevelDepth(integer $id_category)
```

Updates level_depth for all children of the given id_category



* Visibility: **public**
* Source: [classes/Category.php line 426](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L426)


#### Arguments
* $id_category **integer** - parent category



### <a name="method-recurseCategory"></a>recurseCategory

```php
mixed CategoryCore::recurseCategory($categories, $current, $id_category, $id_selected)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 273](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L273)


#### Arguments
* $categories **mixed**
* $current **mixed**
* $id_category **mixed**
* $id_selected **mixed**



### <a name="method-recurseLiteCategTree"></a>recurseLiteCategTree

```php
array CategoryCore::recurseLiteCategTree(integer $max_depth, integer $current_depth, integer $id_lang, array $excluded_ids_array)
```

Recursive scan of subcategories



* Visibility: **public**
* Source: [classes/Category.php line 240](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L240)


#### Arguments
* $max_depth **integer** - Maximum depth of the tree (i.e. 2 =&gt; 3 levels depth)
* $current_depth **integer** - specify the current depth in the tree (don&#039;t use it, only for rucursivity!)
* $id_lang **integer** - Specify the id of the language used
* $excluded_ids_array **array** - specify a list of ids to exclude of results



### <a name="method-recursiveDelete"></a>recursiveDelete

```php
mixed CategoryCore::recursiveDelete($to_delete, integer $id_category)
```

Recursively add specified category childs to $to_delete array



* Visibility: **protected**
* Source: [classes/Category.php line 292](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L292)


#### Arguments
* $to_delete **mixed**
* $id_category **integer** - Parent category ID



### <a name="method-regenerateEntireNtree"></a>regenerateEntireNtree

```php
mixed CategoryCore::regenerateEntireNtree()
```

Re-calculate the values of all branches of the nested tree



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 388](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L388)




### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 446](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L446)


#### Arguments
* $null_values **boolean**
* $autodate **boolean**



### <a name="method-searchByName"></a>searchByName

```php
array CategoryCore::searchByName(integer $id_lang, string $query, boolean $unrestricted)
```

Light back office search for categories



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 959](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L959)


#### Arguments
* $id_lang **integer** - Language ID
* $query **string** - Searched string
* $unrestricted **boolean** - allows search without lang and includes first category and exact match



### <a name="method-searchByNameAndParentCategoryId"></a>searchByNameAndParentCategoryId

```php
array CategoryCore::searchByNameAndParentCategoryId(integer $id_lang, string $category_name, integer $id_parent_category)
```

Retrieve category by name and parent category id



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 984](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L984)


#### Arguments
* $id_lang **integer** - Language ID
* $category_name **string** - Searched category name
* $id_parent_category **integer** - parent category ID



### <a name="method-searchByPath"></a>searchByPath

```php
array CategoryCore::searchByPath(integer $id_lang, string $path, boolean $object_to_create, $method_to_create)
```

Search with Pathes for categories



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1006](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1006)


#### Arguments
* $id_lang **integer** - Language ID
* $path **string** - of category
* $object_to_create **boolean** - a category
  * @param boolean $method_to_create a category
* $method_to_create **mixed**



### <a name="method-setDefinitionRetrocompatibility"></a>setDefinitionRetrocompatibility

```php
mixed ObjectModelCore::setDefinitionRetrocompatibility()
```

Retrocompatibility for classes without $definition static
Remove this in 1.6 !



* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1614](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1614)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1709](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1709)


#### Arguments
* $fields **array**



### <a name="method-setNewGroupForHome"></a>setNewGroupForHome

```php
mixed CategoryCore::setNewGroupForHome($id_group)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1179](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1179)


#### Arguments
* $id_group **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
mixed CategoryCore::toggleStatus()
```





* Visibility: **public**
* Source: [classes/Category.php line 223](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L223)




### <a name="method-update"></a>update

```php
boolean CategoryCore::update(mixed $null_values)
```

update category positions in parent



* Visibility: **public**
* Source: [classes/Category.php line 183](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L183)


#### Arguments
* $null_values **mixed**



### <a name="method-updateFromShop"></a>updateFromShop

```php
array CategoryCore::updateFromShop(string $categories, string $id_shop)
```

Update categories for a shop



* Visibility: **public**
* This method is **static**.
* Source: [classes/Category.php line 1564](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1564)


#### Arguments
* $categories **string** - Categories list to associate a shop
* $id_shop **string** - Categories list to associate a shop



### <a name="method-updateGroup"></a>updateGroup

```php
mixed CategoryCore::updateGroup(array $list)
```

Update customer groups associated to the object



* Visibility: **public**
* Source: [classes/Category.php line 1171](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1171)


#### Arguments
* $list **array** - groups



### <a name="method-updateMultishopTable"></a>updateMultishopTable

```php
boolean ObjectModelCore::updateMultishopTable(string $classname, array $data, string $where, string $specific_where)
```

Update a table and splits the common datas and the shop datas



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1403](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1403)


#### Arguments
* $classname **string**
* $data **array**
* $where **string**
* $specific_where **string** - Only executed for common table



### <a name="method-updatePosition"></a>updatePosition

```php
mixed CategoryCore::updatePosition($way, $position)
```





* Visibility: **public**
* Source: [classes/Category.php line 1189](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/Category.php#L1189)


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
* Source: [classes/ObjectModel.php line 1032](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1032)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1038](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1038)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang, $skip, $human_errors)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 931](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L931)


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
* Source: [classes/ObjectModel.php line 858](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L858)


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
* Source: [classes/ObjectModel.php line 887](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L887)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1200](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/ObjectModel.php#L1200)


#### Arguments
* $htmlentities **mixed**


