Class DbMySQLiCore
=====================





* Class name: DbMySQLiCore
* Parent class: [Db](class.DbCore.md)
* Source: [classes/db/DbMySQLi.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L30)


Contents
--------


### Properties

* [$_servers](#property-$_servers)
* [$database](#property-$database)
* [$instance](#property-$instance)
* [$is_cache_enabled](#property-$is_cache_enabled)
* [$last_cached](#property-$last_cached)
* [$last_query](#property-$last_query)
* [$link](#property-$link)
* [$password](#property-$password)
* [$result](#property-$result)
* [$server](#property-$server)
* [$user](#property-$user)

### Methods

* [Affected_Rows](#method-Affected_Rows)
* [Insert_ID](#method-Insert_ID)
* [__construct](#method-__construct)
* [__destruct](#method-__destruct)
* [_escape](#method-_escape)
* [_numRows](#method-_numRows)
* [_query](#method-_query)
* [autoExecute](#method-autoExecute)
* [autoExecuteWithNullValues](#method-autoExecuteWithNullValues)
* [checkConnection](#method-checkConnection)
* [checkCreatePrivilege](#method-checkCreatePrivilege)
* [checkEncoding](#method-checkEncoding)
* [connect](#method-connect)
* [delete](#method-delete)
* [disconnect](#method-disconnect)
* [displayError](#method-displayError)
* [ds](#method-ds)
* [escape](#method-escape)
* [execute](#method-execute)
* [executeS](#method-executeS)
* [getClass](#method-getClass)
* [getInstance](#method-getInstance)
* [getMsgError](#method-getMsgError)
* [getNumberError](#method-getNumberError)
* [getRow](#method-getRow)
* [getValue](#method-getValue)
* [getVersion](#method-getVersion)
* [hasTableWithSamePrefix](#method-hasTableWithSamePrefix)
* [insert](#method-insert)
* [nextRow](#method-nextRow)
* [numRows](#method-numRows)
* [ps](#method-ps)
* [q](#method-q)
* [query](#method-query)
* [s](#method-s)
* [set_db](#method-set_db)
* [tryToConnect](#method-tryToConnect)
* [tryUTF8](#method-tryUTF8)
* [update](#method-update)




Properties
----------


### <a name="property-$_servers"></a>$_servers

```php
protected array $_servers = array(array('server' => _DB_SERVER_, 'user' => _DB_USER_, 'password' => _DB_PASSWD_, 'database' => _DB_NAME_))
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L82).


### <a name="property-$database"></a>$database

```php
protected string $database
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L57).


### <a name="property-$instance"></a>$instance

```php
protected array $instance = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L77).


### <a name="property-$is_cache_enabled"></a>$is_cache_enabled

```php
protected boolean $is_cache_enabled
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L62).


### <a name="property-$last_cached"></a>$last_cached

```php
protected string $last_cached
```

Last cached query



* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L101).


### <a name="property-$last_query"></a>$last_query

```php
protected string $last_query
```

Store last executed query



* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L94).


### <a name="property-$link"></a>$link

```php
protected mixed $link
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L67).


### <a name="property-$password"></a>$password

```php
protected string $password
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L52).


### <a name="property-$result"></a>$result

```php
protected mixed $result
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L72).


### <a name="property-$server"></a>$server

```php
protected string $server
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L42).


### <a name="property-$user"></a>$user

```php
protected string $user
```





* Visibility: **protected**
* This property is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L47).


Methods
-------


### <a name="method-Affected_Rows"></a>Affected_Rows

```php
mixed DbMySQLiCore::Affected_Rows()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 101](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L101)




### <a name="method-Insert_ID"></a>Insert_ID

```php
mixed DbMySQLiCore::Insert_ID()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L93)




### <a name="method-__construct"></a>__construct

```php
mixed DbCore::__construct(string $server, string $user, string $password, string $database, boolean $connect)
```

Instantiate database connection



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 230](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L230)


#### Arguments
* $server **string** - Server address
* $user **string** - User login
* $password **string** - User password
* $database **string** - Database name
* $connect **boolean** - If false, don&#039;t connect in constructor (since 1.5.0)



### <a name="method-__destruct"></a>__destruct

```php
mixed DbCore::__destruct()
```

Close connection to database



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 248](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L248)




### <a name="method-_escape"></a>_escape

```php
mixed DbMySQLiCore::_escape($str)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L133)


#### Arguments
* $str **mixed**



### <a name="method-_numRows"></a>_numRows

```php
mixed DbMySQLiCore::_numRows($result)
```





* Visibility: **protected**
* Source: [classes/db/DbMySQLi.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L85)


#### Arguments
* $result **mixed**



### <a name="method-_query"></a>_query

```php
mixed DbMySQLiCore::_query($sql)
```





* Visibility: **protected**
* Source: [classes/db/DbMySQLi.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L67)


#### Arguments
* $sql **mixed**



### <a name="method-autoExecute"></a>autoExecute

```php
mixed DbCore::autoExecute($table, $data, $type, $where, $limit, $use_cache, $use_null)
```





* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 257](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L257)


#### Arguments
* $table **mixed**
* $data **mixed**
* $type **mixed**
* $where **mixed**
* $limit **mixed**
* $use_cache **mixed**
* $use_null **mixed**



### <a name="method-autoExecuteWithNullValues"></a>autoExecuteWithNullValues

```php
mixed|boolean DbCore::autoExecuteWithNullValues(string $table, string $values, string $type, string $where, integer $limit)
```

Filter SQL query within a blacklist



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 289](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L289)


#### Arguments
* $table **string** - Table where insert/update data
* $values **string** - Data to insert/update
* $type **string** - INSERT or UPDATE
* $where **string** - WHERE clause, only for UPDATE (optional)
* $limit **integer** - LIMIT clause (optional)



### <a name="method-checkConnection"></a>checkConnection

```php
integer DbCore::checkConnection(string $server, string $user, string $pwd, string $db, boolean $new_db_link, boolean $engine, $timeout)
```

Try a connection to te database



* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 644](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L644)


#### Arguments
* $server **string** - Server address
* $user **string** - Login for database connection
* $pwd **string** - Password for database connection
* $db **string** - Database name
* $new_db_link **boolean**
* $engine **boolean**
* $timeout **mixed**



### <a name="method-checkCreatePrivilege"></a>checkCreatePrivilege

```php
mixed DbMySQLiCore::checkCreatePrivilege($server, $user, $pwd, $db, $prefix, $engine)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 189](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L189)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $prefix **mixed**
* $engine **mixed**



### <a name="method-checkEncoding"></a>checkEncoding

```php
integer DbCore::checkEncoding(string $server, string $user, string $pwd)
```

Try a connection to te database



* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 657](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L657)


#### Arguments
* $server **string** - Server address
* $user **string** - Login for database connection
* $pwd **string** - Password for database connection



### <a name="method-connect"></a>connect

```php
mixed DbMySQLiCore::connect()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L35)




### <a name="method-delete"></a>delete

```php
boolean DbCore::delete(string $table, string $where, integer $limit, boolean $use_cache, boolean $add_prefix)
```

Execute a DELETE query



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 422](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L422)


#### Arguments
* $table **string** - Name of the table to delete
* $where **string** - WHERE clause on query
* $limit **integer** - Number max of rows to delete
* $use_cache **boolean** - Use cache or not
* $add_prefix **boolean** - Add or not _DB_PREFIX_ before table name



### <a name="method-disconnect"></a>disconnect

```php
mixed DbMySQLiCore::disconnect()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L59)




### <a name="method-displayError"></a>displayError

```php
mixed DbCore::displayError(boolean $sql)
```

Display last SQL error



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 594](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L594)


#### Arguments
* $sql **boolean**



### <a name="method-ds"></a>ds

```php
mixed DbCore::ds($sql, $use_cache)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 705](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L705)


#### Arguments
* $sql **mixed**
* $use_cache **mixed**



### <a name="method-escape"></a>escape

```php
string DbCore::escape(string $string, boolean $html_ok)
```

Sanitize data which will be injected into SQL query



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 619](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L619)


#### Arguments
* $string **string** - SQL data which will be injected into SQL query
* $html_ok **boolean** - Does data contain HTML code ? (optional)



### <a name="method-execute"></a>execute

```php
boolean DbCore::execute(string $sql, boolean $use_cache)
```

Execute a query



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 442](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L442)


#### Arguments
* $sql **string**
* $use_cache **boolean**



### <a name="method-executeS"></a>executeS

```php
array DbCore::executeS(string $sql, boolean $array, boolean $use_cache)
```

ExecuteS return the result of $sql as array



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 461](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L461)


#### Arguments
* $sql **string** - query to execute
* $array **boolean** - return an array instead of a mysql_result object (deprecated since 1.5.0, use query method instead)
* $use_cache **boolean** - if query has been already executed, use its result



### <a name="method-getClass"></a>getClass

```php
string DbCore::getClass()
```

Get child layer class



* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 211](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L211)




### <a name="method-getInstance"></a>getInstance

```php
\Db DbCore::getInstance(boolean $master)
```

Get Db object instance



* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 179](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L179)


#### Arguments
* $master **boolean** - Decides whether the connection to be returned by the master server or the slave server



### <a name="method-getMsgError"></a>getMsgError

```php
mixed DbMySQLiCore::getMsgError($query)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 109](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L109)


#### Arguments
* $query **mixed**



### <a name="method-getNumberError"></a>getNumberError

```php
mixed DbMySQLiCore::getNumberError()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L117)




### <a name="method-getRow"></a>getRow

```php
array DbCore::getRow(mixed $sql, boolean $use_cache)
```

getRow return an associative array containing the first row of the query
This function automatically add "limit 1" to the query



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 507](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L507)


#### Arguments
* $sql **mixed** - the select query (without &quot;LIMIT 1&quot;)
* $use_cache **boolean** - find it in cache first



### <a name="method-getValue"></a>getValue

```php
mixed DbCore::getValue(mixed $sql, boolean $use_cache)
```

getValue return the first item of a select query.



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 539](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L539)


#### Arguments
* $sql **mixed**
* $use_cache **boolean**



### <a name="method-getVersion"></a>getVersion

```php
mixed DbMySQLiCore::getVersion()
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 125](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L125)




### <a name="method-hasTableWithSamePrefix"></a>hasTableWithSamePrefix

```php
mixed DbMySQLiCore::hasTableWithSamePrefix($server, $user, $pwd, $db, $prefix)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 149](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L149)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $prefix **mixed**



### <a name="method-insert"></a>insert

```php
boolean DbCore::insert(string $table, array $data, boolean $null_values, boolean $use_cache, integer $type, boolean $add_prefix)
```

Execute an INSERT query



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 322](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L322)


#### Arguments
* $table **string** - Table name without prefix
* $data **array** - Data to insert as associative array. If $data is a list of arrays, multiple insert will be done
* $null_values **boolean** - If we want to use NULL values instead of empty quotes
* $use_cache **boolean**
* $type **integer** - Must be Db::INSERT or Db::INSERT_IGNORE or Db::REPLACE
* $add_prefix **boolean** - Add or not _DB_PREFIX_ before table name



### <a name="method-nextRow"></a>nextRow

```php
mixed DbMySQLiCore::nextRow($result)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L75)


#### Arguments
* $result **mixed**



### <a name="method-numRows"></a>numRows

```php
integer DbCore::numRows()
```

Get number of rows for last result



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 554](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L554)




### <a name="method-ps"></a>ps

```php
mixed DbCore::ps($sql, $use_cache)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 694](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L694)


#### Arguments
* $sql **mixed**
* $use_cache **mixed**



### <a name="method-q"></a>q

```php
mixed DbCore::q(string $sql, boolean $use_cache)
```

Execute a query



* Visibility: **protected**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 575](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L575)


#### Arguments
* $sql **string**
* $use_cache **boolean**



### <a name="method-query"></a>query

```php
mixed DbCore::query(string $sql)
```

Execute a query and get result ressource



* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 300](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L300)


#### Arguments
* $sql **string**



### <a name="method-s"></a>s

```php
mixed DbCore::s($sql, $use_cache)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 685](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L685)


#### Arguments
* $sql **mixed**
* $use_cache **mixed**



### <a name="method-set_db"></a>set_db

```php
mixed DbMySQLiCore::set_db($db_name)
```





* Visibility: **public**
* Source: [classes/db/DbMySQLi.php line 141](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L141)


#### Arguments
* $db_name **mixed**



### <a name="method-tryToConnect"></a>tryToConnect

```php
mixed DbMySQLiCore::tryToConnect($server, $user, $pwd, $db, $newDbLink, $engine, $timeout)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 163](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L163)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**
* $db **mixed**
* $newDbLink **mixed**
* $engine **mixed**
* $timeout **mixed**



### <a name="method-tryUTF8"></a>tryUTF8

```php
mixed DbMySQLiCore::tryUTF8($server, $user, $pwd)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/db/DbMySQLi.php line 211](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/DbMySQLi.php#L211)


#### Arguments
* $server **mixed**
* $user **mixed**
* $pwd **mixed**



### <a name="method-update"></a>update

```php
boolean DbCore::update(string $table, array $data, string $where, integer $limit, boolean $null_values, boolean $use_cache, boolean $add_prefix)
```





* Visibility: **public**
* This method is defined by [DbCore](class.DbCore.md).
* Source: [classes/db/Db.php line 385](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.1/classes/db/Db.php#L385)


#### Arguments
* $table **string** - Table name without prefix
* $data **array** - Data to insert as associative array. If $data is a list of arrays, multiple insert will be done
* $where **string** - WHERE condition
* $limit **integer**
* $null_values **boolean** - If we want to use NULL values instead of empty quotes
* $use_cache **boolean**
* $add_prefix **boolean** - Add or not _DB_PREFIX_ before table name


