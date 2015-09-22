Class ProfileCore
=====================





* Class name: ProfileCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/Profile.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L27)



Properties
----------

* [$_cache_accesses](#property-$_cache_accesses)
* [$definition](#property-$definition)
* [$name](#property-$name)

Methods
-------
* [add](#method-add)
* [delete](#method-delete)
* [getProfile](#method-getProfile)
* [getProfileAccess](#method-getProfileAccess)
* [getProfileAccesses](#method-getProfileAccesses)
* [getProfiles](#method-getProfiles)




Properties
----------


### <a name="property-$_cache_accesses"></a>$_cache_accesses

    protected mixed $_cache_accesses = array()





* Visibility: **protected**
* This property is **static**.
* Source: [classes/Profile.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L45).


### <a name="property-$definition"></a>$definition

    public mixed $definition = array('table' => 'profile', 'primary' => 'id_profile', 'multilang' => true, 'fields' => array('name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 32)))





* Visibility: **public**
* This property is **static**.
* Source: [classes/Profile.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L35).


### <a name="property-$name"></a>$name

    public string $name





* Visibility: **public**
* Source: [classes/Profile.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L30).


Methods
-------


### <a name="method-add"></a>add

    mixed ProfileCore::add($autodate, $null_values)





* Visibility: **public**
* Source: [classes/Profile.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L81)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-delete"></a>delete

    mixed ProfileCore::delete()





* Visibility: **public**
* Source: [classes/Profile.php line 95](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L95)




### <a name="method-getProfile"></a>getProfile

    string ProfileCore::getProfile($id_profile, $id_lang)

Get the current profile name



* Visibility: **public**
* This method is **static**.
* Source: [classes/Profile.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L66)


#### Arguments
* $id_profile **mixed**
* $id_lang **mixed**



### <a name="method-getProfileAccess"></a>getProfileAccess

    mixed ProfileCore::getProfileAccess($id_profile, $id_tab)





* Visibility: **public**
* This method is **static**.
* Source: [classes/Profile.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L106)


#### Arguments
* $id_profile **mixed**
* $id_tab **mixed**



### <a name="method-getProfileAccesses"></a>getProfileAccesses

    mixed ProfileCore::getProfileAccesses($id_profile, $type)





* Visibility: **public**
* This method is **static**.
* Source: [classes/Profile.php line 113](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L113)


#### Arguments
* $id_profile **mixed**
* $type **mixed**



### <a name="method-getProfiles"></a>getProfiles

    array ProfileCore::getProfiles($id_lang)

Get all available profiles



* Visibility: **public**
* This method is **static**.
* Source: [classes/Profile.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/Profile.php#L52)


#### Arguments
* $id_lang **mixed**

