Class GroupReductionCore
=====================





* Class name: GroupReductionCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/GroupReduction.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L27)



Properties
----------

* [$definition](#property-$definition)
* [$id_category](#property-$id_category)
* [$id_group](#property-$id_group)
* [$reduction](#property-$reduction)
* [$reduction_cache](#property-$reduction_cache)

Methods
-------
* [_clearCache](#method-_clearCache)
* [_setCache](#method-_setCache)
* [_updateCache](#method-_updateCache)
* [add](#method-add)
* [delete](#method-delete)
* [deleteCategory](#method-deleteCategory)
* [deleteProductReduction](#method-deleteProductReduction)
* [doesExist](#method-doesExist)
* [duplicateReduction](#method-duplicateReduction)
* [getGroupByCategoryId](#method-getGroupByCategoryId)
* [getGroupReductionByCategoryId](#method-getGroupReductionByCategoryId)
* [getGroupReductions](#method-getGroupReductions)
* [getGroupsByCategoryId](#method-getGroupsByCategoryId)
* [getGroupsReductionByCategoryId](#method-getGroupsReductionByCategoryId)
* [getValueForProduct](#method-getValueForProduct)
* [setProductReduction](#method-setProductReduction)
* [update](#method-update)




Properties
----------


### <a name="property-$definition"></a>$definition

    public mixed $definition = array('table' => 'group_reduction', 'primary' => 'id_group_reduction', 'fields' => array('id_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_category' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'reduction' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true)))





* Visibility: **public**
* This property is **static**.
* Source: [classes/GroupReduction.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L36).


### <a name="property-$id_category"></a>$id_category

    public mixed $id_category





* Visibility: **public**
* Source: [classes/GroupReduction.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L30).


### <a name="property-$id_group"></a>$id_group

    public mixed $id_group





* Visibility: **public**
* Source: [classes/GroupReduction.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L29).


### <a name="property-$reduction"></a>$reduction

    public mixed $reduction





* Visibility: **public**
* Source: [classes/GroupReduction.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L31).


### <a name="property-$reduction_cache"></a>$reduction_cache

    protected mixed $reduction_cache = array()





* Visibility: **protected**
* This property is **static**.
* Source: [classes/GroupReduction.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L46).


Methods
-------


### <a name="method-_clearCache"></a>_clearCache

    mixed GroupReductionCore::_clearCache()





* Visibility: **protected**
* Source: [classes/GroupReduction.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L77)




### <a name="method-_setCache"></a>_setCache

    mixed GroupReductionCore::_setCache()





* Visibility: **protected**
* Source: [classes/GroupReduction.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L82)




### <a name="method-_updateCache"></a>_updateCache

    mixed GroupReductionCore::_updateCache()





* Visibility: **protected**
* Source: [classes/GroupReduction.php line 105](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L105)




### <a name="method-add"></a>add

    mixed GroupReductionCore::add($autodate, $null_values)





* Visibility: **public**
* Source: [classes/GroupReduction.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L48)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-delete"></a>delete

    mixed GroupReductionCore::delete()





* Visibility: **public**
* Source: [classes/GroupReduction.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L58)




### <a name="method-deleteCategory"></a>deleteCategory

    mixed GroupReductionCore::deleteCategory($id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 262](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L262)


#### Arguments
* $id_category **mixed**



### <a name="method-deleteProductReduction"></a>deleteProductReduction

    mixed GroupReductionCore::deleteProductReduction($id_product)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 231](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L231)


#### Arguments
* $id_product **mixed**



### <a name="method-doesExist"></a>doesExist

    mixed GroupReductionCore::doesExist($id_group, $id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 155](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L155)


#### Arguments
* $id_group **mixed**
* $id_category **mixed**



### <a name="method-duplicateReduction"></a>duplicateReduction

    mixed GroupReductionCore::duplicateReduction($id_product_old, $id_product)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 240](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L240)


#### Arguments
* $id_product_old **mixed**
* $id_product **mixed**



### <a name="method-getGroupByCategoryId"></a>getGroupByCategoryId

    array|null GroupReductionCore::getGroupByCategoryId(integer $id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 177](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L177)


#### Arguments
* $id_category **integer**



### <a name="method-getGroupReductionByCategoryId"></a>getGroupReductionByCategoryId

    array|null GroupReductionCore::getGroupReductionByCategoryId(integer $id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 200](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L200)


#### Arguments
* $id_category **integer**



### <a name="method-getGroupReductions"></a>getGroupReductions

    mixed GroupReductionCore::getGroupReductions($id_group, $id_lang)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 128](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L128)


#### Arguments
* $id_group **mixed**
* $id_lang **mixed**



### <a name="method-getGroupsByCategoryId"></a>getGroupsByCategoryId

    mixed GroupReductionCore::getGroupsByCategoryId($id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 163](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L163)


#### Arguments
* $id_category **mixed**



### <a name="method-getGroupsReductionByCategoryId"></a>getGroupsReductionByCategoryId

    mixed GroupReductionCore::getGroupsReductionByCategoryId($id_category)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 186](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L186)


#### Arguments
* $id_category **mixed**



### <a name="method-getValueForProduct"></a>getValueForProduct

    mixed GroupReductionCore::getValueForProduct($id_product, $id_group)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 139](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L139)


#### Arguments
* $id_product **mixed**
* $id_group **mixed**



### <a name="method-setProductReduction"></a>setProductReduction

    mixed GroupReductionCore::setProductReduction($id_product, $id_group, $id_category, $reduction)





* Visibility: **public**
* This method is **static**.
* Source: [classes/GroupReduction.php line 209](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L209)


#### Arguments
* $id_product **mixed**
* $id_group **mixed**
* $id_category **mixed**
* $reduction **mixed**



### <a name="method-update"></a>update

    mixed GroupReductionCore::update($null_values)





* Visibility: **public**
* Source: [classes/GroupReduction.php line 53](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/GroupReduction.php#L53)


#### Arguments
* $null_values **mixed**

