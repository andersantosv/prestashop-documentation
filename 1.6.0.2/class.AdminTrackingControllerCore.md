Class AdminTrackingControllerCore
=====================





* Class name: AdminTrackingControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminTrackingController.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L27)


Contents
--------


### Properties

* [$_helper_list](#property-$_helper_list)
* [$bootstrap](#property-$bootstrap)

### Methods

* [clearFilters](#method-clearFilters)
* [clearListOptions](#method-clearListOptions)
* [displayDeleteLink](#method-displayDeleteLink)
* [displayEditLink](#method-displayEditLink)
* [displayEnableLink](#method-displayEnableLink)
* [getCustomListCategoriesEmpty](#method-getCustomListCategoriesEmpty)
* [getCustomListProductsAttributesNoStock](#method-getCustomListProductsAttributesNoStock)
* [getCustomListProductsDisabled](#method-getCustomListProductsDisabled)
* [getCustomListProductsNoStock](#method-getCustomListProductsNoStock)
* [getList](#method-getList)
* [initContent](#method-initContent)
* [postprocess](#method-postprocess)
* [renderList](#method-renderList)




Properties
----------


### <a name="property-$_helper_list"></a>$_helper_list

```php
protected mixed $_helper_list
```





* Visibility: **protected**
* Source: [controllers/admin/AdminTrackingController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L30).


### <a name="property-$bootstrap"></a>$bootstrap

```php
public mixed $bootstrap = true
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L29).


Methods
-------


### <a name="method-clearFilters"></a>clearFilters

```php
mixed AdminTrackingControllerCore::clearFilters()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminTrackingController.php line 270](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L270)




### <a name="method-clearListOptions"></a>clearListOptions

```php
mixed AdminTrackingControllerCore::clearListOptions()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 285](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L285)




### <a name="method-displayDeleteLink"></a>displayDeleteLink

```php
mixed AdminTrackingControllerCore::displayDeleteLink($token, $id, $name)
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 252](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L252)


#### Arguments
* $token **mixed**
* $id **mixed**
* $name **mixed**



### <a name="method-displayEditLink"></a>displayEditLink

```php
mixed AdminTrackingControllerCore::displayEditLink($token, $id, $name)
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 261](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L261)


#### Arguments
* $token **mixed**
* $id **mixed**
* $name **mixed**



### <a name="method-displayEnableLink"></a>displayEnableLink

```php
mixed AdminTrackingControllerCore::displayEnableLink($token, $id, $value, $active, $id_category, $id_product)
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 243](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L243)


#### Arguments
* $token **mixed**
* $id **mixed**
* $value **mixed**
* $active **mixed**
* $id_category **mixed**
* $id_product **mixed**



### <a name="method-getCustomListCategoriesEmpty"></a>getCustomListCategoriesEmpty

```php
mixed AdminTrackingControllerCore::getCustomListCategoriesEmpty()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L84)




### <a name="method-getCustomListProductsAttributesNoStock"></a>getCustomListProductsAttributesNoStock

```php
mixed AdminTrackingControllerCore::getCustomListProductsAttributesNoStock()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L120)




### <a name="method-getCustomListProductsDisabled"></a>getCustomListProductsDisabled

```php
mixed AdminTrackingControllerCore::getCustomListProductsDisabled()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 206](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L206)




### <a name="method-getCustomListProductsNoStock"></a>getCustomListProductsNoStock

```php
mixed AdminTrackingControllerCore::getCustomListProductsNoStock()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 163](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L163)




### <a name="method-getList"></a>getList

```php
mixed AdminTrackingControllerCore::getList($id_lang, $order_by, $order_way, $start, $limit, $id_lang_shop)
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 300](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L300)


#### Arguments
* $id_lang **mixed**
* $order_by **mixed**
* $order_way **mixed**
* $start **mixed**
* $limit **mixed**
* $id_lang_shop **mixed**



### <a name="method-initContent"></a>initContent

```php
mixed AdminTrackingControllerCore::initContent()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L54)




### <a name="method-postprocess"></a>postprocess

```php
mixed AdminTrackingControllerCore::postprocess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L32)




### <a name="method-renderList"></a>renderList

```php
mixed AdminTrackingControllerCore::renderList()
```





* Visibility: **public**
* Source: [controllers/admin/AdminTrackingController.php line 237](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.2/controllers/admin/AdminTrackingController.php#L237)


