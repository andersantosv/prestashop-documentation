Class OrderOpcControllerCore
=====================





* Class name: OrderOpcControllerCore
* Parent class: [ParentOrderController](class.ParentOrderControllerCore.md)
* Source: [controllers/front/OrderOpcController.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L27)


Contents
--------


### Properties

* [$ajax_refresh](#property-$ajax_refresh)
* [$isLogged](#property-$isLogged)
* [$php_self](#property-$php_self)
* [$nbProducts](#property-$nbProducts)
* [$ssl](#property-$ssl)
* [$auth](#property-$auth)
* [$authRedirection](#property-$authRedirection)
* [$cart](#property-$cart)
* [$cookie](#property-$cookie)
* [$currentCustomerGroups](#property-$currentCustomerGroups)
* [$display_column_left](#property-$display_column_left)
* [$display_column_right](#property-$display_column_right)
* [$errors](#property-$errors)
* [$guestAllowed](#property-$guestAllowed)
* [$initialized](#property-$initialized)
* [$iso](#property-$iso)
* [$link](#property-$link)
* [$maintenance](#property-$maintenance)
* [$n](#property-$n)
* [$nb_items_per_page](#property-$nb_items_per_page)
* [$orderBy](#property-$orderBy)
* [$orderWay](#property-$orderWay)
* [$p](#property-$p)
* [$restrictedCountry](#property-$restrictedCountry)
* [$smarty](#property-$smarty)
* [$ajax](#property-$ajax)
* [$content_only](#property-$content_only)
* [$context](#property-$context)
* [$controller_type](#property-$controller_type)
* [$css_files](#property-$css_files)
* [$display_footer](#property-$display_footer)
* [$display_header](#property-$display_header)
* [$js_files](#property-$js_files)
* [$json](#property-$json)
* [$php_errors](#property-$php_errors)
* [$redirect_after](#property-$redirect_after)
* [$status](#property-$status)
* [$template](#property-$template)

### Methods

* [__construct](#method-__construct)
* [_assignAddress](#method-_assignAddress)
* [_assignCarrier](#method-_assignCarrier)
* [_assignPayment](#method-_assignPayment)
* [_assignSummaryInformations](#method-_assignSummaryInformations)
* [_assignWrappingAndTOS](#method-_assignWrappingAndTOS)
* [_checkFreeOrder](#method-_checkFreeOrder)
* [_getCarrierList](#method-_getCarrierList)
* [_getGuestInformations](#method-_getGuestInformations)
* [_getPaymentMethods](#method-_getPaymentMethods)
* [_processAddressFormat](#method-_processAddressFormat)
* [_processCarrier](#method-_processCarrier)
* [_setDefaultCarrierSelection](#method-_setDefaultCarrierSelection)
* [_updateMessage](#method-_updateMessage)
* [addCSS](#method-addCSS)
* [addColorsToProductList](#method-addColorsToProductList)
* [addJS](#method-addJS)
* [addJquery](#method-addJquery)
* [addJqueryPlugin](#method-addJqueryPlugin)
* [addJqueryUI](#method-addJqueryUI)
* [addMedia](#method-addMedia)
* [ajaxDie](#method-ajaxDie)
* [canonicalRedirection](#method-canonicalRedirection)
* [checkAccess](#method-checkAccess)
* [checkLiveEditAccess](#method-checkLiveEditAccess)
* [display](#method-display)
* [displayContent](#method-displayContent)
* [displayFooter](#method-displayFooter)
* [displayHeader](#method-displayHeader)
* [displayMaintenancePage](#method-displayMaintenancePage)
* [displayRestrictedCountryPage](#method-displayRestrictedCountryPage)
* [geolocationManagement](#method-geolocationManagement)
* [getColorsListCacheId](#method-getColorsListCacheId)
* [getController](#method-getController)
* [getCurrentCustomerGroups](#method-getCurrentCustomerGroups)
* [getFormatedSummaryDetail](#method-getFormatedSummaryDetail)
* [getLayout](#method-getLayout)
* [getLiveEditFooter](#method-getLiveEditFooter)
* [getOverrideTemplate](#method-getOverrideTemplate)
* [getOverrideThemeDir](#method-getOverrideThemeDir)
* [getTemplatePath](#method-getTemplatePath)
* [getThemeDir](#method-getThemeDir)
* [init](#method-init)
* [initContent](#method-initContent)
* [initCursedPage](#method-initCursedPage)
* [initFooter](#method-initFooter)
* [initHeader](#method-initHeader)
* [initLogoAndFavicon](#method-initLogoAndFavicon)
* [isCached](#method-isCached)
* [isInWhitelistForGeolocation](#method-isInWhitelistForGeolocation)
* [isTokenValid](#method-isTokenValid)
* [isXmlHttpRequest](#method-isXmlHttpRequest)
* [myErrorHandler](#method-myErrorHandler)
* [pagination](#method-pagination)
* [postProcess](#method-postProcess)
* [process](#method-process)
* [productSort](#method-productSort)
* [recoverCart](#method-recoverCart)
* [redirect](#method-redirect)
* [removeCSS](#method-removeCSS)
* [removeJS](#method-removeJS)
* [removeMedia](#method-removeMedia)
* [run](#method-run)
* [setDefaultCarrierSelection](#method-setDefaultCarrierSelection)
* [setMedia](#method-setMedia)
* [setMobileMedia](#method-setMobileMedia)
* [setMobileTemplate](#method-setMobileTemplate)
* [setNoCarrier](#method-setNoCarrier)
* [setTemplate](#method-setTemplate)
* [smartyOutputContent](#method-smartyOutputContent)
* [sslRedirection](#method-sslRedirection)
* [useMobileTheme](#method-useMobileTheme)
* [validateDeliveryOption](#method-validateDeliveryOption)
* [viewAccess](#method-viewAccess)




Properties
----------


### <a name="property-$ajax_refresh"></a>$ajax_refresh

```php
protected mixed $ajax_refresh = false
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L32).


### <a name="property-$isLogged"></a>$isLogged

```php
public mixed $isLogged
```





* Visibility: **public**
* Source: [controllers/front/OrderOpcController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L30).


### <a name="property-$php_self"></a>$php_self

```php
public mixed $php_self = 'order-opc'
```





* Visibility: **public**
* Source: [controllers/front/OrderOpcController.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L29).


### <a name="property-$nbProducts"></a>$nbProducts

```php
public mixed $nbProducts
```





* Visibility: **public**
* This property is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L42).


### <a name="property-$ssl"></a>$ssl

```php
public mixed $ssl = true
```





* Visibility: **public**
* This property is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L39).


### <a name="property-$auth"></a>$auth

```php
public mixed $auth = false
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L43).


### <a name="property-$authRedirection"></a>$authRedirection

```php
public mixed $authRedirection = false
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L45).


### <a name="property-$cart"></a>$cart

```php
protected mixed $cart
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L34).


### <a name="property-$cookie"></a>$cookie

```php
protected mixed $cookie
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L34).


### <a name="property-$currentCustomerGroups"></a>$currentCustomerGroups

```php
protected mixed $currentCustomerGroups
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L56).


### <a name="property-$display_column_left"></a>$display_column_left

```php
public mixed $display_column_left = true
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L51).


### <a name="property-$display_column_right"></a>$display_column_right

```php
public mixed $display_column_right = true
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L52).


### <a name="property-$errors"></a>$errors

```php
public mixed $errors = array()
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L29).


### <a name="property-$guestAllowed"></a>$guestAllowed

```php
public mixed $guestAllowed = false
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 44](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L44).


### <a name="property-$initialized"></a>$initialized

```php
public mixed $initialized = false
```





* Visibility: **public**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L54).


### <a name="property-$iso"></a>$iso

```php
public mixed $iso
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L36).


### <a name="property-$link"></a>$link

```php
protected mixed $link
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L34).


### <a name="property-$maintenance"></a>$maintenance

```php
protected mixed $maintenance = false
```





* Visibility: **protected**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L49).


### <a name="property-$n"></a>$n

```php
public mixed $n
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L41).


### <a name="property-$nb_items_per_page"></a>$nb_items_per_page

```php
public mixed $nb_items_per_page
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L58).


### <a name="property-$orderBy"></a>$orderBy

```php
public mixed $orderBy
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L38).


### <a name="property-$orderWay"></a>$orderWay

```php
public mixed $orderWay
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L39).


### <a name="property-$p"></a>$p

```php
public mixed $p
```





* Visibility: **public**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L40).


### <a name="property-$restrictedCountry"></a>$restrictedCountry

```php
protected mixed $restrictedCountry = false
```





* Visibility: **protected**
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L48).


### <a name="property-$smarty"></a>$smarty

```php
protected mixed $smarty
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L34).


### <a name="property-$ajax"></a>$ajax

```php
public boolean $ajax = false
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L75).


### <a name="property-$content_only"></a>$content_only

```php
protected string $content_only = false
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L70).


### <a name="property-$context"></a>$context

```php
protected \Context $context
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L35).


### <a name="property-$controller_type"></a>$controller_type

```php
public mixed $controller_type
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L81).


### <a name="property-$css_files"></a>$css_files

```php
public array $css_files = array()
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L40).


### <a name="property-$display_footer"></a>$display_footer

```php
protected string $display_footer
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L65).


### <a name="property-$display_header"></a>$display_header

```php
protected boolean $display_header
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L55).


### <a name="property-$js_files"></a>$js_files

```php
public array $js_files = array()
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L45).


### <a name="property-$json"></a>$json

```php
protected mixed $json = false
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L76).


### <a name="property-$php_errors"></a>$php_errors

```php
public array $php_errors = array()
```





* Visibility: **public**
* This property is **static**.
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L50).


### <a name="property-$redirect_after"></a>$redirect_after

```php
protected mixed $redirect_after = null
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L79).


### <a name="property-$status"></a>$status

```php
protected mixed $status = ''
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 77](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L77).


### <a name="property-$template"></a>$template

```php
protected string $template
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L60).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed FrontControllerCore::__construct()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L60)




### <a name="method-_assignAddress"></a>_assignAddress

```php
mixed ParentOrderControllerCore::_assignAddress()
```





* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 385](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L385)




### <a name="method-_assignCarrier"></a>_assignCarrier

```php
mixed OrderOpcControllerCore::_assignCarrier()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 486](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L486)




### <a name="method-_assignPayment"></a>_assignPayment

```php
mixed OrderOpcControllerCore::_assignPayment()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 508](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L508)




### <a name="method-_assignSummaryInformations"></a>_assignSummaryInformations

```php
mixed ParentOrderControllerCore::_assignSummaryInformations()
```





* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 289](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L289)




### <a name="method-_assignWrappingAndTOS"></a>_assignWrappingAndTOS

```php
mixed ParentOrderControllerCore::_assignWrappingAndTOS()
```





* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 521](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L521)




### <a name="method-_checkFreeOrder"></a>_checkFreeOrder

```php
boolean ParentOrderControllerCore::_checkFreeOrder()
```

Check if order is free



* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 169](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L169)




### <a name="method-_getCarrierList"></a>_getCarrierList

```php
mixed OrderOpcControllerCore::_getCarrierList()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 569](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L569)




### <a name="method-_getGuestInformations"></a>_getGuestInformations

```php
mixed OrderOpcControllerCore::_getGuestInformations()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 418](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L418)




### <a name="method-_getPaymentMethods"></a>_getPaymentMethods

```php
mixed OrderOpcControllerCore::_getPaymentMethods()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 516](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L516)




### <a name="method-_processAddressFormat"></a>_processAddressFormat

```php
mixed OrderOpcControllerCore::_processAddressFormat()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 655](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L655)




### <a name="method-_processCarrier"></a>_processCarrier

```php
mixed ParentOrderControllerCore::_processCarrier()
```





* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 213](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L213)




### <a name="method-_setDefaultCarrierSelection"></a>_setDefaultCarrierSelection

```php
\number ParentOrderControllerCore::_setDefaultCarrierSelection(array $carriers)
```

Decides what the default carrier is and update the cart with it



* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 606](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L606)


#### Arguments
* $carriers **array**



### <a name="method-_updateMessage"></a>_updateMessage

```php
mixed ParentOrderControllerCore::_updateMessage($messageContent)
```





* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 181](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L181)


#### Arguments
* $messageContent **mixed**



### <a name="method-addCSS"></a>addCSS

```php
mixed FrontControllerCore::addCSS($css_uri, string $css_media_type, integer $offset, boolean $check_path)
```

Add one or several CSS for front, checking if css files are overriden in theme/css/modules/ directory



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1092](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1092)


#### Arguments
* $css_uri **mixed**
* $css_media_type **string**
* $offset **integer**
* $check_path **boolean**



### <a name="method-addColorsToProductList"></a>addColorsToProductList

```php
mixed FrontControllerCore::addColorsToProductList($products)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1310](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1310)


#### Arguments
* $products **mixed**



### <a name="method-addJS"></a>addJS

```php
mixed FrontControllerCore::addJS($js_uri, boolean $check_path)
```

Add one or several JS files for front, checking if js files are overriden in theme/js/modules/ directory



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1108](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1108)


#### Arguments
* $js_uri **mixed**
* $check_path **boolean**



### <a name="method-addJquery"></a>addJquery

```php
void ControllerCore::addJquery($version, $folder, $minifier)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 371](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L371)


#### Arguments
* $version **mixed**
* $folder **mixed**
* $minifier **mixed**



### <a name="method-addJqueryPlugin"></a>addJqueryPlugin

```php
mixed ControllerCore::addJqueryPlugin($name, null $folder, boolean $css)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 403](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L403)


#### Arguments
* $name **mixed**
* $folder **null**
* $css **boolean**



### <a name="method-addJqueryUI"></a>addJqueryUI

```php
void ControllerCore::addJqueryUI($component, $theme, $check_dependencies)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 382](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L382)


#### Arguments
* $component **mixed**
* $theme **mixed**
* $check_dependencies **mixed**



### <a name="method-addMedia"></a>addMedia

```php
mixed FrontControllerCore::addMedia($media_uri, $css_media_type, $offset, $remove, $check_path)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1022](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1022)


#### Arguments
* $media_uri **mixed**
* $css_media_type **mixed**
* $offset **mixed**
* $remove **mixed**
* $check_path **mixed**



### <a name="method-ajaxDie"></a>ajaxDie

```php
mixed ControllerCore::ajaxDie($value, $controller, $method)
```





* Visibility: **protected**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 513](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L513)


#### Arguments
* $value **mixed**
* $controller **mixed**
* $method **mixed**



### <a name="method-canonicalRedirection"></a>canonicalRedirection

```php
mixed FrontControllerCore::canonicalRedirection($canonical_url)
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 643](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L643)


#### Arguments
* $canonical_url **mixed**



### <a name="method-checkAccess"></a>checkAccess

```php
boolean FrontControllerCore::checkAccess()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L93)




### <a name="method-checkLiveEditAccess"></a>checkLiveEditAccess

```php
mixed FrontControllerCore::checkLiveEditAccess()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 851](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L851)




### <a name="method-display"></a>display

```php
mixed FrontControllerCore::display()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 534](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L534)




### <a name="method-displayContent"></a>displayContent

```php
mixed FrontControllerCore::displayContent()
```

1.4 retrocompatibility



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 530](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L530)




### <a name="method-displayFooter"></a>displayFooter

```php
mixed FrontControllerCore::displayFooter($display)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 507](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L507)


#### Arguments
* $display **mixed**



### <a name="method-displayHeader"></a>displayHeader

```php
mixed FrontControllerCore::displayHeader($display)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 469](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L469)


#### Arguments
* $display **mixed**



### <a name="method-displayMaintenancePage"></a>displayMaintenancePage

```php
mixed FrontControllerCore::displayMaintenancePage()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 592](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L592)




### <a name="method-displayRestrictedCountryPage"></a>displayRestrictedCountryPage

```php
mixed FrontControllerCore::displayRestrictedCountryPage()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 615](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L615)




### <a name="method-geolocationManagement"></a>geolocationManagement

```php
mixed FrontControllerCore::geolocationManagement($default_country)
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 685](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L685)


#### Arguments
* $default_country **mixed**



### <a name="method-getColorsListCacheId"></a>getColorsListCacheId

```php
mixed FrontControllerCore::getColorsListCacheId($id_product)
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1347](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1347)


#### Arguments
* $id_product **mixed**



### <a name="method-getController"></a>getController

```php
mixed ControllerCore::getController(string $class_name, boolean $auth, boolean $ssl)
```

Get an instance of a controller



* Visibility: **public**
* This method is **static**.
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L133)


#### Arguments
* $class_name **string**
* $auth **boolean**
* $ssl **boolean**



### <a name="method-getCurrentCustomerGroups"></a>getCurrentCustomerGroups

```php
mixed FrontControllerCore::getCurrentCustomerGroups()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 963](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L963)




### <a name="method-getFormatedSummaryDetail"></a>getFormatedSummaryDetail

```php
mixed OrderOpcControllerCore::getFormatedSummaryDetail()
```





* Visibility: **protected**
* Source: [controllers/front/OrderOpcController.php line 693](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L693)




### <a name="method-getLayout"></a>getLayout

```php
boolean|string FrontControllerCore::getLayout()
```

Returns the layout corresponding to the current page by using the override system
Ex:
On the url: http://localhost/index.php?id_product=1&controller=product, this method will
check if the layout exists in the following files (in that order), and return the first found:
- /themes/default/override/layout-product-1.tpl
- /themes/default/override/layout-product.tpl
- /themes/default/layout.tpl



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1209](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1209)




### <a name="method-getLiveEditFooter"></a>getLiveEditFooter

```php
mixed FrontControllerCore::getLiveEditFooter()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 860](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L860)




### <a name="method-getOverrideTemplate"></a>getOverrideTemplate

```php
boolean FrontControllerCore::getOverrideTemplate()
```

Returns the template corresponding to the current page.

By default this method return false but could easily be overridden in a specific controller

* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1171](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1171)




### <a name="method-getOverrideThemeDir"></a>getOverrideThemeDir

```php
mixed FrontControllerCore::getOverrideThemeDir()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1192](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1192)




### <a name="method-getTemplatePath"></a>getTemplatePath

```php
mixed FrontControllerCore::getTemplatePath($template)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1232](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1232)


#### Arguments
* $template **mixed**



### <a name="method-getThemeDir"></a>getThemeDir

```php
mixed FrontControllerCore::getThemeDir()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1187](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1187)




### <a name="method-init"></a>init

```php
mixed OrderOpcControllerCore::init()
```

Initialize order opc controller



* Visibility: **public**
* Source: [controllers/front/OrderOpcController.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L38)




### <a name="method-initContent"></a>initContent

```php
mixed OrderOpcControllerCore::initContent()
```

Assign template vars related to page content



* Visibility: **public**
* Source: [controllers/front/OrderOpcController.php line 339](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L339)




### <a name="method-initCursedPage"></a>initCursedPage

```php
mixed FrontControllerCore::initCursedPage()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 513](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L513)




### <a name="method-initFooter"></a>initFooter

```php
mixed FrontControllerCore::initFooter()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 831](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L831)




### <a name="method-initHeader"></a>initHeader

```php
mixed FrontControllerCore::initHeader()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 812](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L812)




### <a name="method-initLogoAndFavicon"></a>initLogoAndFavicon

```php
array FrontControllerCore::initLogoAndFavicon()
```

Return an array with specific logo and favicon,
if mobile device



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1293](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1293)




### <a name="method-isCached"></a>isCached

```php
mixed ControllerCore::isCached($template, $cacheId, $compileId)
```





* Visibility: **protected**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 471](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L471)


#### Arguments
* $template **mixed**
* $cacheId **mixed**
* $compileId **mixed**



### <a name="method-isInWhitelistForGeolocation"></a>isInWhitelistForGeolocation

```php
mixed FrontControllerCore::isInWhitelistForGeolocation()
```





* Visibility: **protected**
* This method is **static**.
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 982](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L982)




### <a name="method-isTokenValid"></a>isTokenValid

```php
boolean FrontControllerCore::isTokenValid()
```

Check if token is valid



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1014](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1014)




### <a name="method-isXmlHttpRequest"></a>isXmlHttpRequest

```php
boolean ControllerCore::isXmlHttpRequest()
```





* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 425](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L425)




### <a name="method-myErrorHandler"></a>myErrorHandler

```php
mixed ControllerCore::myErrorHandler($errno, $errstr, $errfile, $errline)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 479](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L479)


#### Arguments
* $errno **mixed**
* $errstr **mixed**
* $errfile **mixed**
* $errline **mixed**



### <a name="method-pagination"></a>pagination

```php
mixed FrontControllerCore::pagination($total_products)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 904](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L904)


#### Arguments
* $total_products **mixed**



### <a name="method-postProcess"></a>postProcess

```php
mixed FrontControllerCore::postProcess()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 442](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L442)




### <a name="method-process"></a>process

```php
mixed FrontControllerCore::process()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 518](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L518)




### <a name="method-productSort"></a>productSort

```php
mixed FrontControllerCore::productSort()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 877](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L877)




### <a name="method-recoverCart"></a>recoverCart

```php
mixed FrontControllerCore::recoverCart()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1118](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1118)




### <a name="method-redirect"></a>redirect

```php
mixed FrontControllerCore::redirect()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 522](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L522)




### <a name="method-removeCSS"></a>removeCSS

```php
mixed FrontControllerCore::removeCSS($css_uri, $css_media_type, $check_path)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1097](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1097)


#### Arguments
* $css_uri **mixed**
* $css_media_type **mixed**
* $check_path **mixed**



### <a name="method-removeJS"></a>removeJS

```php
mixed FrontControllerCore::removeJS($js_uri, $check_path)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1113](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1113)


#### Arguments
* $js_uri **mixed**
* $check_path **mixed**



### <a name="method-removeMedia"></a>removeMedia

```php
mixed FrontControllerCore::removeMedia($media_uri, $css_media_type, $check_path)
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1079](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1079)


#### Arguments
* $media_uri **mixed**
* $css_media_type **mixed**
* $check_path **mixed**



### <a name="method-run"></a>run

```php
mixed ControllerCore::run()
```

Start controller process (this method shouldn't be overriden !)



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 161](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L161)




### <a name="method-setDefaultCarrierSelection"></a>setDefaultCarrierSelection

```php
\number ParentOrderControllerCore::setDefaultCarrierSelection(array $carriers)
```

Decides what the default carrier is and update the cart with it



* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 591](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L591)


#### Arguments
* $carriers **array**



### <a name="method-setMedia"></a>setMedia

```php
mixed OrderOpcControllerCore::setMedia()
```





* Visibility: **public**
* Source: [controllers/front/OrderOpcController.php line 312](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/OrderOpcController.php#L312)




### <a name="method-setMobileMedia"></a>setMobileMedia

```php
mixed FrontControllerCore::setMobileMedia()
```

Specific medias for mobile device.

if autoload directory is present in the mobile theme, these files will not be loaded

* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 746](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L746)




### <a name="method-setMobileTemplate"></a>setMobileTemplate

```php
mixed FrontControllerCore::setMobileTemplate($template)
```

This checks if the template set is available for mobile themes,
otherwise the front template is choosen.



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1258](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1258)


#### Arguments
* $template **mixed**



### <a name="method-setNoCarrier"></a>setNoCarrier

```php
mixed ParentOrderControllerCore::setNoCarrier()
```

Set id_carrier to 0 (no shipping price)



* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 574](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L574)




### <a name="method-setTemplate"></a>setTemplate

```php
mixed FrontControllerCore::setTemplate($default_template)
```

This is overrided to manage is behaviour
if a customer access to the site with mobile device.



* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1150](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1150)


#### Arguments
* $default_template **mixed**



### <a name="method-smartyOutputContent"></a>smartyOutputContent

```php
mixed ControllerCore::smartyOutputContent($content)
```





* Visibility: **protected**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/controller/Controller.php line 430](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/Controller.php#L430)


#### Arguments
* $content **mixed**



### <a name="method-sslRedirection"></a>sslRedirection

```php
mixed FrontControllerCore::sslRedirection()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 627](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L627)




### <a name="method-useMobileTheme"></a>useMobileTheme

```php
mixed FrontControllerCore::useMobileTheme()
```





* Visibility: **protected**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 1176](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L1176)




### <a name="method-validateDeliveryOption"></a>validateDeliveryOption

```php
mixed ParentOrderControllerCore::validateDeliveryOption(array $delivery_option)
```

Validate get/post param delivery option



* Visibility: **protected**
* This method is defined by [ParentOrderControllerCore](class.ParentOrderControllerCore.md).
* Source: [controllers/front/ParentOrderController.php line 277](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/controllers/front/ParentOrderController.php#L277)


#### Arguments
* $delivery_option **array**



### <a name="method-viewAccess"></a>viewAccess

```php
boolean FrontControllerCore::viewAccess()
```





* Visibility: **public**
* This method is defined by [FrontControllerCore](class.FrontControllerCore.md).
* Source: [classes/controller/FrontController.php line 103](https://github.com/PrestaShop/PrestaShop/blob/1.6.0.14/classes/controller/FrontController.php#L103)



