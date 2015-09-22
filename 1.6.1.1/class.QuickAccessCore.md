Class QuickAccessCore
=====================





* Class name: QuickAccessCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/QuickAccess.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L27)



Properties
----------

* [$definition](#property-$definition)
* [$link](#property-$link)
* [$name](#property-$name)
* [$new_window](#property-$new_window)

Methods
-------
* [getQuickAccesses](#method-getQuickAccesses)
* [toggleNewWindow](#method-toggleNewWindow)




Properties
----------


### <a name="property-$definition"></a>$definition

    public mixed $definition = array('table' => 'quick_access', 'primary' => 'id_quick_access', 'multilang' => true, 'fields' => array('link' => array('type' => self::TYPE_STRING, 'validate' => 'isUrl', 'required' => true, 'size' => 255), 'new_window' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool', 'required' => true), 'name' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isCleanHtml', 'required' => true, 'size' => 32)))





* Visibility: **public**
* This property is **static**.
* Source: [classes/QuickAccess.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L41).


### <a name="property-$link"></a>$link

    public string $link





* Visibility: **public**
* Source: [classes/QuickAccess.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L33).


### <a name="property-$name"></a>$name

    public string $name





* Visibility: **public**
* Source: [classes/QuickAccess.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L30).


### <a name="property-$new_window"></a>$new_window

    public boolean $new_window





* Visibility: **public**
* Source: [classes/QuickAccess.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L36).


Methods
-------


### <a name="method-getQuickAccesses"></a>getQuickAccesses

    array QuickAccessCore::getQuickAccesses($id_lang)

Get all available quick_accesses



* Visibility: **public**
* This method is **static**.
* Source: [classes/QuickAccess.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L59)


#### Arguments
* $id_lang **mixed**



### <a name="method-toggleNewWindow"></a>toggleNewWindow

    mixed QuickAccessCore::toggleNewWindow()





* Visibility: **public**
* Source: [classes/QuickAccess.php line 68](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/QuickAccess.php#L68)


