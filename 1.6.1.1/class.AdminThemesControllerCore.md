Class AdminThemesControllerCore
=====================





* Class name: AdminThemesControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminThemesController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L30)

Constants
----------

* [MAX_NAME_LENGTH](#constant-MAX_NAME_LENGTH)

Properties
----------

* [$check_features](#property-$check_features)
* [$check_features_version](#property-$check_features_version)
* [$className](#property-$className)
* [$img_error](#property-$img_error)
* [$object](#property-$object)
* [$table](#property-$table)
* [$toolbar_scroll](#property-$toolbar_scroll)

Methods
-------
* [__construct](#method-__construct)
* [_checkConfigForFeatures](#method-_checkConfigForFeatures)
* [_isThemeCompatible](#method-_isThemeCompatible)
* [ajaxProcessGetAddonsThemes](#method-ajaxProcessGetAddonsThemes)
* [ajaxProcessLeftMeta](#method-ajaxProcessLeftMeta)
* [ajaxProcessRightMeta](#method-ajaxProcessRightMeta)
* [archiveThisFile](#method-archiveThisFile)
* [checkDocumentation](#method-checkDocumentation)
* [checkNames](#method-checkNames)
* [checkParentClass](#method-checkParentClass)
* [checkPostedDatas](#method-checkPostedDatas)
* [checkVersionsAndCompatibility](#method-checkVersionsAndCompatibility)
* [checkXmlFields](#method-checkXmlFields)
* [copyTheme](#method-copyTheme)
* [downloadAddonsThemes](#method-downloadAddonsThemes)
* [extractTheme](#method-extractTheme)
* [formatHelperArray](#method-formatHelperArray)
* [formatHelperValuesArray](#method-formatHelperValuesArray)
* [generateArchive](#method-generateArchive)
* [generateXML](#method-generateXML)
* [getModules](#method-getModules)
* [getNativeModule](#method-getNativeModule)
* [hookModule](#method-hookModule)
* [importThemeXmlConfig](#method-importThemeXmlConfig)
* [init](#method-init)
* [initContent](#method-initContent)
* [initPageHeaderToolbar](#method-initPageHeaderToolbar)
* [initProcess](#method-initProcess)
* [installTheme](#method-installTheme)
* [isThemeInstalled](#method-isThemeInstalled)
* [postProcess](#method-postProcess)
* [printResponsiveIcon](#method-printResponsiveIcon)
* [processAdd](#method-processAdd)
* [processDefaultLeftColumn](#method-processDefaultLeftColumn)
* [processDefaultRightColumn](#method-processDefaultRightColumn)
* [processDelete](#method-processDelete)
* [processExportTheme](#method-processExportTheme)
* [processImportTheme](#method-processImportTheme)
* [processLeftMeta](#method-processLeftMeta)
* [processResponsive](#method-processResponsive)
* [processRightMeta](#method-processRightMeta)
* [processThemeInstall](#method-processThemeInstall)
* [processUpdate](#method-processUpdate)
* [processUpdateOptions](#method-processUpdateOptions)
* [recurseCopy](#method-recurseCopy)
* [renderChooseThemeModule](#method-renderChooseThemeModule)
* [renderExportTheme](#method-renderExportTheme)
* [renderExportTheme1](#method-renderExportTheme1)
* [renderForm](#method-renderForm)
* [renderImportTheme](#method-renderImportTheme)
* [renderList](#method-renderList)
* [renderOptions](#method-renderOptions)
* [renderView](#method-renderView)
* [setMedia](#method-setMedia)
* [updateImages](#method-updateImages)
* [updateLogo](#method-updateLogo)
* [updateOptionPsFavicon](#method-updateOptionPsFavicon)
* [updateOptionPsLogo](#method-updateOptionPsLogo)
* [updateOptionPsLogoInvoice](#method-updateOptionPsLogoInvoice)
* [updateOptionPsLogoMail](#method-updateOptionPsLogoMail)
* [updateOptionPsLogoMobile](#method-updateOptionPsLogoMobile)
* [updateOptionPsStoresIcon](#method-updateOptionPsStoresIcon)
* [updateOptionThemeForShop](#method-updateOptionThemeForShop)
* [uploadIco](#method-uploadIco)


Constants
----------


### <a name="constant-MAX_NAME_LENGTH"></a>MAX_NAME_LENGTH

    const MAX_NAME_LENGTH = 128





* Source: [controllers/admin/AdminThemesController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L32).


Properties
----------


### <a name="property-$check_features"></a>$check_features

    public array $check_features = array('ccc' => array('attributes' => array('available' => array('value' => 'true', 'check_if_not_valid' => array('PS_CSS_THEME_CACHE' => 0, 'PS_JS_THEME_CACHE' => 0, 'PS_HTML_THEME_COMPRESSION' => 0, 'PS_JS_HTML_THEME_COMPRESSION' => 0))), 'error' => 'This theme may not correctly use PrestaShop\'s "combine, compress and cache" options.', 'tab' => 'AdminPerformance'), 'guest_checkout' => array('attributes' => array('available' => array('value' => 'true', 'check_if_not_valid' => array('PS_GUEST_CHECKOUT_ENABLED' => 0))), 'error' => 'This theme may not correctly use PrestaShop\'s "guest checkout" feature.', 'tab' => 'AdminPreferences'), 'one_page_checkout' => array('attributes' => array('available' => array('value' => 'true', 'check_if_not_valid' => array('PS_ORDER_PROCESS_TYPE' => 0))), 'error' => 'This theme may not correctly use PrestaShop\'s "one-page checkout" feature.', 'tab' => 'AdminPreferences'), 'store_locator' => array('attributes' => array('available' => array('value' => 'true', 'check_if_not_valid' => array('PS_STORES_SIMPLIFIED' => 0, 'PS_STORES_DISPLAY_FOOTER' => 0))), 'error' => 'This theme may not correctly use PrestaShop\'s "store locator" feature.', 'tab' => 'AdminStores'))

Multidimensional array used to check [theme]/config.xml values,
and also checks prestashop current configuration if not match.



* Visibility: **public**
* This property is **static**.
* Source: [controllers/admin/AdminThemesController.php line 55](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L55).


### <a name="property-$check_features_version"></a>$check_features_version

    public string $check_features_version = '1.4'

This value is used in isThemeCompatible method. only version node with an
higher version number will be used in [theme]/config.xml



* Visibility: **public**
* This property is **static**.
* Source: [controllers/admin/AdminThemesController.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L47).


### <a name="property-$className"></a>$className

    public mixed $className = 'Theme'





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 109](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L109).


### <a name="property-$img_error"></a>$img_error

    private mixed $img_error





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 112](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L112).


### <a name="property-$object"></a>$object

    public \Theme $object





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L30).


### <a name="property-$table"></a>$table

    public mixed $table = 'theme'





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 110](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L110).


### <a name="property-$toolbar_scroll"></a>$toolbar_scroll

    protected mixed $toolbar_scroll = false





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L111).


Methods
-------


### <a name="method-__construct"></a>__construct

    mixed AdminThemesControllerCore::__construct()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L34)




### <a name="method-_checkConfigForFeatures"></a>_checkConfigForFeatures

    boolean AdminThemesControllerCore::_checkConfigForFeatures(array $arrFeatures, mixed $configItem)

_checkConfigForFeatures



* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1925](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1925)


#### Arguments
* $arrFeatures **array** - array of feature code to check
* $configItem **mixed** - will precise the attribute which not matches. If empty, will check every attributes



### <a name="method-_isThemeCompatible"></a>_isThemeCompatible

    boolean AdminThemesControllerCore::_isThemeCompatible(string $theme_dir)

This function checks if the theme designer has thunk to make his theme compatible 1.4,
and noticed it on the $theme_dir/config.xml file. If not, some new functionnalities has
to be desactivated



* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1874](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1874)


#### Arguments
* $theme_dir **string** - theme directory



### <a name="method-ajaxProcessGetAddonsThemes"></a>ajaxProcessGetAddonsThemes

    mixed AdminThemesControllerCore::ajaxProcessGetAddonsThemes()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1851](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1851)




### <a name="method-ajaxProcessLeftMeta"></a>ajaxProcessLeftMeta

    mixed AdminThemesControllerCore::ajaxProcessLeftMeta()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2865](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2865)




### <a name="method-ajaxProcessRightMeta"></a>ajaxProcessRightMeta

    mixed AdminThemesControllerCore::ajaxProcessRightMeta()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2903](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2903)




### <a name="method-archiveThisFile"></a>archiveThisFile

    mixed AdminThemesControllerCore::archiveThisFile(\ZipArchive $obj, string $file, string $server_path, string $archive_path)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 843](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L843)


#### Arguments
* $obj **ZipArchive**
* $file **string**
* $server_path **string**
* $archive_path **string**



### <a name="method-checkDocumentation"></a>checkDocumentation

    mixed AdminThemesControllerCore::checkDocumentation()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 772](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L772)




### <a name="method-checkNames"></a>checkNames

    mixed AdminThemesControllerCore::checkNames()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 754](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L754)




### <a name="method-checkParentClass"></a>checkParentClass

    mixed AdminThemesControllerCore::checkParentClass($name)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 730](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L730)


#### Arguments
* $name **mixed**



### <a name="method-checkPostedDatas"></a>checkPostedDatas

    mixed AdminThemesControllerCore::checkPostedDatas()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 819](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L819)




### <a name="method-checkVersionsAndCompatibility"></a>checkVersionsAndCompatibility

    mixed AdminThemesControllerCore::checkVersionsAndCompatibility()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 801](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L801)




### <a name="method-checkXmlFields"></a>checkXmlFields

    mixed AdminThemesControllerCore::checkXmlFields($xml_file)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 1394](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1394)


#### Arguments
* $xml_file **mixed**



### <a name="method-copyTheme"></a>copyTheme

    boolean AdminThemesControllerCore::copyTheme(string $base_theme_dir, string $target_theme_dir)

copy $base_theme_dir into $target_theme_dir.



* Visibility: **protected**
* This method is **static**.
* Source: [controllers/admin/AdminThemesController.php line 482](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L482)


#### Arguments
* $base_theme_dir **string** - relative path to base dir
* $target_theme_dir **string** - relative path to target dir



### <a name="method-downloadAddonsThemes"></a>downloadAddonsThemes

    mixed AdminThemesControllerCore::downloadAddonsThemes()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 508](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L508)




### <a name="method-extractTheme"></a>extractTheme

    mixed AdminThemesControllerCore::extractTheme($theme_zip_file, $sandbox)





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1512](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1512)


#### Arguments
* $theme_zip_file **mixed**
* $sandbox **mixed**



### <a name="method-formatHelperArray"></a>formatHelperArray

    mixed AdminThemesControllerCore::formatHelperArray($origin_arr)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 2139](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2139)


#### Arguments
* $origin_arr **mixed**



### <a name="method-formatHelperValuesArray"></a>formatHelperValuesArray

    mixed AdminThemesControllerCore::formatHelperValuesArray($originArr)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 2160](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2160)


#### Arguments
* $originArr **mixed**



### <a name="method-generateArchive"></a>generateArchive

    mixed AdminThemesControllerCore::generateArchive()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 857](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L857)




### <a name="method-generateXML"></a>generateXML

    mixed AdminThemesControllerCore::generateXML($theme_to_export, $metas)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 923](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L923)


#### Arguments
* $theme_to_export **mixed**
* $metas **mixed**



### <a name="method-getModules"></a>getModules

    mixed AdminThemesControllerCore::getModules($xml)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 2118](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2118)


#### Arguments
* $xml **mixed**



### <a name="method-getNativeModule"></a>getNativeModule

    array AdminThemesControllerCore::getNativeModule(integer $type)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 1980](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1980)


#### Arguments
* $type **integer** - $type = 0 both native &amp; partner (default)
$type = 1 native
$type = 2 partner



### <a name="method-hookModule"></a>hookModule

    mixed AdminThemesControllerCore::hookModule($id_module, $module_hooks, $shop)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 2406](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2406)


#### Arguments
* $id_module **mixed**
* $module_hooks **mixed**
* $shop **mixed**



### <a name="method-importThemeXmlConfig"></a>importThemeXmlConfig

    array|string AdminThemesControllerCore::importThemeXmlConfig(\SimpleXMLElement $xml, boolean $theme_dir)





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1596](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1596)


#### Arguments
* $xml **SimpleXMLElement**
* $theme_dir **boolean** - only used if the theme directory to import is already located on the shop



### <a name="method-init"></a>init

    mixed AdminThemesControllerCore::init()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L114)




### <a name="method-initContent"></a>initContent

    mixed AdminThemesControllerCore::initContent()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1815](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1815)




### <a name="method-initPageHeaderToolbar"></a>initPageHeaderToolbar

    mixed AdminThemesControllerCore::initPageHeaderToolbar()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 696](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L696)




### <a name="method-initProcess"></a>initProcess

    mixed AdminThemesControllerCore::initProcess()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2765](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2765)




### <a name="method-installTheme"></a>installTheme

    mixed AdminThemesControllerCore::installTheme($theme_dir, $sandbox, $redirect)





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1522](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1522)


#### Arguments
* $theme_dir **mixed**
* $sandbox **mixed**
* $redirect **mixed**



### <a name="method-isThemeInstalled"></a>isThemeInstalled

    mixed AdminThemesControllerCore::isThemeInstalled($theme_name)





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 1577](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1577)


#### Arguments
* $theme_name **mixed**



### <a name="method-postProcess"></a>postProcess

    mixed AdminThemesControllerCore::postProcess()

This functions make checks about AdminThemes configuration edition only.



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2579](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2579)




### <a name="method-printResponsiveIcon"></a>printResponsiveIcon

    mixed AdminThemesControllerCore::printResponsiveIcon($value)





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2806](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2806)


#### Arguments
* $value **mixed**



### <a name="method-processAdd"></a>processAdd

    mixed AdminThemesControllerCore::processAdd()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 553](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L553)




### <a name="method-processDefaultLeftColumn"></a>processDefaultLeftColumn

    mixed AdminThemesControllerCore::processDefaultLeftColumn()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2829](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2829)




### <a name="method-processDefaultRightColumn"></a>processDefaultRightColumn

    mixed AdminThemesControllerCore::processDefaultRightColumn()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2847](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2847)




### <a name="method-processDelete"></a>processDelete

    mixed AdminThemesControllerCore::processDelete()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 656](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L656)




### <a name="method-processExportTheme"></a>processExportTheme

    mixed AdminThemesControllerCore::processExportTheme()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1024](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1024)




### <a name="method-processImportTheme"></a>processImportTheme

    mixed AdminThemesControllerCore::processImportTheme()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1441](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1441)




### <a name="method-processLeftMeta"></a>processLeftMeta

    mixed AdminThemesControllerCore::processLeftMeta()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2884](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2884)




### <a name="method-processResponsive"></a>processResponsive

    mixed AdminThemesControllerCore::processResponsive()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2811](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2811)




### <a name="method-processRightMeta"></a>processRightMeta

    mixed AdminThemesControllerCore::processRightMeta()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2922](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2922)




### <a name="method-processThemeInstall"></a>processThemeInstall

    mixed AdminThemesControllerCore::processThemeInstall()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2428](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2428)




### <a name="method-processUpdate"></a>processUpdate

    mixed AdminThemesControllerCore::processUpdate()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 613](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L613)




### <a name="method-processUpdateOptions"></a>processUpdateOptions

    mixed AdminThemesControllerCore::processUpdateOptions()





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 647](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L647)




### <a name="method-recurseCopy"></a>recurseCopy

    mixed AdminThemesControllerCore::recurseCopy($src, $dst)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 1421](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1421)


#### Arguments
* $src **mixed**
* $dst **mixed**



### <a name="method-renderChooseThemeModule"></a>renderChooseThemeModule

    mixed AdminThemesControllerCore::renderChooseThemeModule()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2172](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2172)




### <a name="method-renderExportTheme"></a>renderExportTheme

    mixed AdminThemesControllerCore::renderExportTheme()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1343](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1343)




### <a name="method-renderExportTheme1"></a>renderExportTheme1

    mixed AdminThemesControllerCore::renderExportTheme1()





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 1147](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1147)




### <a name="method-renderForm"></a>renderForm

    mixed AdminThemesControllerCore::renderForm()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 249](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L249)




### <a name="method-renderImportTheme"></a>renderImportTheme

    mixed AdminThemesControllerCore::renderImportTheme()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 1694](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L1694)




### <a name="method-renderList"></a>renderList

    mixed AdminThemesControllerCore::renderList()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 469](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L469)




### <a name="method-renderOptions"></a>renderOptions

    mixed AdminThemesControllerCore::renderOptions()

Function used to render the options for this controller



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2945](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2945)




### <a name="method-renderView"></a>renderView

    mixed AdminThemesControllerCore::renderView()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2560](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2560)




### <a name="method-setMedia"></a>setMedia

    mixed AdminThemesControllerCore::setMedia()





* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2969](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2969)




### <a name="method-updateImages"></a>updateImages

    mixed AdminThemesControllerCore::updateImages($xml)





* Visibility: **private**
* Source: [controllers/admin/AdminThemesController.php line 2377](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2377)


#### Arguments
* $xml **mixed**



### <a name="method-updateLogo"></a>updateLogo

    boolean AdminThemesControllerCore::updateLogo($field_name, $logo_prefix)

Generic function which allows logo upload



* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 2648](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2648)


#### Arguments
* $field_name **mixed**
* $logo_prefix **mixed**



### <a name="method-updateOptionPsFavicon"></a>updateOptionPsFavicon

    mixed AdminThemesControllerCore::updateOptionPsFavicon()

Update PS_FAVICON



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2719](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2719)




### <a name="method-updateOptionPsLogo"></a>updateOptionPsLogo

    mixed AdminThemesControllerCore::updateOptionPsLogo()

Update PS_LOGO



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2603](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2603)




### <a name="method-updateOptionPsLogoInvoice"></a>updateOptionPsLogoInvoice

    mixed AdminThemesControllerCore::updateOptionPsLogoInvoice()

Update PS_LOGO_INVOICE



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2627](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2627)




### <a name="method-updateOptionPsLogoMail"></a>updateOptionPsLogoMail

    mixed AdminThemesControllerCore::updateOptionPsLogoMail()

Update PS_LOGO_MAIL



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2619](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2619)




### <a name="method-updateOptionPsLogoMobile"></a>updateOptionPsLogoMobile

    mixed AdminThemesControllerCore::updateOptionPsLogoMobile()

Update PS_LOGO_MOBILE



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2611](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2611)




### <a name="method-updateOptionPsStoresIcon"></a>updateOptionPsStoresIcon

    mixed AdminThemesControllerCore::updateOptionPsStoresIcon()

Update PS_STORES_ICON



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2635](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2635)




### <a name="method-updateOptionThemeForShop"></a>updateOptionThemeForShop

    mixed AdminThemesControllerCore::updateOptionThemeForShop()

Update theme for current shop



* Visibility: **public**
* Source: [controllers/admin/AdminThemesController.php line 2736](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2736)




### <a name="method-uploadIco"></a>uploadIco

    mixed AdminThemesControllerCore::uploadIco($name, $dest)





* Visibility: **protected**
* Source: [controllers/admin/AdminThemesController.php line 2750](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/controllers/admin/AdminThemesController.php#L2750)


#### Arguments
* $name **mixed**
* $dest **mixed**

