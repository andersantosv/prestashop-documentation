Class PaymentModuleCore
=====================





* Class name: PaymentModuleCore
* This is an **abstract** class
* Parent class: [Module](class.ModuleCore.md)
* Source: [classes/PaymentModule.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L27)


Contents
--------


### Properties

* [$currencies](#property-$currencies)
* [$currencies_mode](#property-$currencies_mode)
* [$currentOrder](#property-$currentOrder)
* [$_INSTANCE](#property-$_INSTANCE)
* [$_confirmations](#property-$_confirmations)
* [$_errors](#property-$_errors)
* [$_generate_config_xml_mode](#property-$_generate_config_xml_mode)
* [$_lang](#property-$_lang)
* [$_path](#property-$_path)
* [$active](#property-$active)
* [$author](#property-$author)
* [$cache_permissions](#property-$cache_permissions)
* [$classInModule](#property-$classInModule)
* [$context](#property-$context)
* [$database_version](#property-$database_version)
* [$dependencies](#property-$dependencies)
* [$description](#property-$description)
* [$displayName](#property-$displayName)
* [$exceptionsCache](#property-$exceptionsCache)
* [$id](#property-$id)
* [$identifier](#property-$identifier)
* [$l_cache](#property-$l_cache)
* [$limited_countries](#property-$limited_countries)
* [$local_path](#property-$local_path)
* [$modules_cache](#property-$modules_cache)
* [$name](#property-$name)
* [$need_instance](#property-$need_instance)
* [$ps_versions_compliancy](#property-$ps_versions_compliancy)
* [$registered_version](#property-$registered_version)
* [$smarty](#property-$smarty)
* [$tab](#property-$tab)
* [$table](#property-$table)
* [$version](#property-$version)
* [$warning](#property-$warning)

### Methods

* [__construct](#method-__construct)
* [_clearCache](#method-_clearCache)
* [_generateConfigXml](#method-_generateConfigXml)
* [_getApplicableTemplateDir](#method-_getApplicableTemplateDir)
* [_getFormatedAddress](#method-_getFormatedAddress)
* [_getTxtFormatedAddress](#method-_getTxtFormatedAddress)
* [_isTemplateOverloaded](#method-_isTemplateOverloaded)
* [_isTemplateOverloadedStatic](#method-_isTemplateOverloadedStatic)
* [addCheckboxCountryRestrictionsForModule](#method-addCheckboxCountryRestrictionsForModule)
* [addCheckboxCurrencyRestrictionsForModule](#method-addCheckboxCurrencyRestrictionsForModule)
* [addCurrencyPermissions](#method-addCurrencyPermissions)
* [addOverride](#method-addOverride)
* [addRadioCurrencyRestrictionsForModule](#method-addRadioCurrencyRestrictionsForModule)
* [adminDisplayInformation](#method-adminDisplayInformation)
* [adminDisplayWarning](#method-adminDisplayWarning)
* [cleanPositions](#method-cleanPositions)
* [configXmlStringFormat](#method-configXmlStringFormat)
* [disable](#method-disable)
* [disableByName](#method-disableByName)
* [display](#method-display)
* [displayConfirmation](#method-displayConfirmation)
* [displayError](#method-displayError)
* [displayFlags](#method-displayFlags)
* [editExceptions](#method-editExceptions)
* [enable](#method-enable)
* [enableByName](#method-enableByName)
* [findTranslation](#method-findTranslation)
* [formatProductAndVoucherForEmail](#method-formatProductAndVoucherForEmail)
* [getAuthorizedModules](#method-getAuthorizedModules)
* [getCacheId](#method-getCacheId)
* [getConfirmations](#method-getConfirmations)
* [getCurrency](#method-getCurrency)
* [getErrors](#method-getErrors)
* [getExceptions](#method-getExceptions)
* [getInstalledPaymentModules](#method-getInstalledPaymentModules)
* [getInstanceById](#method-getInstanceById)
* [getInstanceByName](#method-getInstanceByName)
* [getLocalPath](#method-getLocalPath)
* [getModuleIdByName](#method-getModuleIdByName)
* [getModuleName](#method-getModuleName)
* [getModuleNameFromClass](#method-getModuleNameFromClass)
* [getModulesDirOnDisk](#method-getModulesDirOnDisk)
* [getModulesInstalled](#method-getModulesInstalled)
* [getModulesOnDisk](#method-getModulesOnDisk)
* [getNonNativeModuleList](#method-getNonNativeModuleList)
* [getPathUri](#method-getPathUri)
* [getPaymentModules](#method-getPaymentModules)
* [getPaypalIgnore](#method-getPaypalIgnore)
* [getPermission](#method-getPermission)
* [getPermissionStatic](#method-getPermissionStatic)
* [getPosition](#method-getPosition)
* [getTemplatePath](#method-getTemplatePath)
* [getUpgradeStatus](#method-getUpgradeStatus)
* [hookExec](#method-hookExec)
* [hookExecPayment](#method-hookExecPayment)
* [initUpgradeModule](#method-initUpgradeModule)
* [install](#method-install)
* [installOverrides](#method-installOverrides)
* [isCached](#method-isCached)
* [isEnabled](#method-isEnabled)
* [isHookableOn](#method-isHookableOn)
* [isInstalled](#method-isInstalled)
* [isRegisteredInHook](#method-isRegisteredInHook)
* [l](#method-l)
* [loadUpgradeVersionList](#method-loadUpgradeVersionList)
* [needUpgrade](#method-needUpgrade)
* [preCall](#method-preCall)
* [registerExceptions](#method-registerExceptions)
* [registerHook](#method-registerHook)
* [removeOverride](#method-removeOverride)
* [runUpgradeModule](#method-runUpgradeModule)
* [setUpgradeMessage](#method-setUpgradeMessage)
* [uninstall](#method-uninstall)
* [uninstallOverrides](#method-uninstallOverrides)
* [unregisterExceptions](#method-unregisterExceptions)
* [unregisterHook](#method-unregisterHook)
* [updatePosition](#method-updatePosition)
* [upgradeModuleVersion](#method-upgradeModuleVersion)
* [validateOrder](#method-validateOrder)




Properties
----------


### <a name="property-$currencies"></a>$currencies

```php
public mixed $currencies = true
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L31).


### <a name="property-$currencies_mode"></a>$currencies_mode

```php
public mixed $currencies_mode = 'checkbox'
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L32).


### <a name="property-$currentOrder"></a>$currentOrder

```php
public integer $currentOrder
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L30).


### <a name="property-$_INSTANCE"></a>$_INSTANCE

```php
protected \protected $_INSTANCE = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 105](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L105).


### <a name="property-$_confirmations"></a>$_confirmations

```php
protected \protected $_confirmations = array()
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 93](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L93).


### <a name="property-$_errors"></a>$_errors

```php
protected \protected $_errors = array()
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 90](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L90).


### <a name="property-$_generate_config_xml_mode"></a>$_generate_config_xml_mode

```php
protected \protected $_generate_config_xml_mode = false
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L108).


### <a name="property-$_lang"></a>$_lang

```php
protected array $_lang = array()
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L79).


### <a name="property-$_path"></a>$_path

```php
protected string $_path = null
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L82).


### <a name="property-$active"></a>$active

```php
public boolean $active = false
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L67).


### <a name="property-$author"></a>$author

```php
public string $author
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 58](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L58).


### <a name="property-$cache_permissions"></a>$cache_permissions

```php
protected \protected $cache_permissions = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L114).


### <a name="property-$classInModule"></a>$classInModule

```php
public array $classInModule = array()
```





* Visibility: **public**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L76).


### <a name="property-$context"></a>$context

```php
protected \Context $context
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L117).


### <a name="property-$database_version"></a>$database_version

```php
public mixed $database_version
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L34).


### <a name="property-$dependencies"></a>$dependencies

```php
public array $dependencies = array()
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L46).


### <a name="property-$description"></a>$description

```php
public string $description
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L55).


### <a name="property-$displayName"></a>$displayName

```php
public string $displayName
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 52](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L52).


### <a name="property-$exceptionsCache"></a>$exceptionsCache

```php
protected mixed $exceptionsCache = null
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1497](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1497).


### <a name="property-$id"></a>$id

```php
public integer $id = null
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L30).


### <a name="property-$identifier"></a>$identifier

```php
protected \protected $identifier = 'id_module'
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 99](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L99).


### <a name="property-$l_cache"></a>$l_cache

```php
protected \protected $l_cache = array()
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L111).


### <a name="property-$limited_countries"></a>$limited_countries

```php
public array $limited_countries = array()
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L73).


### <a name="property-$local_path"></a>$local_path

```php
protected string $local_path = null
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 87](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L87).


### <a name="property-$modules_cache"></a>$modules_cache

```php
protected \protected $modules_cache
```





* Visibility: **protected**
* This property is **static**.
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 102](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L102).


### <a name="property-$name"></a>$name

```php
public string $name
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 49](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L49).


### <a name="property-$need_instance"></a>$need_instance

```php
public integer $need_instance = 1
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L61).


### <a name="property-$ps_versions_compliancy"></a>$ps_versions_compliancy

```php
public array $ps_versions_compliancy = array('min' => '1.4', 'max' => '1.6')
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L43).


### <a name="property-$registered_version"></a>$registered_version

```php
public string $registered_version
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L40).


### <a name="property-$smarty"></a>$smarty

```php
protected \Smarty_Data $smarty
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L120).


### <a name="property-$tab"></a>$tab

```php
public string $tab = null
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L64).


### <a name="property-$table"></a>$table

```php
protected \protected $table = 'module'
```





* Visibility: **protected**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L96).


### <a name="property-$version"></a>$version

```php
public float $version
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L33).


### <a name="property-$warning"></a>$warning

```php
public string $warning
```





* Visibility: **public**
* This property is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L70).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed ModuleCore::__construct(string $name, \Context $context)
```

Constructor



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 139](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L139)


#### Arguments
* $name **string** - Module unique name
* $context **[Context](class.ContextCore.md)**



### <a name="method-_clearCache"></a>_clearCache

```php
mixed ModuleCore::_clearCache($template, $cache_id, $compile_id)
```





* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1666](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1666)


#### Arguments
* $template **mixed**
* $cache_id **mixed**
* $compile_id **mixed**



### <a name="method-_generateConfigXml"></a>_generateConfigXml

```php
mixed ModuleCore::_generateConfigXml()
```





* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1673](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1673)




### <a name="method-_getApplicableTemplateDir"></a>_getApplicableTemplateDir

```php
mixed ModuleCore::_getApplicableTemplateDir($template)
```





* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1650](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1650)


#### Arguments
* $template **mixed**



### <a name="method-_getFormatedAddress"></a>_getFormatedAddress

```php
String PaymentModuleCore::_getFormatedAddress(\Address $the_address, $line_sep, $fields_style)
```





* Visibility: **protected**
* Source: [classes/PaymentModule.php line 701](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L701)


#### Arguments
* $the_address **[Address](class.AddressCore.md)**
* $line_sep **mixed**
* $fields_style **mixed**



### <a name="method-_getTxtFormatedAddress"></a>_getTxtFormatedAddress

```php
String PaymentModuleCore::_getTxtFormatedAddress($the_address)
```





* Visibility: **protected**
* Source: [classes/PaymentModule.php line 677](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L677)


#### Arguments
* $the_address **mixed**



### <a name="method-_isTemplateOverloaded"></a>_isTemplateOverloaded

```php
mixed ModuleCore::_isTemplateOverloaded($template)
```





* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1589](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1589)


#### Arguments
* $template **mixed**



### <a name="method-_isTemplateOverloadedStatic"></a>_isTemplateOverloadedStatic

```php
mixed ModuleCore::_isTemplateOverloadedStatic($module_name, $template)
```





* Visibility: **protected**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1578](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1578)


#### Arguments
* $module_name **mixed**
* $template **mixed**



### <a name="method-addCheckboxCountryRestrictionsForModule"></a>addCheckboxCountryRestrictionsForModule

```php
mixed PaymentModuleCore::addCheckboxCountryRestrictionsForModule(array $shops)
```

Add checkbox country restrictions for a new module



* Visibility: **public**
* Source: [classes/PaymentModule.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L111)


#### Arguments
* $shops **array**



### <a name="method-addCheckboxCurrencyRestrictionsForModule"></a>addCheckboxCurrencyRestrictionsForModule

```php
mixed PaymentModuleCore::addCheckboxCurrencyRestrictionsForModule(array $shops)
```

Add checkbox currency restrictions for a new module



* Visibility: **public**
* Source: [classes/PaymentModule.php line 74](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L74)


#### Arguments
* $shops **array**



### <a name="method-addCurrencyPermissions"></a>addCurrencyPermissions

```php
boolean PaymentModuleCore::addCurrencyPermissions(integer $id_currency, array $id_module_list)
```

Allows specified payment modules to be used by a specific currency



* Visibility: **public**
* This method is **static**.
* Source: [classes/PaymentModule.php line 746](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L746)


#### Arguments
* $id_currency **integer**
* $id_module_list **array**



### <a name="method-addOverride"></a>addOverride

```php
boolean ModuleCore::addOverride(string $classname)
```

Add all methods in a module override to the override class



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1907](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1907)


#### Arguments
* $classname **string**



### <a name="method-addRadioCurrencyRestrictionsForModule"></a>addRadioCurrencyRestrictionsForModule

```php
mixed PaymentModuleCore::addRadioCurrencyRestrictionsForModule(array $shops)
```

Add radio currency restrictions for a new module



* Visibility: **public**
* Source: [classes/PaymentModule.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L94)


#### Arguments
* $shops **array**



### <a name="method-adminDisplayInformation"></a>adminDisplayInformation

```php
mixed ModuleCore::adminDisplayInformation(string $msg)
```

add a info message to display at the top of the admin page



* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1853](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1853)


#### Arguments
* $msg **string**



### <a name="method-adminDisplayWarning"></a>adminDisplayWarning

```php
mixed ModuleCore::adminDisplayWarning(string $msg)
```

add a warning message to display at the top of the admin page



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1841](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1841)


#### Arguments
* $msg **string**



### <a name="method-cleanPositions"></a>cleanPositions

```php
mixed ModuleCore::cleanPositions($id_hook, $shop_list)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1447](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1447)


#### Arguments
* $id_hook **mixed**
* $shop_list **mixed**



### <a name="method-configXmlStringFormat"></a>configXmlStringFormat

```php
mixed ModuleCore::configXmlStringFormat($string)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 907](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L907)


#### Arguments
* $string **mixed**



### <a name="method-disable"></a>disable

```php
mixed ModuleCore::disable(boolean $forceAll)
```

Desactivate current module.



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 604](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L604)


#### Arguments
* $forceAll **boolean** - If true, disable module for all shop



### <a name="method-disableByName"></a>disableByName

```php
true ModuleCore::disableByName(array|string $name)
```

This function disable module $name. If an $name is an array,
this will disable all of them



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 586](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L586)


#### Arguments
* $name **array|string**



### <a name="method-display"></a>display

```php
mixed ModuleCore::display($file, $template, $cacheId, $compileId)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1601](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1601)


#### Arguments
* $file **mixed**
* $template **mixed**
* $cacheId **mixed**
* $compileId **mixed**



### <a name="method-displayConfirmation"></a>displayConfirmation

```php
mixed ModuleCore::displayConfirmation($string)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1482](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1482)


#### Arguments
* $string **mixed**



### <a name="method-displayError"></a>displayError

```php
mixed ModuleCore::displayError($error)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1472](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1472)


#### Arguments
* $error **mixed**



### <a name="method-displayFlags"></a>displayFlags

```php
mixed ModuleCore::displayFlags(array $languages, integer $default_language, string $ids, string $id, boolean $return, boolean $use_vars_instead_of_ids)
```

Display flags in forms for translations



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 621](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L621)


#### Arguments
* $languages **array** - All languages available
* $default_language **integer** - Default language id
* $ids **string** - Multilingual div ids in form
* $id **string** - Current div id]
* $return **boolean** - define the return way : false for a display, true for a return
* $use_vars_instead_of_ids **boolean** - use an js vars instead of ids seperate by &quot;¤&quot;



### <a name="method-editExceptions"></a>editExceptions

```php
boolean ModuleCore::editExceptions($id_hook, array $excepts)
```

Edit exceptions for module->Hook



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 799](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L799)


#### Arguments
* $id_hook **mixed**
* $excepts **array** - List of shopID and file name



### <a name="method-enable"></a>enable

```php
mixed ModuleCore::enable(boolean $forceAll)
```

Activate current module.



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 553](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L553)


#### Arguments
* $forceAll **boolean** - If true, enable module for all shop



### <a name="method-enableByName"></a>enableByName

```php
true ModuleCore::enableByName(array|string $name)
```

This function enable module $name. If an $name is an array,
this will enable all of them



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 535](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L535)


#### Arguments
* $name **array|string**



### <a name="method-findTranslation"></a>findTranslation

```php
mixed ModuleCore::findTranslation($name, $string, $source)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1367](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1367)


#### Arguments
* $name **mixed**
* $string **mixed**
* $source **mixed**



### <a name="method-formatProductAndVoucherForEmail"></a>formatProductAndVoucherForEmail

```php
mixed PaymentModuleCore::formatProductAndVoucherForEmail($content)
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 668](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L668)


#### Arguments
* $content **mixed**



### <a name="method-getAuthorizedModules"></a>getAuthorizedModules

```php
mixed ModuleCore::getAuthorizedModules($group_id)
```

Get Unauthorized modules for a client group



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1750](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1750)


#### Arguments
* $group_id **mixed**



### <a name="method-getCacheId"></a>getCacheId

```php
mixed ModuleCore::getCacheId($name)
```





* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1594](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1594)


#### Arguments
* $name **mixed**



### <a name="method-getConfirmations"></a>getConfirmations

```php
array ModuleCore::getConfirmations()
```

Get module messages confirmation



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1785](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1785)




### <a name="method-getCurrency"></a>getCurrency

```php
\Currency PaymentModuleCore::getCurrency($current_id_currency)
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 710](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L710)


#### Arguments
* $current_id_currency **mixed**



### <a name="method-getErrors"></a>getErrors

```php
array ModuleCore::getErrors()
```

Get module errors



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1774](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1774)




### <a name="method-getExceptions"></a>getExceptions

```php
mixed ModuleCore::getExceptions($hookID, $dispatch)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1498](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1498)


#### Arguments
* $hookID **mixed**
* $dispatch **mixed**



### <a name="method-getInstalledPaymentModules"></a>getInstalledPaymentModules

```php
array PaymentModuleCore::getInstalledPaymentModules()
```

List all installed and active payment modules



* Visibility: **public**
* This method is **static**.
* Source: [classes/PaymentModule.php line 778](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L778)




### <a name="method-getInstanceById"></a>getInstanceById

```php
\Module ModuleCore::getInstanceById(integer $id_module)
```

Return an instance of the specified module



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 888](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L888)


#### Arguments
* $id_module **integer** - Module ID



### <a name="method-getInstanceByName"></a>getInstanceByName

```php
\Module ModuleCore::getInstanceByName(string $module_name)
```

Return an instance of the specified module



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 859](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L859)


#### Arguments
* $module_name **string** - Module name



### <a name="method-getLocalPath"></a>getLocalPath

```php
string ModuleCore::getLocalPath()
```

Get local path for module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1796](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1796)




### <a name="method-getModuleIdByName"></a>getModuleIdByName

```php
integer ModuleCore::getModuleIdByName($name)
```

Get id module by name



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1763](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1763)


#### Arguments
* $name **mixed**



### <a name="method-getModuleName"></a>getModuleName

```php
mixed ModuleCore::getModuleName($module)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 913](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L913)


#### Arguments
* $module **mixed**



### <a name="method-getModuleNameFromClass"></a>getModuleNameFromClass

```php
boolean|string ModuleCore::getModuleNameFromClass(mixed $currentClass)
```

This function is used to determine the module name
of an AdminTab which belongs to a module, in order to keep translation
related to a module in its directory (instead of $_LANGADM)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 821](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L821)


#### Arguments
* $currentClass **mixed** - the



### <a name="method-getModulesDirOnDisk"></a>getModulesDirOnDisk

```php
array ModuleCore::getModulesDirOnDisk()
```

Return modules directory list



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1227](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1227)




### <a name="method-getModulesInstalled"></a>getModulesInstalled

```php
array ModuleCore::getModulesInstalled(integer $position)
```

Return installed modules



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1274](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1274)


#### Arguments
* $position **integer** - Take only positionnables modules



### <a name="method-getModulesOnDisk"></a>getModulesOnDisk

```php
array ModuleCore::getModulesOnDisk(boolean $useConfig, $loggedOnAddons, $id_employee)
```

Return available modules



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 948](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L948)


#### Arguments
* $useConfig **boolean** - in order to use config.xml file in module dir
* $loggedOnAddons **mixed**
* $id_employee **mixed**



### <a name="method-getNonNativeModuleList"></a>getNonNativeModuleList

```php
array ModuleCore::getNonNativeModuleList()
```

Return non native module



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1250](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1250)




### <a name="method-getPathUri"></a>getPathUri

```php
string ModuleCore::getPathUri()
```

Get uri path for module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1807](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1807)




### <a name="method-getPaymentModules"></a>getPaymentModules

```php
array ModuleCore::getPaymentModules()
```

Returns the list of the payment module associated to the current customer



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1323](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1323)




### <a name="method-getPaypalIgnore"></a>getPaypalIgnore

```php
mixed ModuleCore::getPaypalIgnore()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1309](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1309)




### <a name="method-getPermission"></a>getPermission

```php
boolean ModuleCore::getPermission(array $variable, object $employee)
```

Check employee permission for module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1707](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1707)


#### Arguments
* $variable **array** - (action)
* $employee **object**



### <a name="method-getPermissionStatic"></a>getPermissionStatic

```php
boolean ModuleCore::getPermissionStatic(integer $id_module, array $variable, object $employee)
```

Check employee permission for module (static method)



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1719](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1719)


#### Arguments
* $id_module **integer**
* $variable **array** - (action)
* $employee **object**



### <a name="method-getPosition"></a>getPosition

```php
mixed ModuleCore::getPosition($id_hook)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1818](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1818)


#### Arguments
* $id_hook **mixed**



### <a name="method-getTemplatePath"></a>getTemplatePath

```php
string ModuleCore::getTemplatePath(string $template)
```

Get realpath of a template of current module (check if template is overriden too)



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1637](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1637)


#### Arguments
* $template **string**



### <a name="method-getUpgradeStatus"></a>getUpgradeStatus

```php
boolean ModuleCore::getUpgradeStatus($module_name)
```

Return the status of the upgraded module



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 475](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L475)


#### Arguments
* $module_name **mixed**



### <a name="method-hookExec"></a>hookExec

```php
string ModuleCore::hookExec(string $hook_name, array $hookArgs, $id_module)
```

Execute modules for specified hook



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1292](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1292)


#### Arguments
* $hook_name **string** - Hook Name
* $hookArgs **array** - Parameters for the functions
* $id_module **mixed**



### <a name="method-hookExecPayment"></a>hookExecPayment

```php
mixed ModuleCore::hookExecPayment()
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1298](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1298)




### <a name="method-initUpgradeModule"></a>initUpgradeModule

```php
boolean ModuleCore::initUpgradeModule($module)
```

Init the upgrade module



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 310](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L310)


#### Arguments
* $module **mixed**



### <a name="method-install"></a>install

```php
mixed PaymentModuleCore::install()
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L34)




### <a name="method-installOverrides"></a>installOverrides

```php
boolean ModuleCore::installOverrides()
```

Install overrides files for the module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1865](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1865)




### <a name="method-isCached"></a>isCached

```php
mixed ModuleCore::isCached($template, $cacheId, $compileId)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1655](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1655)


#### Arguments
* $template **mixed**
* $cacheId **mixed**
* $compileId **mixed**



### <a name="method-isEnabled"></a>isEnabled

```php
mixed ModuleCore::isEnabled($module_name)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1550](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1550)


#### Arguments
* $module_name **mixed**



### <a name="method-isHookableOn"></a>isHookableOn

```php
boolean ModuleCore::isHookableOn(string $hook_name)
```

Check if the module is transplantable on the hook in parameter



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1695](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1695)


#### Arguments
* $hook_name **string**



### <a name="method-isInstalled"></a>isInstalled

```php
mixed ModuleCore::isInstalled($module_name)
```





* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1540](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1540)


#### Arguments
* $module_name **mixed**



### <a name="method-isRegisteredInHook"></a>isRegisteredInHook

```php
mixed ModuleCore::isRegisteredInHook($hook)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1563](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1563)


#### Arguments
* $hook **mixed**



### <a name="method-l"></a>l

```php
string ModuleCore::l(string $string, boolean|string $specific)
```

Get translation for a given module text

Note: $specific parameter is mandatory for library files.
Otherwise, translation key will not match for Module library
when module is loaded with eval() Module::getModulesOnDisk()

* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1383](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1383)


#### Arguments
* $string **string** - String to translate
* $specific **boolean|string** - filename to use in translation key



### <a name="method-loadUpgradeVersionList"></a>loadUpgradeVersionList

```php
boolean ModuleCore::loadUpgradeVersionList($module_name, $module_version, $registered_version)
```

Load the available list of upgrade of a specified module
with an associated version



* Visibility: **protected**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 425](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L425)


#### Arguments
* $module_name **mixed**
* $module_version **mixed**
* $registered_version **mixed**



### <a name="method-needUpgrade"></a>needUpgrade

```php
boolean ModuleCore::needUpgrade($module)
```

Check if a module need to be upgraded.

This method modify the module_cache adding an upgrade list file

* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 401](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L401)


#### Arguments
* $module **mixed**



### <a name="method-preCall"></a>preCall

```php
mixed PaymentModuleCore::preCall($module_name)
```





* Visibility: **public**
* This method is **static**.
* Source: [classes/PaymentModule.php line 795](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L795)


#### Arguments
* $module_name **mixed**



### <a name="method-registerExceptions"></a>registerExceptions

```php
boolean ModuleCore::registerExceptions(integer $id_hook, array $excepts, array $shop_list)
```

Add exceptions for module->Hook



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 765](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L765)


#### Arguments
* $id_hook **integer** - Hook id
* $excepts **array** - List of file name
* $shop_list **array** - List of shop



### <a name="method-registerHook"></a>registerHook

```php
boolean ModuleCore::registerHook(string $hook_name, array $shop_list)
```

Connect module to a hook



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 651](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L651)


#### Arguments
* $hook_name **string** - Hook name
* $shop_list **array** - List of shop linked to the hook (if null, link hook to all shops)



### <a name="method-removeOverride"></a>removeOverride

```php
boolean ModuleCore::removeOverride(string $classname)
```

Remove all methods in a module override from the override class



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1963](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1963)


#### Arguments
* $classname **string**



### <a name="method-runUpgradeModule"></a>runUpgradeModule

```php
array ModuleCore::runUpgradeModule()
```

Run the upgrade for a given module name and version



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 334](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L334)




### <a name="method-setUpgradeMessage"></a>setUpgradeMessage

```php
mixed ModuleCore::setUpgradeMessage($upgrade_detail)
```

Set errors, warning or success message of a module upgrade



* Visibility: **protected**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 276](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L276)


#### Arguments
* $upgrade_detail **mixed**



### <a name="method-uninstall"></a>uninstall

```php
mixed PaymentModuleCore::uninstall()
```





* Visibility: **public**
* Source: [classes/PaymentModule.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L59)




### <a name="method-uninstallOverrides"></a>uninstallOverrides

```php
boolean ModuleCore::uninstallOverrides()
```

Uninstall overrides files for the module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1886](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1886)




### <a name="method-unregisterExceptions"></a>unregisterExceptions

```php
boolean ModuleCore::unregisterExceptions($hook_id, array $shop_list)
```

Unregister exceptions linked to module



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 749](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L749)


#### Arguments
* $hook_id **mixed**
* $shop_list **array** - List of shop



### <a name="method-unregisterHook"></a>unregisterHook

```php
boolean ModuleCore::unregisterHook($hook_id, array $shop_list)
```

Unregister module from hook



* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 719](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L719)


#### Arguments
* $hook_id **mixed**
* $shop_list **array** - List of shop



### <a name="method-updatePosition"></a>updatePosition

```php
mixed ModuleCore::updatePosition($id_hook, $way, $position)
```





* Visibility: **public**
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 1398](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L1398)


#### Arguments
* $id_hook **mixed**
* $way **mixed**
* $position **mixed**



### <a name="method-upgradeModuleVersion"></a>upgradeModuleVersion

```php
boolean ModuleCore::upgradeModuleVersion($name, $version)
```

Upgrade the registered version to a new one



* Visibility: **public**
* This method is **static**.
* This method is defined by [ModuleCore](class.ModuleCore.md).
* Source: [classes/module/Module.php line 384](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/module/Module.php#L384)


#### Arguments
* $name **mixed**
* $version **mixed**



### <a name="method-validateOrder"></a>validateOrder

```php
mixed PaymentModuleCore::validateOrder(integer $id_cart, integer $id_order_state, float $amount_paid, string $payment_method, string $message, $extra_vars, $currency_special, $dont_touch_amount, $secure_key, \Shop $shop)
```

Validate an order in database
Function called from a payment module



* Visibility: **public**
* Source: [classes/PaymentModule.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.5.4.0/classes/PaymentModule.php#L130)


#### Arguments
* $id_cart **integer** - Value
* $id_order_state **integer** - Value
* $amount_paid **float** - Amount really paid by customer (in the default currency)
* $payment_method **string** - Payment method (eg. &#039;Credit card&#039;)
* $message **string** - Message to attach to order
* $extra_vars **mixed**
* $currency_special **mixed**
* $dont_touch_amount **mixed**
* $secure_key **mixed**
* $shop **[Shop](class.ShopCore.md)**


