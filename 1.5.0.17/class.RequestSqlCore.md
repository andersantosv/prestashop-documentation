Class RequestSqlCore
=====================





* Class name: RequestSqlCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/RequestSql.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L28)


Contents
--------


### Properties

* [$attributes](#property-$attributes)
* [$definition](#property-$definition)
* [$error_sql](#property-$error_sql)
* [$name](#property-$name)
* [$sql](#property-$sql)
* [$tested](#property-$tested)
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
* [attributExistInTable](#method-attributExistInTable)
* [checkedFrom](#method-checkedFrom)
* [checkedGroupBy](#method-checkedGroupBy)
* [checkedHaving](#method-checkedHaving)
* [checkedLimit](#method-checkedLimit)
* [checkedOrder](#method-checkedOrder)
* [checkedSelect](#method-checkedSelect)
* [checkedWhere](#method-checkedWhere)
* [clearCache](#method-clearCache)
* [cutAttribute](#method-cutAttribute)
* [cutJoin](#method-cutJoin)
* [delete](#method-delete)
* [deleteImage](#method-deleteImage)
* [deleteSelection](#method-deleteSelection)
* [displayFieldName](#method-displayFieldName)
* [duplicateShops](#method-duplicateShops)
* [existsInDatabase](#method-existsInDatabase)
* [formatFields](#method-formatFields)
* [formatValue](#method-formatValue)
* [getAssociatedShops](#method-getAssociatedShops)
* [getAttributesByTable](#method-getAttributesByTable)
* [getDefinition](#method-getDefinition)
* [getFieldByLang](#method-getFieldByLang)
* [getFields](#method-getFields)
* [getFieldsLang](#method-getFieldsLang)
* [getFieldsRequiredDatabase](#method-getFieldsRequiredDatabase)
* [getFieldsShop](#method-getFieldsShop)
* [getRequestSql](#method-getRequestSql)
* [getRequestSqlById](#method-getRequestSqlById)
* [getTables](#method-getTables)
* [getTranslationsFields](#method-getTranslationsFields)
* [getValidationRules](#method-getValidationRules)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWebserviceParameters](#method-getWebserviceParameters)
* [hasMultishopEntries](#method-hasMultishopEntries)
* [hydrate](#method-hydrate)
* [hydrateCollection](#method-hydrateCollection)
* [isAssociatedToShop](#method-isAssociatedToShop)
* [isCurrentlyUsed](#method-isCurrentlyUsed)
* [isLangMultishop](#method-isLangMultishop)
* [isMultishop](#method-isMultishop)
* [makeTranslationFields](#method-makeTranslationFields)
* [parsingSql](#method-parsingSql)
* [returnNameTable](#method-returnNameTable)
* [save](#method-save)
* [setDefinitionRetrocompatibility](#method-setDefinitionRetrocompatibility)
* [setFieldsToUpdate](#method-setFieldsToUpdate)
* [testedRequired](#method-testedRequired)
* [testedUnauthorized](#method-testedUnauthorized)
* [toggleStatus](#method-toggleStatus)
* [update](#method-update)
* [updateMultishopTable](#method-updateMultishopTable)
* [validateControler](#method-validateControler)
* [validateController](#method-validateController)
* [validateField](#method-validateField)
* [validateFields](#method-validateFields)
* [validateFieldsLang](#method-validateFieldsLang)
* [validateFieldsRequiredDatabase](#method-validateFieldsRequiredDatabase)
* [validateParser](#method-validateParser)
* [validateSql](#method-validateSql)




Properties
----------


### <a name="property-$attributes"></a>$attributes

```php
public mixed $attributes = array('passwd' => '*******************', 'secure_key' => '*******************')
```





* Visibility: **public**
* Source: [classes/RequestSql.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L69).


### <a name="property-$definition"></a>$definition

```php
public mixed $definition = array('table' => 'request_sql', 'primary' => 'id_request_sql', 'fields' => array('name' => array('type' => self::TYPE_STRING, 'validate' => 'isString', 'required' => true, 'size' => 200), 'sql' => array('type' => self::TYPE_STRING, 'validate' => 'isString', 'required' => true, 'size' => 1000)))
```





* Visibility: **public**
* This property is **static**.
* Source: [classes/RequestSql.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L36).


### <a name="property-$error_sql"></a>$error_sql

```php
public array $error_sql = array()
```





* Visibility: **public**
* Source: [classes/RequestSql.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L75).


### <a name="property-$name"></a>$name

```php
public mixed $name
```





* Visibility: **public**
* Source: [classes/RequestSql.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L30).


### <a name="property-$sql"></a>$sql

```php
public mixed $sql
```





* Visibility: **public**
* Source: [classes/RequestSql.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L31).


### <a name="property-$tested"></a>$tested

```php
public array $tested = array('required' => array('SELECT', 'FROM'), 'option' => array('WHERE', 'ORDER', 'LIMIT', 'HAVING', 'GROUP', 'UNION'), 'operator' => array('AND', '&&', 'BETWEEN', 'AND', 'BINARY', '&', '~', '|', '^', 'CASE', 'WHEN', 'END', 'DIV', '/', '<=>', '=', '>=', '>', 'IS', 'NOT', 'NULL', '<<', '<=', '<', 'LIKE', '-', '%', '!=', '<>', 'REGEXP', '!', '||', 'OR', '+', '>>', 'RLIKE', 'SOUNDS', '*', '-', 'XOR', 'IN'), 'function' => array('AVG', 'SUM', 'COUNT', 'MIN', 'MAX', 'STDDEV', 'STDDEV_SAMP', 'STDDEV_POP', 'VARIANCE', 'VAR_SAMP', 'VAR_POP', 'GROUP_CONCAT', 'BIT_AND', 'BIT_OR', 'BIT_XOR'), 'unauthorized' => array('DELETE', 'ALTER', 'INSERT', 'REPLACE', 'CREATE', 'TRUNCATE', 'OPTIMIZE', 'GRANT', 'REVOKE', 'SHOW', 'HANDLER', 'LOAD', 'ROLLBACK', 'SAVEPOINT', 'UNLOCK', 'INSTALL', 'UNINSTALL', 'ANALZYE', 'BACKUP', 'CHECK', 'CHECKSUM', 'REPAIR', 'RESTORE', 'CACHE', 'DESCRIBE', 'EXPLAIN', 'USE', 'HELP', 'SET', 'DUPLICATE', 'VALUES', 'INTO', 'RENAME', 'CALL', 'PROCEDURE', 'FUNCTION', 'DATABASE', 'SERVER', 'LOGFILE', 'DEFINER', 'RETURNS', 'EVENT', 'TABLESPACE', 'VIEW', 'TRIGGER', 'DATA', 'DO', 'PASSWORD', 'USER', 'PLUGIN', 'FLUSH', 'KILL', 'RESET', 'START', 'STOP', 'PURGE', 'EXECUTE', 'PREPARE', 'DEALLOCATE', 'LOCK', 'USING', 'DROP', 'FOR', 'UPDATE', 'BEGIN', 'BY', 'ALL', 'SHARE', 'MODE', 'TO', 'KEY', 'DISTINCTROW', 'DISTINCT', 'HIGH_PRIORITY', 'LOW_PRIORITY', 'DELAYED', 'IGNORE', 'FORCE', 'STRAIGHT_JOIN', 'SQL_SMALL_RESULT', 'SQL_BIG_RESULT', 'QUICK', 'SQL_BUFFER_RESULT', 'SQL_CACHE', 'SQL_NO_CACHE', 'SQL_CALC_FOUND_ROWS', 'WITH'))
```





* Visibility: **public**
* Source: [classes/RequestSql.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L46).


### <a name="property-$db"></a>$db

```php
protected \Db $db = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 141](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L141).


### <a name="property-$def"></a>$def

```php
protected array $def
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 131](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L131).


### <a name="property-$fieldsRequired"></a>$fieldsRequired

```php
protected mixed $fieldsRequired = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L81).


### <a name="property-$fieldsRequiredDatabase"></a>$fieldsRequiredDatabase

```php
protected mixed $fieldsRequiredDatabase = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L66).


### <a name="property-$fieldsRequiredLang"></a>$fieldsRequiredLang

```php
protected mixed $fieldsRequiredLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L96).


### <a name="property-$fieldsSize"></a>$fieldsSize

```php
protected mixed $fieldsSize = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L86).


### <a name="property-$fieldsSizeLang"></a>$fieldsSizeLang

```php
protected mixed $fieldsSizeLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L101).


### <a name="property-$fieldsValidate"></a>$fieldsValidate

```php
protected mixed $fieldsValidate = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L91).


### <a name="property-$fieldsValidateLang"></a>$fieldsValidateLang

```php
protected mixed $fieldsValidateLang = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L106).


### <a name="property-$get_shop_from_context"></a>$get_shop_from_context

```php
protected mixed $get_shop_from_context = true
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L64).


### <a name="property-$id"></a>$id

```php
public integer $id
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L55).


### <a name="property-$id_lang"></a>$id_lang

```php
protected integer $id_lang = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L58).


### <a name="property-$id_shop"></a>$id_shop

```php
protected mixed $id_shop = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L60).


### <a name="property-$id_shop_list"></a>$id_shop_list

```php
public mixed $id_shop_list = null
```





* Visibility: **public**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L62).


### <a name="property-$identifier"></a>$identifier

```php
protected mixed $identifier
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L76).


### <a name="property-$image_dir"></a>$image_dir

```php
protected string $image_dir = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L117).


### <a name="property-$image_format"></a>$image_format

```php
protected string $image_format = 'jpg'
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L120).


### <a name="property-$table"></a>$table

```php
protected mixed $table
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L71).


### <a name="property-$tables"></a>$tables

```php
protected mixed $tables = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L111).


### <a name="property-$update_fields"></a>$update_fields

```php
protected array $update_fields = null
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 136](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L136).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

```php
protected array $webserviceParameters = array()
```





* Visibility: **protected**
* This property is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L114).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ObjectModelCore::__construct(integer $id, integer $id_lang, integer $id_shop)
```

Build object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 169](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L169)


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
* Source: [classes/ObjectModel.php line 437](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L437)


#### Arguments
* $autodate **boolean**
* $null_values **boolean**



### <a name="method-addFieldsRequiredDatabase"></a>addFieldsRequiredDatabase

```php
mixed ObjectModelCore::addFieldsRequiredDatabase($fields)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1092](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1092)


#### Arguments
* $fields **mixed**



### <a name="method-associateTo"></a>associateTo

```php
boolean ObjectModelCore::associateTo(integer|array $id_shops)
```

This function associate an item to its context



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1139](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1139)


#### Arguments
* $id_shops **integer|array**



### <a name="method-attributExistInTable"></a>attributExistInTable

```php
boolean RequestSqlCore::attributExistInTable($attr, $table)
```

Check if an attributes existe in an table



* Visibility: **public**
* Source: [classes/RequestSql.php line 313](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L313)


#### Arguments
* $attr **mixed**
* $table **mixed**



### <a name="method-checkedFrom"></a>checkedFrom

```php
boolean RequestSqlCore::checkedFrom($from)
```

Check a "FROM" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 364](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L364)


#### Arguments
* $from **mixed**



### <a name="method-checkedGroupBy"></a>checkedGroupBy

```php
boolean RequestSqlCore::checkedGroupBy($group, $from)
```

Check a "GROUP BY" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 608](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L608)


#### Arguments
* $group **mixed**
* $from **mixed**



### <a name="method-checkedHaving"></a>checkedHaving

```php
boolean RequestSqlCore::checkedHaving($having, $from)
```

Check a "HAVING" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 521](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L521)


#### Arguments
* $having **mixed**
* $from **mixed**



### <a name="method-checkedLimit"></a>checkedLimit

```php
boolean RequestSqlCore::checkedLimit($limit)
```

Check a "LIMIT" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 644](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L644)


#### Arguments
* $limit **mixed**



### <a name="method-checkedOrder"></a>checkedOrder

```php
boolean RequestSqlCore::checkedOrder($order, $from)
```

Check a "ORDER" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 571](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L571)


#### Arguments
* $order **mixed**
* $from **mixed**



### <a name="method-checkedSelect"></a>checkedSelect

```php
boolean RequestSqlCore::checkedSelect($select, $from, boolean $in)
```

Check a "SELECT" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 414](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L414)


#### Arguments
* $select **mixed**
* $from **mixed**
* $in **boolean**



### <a name="method-checkedWhere"></a>checkedWhere

```php
boolean RequestSqlCore::checkedWhere($where, $from, $sql)
```

Check a "WHERE" sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 467](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L467)


#### Arguments
* $where **mixed**
* $from **mixed**
* $sql **mixed**



### <a name="method-clearCache"></a>clearCache

```php
mixed ObjectModelCore::clearCache($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1106](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1106)


#### Arguments
* $all **mixed**



### <a name="method-cutAttribute"></a>cutAttribute

```php
array|boolean RequestSqlCore::cutAttribute($attr, $from)
```

Cut an attribute with or without the alias



* Visibility: **public**
* Source: [classes/RequestSql.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L249)


#### Arguments
* $attr **mixed**
* $from **mixed**



### <a name="method-cutJoin"></a>cutJoin

```php
array|boolean RequestSqlCore::cutJoin($attrs, $from)
```

Cut an join sentence



* Visibility: **public**
* Source: [classes/RequestSql.php line 229](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L229)


#### Arguments
* $attrs **mixed**
* $from **mixed**



### <a name="method-delete"></a>delete

```php
boolean ObjectModelCore::delete()
```

Delete current object from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 644](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L644)




### <a name="method-deleteImage"></a>deleteImage

```php
boolean ObjectModelCore::deleteImage($force_delete)
```

Delete images associated with the object



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1265](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1265)


#### Arguments
* $force_delete **mixed**



### <a name="method-deleteSelection"></a>deleteSelection

```php
boolean ObjectModelCore::deleteSelection(array $selection)
```

Delete several objects from database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 690](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L690)


#### Arguments
* $selection **array**



### <a name="method-displayFieldName"></a>displayFieldName

```php
mixed ObjectModelCore::displayFieldName($field, $class, $htmlentities, \Context $context)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 890](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L890)


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
* Source: [classes/ObjectModel.php line 1183](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1183)


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
* Source: [classes/ObjectModel.php line 1302](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1302)


#### Arguments
* $id_entity **integer**
* $table **string**



### <a name="method-formatFields"></a>formatFields

```php
array ObjectModelCore::formatFields(integer $type, integer $id_lang)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 335](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L335)


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
* Source: [classes/ObjectModel.php line 381](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L381)


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
* Source: [classes/ObjectModel.php line 1168](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1168)




### <a name="method-getAttributesByTable"></a>getAttributesByTable

```php
array RequestSqlCore::getAttributesByTable($table)
```

Get list of all attributes by an table



* Visibility: **public**
* Source: [classes/RequestSql.php line 217](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L217)


#### Arguments
* $table **mixed**



### <a name="method-getDefinition"></a>getDefinition

```php
array ObjectModelCore::getDefinition(string $class, string $field)
```

Get object definition



* Visibility: **public**
* This method is **static**.
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1408](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1408)


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
* Source: [classes/ObjectModel.php line 1485](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1485)


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
* Source: [classes/ObjectModel.php line 263](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L263)




### <a name="method-getFieldsLang"></a>getFieldsLang

```php
array ObjectModelCore::getFieldsLang()
```

Prepare multilang fields



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 300](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L300)




### <a name="method-getFieldsRequiredDatabase"></a>getFieldsRequiredDatabase

```php
mixed ObjectModelCore::getFieldsRequiredDatabase($all)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1084](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1084)


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
* Source: [classes/ObjectModel.php line 286](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L286)




### <a name="method-getRequestSql"></a>getRequestSql

```php
array|boolean RequestSqlCore::getRequestSql()
```

Get list of request SQL



* Visibility: **public**
* This method is **static**.
* Source: [classes/RequestSql.php line 83](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L83)




### <a name="method-getRequestSqlById"></a>getRequestSqlById

```php
array RequestSqlCore::getRequestSqlById($id)
```

Get list of request SQL by id request



* Visibility: **public**
* This method is **static**.
* Source: [classes/RequestSql.php line 102](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L102)


#### Arguments
* $id **mixed**



### <a name="method-getTables"></a>getTables

```php
array RequestSqlCore::getTables()
```

Get list of all tables



* Visibility: **public**
* Source: [classes/RequestSql.php line 200](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L200)




### <a name="method-getTranslationsFields"></a>getTranslationsFields

```php
mixed ObjectModelCore::getTranslationsFields($fields_array)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 722](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L722)


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
* Source: [classes/ObjectModel.php line 149](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L149)


#### Arguments
* $class **string** - Child class name for static use (optional)



### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

```php
mixed ObjectModelCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1026](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1026)


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
* Source: [classes/ObjectModel.php line 952](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L952)


#### Arguments
* $ws_params_attribute_name **mixed**



### <a name="method-hasMultishopEntries"></a>hasMultishopEntries

```php
boolean ObjectModelCore::hasMultishopEntries()
```

Check if there is more than one entries in associated shop table for current entity



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1208](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1208)




### <a name="method-hydrate"></a>hydrate

```php
mixed ObjectModelCore::hydrate(array $data, integer $id_lang)
```

Fill an object with given data. Data must be an array with this syntax: array(objProperty => value, objProperty2 => value, etc.)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1340](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1340)


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
* Source: [classes/ObjectModel.php line 1359](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1359)


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
* Source: [classes/ObjectModel.php line 1121](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1121)


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
* Source: [classes/ObjectModel.php line 1320](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1320)


#### Arguments
* $table **string** - name of table linked to entity
* $has_active_column **boolean** - true if the table has an active column



### <a name="method-isLangMultishop"></a>isLangMultishop

```php
mixed ObjectModelCore::isLangMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1220](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1220)




### <a name="method-isMultishop"></a>isMultishop

```php
mixed ObjectModelCore::isMultishop()
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1215](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1215)




### <a name="method-makeTranslationFields"></a>makeTranslationFields

```php
mixed ObjectModelCore::makeTranslationFields($fields, $fields_array, $id_language)
```





* Visibility: **protected**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 738](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L738)


#### Arguments
* $fields **mixed**
* $fields_array **mixed**
* $id_language **mixed**



### <a name="method-parsingSql"></a>parsingSql

```php
boolean RequestSqlCore::parsingSql($sql)
```

Call the parserSQL() method in Tools class
Cut the request in table for check it



* Visibility: **public**
* Source: [classes/RequestSql.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L114)


#### Arguments
* $sql **mixed**



### <a name="method-returnNameTable"></a>returnNameTable

```php
array|boolean RequestSqlCore::returnNameTable(boolean $alias, $tables)
```

Get name of table by alias



* Visibility: **public**
* Source: [classes/RequestSql.php line 283](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L283)


#### Arguments
* $alias **boolean**
* $tables **mixed**



### <a name="method-save"></a>save

```php
boolean ObjectModelCore::save(boolean $null_values, boolean $autodate)
```

Save current object to database (add or update)



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 425](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L425)


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
* Source: [classes/ObjectModel.php line 1431](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1431)




### <a name="method-setFieldsToUpdate"></a>setFieldsToUpdate

```php
mixed ObjectModelCore::setFieldsToUpdate(array $fields)
```

Set a list of specific fields to update
array(field1 => true, field2 => false, langfield1 => array(1 => true, 2 => false))



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1511](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1511)


#### Arguments
* $fields **array**



### <a name="method-testedRequired"></a>testedRequired

```php
boolean RequestSqlCore::testedRequired($tab)
```

Check if all required sentence existing



* Visibility: **public**
* Source: [classes/RequestSql.php line 330](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L330)


#### Arguments
* $tab **mixed**



### <a name="method-testedUnauthorized"></a>testedUnauthorized

```php
boolean RequestSqlCore::testedUnauthorized($tab)
```

Check if an unauthorized existing in an array



* Visibility: **public**
* Source: [classes/RequestSql.php line 347](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L347)


#### Arguments
* $tab **mixed**



### <a name="method-toggleStatus"></a>toggleStatus

```php
boolean ObjectModelCore::toggleStatus()
```

Toggle object status in database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 706](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L706)




### <a name="method-update"></a>update

```php
boolean ObjectModelCore::update(boolean $null_values)
```

Update current object to database



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 529](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L529)


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
* Source: [classes/ObjectModel.php line 1235](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1235)


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
* Source: [classes/ObjectModel.php line 905](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L905)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateController"></a>validateController

```php
mixed ObjectModelCore::validateController($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 911](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L911)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateField"></a>validateField

```php
boolean|string ObjectModelCore::validateField(string $field, mixed $value, integer $id_lang)
```

Validate a single field



* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 843](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L843)


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
* Source: [classes/ObjectModel.php line 776](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L776)


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
* Source: [classes/ObjectModel.php line 805](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L805)


#### Arguments
* $die **boolean**
* $error_return **boolean**



### <a name="method-validateFieldsRequiredDatabase"></a>validateFieldsRequiredDatabase

```php
mixed ObjectModelCore::validateFieldsRequiredDatabase($htmlentities)
```





* Visibility: **public**
* This method is defined by [ObjectModelCore](class.ObjectModelCore.md).
* Source: [classes/ObjectModel.php line 1062](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/ObjectModel.php#L1062)


#### Arguments
* $htmlentities **mixed**



### <a name="method-validateParser"></a>validateParser

```php
boolean RequestSqlCore::validateParser($tab, boolean $in, $sql)
```

Check if the parsing of the SQL request is good or not



* Visibility: **public**
* Source: [classes/RequestSql.php line 127](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L127)


#### Arguments
* $tab **mixed**
* $in **boolean**
* $sql **mixed**



### <a name="method-validateSql"></a>validateSql

```php
boolean RequestSqlCore::validateSql($tab, $in, $sql)
```

Cut the request for check each cutting



* Visibility: **public**
* Source: [classes/RequestSql.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.17/classes/RequestSql.php#L153)


#### Arguments
* $tab **mixed**
* $in **mixed**
* $sql **mixed**


