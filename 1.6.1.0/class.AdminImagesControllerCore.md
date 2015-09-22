Class AdminImagesControllerCore
=====================





* Class name: AdminImagesControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminImagesController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L30)


Contents
--------


### Properties

* [$display_move](#property-$display_move)
* [$max_execution_time](#property-$max_execution_time)
* [$object](#property-$object)
* [$start_time](#property-$start_time)

### Methods

* [__construct](#method-__construct)
* [_childValidation](#method-_childValidation)
* [_deleteOldImages](#method-_deleteOldImages)
* [_moveImagesToNewFileSystem](#method-_moveImagesToNewFileSystem)
* [_regenerateNewImages](#method-_regenerateNewImages)
* [_regenerateNoPictureImages](#method-_regenerateNoPictureImages)
* [_regenerateThumbnails](#method-_regenerateThumbnails)
* [_regenerateWatermark](#method-_regenerateWatermark)
* [initContent](#method-initContent)
* [initMoveImages](#method-initMoveImages)
* [initPageHeaderToolbar](#method-initPageHeaderToolbar)
* [initRegenerate](#method-initRegenerate)
* [postProcess](#method-postProcess)
* [printEntityActiveIcon](#method-printEntityActiveIcon)




Properties
----------


### <a name="property-$display_move"></a>$display_move

```php
protected mixed $display_move
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L34).


### <a name="property-$max_execution_time"></a>$max_execution_time

```php
protected mixed $max_execution_time = 7200
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L33).


### <a name="property-$object"></a>$object

```php
public \ImageType $object
```





* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L30).


### <a name="property-$start_time"></a>$start_time

```php
protected mixed $start_time
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L32).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed AdminImagesControllerCore::__construct()
```





* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L36)




### <a name="method-_childValidation"></a>_childValidation

```php
mixed AdminImagesControllerCore::_childValidation()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 412](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L412)




### <a name="method-_deleteOldImages"></a>_deleteOldImages

```php
boolean AdminImagesControllerCore::_deleteOldImages(string $dir, array $type, boolean $product)
```

Delete resized image then regenerate new one with updated settings



* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 451](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L451)


#### Arguments
* $dir **string**
* $type **array**
* $product **boolean**



### <a name="method-_moveImagesToNewFileSystem"></a>_moveImagesToNewFileSystem

```php
mixed AdminImagesControllerCore::_moveImagesToNewFileSystem()
```

Move product images to the new filesystem



* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 706](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L706)




### <a name="method-_regenerateNewImages"></a>_regenerateNewImages

```php
boolean|string AdminImagesControllerCore::_regenerateNewImages($dir, $type, boolean $productsImages)
```

Regenerate images



* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 494](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L494)


#### Arguments
* $dir **mixed**
* $type **mixed**
* $productsImages **boolean**



### <a name="method-_regenerateNoPictureImages"></a>_regenerateNoPictureImages

```php
boolean AdminImagesControllerCore::_regenerateNoPictureImages($dir, $type, $languages)
```

Regenerate no-pictures images



* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 572](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L572)


#### Arguments
* $dir **mixed**
* $type **mixed**
* $languages **mixed**



### <a name="method-_regenerateThumbnails"></a>_regenerateThumbnails

```php
mixed AdminImagesControllerCore::_regenerateThumbnails($type, $deleteOldImages)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 625](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L625)


#### Arguments
* $type **mixed**
* $deleteOldImages **mixed**



### <a name="method-_regenerateWatermark"></a>_regenerateWatermark

```php
mixed AdminImagesControllerCore::_regenerateWatermark($dir, $type)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminImagesController.php line 597](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L597)


#### Arguments
* $dir **mixed**
* $type **mixed**



### <a name="method-initContent"></a>initContent

```php
mixed AdminImagesControllerCore::initContent()
```





* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 723](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L723)




### <a name="method-initMoveImages"></a>initMoveImages

```php
mixed AdminImagesControllerCore::initMoveImages()
```

Init display for move images block



* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 683](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L683)




### <a name="method-initPageHeaderToolbar"></a>initPageHeaderToolbar

```php
mixed AdminImagesControllerCore::initPageHeaderToolbar()
```





* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 691](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L691)




### <a name="method-initRegenerate"></a>initRegenerate

```php
mixed AdminImagesControllerCore::initRegenerate()
```

Init display for the thumbnails regeneration block



* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 421](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L421)




### <a name="method-postProcess"></a>postProcess

```php
mixed AdminImagesControllerCore::postProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminImagesController.php line 356](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L356)




### <a name="method-printEntityActiveIcon"></a>printEntityActiveIcon

```php
mixed AdminImagesControllerCore::printEntityActiveIcon($value, $object)
```





* Visibility: **public**
* This method is **static**.
* Source: [controllers/admin/AdminImagesController.php line 407](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.0/controllers/admin/AdminImagesController.php#L407)


#### Arguments
* $value **mixed**
* $object **mixed**

