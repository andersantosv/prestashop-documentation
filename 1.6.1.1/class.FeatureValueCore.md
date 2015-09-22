Class FeatureValueCore
=====================





* Class name: FeatureValueCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/FeatureValue.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L27)



Properties
----------

* [$custom](#property-$custom)
* [$definition](#property-$definition)
* [$id_feature](#property-$id_feature)
* [$value](#property-$value)
* [$webserviceParameters](#property-$webserviceParameters)

Methods
-------
* [add](#method-add)
* [addFeatureValueImport](#method-addFeatureValueImport)
* [delete](#method-delete)
* [getFeatureValueLang](#method-getFeatureValueLang)
* [getFeatureValues](#method-getFeatureValues)
* [getFeatureValuesWithLang](#method-getFeatureValuesWithLang)
* [selectLang](#method-selectLang)
* [update](#method-update)




Properties
----------


### <a name="property-$custom"></a>$custom

    public boolean $custom





* Visibility: **public**
* Source: [classes/FeatureValue.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L36).


### <a name="property-$definition"></a>$definition

    public mixed $definition = array('table' => 'feature_value', 'primary' => 'id_feature_value', 'multilang' => true, 'fields' => array('id_feature' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'custom' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'value' => array('type' => self::TYPE_STRING, 'lang' => true, 'validate' => 'isGenericName', 'required' => true, 'size' => 255)))





* Visibility: **public**
* This property is **static**.
* Source: [classes/FeatureValue.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L41).


### <a name="property-$id_feature"></a>$id_feature

    public integer $id_feature





* Visibility: **public**
* Source: [classes/FeatureValue.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L30).


### <a name="property-$value"></a>$value

    public string $value





* Visibility: **public**
* Source: [classes/FeatureValue.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L33).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

    protected mixed $webserviceParameters = array('objectsNodeName' => 'product_feature_values', 'objectNodeName' => 'product_feature_value', 'fields' => array('id_feature' => array('xlink_resource' => 'product_features')))





* Visibility: **protected**
* Source: [classes/FeatureValue.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L54).


Methods
-------


### <a name="method-add"></a>add

    mixed FeatureValueCore::add($autodate, $nullValues)





* Visibility: **public**
* Source: [classes/FeatureValue.php line 176](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L176)


#### Arguments
* $autodate **mixed**
* $nullValues **mixed**



### <a name="method-addFeatureValueImport"></a>addFeatureValueImport

    mixed FeatureValueCore::addFeatureValueImport($id_feature, $value, $id_product, $id_lang, $custom)





* Visibility: **public**
* This method is **static**.
* Source: [classes/FeatureValue.php line 129](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L129)


#### Arguments
* $id_feature **mixed**
* $value **mixed**
* $id_product **mixed**
* $id_lang **mixed**
* $custom **mixed**



### <a name="method-delete"></a>delete

    mixed FeatureValueCore::delete()





* Visibility: **public**
* Source: [classes/FeatureValue.php line 185](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L185)




### <a name="method-getFeatureValueLang"></a>getFeatureValueLang

    array FeatureValueCore::getFeatureValueLang(boolean $id_feature_value)

Get all language for a given value



* Visibility: **public**
* This method is **static**.
* Source: [classes/FeatureValue.php line 103](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L103)


#### Arguments
* $id_feature_value **boolean** - Feature value id



### <a name="method-getFeatureValues"></a>getFeatureValues

    array FeatureValueCore::getFeatureValues(boolean $id_feature)

Get all values for a given feature



* Visibility: **public**
* This method is **static**.
* Source: [classes/FeatureValue.php line 68](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L68)


#### Arguments
* $id_feature **boolean** - Feature id



### <a name="method-getFeatureValuesWithLang"></a>getFeatureValuesWithLang

    array FeatureValueCore::getFeatureValuesWithLang(integer $id_lang, boolean $id_feature, $custom)

Get all values for a given feature and language



* Visibility: **public**
* This method is **static**.
* Source: [classes/FeatureValue.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L84)


#### Arguments
* $id_lang **integer** - Language id
* $id_feature **boolean** - Feature id
* $custom **mixed**



### <a name="method-selectLang"></a>selectLang

    string FeatureValueCore::selectLang(array $lang, integer $id_lang)

Select the good lang in tab



* Visibility: **public**
* This method is **static**.
* Source: [classes/FeatureValue.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L120)


#### Arguments
* $lang **array** - Array with all language
* $id_lang **integer** - Language id



### <a name="method-update"></a>update

    mixed FeatureValueCore::update($nullValues)





* Visibility: **public**
* Source: [classes/FeatureValue.php line 200](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/FeatureValue.php#L200)


#### Arguments
* $nullValues **mixed**

