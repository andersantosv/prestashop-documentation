Class PrestaShopCollectionCore
=====================

Create a collection of ObjectModel objects



* Class name: PrestaShopCollectionCore
* Source: [classes/PrestaShopCollection.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L32)
* This class implements: Iterator, ArrayAccess, Countable
Constants
----------

* [INNER_JOIN](#constant-INNER_JOIN)
* [LANG_ALIAS](#constant-LANG_ALIAS)
* [LEFT_JOIN](#constant-LEFT_JOIN)
* [LEFT_OUTER_JOIN](#constant-LEFT_OUTER_JOIN)

Properties
----------

* [$alias](#property-$alias)
* [$alias_iterator](#property-$alias_iterator)
* [$association_definition](#property-$association_definition)
* [$classname](#property-$classname)
* [$definition](#property-$definition)
* [$fields](#property-$fields)
* [$id_lang](#property-$id_lang)
* [$is_hydrated](#property-$is_hydrated)
* [$iterator](#property-$iterator)
* [$join_list](#property-$join_list)
* [$page_number](#property-$page_number)
* [$page_size](#property-$page_size)
* [$query](#property-$query)
* [$results](#property-$results)
* [$total](#property-$total)

Methods
-------
* [__construct](#method-__construct)
* [count](#method-count)
* [current](#method-current)
* [formatValue](#method-formatValue)
* [generateAlias](#method-generateAlias)
* [getAll](#method-getAll)
* [getDefinition](#method-getDefinition)
* [getFieldInfo](#method-getFieldInfo)
* [getFirst](#method-getFirst)
* [getResults](#method-getResults)
* [groupBy](#method-groupBy)
* [having](#method-having)
* [join](#method-join)
* [key](#method-key)
* [next](#method-next)
* [offsetExists](#method-offsetExists)
* [offsetGet](#method-offsetGet)
* [offsetSet](#method-offsetSet)
* [offsetUnset](#method-offsetUnset)
* [orderBy](#method-orderBy)
* [parseField](#method-parseField)
* [parseFields](#method-parseFields)
* [rewind](#method-rewind)
* [setPageNumber](#method-setPageNumber)
* [setPageSize](#method-setPageSize)
* [sqlGroupBy](#method-sqlGroupBy)
* [sqlHaving](#method-sqlHaving)
* [sqlOrderBy](#method-sqlOrderBy)
* [sqlWhere](#method-sqlWhere)
* [valid](#method-valid)
* [where](#method-where)


Constants
----------


### <a name="constant-INNER_JOIN"></a>INNER_JOIN

    const INNER_JOIN = 2





* Source: [classes/PrestaShopCollection.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L35).


### <a name="constant-LANG_ALIAS"></a>LANG_ALIAS

    const LANG_ALIAS = 'l'





* Source: [classes/PrestaShopCollection.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L94).


### <a name="constant-LEFT_JOIN"></a>LEFT_JOIN

    const LEFT_JOIN = 1





* Source: [classes/PrestaShopCollection.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L34).


### <a name="constant-LEFT_OUTER_JOIN"></a>LEFT_OUTER_JOIN

    const LEFT_OUTER_JOIN = 3





* Source: [classes/PrestaShopCollection.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L36).


Properties
----------


### <a name="property-$alias"></a>$alias

    protected mixed $alias = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 89](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L89).


### <a name="property-$alias_iterator"></a>$alias_iterator

    protected mixed $alias_iterator





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L90).


### <a name="property-$association_definition"></a>$association_definition

    protected mixed $association_definition = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 92](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L92).


### <a name="property-$classname"></a>$classname

    protected string $classname





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L41).


### <a name="property-$definition"></a>$definition

    protected array $definition = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L51).


### <a name="property-$fields"></a>$fields

    protected mixed $fields = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 88](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L88).


### <a name="property-$id_lang"></a>$id_lang

    protected integer $id_lang





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L46).


### <a name="property-$is_hydrated"></a>$is_hydrated

    protected boolean $is_hydrated = false





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L66).


### <a name="property-$iterator"></a>$iterator

    protected integer $iterator





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L71).


### <a name="property-$join_list"></a>$join_list

    protected mixed $join_list = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L91).


### <a name="property-$page_number"></a>$page_number

    protected integer $page_number





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L81).


### <a name="property-$page_size"></a>$page_size

    protected integer $page_size





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L86).


### <a name="property-$query"></a>$query

    protected \DbQuery $query





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L56).


### <a name="property-$results"></a>$results

    protected array $results = array()





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L61).


### <a name="property-$total"></a>$total

    protected integer $total





* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L76).


Methods
-------


### <a name="method-__construct"></a>__construct

    mixed PrestaShopCollectionCore::__construct(string $classname, integer $id_lang)





* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L100)


#### Arguments
* $classname **string**
* $id_lang **integer**



### <a name="method-count"></a>count

    integer PrestaShopCollectionCore::count()

Get total of results



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 452](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L452)




### <a name="method-current"></a>current

    \ObjectModel PrestaShopCollectionCore::current()

Get current result



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 409](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L409)




### <a name="method-formatValue"></a>formatValue

    mixed PrestaShopCollectionCore::formatValue(mixed $value, string $field)

Format a value with the type of the given field



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 618](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L618)


#### Arguments
* $value **mixed**
* $field **string** - Field name



### <a name="method-generateAlias"></a>generateAlias

    string PrestaShopCollectionCore::generateAlias(string $association)

Generate uniq alias from association name



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 719](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L719)


#### Arguments
* $association **string** - Use empty association for alias on current table



### <a name="method-getAll"></a>getAll

    \PrestaShopCollection PrestaShopCollectionCore::getAll(boolean $display_query)

Launch sql query to create collection of objects



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 311](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L311)


#### Arguments
* $display_query **boolean** - If true, query will be displayed (for debug purpose)



### <a name="method-getDefinition"></a>getDefinition

    array PrestaShopCollectionCore::getDefinition(string $association)

Get definition of an association



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 526](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L526)


#### Arguments
* $association **string**



### <a name="method-getFieldInfo"></a>getFieldInfo

    array PrestaShopCollectionCore::getFieldInfo(string $field)

Obtain some information on a field (alias, name, type, etc.)



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 637](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L637)


#### Arguments
* $field **string** - Field name



### <a name="method-getFirst"></a>getFirst

    \ObjectModel PrestaShopCollectionCore::getFirst()

Retrieve the first result



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 370](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L370)




### <a name="method-getResults"></a>getResults

    array PrestaShopCollectionCore::getResults()

Get results array



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 384](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L384)




### <a name="method-groupBy"></a>groupBy

    \PrestaShopCollection PrestaShopCollectionCore::groupBy(string $field)

Add GROUP BY restriction on query



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 287](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L287)


#### Arguments
* $field **string** - Field name



### <a name="method-having"></a>having

    \PrestaShopCollection PrestaShopCollectionCore::having(string $field, string $operator, mixed $value)

Add HAVING restriction on query



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 235](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L235)


#### Arguments
* $field **string** - Field name
* $operator **string** - List of operators : =, !=, , =, like, notlike, regexp, notregexp
* $value **mixed**



### <a name="method-join"></a>join

    \PrestaShopCollection PrestaShopCollectionCore::join(string $association, string $on, integer $type)

Join current entity to an associated entity



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 123](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L123)


#### Arguments
* $association **string** - Association name
* $on **string**
* $type **integer**



### <a name="method-key"></a>key

    integer PrestaShopCollectionCore::key()

Get current result index



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 431](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L431)




### <a name="method-next"></a>next

    mixed PrestaShopCollectionCore::next()

Go to next result



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 441](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L441)




### <a name="method-offsetExists"></a>offsetExists

    boolean PrestaShopCollectionCore::offsetExists($offset)

Check if a result exist



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 465](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L465)


#### Arguments
* $offset **mixed**



### <a name="method-offsetGet"></a>offsetGet

    \ObjectModel PrestaShopCollectionCore::offsetGet($offset)

Get a result by offset



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 478](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L478)


#### Arguments
* $offset **mixed**



### <a name="method-offsetSet"></a>offsetSet

    mixed PrestaShopCollectionCore::offsetSet($offset, $value)

Add an element in the collection



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 494](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L494)


#### Arguments
* $offset **mixed**
* $value **mixed**



### <a name="method-offsetUnset"></a>offsetUnset

    mixed PrestaShopCollectionCore::offsetUnset($offset)

Delete an element from the collection



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 514](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L514)


#### Arguments
* $offset **mixed**



### <a name="method-orderBy"></a>orderBy

    \PrestaShopCollection PrestaShopCollectionCore::orderBy(string $field, string $order)

Add ORDER BY restriction on query



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 259](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L259)


#### Arguments
* $field **string** - Field name
* $order **string** - asc|desc



### <a name="method-parseField"></a>parseField

    string PrestaShopCollectionCore::parseField(string $field)

Replace a field with its SQL version (E.g. manufacturer.name with a2.name)



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 605](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L605)


#### Arguments
* $field **string** - Field name



### <a name="method-parseFields"></a>parseFields

    string PrestaShopCollectionCore::parseFields(string $str)

Parse all fields with {field} syntax in a string



* Visibility: **protected**
* Source: [classes/PrestaShopCollection.php line 590](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L590)


#### Arguments
* $str **string**



### <a name="method-rewind"></a>rewind

    mixed PrestaShopCollectionCore::rewind()

This method is called when a foreach begin



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 395](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L395)




### <a name="method-setPageNumber"></a>setPageNumber

    \PrestaShopCollection PrestaShopCollectionCore::setPageNumber(integer $page_number)

Set the page number



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 690](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L690)


#### Arguments
* $page_number **integer**



### <a name="method-setPageSize"></a>setPageSize

    \PrestaShopCollection PrestaShopCollectionCore::setPageSize(integer $page_size)

Set the nuber of item per page



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 707](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L707)


#### Arguments
* $page_size **integer**



### <a name="method-sqlGroupBy"></a>sqlGroupBy

    \PrestaShopCollection PrestaShopCollectionCore::sqlGroupBy(string $sql)

Add GROUP BY restriction on query using real SQL syntax



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 299](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L299)


#### Arguments
* $sql **string**



### <a name="method-sqlHaving"></a>sqlHaving

    \PrestaShopCollection PrestaShopCollectionCore::sqlHaving(string $sql)

Add HAVING restriction on query using real SQL syntax



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 246](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L246)


#### Arguments
* $sql **string**



### <a name="method-sqlOrderBy"></a>sqlOrderBy

    \PrestaShopCollection PrestaShopCollectionCore::sqlOrderBy(string $sql)

Add ORDER BY restriction on query using real SQL syntax



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 275](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L275)


#### Arguments
* $sql **string**



### <a name="method-sqlWhere"></a>sqlWhere

    \PrestaShopCollection PrestaShopCollectionCore::sqlWhere(string $sql)

Add WHERE restriction on query using real SQL syntax



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 221](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L221)


#### Arguments
* $sql **string**



### <a name="method-valid"></a>valid

    boolean PrestaShopCollectionCore::valid()

Check if there is a current result



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 420](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L420)




### <a name="method-where"></a>where

    \PrestaShopCollection PrestaShopCollectionCore::where(string $field, string $operator, mixed $value, $method)

Add WHERE restriction on query



* Visibility: **public**
* Source: [classes/PrestaShopCollection.php line 160](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/PrestaShopCollection.php#L160)


#### Arguments
* $field **string** - Field name
* $operator **string** - List of operators : =, !=, , =, like, notlike, regexp, notregexp
* $value **mixed**
* $method **mixed**

