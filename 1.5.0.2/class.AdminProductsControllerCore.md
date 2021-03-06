Class AdminProductsControllerCore
=====================





* Class name: AdminProductsControllerCore
* Parent class: [AdminController](class.AdminControllerCore.md)
* Source: [controllers/admin/AdminProductsController.php line 28](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L28)


Contents
--------


### Properties

* [$_category](#property-$_category)
* [$available_tabs](#property-$available_tabs)
* [$available_tabs_lang](#property-$available_tabs_lang)
* [$max_file_size](#property-$max_file_size)
* [$max_image_size](#property-$max_image_size)
* [$tab_display](#property-$tab_display)
* [$tabs_preloaded](#property-$tabs_preloaded)
* [$_defaultOrderBy](#property-$_defaultOrderBy)
* [$_errors](#property-$_errors)
* [$_filter](#property-$_filter)
* [$_group](#property-$_group)
* [$_having](#property-$_having)
* [$_includeContainer](#property-$_includeContainer)
* [$_join](#property-$_join)
* [$_languages](#property-$_languages)
* [$_list](#property-$_list)
* [$_listTotal](#property-$_listTotal)
* [$_orderBy](#property-$_orderBy)
* [$_orderWay](#property-$_orderWay)
* [$_pagination](#property-$_pagination)
* [$_redirect](#property-$_redirect)
* [$_select](#property-$_select)
* [$_tmpTableFilter](#property-$_tmpTableFilter)
* [$_where](#property-$_where)
* [$action](#property-$action)
* [$actions](#property-$actions)
* [$actions_available](#property-$actions_available)
* [$allow_employee_form_lang](#property-$allow_employee_form_lang)
* [$base_tpl_form](#property-$base_tpl_form)
* [$base_tpl_view](#property-$base_tpl_view)
* [$boxes](#property-$boxes)
* [$bulk_actions](#property-$bulk_actions)
* [$cache_lang](#property-$cache_lang)
* [$className](#property-$className)
* [$colorOnBackground](#property-$colorOnBackground)
* [$confirmations](#property-$confirmations)
* [$content](#property-$content)
* [$currentIndex](#property-$currentIndex)
* [$default_form_language](#property-$default_form_language)
* [$deleted](#property-$deleted)
* [$display](#property-$display)
* [$fieldImageSettings](#property-$fieldImageSettings)
* [$fieldsDisplay](#property-$fieldsDisplay)
* [$fields_form](#property-$fields_form)
* [$fields_value](#property-$fields_value)
* [$filter](#property-$filter)
* [$id](#property-$id)
* [$id_object](#property-$id_object)
* [$identifier](#property-$identifier)
* [$identifiersDnd](#property-$identifiersDnd)
* [$imageType](#property-$imageType)
* [$informations](#property-$informations)
* [$is_cms](#property-$is_cms)
* [$is_dnd_identifier](#property-$is_dnd_identifier)
* [$lang](#property-$lang)
* [$layout](#property-$layout)
* [$list_no_link](#property-$list_no_link)
* [$list_simple_header](#property-$list_simple_header)
* [$list_skip_actions](#property-$list_skip_actions)
* [$meta_title](#property-$meta_title)
* [$multiple_fieldsets](#property-$multiple_fieldsets)
* [$noLink](#property-$noLink)
* [$noTabLink](#property-$noTabLink)
* [$object](#property-$object)
* [$options](#property-$options)
* [$path](#property-$path)
* [$required_database](#property-$required_database)
* [$required_fields](#property-$required_fields)
* [$shopLink](#property-$shopLink)
* [$shopLinkType](#property-$shopLinkType)
* [$shopShareDatas](#property-$shopShareDatas)
* [$show_toolbar](#property-$show_toolbar)
* [$show_toolbar_options](#property-$show_toolbar_options)
* [$specificConfirmDelete](#property-$specificConfirmDelete)
* [$tabAccess](#property-$tabAccess)
* [$table](#property-$table)
* [$template](#property-$template)
* [$token](#property-$token)
* [$toolbar_btn](#property-$toolbar_btn)
* [$toolbar_fix](#property-$toolbar_fix)
* [$toolbar_title](#property-$toolbar_title)
* [$tpl_delete_link_vars](#property-$tpl_delete_link_vars)
* [$tpl_folder](#property-$tpl_folder)
* [$tpl_form_vars](#property-$tpl_form_vars)
* [$tpl_list_vars](#property-$tpl_list_vars)
* [$tpl_option_vars](#property-$tpl_option_vars)
* [$tpl_required_fields_vars](#property-$tpl_required_fields_vars)
* [$tpl_view_vars](#property-$tpl_view_vars)
* [$warnings](#property-$warnings)
* [$ajax](#property-$ajax)
* [$content_only](#property-$content_only)
* [$context](#property-$context)
* [$css_files](#property-$css_files)
* [$display_footer](#property-$display_footer)
* [$display_header](#property-$display_header)
* [$hook_list](#property-$hook_list)
* [$js_files](#property-$js_files)
* [$json](#property-$json)
* [$redirect_after](#property-$redirect_after)
* [$status](#property-$status)

### Methods

* [__construct](#method-__construct)
* [_applyTaxToEcotax](#method-_applyTaxToEcotax)
* [_childValidation](#method-_childValidation)
* [_cleanMetaKeywords](#method-_cleanMetaKeywords)
* [_displayDraftWarning](#method-_displayDraftWarning)
* [_displayLabelField](#method-_displayLabelField)
* [_displayLabelFields](#method-_displayLabelFields)
* [_displaySpecificPriceModificationForm](#method-_displaySpecificPriceModificationForm)
* [_displayUnavailableProductWarning](#method-_displayUnavailableProductWarning)
* [_getCustomizationFieldIds](#method-_getCustomizationFieldIds)
* [_getFinalPrice](#method-_getFinalPrice)
* [_removeTaxFromEcotax](#method-_removeTaxFromEcotax)
* [_validateSpecificPrice](#method-_validateSpecificPrice)
* [addCSS](#method-addCSS)
* [addCarriers](#method-addCarriers)
* [addJS](#method-addJS)
* [addJquery](#method-addJquery)
* [addJqueryPlugin](#method-addJqueryPlugin)
* [addJqueryUI](#method-addJqueryUI)
* [addProductImage](#method-addProductImage)
* [addRowAction](#method-addRowAction)
* [addRowActionSkipList](#method-addRowActionSkipList)
* [afterAdd](#method-afterAdd)
* [afterDelete](#method-afterDelete)
* [afterImageUpload](#method-afterImageUpload)
* [afterUpdate](#method-afterUpdate)
* [ajaxPreProcess](#method-ajaxPreProcess)
* [ajaxProcessAddImage](#method-ajaxProcessAddImage)
* [ajaxProcessDefaultProductAttribute](#method-ajaxProcessDefaultProductAttribute)
* [ajaxProcessDeleteProductAttribute](#method-ajaxProcessDeleteProductAttribute)
* [ajaxProcessDeleteProductImage](#method-ajaxProcessDeleteProductImage)
* [ajaxProcessEditProductAttribute](#method-ajaxProcessEditProductAttribute)
* [ajaxProcessHelpAccess](#method-ajaxProcessHelpAccess)
* [ajaxProcessProductManufacturers](#method-ajaxProcessProductManufacturers)
* [ajaxProcessProductQuantity](#method-ajaxProcessProductQuantity)
* [ajaxProcessSearchCustomers](#method-ajaxProcessSearchCustomers)
* [ajaxProcessUpdateCover](#method-ajaxProcessUpdateCover)
* [ajaxProcessUpdateImagePosition](#method-ajaxProcessUpdateImagePosition)
* [ajaxProcessUpdateProductImageShopAsso](#method-ajaxProcessUpdateProductImageShopAsso)
* [beforeAdd](#method-beforeAdd)
* [beforeDelete](#method-beforeDelete)
* [beforeUpdateOptions](#method-beforeUpdateOptions)
* [checkAccess](#method-checkAccess)
* [checkFeatures](#method-checkFeatures)
* [checkProduct](#method-checkProduct)
* [checkToken](#method-checkToken)
* [copyFromPost](#method-copyFromPost)
* [copyImage](#method-copyImage)
* [deleteDownloadProduct](#method-deleteDownloadProduct)
* [display](#method-display)
* [displayAjax](#method-displayAjax)
* [displayFooter](#method-displayFooter)
* [displayHeader](#method-displayHeader)
* [displayInformation](#method-displayInformation)
* [displayNoSmarty](#method-displayNoSmarty)
* [displayRequiredFields](#method-displayRequiredFields)
* [displayWarning](#method-displayWarning)
* [filterToField](#method-filterToField)
* [getAssoShop](#method-getAssoShop)
* [getCarrierList](#method-getCarrierList)
* [getCombinationImagesJS](#method-getCombinationImagesJS)
* [getController](#method-getController)
* [getFieldValue](#method-getFieldValue)
* [getFieldsValue](#method-getFieldsValue)
* [getL](#method-getL)
* [getList](#method-getList)
* [getPreviewUrl](#method-getPreviewUrl)
* [getTranslationsFlags](#method-getTranslationsFlags)
* [getlanguages](#method-getlanguages)
* [haveThisAccessory](#method-haveThisAccessory)
* [init](#method-init)
* [initContent](#method-initContent)
* [initCursedPage](#method-initCursedPage)
* [initFooter](#method-initFooter)
* [initFormAccounting](#method-initFormAccounting)
* [initFormAssociations](#method-initFormAssociations)
* [initFormAttachments](#method-initFormAttachments)
* [initFormAttributes](#method-initFormAttributes)
* [initFormCombinations](#method-initFormCombinations)
* [initFormCustomization](#method-initFormCustomization)
* [initFormFeatures](#method-initFormFeatures)
* [initFormImages](#method-initFormImages)
* [initFormInformations](#method-initFormInformations)
* [initFormPack](#method-initFormPack)
* [initFormPrices](#method-initFormPrices)
* [initFormQuantities](#method-initFormQuantities)
* [initFormSeo](#method-initFormSeo)
* [initFormShipping](#method-initFormShipping)
* [initFormSuppliers](#method-initFormSuppliers)
* [initFormVirtualProduct](#method-initFormVirtualProduct)
* [initFormWarehouses](#method-initFormWarehouses)
* [initHeader](#method-initHeader)
* [initPack](#method-initPack)
* [initProcess](#method-initProcess)
* [initToolbar](#method-initToolbar)
* [initToolbarTitle](#method-initToolbarTitle)
* [l](#method-l)
* [loadObject](#method-loadObject)
* [postImage](#method-postImage)
* [postProcess](#method-postProcess)
* [processAccounting](#method-processAccounting)
* [processAdd](#method-processAdd)
* [processAddAttachments](#method-processAddAttachments)
* [processAttachments](#method-processAttachments)
* [processBulkAffectZone](#method-processBulkAffectZone)
* [processBulkDelete](#method-processBulkDelete)
* [processCustomizationConfiguration](#method-processCustomizationConfiguration)
* [processDelete](#method-processDelete)
* [processDeleteImage](#method-processDeleteImage)
* [processDeleteSpecificPrice](#method-processDeleteSpecificPrice)
* [processDeleteVirtualProduct](#method-processDeleteVirtualProduct)
* [processDeleteVirtualProductAttribute](#method-processDeleteVirtualProductAttribute)
* [processDuplicate](#method-processDuplicate)
* [processFeatures](#method-processFeatures)
* [processFilter](#method-processFilter)
* [processImage](#method-processImage)
* [processPosition](#method-processPosition)
* [processPriceAddition](#method-processPriceAddition)
* [processPricesModification](#method-processPricesModification)
* [processProductAttribute](#method-processProductAttribute)
* [processProductCustomization](#method-processProductCustomization)
* [processResetFilters](#method-processResetFilters)
* [processSave](#method-processSave)
* [processSpecificPricePriorities](#method-processSpecificPricePriorities)
* [processStatus](#method-processStatus)
* [processSuppliers](#method-processSuppliers)
* [processUpdate](#method-processUpdate)
* [processUpdateFields](#method-processUpdateFields)
* [processUpdateOptions](#method-processUpdateOptions)
* [processWarehouses](#method-processWarehouses)
* [recurseCategoryForInclude](#method-recurseCategoryForInclude)
* [redirect](#method-redirect)
* [renderForm](#method-renderForm)
* [renderList](#method-renderList)
* [renderListAttributes](#method-renderListAttributes)
* [renderOptions](#method-renderOptions)
* [renderView](#method-renderView)
* [run](#method-run)
* [setHelperDisplay](#method-setHelperDisplay)
* [setMedia](#method-setMedia)
* [setTemplate](#method-setTemplate)
* [translate](#method-translate)
* [updateAccessories](#method-updateAccessories)
* [updateAssoShop](#method-updateAssoShop)
* [updateDownloadProduct](#method-updateDownloadProduct)
* [updatePackItems](#method-updatePackItems)
* [updateTags](#method-updateTags)
* [uploadImage](#method-uploadImage)
* [validateField](#method-validateField)
* [validateRules](#method-validateRules)
* [viewAccess](#method-viewAccess)
* [viewDetails](#method-viewDetails)




Properties
----------


### <a name="property-$_category"></a>$_category

```php
private mixed $_category
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L37).


### <a name="property-$available_tabs"></a>$available_tabs

```php
protected mixed $available_tabs = array('Informations', 'Pack', 'VirtualProduct', 'Prices', 'Seo', 'Associations', 'Images', 'Shipping', 'Combinations', 'Features', 'Customization', 'Attachments', 'Quantities', 'Suppliers', 'Warehouses', 'Accounting')
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L43).


### <a name="property-$available_tabs_lang"></a>$available_tabs_lang

```php
protected mixed $available_tabs_lang = array()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L62).


### <a name="property-$max_file_size"></a>$max_file_size

```php
protected mixed $max_file_size = NULL
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L30).


### <a name="property-$max_image_size"></a>$max_image_size

```php
protected integer $max_image_size = NULL
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L35).


### <a name="property-$tab_display"></a>$tab_display

```php
protected string $tab_display
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L41).


### <a name="property-$tabs_preloaded"></a>$tabs_preloaded

```php
protected mixed $tabs_preloaded = array('Informations' => true, 'Prices' => true, 'Seo' => true, 'Associations' => true, 'Images' => false, 'Shipping' => true, 'Combinations' => true, 'Features' => false, 'Customization' => false, 'Attachments' => false, 'Quantities' => true, 'Suppliers' => false, 'Warehouses' => false, 'Accounting' => false, 'Pack' => true, 'VirtualProduct' => true)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 64](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L64).


### <a name="property-$_defaultOrderBy"></a>$_defaultOrderBy

```php
protected string $_defaultOrderBy = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 76](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L76).


### <a name="property-$_errors"></a>$_errors

```php
public array $_errors = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L94).


### <a name="property-$_filter"></a>$_filter

```php
protected array $_filter
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 135](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L135).


### <a name="property-$_group"></a>$_group

```php
protected string $_group
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 196](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L196).


### <a name="property-$_having"></a>$_having

```php
protected string $_having
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 199](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L199).


### <a name="property-$_includeContainer"></a>$_includeContainer

```php
protected mixed $_includeContainer = true
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 225](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L225).


### <a name="property-$_join"></a>$_join

```php
protected string $_join
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 190](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L190).


### <a name="property-$_languages"></a>$_languages

```php
public mixed $_languages = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 39](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L39).


### <a name="property-$_list"></a>$_list

```php
protected array $_list = array()
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 111](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L111).


### <a name="property-$_listTotal"></a>$_listTotal

```php
protected integer $_listTotal
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 129](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L129).


### <a name="property-$_orderBy"></a>$_orderBy

```php
protected string $_orderBy
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 144](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L144).


### <a name="property-$_orderWay"></a>$_orderWay

```php
protected string $_orderWay
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 147](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L147).


### <a name="property-$_pagination"></a>$_pagination

```php
protected array $_pagination = array(20, 50, 100, 300)
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 141](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L141).


### <a name="property-$_redirect"></a>$_redirect

```php
protected boolean $_redirect = true
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 230](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L230).


### <a name="property-$_select"></a>$_select

```php
protected string $_select
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 187](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L187).


### <a name="property-$_tmpTableFilter"></a>$_tmpTableFilter

```php
protected array $_tmpTableFilter = ''
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 138](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L138).


### <a name="property-$_where"></a>$_where

```php
protected string $_where
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 193](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L193).


### <a name="property-$action"></a>$action

```php
protected mixed $action
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 223](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L223).


### <a name="property-$actions"></a>$actions

```php
protected array $actions = array()
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 153](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L153).


### <a name="property-$actions_available"></a>$actions_available

```php
protected array $actions_available = array('view', 'edit', 'delete', 'duplicate')
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 150](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L150).


### <a name="property-$allow_employee_form_lang"></a>$allow_employee_form_lang

```php
public mixed $allow_employee_form_lang
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L41).


### <a name="property-$base_tpl_form"></a>$base_tpl_form

```php
public mixed $base_tpl_form = null
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 86](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L86).


### <a name="property-$base_tpl_view"></a>$base_tpl_view

```php
public mixed $base_tpl_view = null
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 85](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L85).


### <a name="property-$boxes"></a>$boxes

```php
protected array $boxes
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 184](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L184).


### <a name="property-$bulk_actions"></a>$bulk_actions

```php
protected array $bulk_actions
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 179](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L179).


### <a name="property-$cache_lang"></a>$cache_lang

```php
public array $cache_lang = array()
```





* Visibility: **public**
* This property is **static**.
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 162](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L162).


### <a name="property-$className"></a>$className

```php
public string $className
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 56](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L56).


### <a name="property-$colorOnBackground"></a>$colorOnBackground

```php
protected mixed $colorOnBackground
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 221](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L221).


### <a name="property-$confirmations"></a>$confirmations

```php
public mixed $confirmations = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L36).


### <a name="property-$content"></a>$content

```php
public mixed $content
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 33](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L33).


### <a name="property-$currentIndex"></a>$currentIndex

```php
public mixed $currentIndex
```





* Visibility: **public**
* This property is **static**.
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 32](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L32).


### <a name="property-$default_form_language"></a>$default_form_language

```php
public mixed $default_form_language
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L40).


### <a name="property-$deleted"></a>$deleted

```php
protected boolean $deleted = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 214](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L214).


### <a name="property-$display"></a>$display

```php
protected mixed $display
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 224](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L224).


### <a name="property-$fieldImageSettings"></a>$fieldImageSettings

```php
public array $fieldImageSettings = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 233](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L233).


### <a name="property-$fieldsDisplay"></a>$fieldsDisplay

```php
protected array $fieldsDisplay
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L100).


### <a name="property-$fields_form"></a>$fields_form

```php
protected array $fields_form
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 103](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L103).


### <a name="property-$fields_value"></a>$fields_value

```php
public mixed $fields_value = false
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L91).


### <a name="property-$filter"></a>$filter

```php
protected boolean $filter
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 218](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L218).


### <a name="property-$id"></a>$id

```php
public integer $id = -1
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 62](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L62).


### <a name="property-$id_object"></a>$id_object

```php
protected \current $id_object
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 242](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L242).


### <a name="property-$identifier"></a>$identifier

```php
protected string $identifier = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 53](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L53).


### <a name="property-$identifiersDnd"></a>$identifiersDnd

```php
protected mixed $identifiersDnd = array('id_product' => 'id_product', 'id_category' => 'id_category_to_move', 'id_cms_category' => 'id_cms_category_to_move', 'id_cms' => 'id_cms', 'id_attribute' => 'id_attribute')
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 205](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L205).


### <a name="property-$imageType"></a>$imageType

```php
public string $imageType = 'jpg'
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 236](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L236).


### <a name="property-$informations"></a>$informations

```php
public mixed $informations = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L35).


### <a name="property-$is_cms"></a>$is_cms

```php
protected mixed $is_cms = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 201](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L201).


### <a name="property-$is_dnd_identifier"></a>$is_dnd_identifier

```php
protected mixed $is_dnd_identifier = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 203](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L203).


### <a name="property-$lang"></a>$lang

```php
public boolean $lang = false
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 132](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L132).


### <a name="property-$layout"></a>$layout

```php
public mixed $layout = 'layout.tpl'
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 43](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L43).


### <a name="property-$list_no_link"></a>$list_no_link

```php
protected boolean $list_no_link = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 159](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L159).


### <a name="property-$list_simple_header"></a>$list_simple_header

```php
protected \define $list_simple_header
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L97).


### <a name="property-$list_skip_actions"></a>$list_skip_actions

```php
protected array $list_skip_actions = array()
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 156](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L156).


### <a name="property-$meta_title"></a>$meta_title

```php
public mixed $meta_title = 'Administration panel'
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L45).


### <a name="property-$multiple_fieldsets"></a>$multiple_fieldsets

```php
public boolean $multiple_fieldsets = false
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 89](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L89).


### <a name="property-$noLink"></a>$noLink

```php
protected mixed $noLink
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 219](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L219).


### <a name="property-$noTabLink"></a>$noTabLink

```php
public array $noTabLink = array('AdminCatalog', 'AdminTools', 'AdminStock', 'AdminAccounting')
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 65](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L65).


### <a name="property-$object"></a>$object

```php
protected \instanciation $object
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 239](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L239).


### <a name="property-$options"></a>$options

```php
protected array $options
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L106).


### <a name="property-$path"></a>$path

```php
public mixed $path
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L30).


### <a name="property-$required_database"></a>$required_database

```php
public mixed $required_database = false
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 67](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L67).


### <a name="property-$required_fields"></a>$required_fields

```php
public array $required_fields = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 165](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L165).


### <a name="property-$shopLink"></a>$shopLink

```php
protected mixed $shopLink
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 108](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L108).


### <a name="property-$shopLinkType"></a>$shopLinkType

```php
public string $shopLinkType
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L73).


### <a name="property-$shopShareDatas"></a>$shopShareDatas

```php
public mixed $shopShareDatas = false
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 37](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L37).


### <a name="property-$show_toolbar"></a>$show_toolbar

```php
protected boolean $show_toolbar = true
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 123](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L123).


### <a name="property-$show_toolbar_options"></a>$show_toolbar_options

```php
protected boolean $show_toolbar_options = false
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 126](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L126).


### <a name="property-$specificConfirmDelete"></a>$specificConfirmDelete

```php
protected mixed $specificConfirmDelete
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 220](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L220).


### <a name="property-$tabAccess"></a>$tabAccess

```php
public array $tabAccess
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 59](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L59).


### <a name="property-$table"></a>$table

```php
public string $table
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 50](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L50).


### <a name="property-$template"></a>$template

```php
public mixed $template = 'content.tpl'
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 47](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L47).


### <a name="property-$token"></a>$token

```php
public string $token
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 70](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L70).


### <a name="property-$toolbar_btn"></a>$toolbar_btn

```php
protected array $toolbar_btn = null
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 117](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L117).


### <a name="property-$toolbar_fix"></a>$toolbar_fix

```php
protected array $toolbar_fix = true
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 120](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L120).


### <a name="property-$toolbar_title"></a>$toolbar_title

```php
protected \define $toolbar_title
```





* Visibility: **protected**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 114](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L114).


### <a name="property-$tpl_delete_link_vars"></a>$tpl_delete_link_vars

```php
public mixed $tpl_delete_link_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 80](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L80).


### <a name="property-$tpl_folder"></a>$tpl_folder

```php
public mixed $tpl_folder
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 227](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L227).


### <a name="property-$tpl_form_vars"></a>$tpl_form_vars

```php
public mixed $tpl_form_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L78).


### <a name="property-$tpl_list_vars"></a>$tpl_list_vars

```php
public mixed $tpl_list_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 79](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L79).


### <a name="property-$tpl_option_vars"></a>$tpl_option_vars

```php
public mixed $tpl_option_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L81).


### <a name="property-$tpl_required_fields_vars"></a>$tpl_required_fields_vars

```php
public mixed $tpl_required_fields_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 83](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L83).


### <a name="property-$tpl_view_vars"></a>$tpl_view_vars

```php
public mixed $tpl_view_vars = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 82](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L82).


### <a name="property-$warnings"></a>$warnings

```php
public mixed $warnings = array()
```





* Visibility: **public**
* This property is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 34](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L34).


### <a name="property-$ajax"></a>$ajax

```php
protected boolean $ajax = false
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 71](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L71).


### <a name="property-$content_only"></a>$content_only

```php
protected string $content_only = false
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L66).


### <a name="property-$context"></a>$context

```php
protected \Context $context
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 36](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L36).


### <a name="property-$css_files"></a>$css_files

```php
public array $css_files = array()
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 41](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L41).


### <a name="property-$display_footer"></a>$display_footer

```php
protected string $display_footer
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 61](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L61).


### <a name="property-$display_header"></a>$display_header

```php
protected boolean $display_header
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L51).


### <a name="property-$hook_list"></a>$hook_list

```php
public mixed $hook_list = array()
```

hook_list is used with liveEdit



* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L78).


### <a name="property-$js_files"></a>$js_files

```php
public array $js_files = array()
```





* Visibility: **public**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 46](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L46).


### <a name="property-$json"></a>$json

```php
protected mixed $json = false
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L72).


### <a name="property-$redirect_after"></a>$redirect_after

```php
protected mixed $redirect_after = null
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L75).


### <a name="property-$status"></a>$status

```php
protected mixed $status = ''
```





* Visibility: **protected**
* This property is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 73](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L73).


Methods
-------


### <a name="method-__construct"></a>__construct

```php
mixed AdminProductsControllerCore::__construct()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 83](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L83)




### <a name="method-_applyTaxToEcotax"></a>_applyTaxToEcotax

```php
mixed AdminProductsControllerCore::_applyTaxToEcotax($product)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 1622](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1622)


#### Arguments
* $product **mixed**



### <a name="method-_childValidation"></a>_childValidation

```php
mixed AdminControllerCore::_childValidation()
```

Overload this method for custom checking



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2204](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2204)




### <a name="method-_cleanMetaKeywords"></a>_cleanMetaKeywords

```php
mixed AdminProductsControllerCore::_cleanMetaKeywords($keywords)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 216](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L216)


#### Arguments
* $keywords **mixed**



### <a name="method-_displayDraftWarning"></a>_displayDraftWarning

```php
mixed AdminProductsControllerCore::_displayDraftWarning($active)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 1999](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1999)


#### Arguments
* $active **mixed**



### <a name="method-_displayLabelField"></a>_displayLabelField

```php
mixed AdminProductsControllerCore::_displayLabelField($label, $languages, $default_language, $type, $fieldIds, $id_customization_field)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 2985](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2985)


#### Arguments
* $label **mixed**
* $languages **mixed**
* $default_language **mixed**
* $type **mixed**
* $fieldIds **mixed**
* $id_customization_field **mixed**



### <a name="method-_displayLabelFields"></a>_displayLabelFields

```php
mixed AdminProductsControllerCore::_displayLabelFields($obj, $labels, $languages, $default_language, $type)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 3008](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3008)


#### Arguments
* $obj **mixed**
* $labels **mixed**
* $languages **mixed**
* $default_language **mixed**
* $type **mixed**



### <a name="method-_displaySpecificPriceModificationForm"></a>_displaySpecificPriceModificationForm

```php
mixed AdminProductsControllerCore::_displaySpecificPriceModificationForm($defaultCurrency, $shops, $currencies, $countries, $groups)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 2800](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2800)


#### Arguments
* $defaultCurrency **mixed**
* $shops **mixed**
* $currencies **mixed**
* $countries **mixed**
* $groups **mixed**



### <a name="method-_displayUnavailableProductWarning"></a>_displayUnavailableProductWarning

```php
mixed AdminProductsControllerCore::_displayUnavailableProductWarning()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 3916](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3916)




### <a name="method-_getCustomizationFieldIds"></a>_getCustomizationFieldIds

```php
mixed AdminProductsControllerCore::_getCustomizationFieldIds($labels, $alreadyGenerated, $obj)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 2967](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2967)


#### Arguments
* $labels **mixed**
* $alreadyGenerated **mixed**
* $obj **mixed**



### <a name="method-_getFinalPrice"></a>_getFinalPrice

```php
mixed AdminProductsControllerCore::_getFinalPrice($specific_price, $productPrice, $taxRate)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 2792](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2792)


#### Arguments
* $specific_price **mixed**
* $productPrice **mixed**
* $taxRate **mixed**



### <a name="method-_removeTaxFromEcotax"></a>_removeTaxFromEcotax

```php
mixed AdminProductsControllerCore::_removeTaxFromEcotax()
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 1615](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1615)




### <a name="method-_validateSpecificPrice"></a>_validateSpecificPrice

```php
mixed AdminProductsControllerCore::_validateSpecificPrice($id_shop, $id_currency, $id_country, $id_group, $id_customer, $price, $from_quantity, $reduction, $reduction_type, $from, $to)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 1273](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1273)


#### Arguments
* $id_shop **mixed**
* $id_currency **mixed**
* $id_country **mixed**
* $id_group **mixed**
* $id_customer **mixed**
* $price **mixed**
* $from_quantity **mixed**
* $reduction **mixed**
* $reduction_type **mixed**
* $from **mixed**
* $to **mixed**



### <a name="method-addCSS"></a>addCSS

```php
true ControllerCore::addCSS(mixed $css_uri, string $css_media_type)
```

Add a new stylesheet in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 228](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L228)


#### Arguments
* $css_uri **mixed** - Path to css file, or list of css files like this : array(array(uri =&gt; media_type), ...)
* $css_media_type **string**



### <a name="method-addCarriers"></a>addCarriers

```php
mixed AdminProductsControllerCore::addCarriers()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 3199](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3199)




### <a name="method-addJS"></a>addJS

```php
void ControllerCore::addJS(mixed $js_uri)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 260](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L260)


#### Arguments
* $js_uri **mixed**



### <a name="method-addJquery"></a>addJquery

```php
void ControllerCore::addJquery($version, $folder, $minifier)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 283](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L283)


#### Arguments
* $version **mixed**
* $folder **mixed**
* $minifier **mixed**



### <a name="method-addJqueryPlugin"></a>addJqueryPlugin

```php
void ControllerCore::addJqueryPlugin($name, $folder)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 313](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L313)


#### Arguments
* $name **mixed**
* $folder **mixed**



### <a name="method-addJqueryUI"></a>addJqueryUI

```php
void ControllerCore::addJqueryUI($component, $theme, $check_dependencies)
```

Add a new javascript file in page header.



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 294](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L294)


#### Arguments
* $component **mixed**
* $theme **mixed**
* $check_dependencies **mixed**



### <a name="method-addProductImage"></a>addProductImage

```php
mixed AdminProductsControllerCore::addProductImage(object $product, $method)
```

Add or update a product image



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1318](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1318)


#### Arguments
* $product **object** - Product object to add image
* $method **mixed**



### <a name="method-addRowAction"></a>addRowAction

```php
mixed AdminControllerCore::addRowAction($action)
```

Declare an action to use for each row in the list



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1330](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1330)


#### Arguments
* $action **mixed**



### <a name="method-addRowActionSkipList"></a>addRowActionSkipList

```php
mixed AdminControllerCore::addRowActionSkipList($action, $list)
```

Add  an action to use for each row in the list



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1339](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1339)


#### Arguments
* $action **mixed**
* $list **mixed**



### <a name="method-afterAdd"></a>afterAdd

```php
mixed AdminControllerCore::afterAdd($object)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2233](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2233)


#### Arguments
* $object **mixed**



### <a name="method-afterDelete"></a>afterDelete

```php
boolean AdminControllerCore::afterDelete(object $object, $oldId)
```

Called before deletion



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2228](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2228)


#### Arguments
* $object **object** - Object
* $oldId **mixed**



### <a name="method-afterImageUpload"></a>afterImageUpload

```php
boolean AdminControllerCore::afterImageUpload()
```

Check rights to view the current tab



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2249](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2249)




### <a name="method-afterUpdate"></a>afterUpdate

```php
mixed AdminControllerCore::afterUpdate($object)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2238](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2238)


#### Arguments
* $object **mixed**



### <a name="method-ajaxPreProcess"></a>ajaxPreProcess

```php
mixed AdminProductsControllerCore::ajaxPreProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1167](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1167)




### <a name="method-ajaxProcessAddImage"></a>ajaxProcessAddImage

```php
mixed AdminProductsControllerCore::ajaxProcessAddImage()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1039](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1039)




### <a name="method-ajaxProcessDefaultProductAttribute"></a>ajaxProcessDefaultProductAttribute

```php
mixed AdminProductsControllerCore::ajaxProcessDefaultProductAttribute()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1112](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1112)




### <a name="method-ajaxProcessDeleteProductAttribute"></a>ajaxProcessDeleteProductAttribute

```php
mixed AdminProductsControllerCore::ajaxProcessDeleteProductAttribute()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1063](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1063)




### <a name="method-ajaxProcessDeleteProductImage"></a>ajaxProcessDeleteProductImage

```php
mixed AdminProductsControllerCore::ajaxProcessDeleteProductImage()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1242](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1242)




### <a name="method-ajaxProcessEditProductAttribute"></a>ajaxProcessEditProductAttribute

```php
mixed AdminProductsControllerCore::ajaxProcessEditProductAttribute()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1138](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1138)




### <a name="method-ajaxProcessHelpAccess"></a>ajaxProcessHelpAccess

```php
mixed AdminControllerCore::ajaxProcessHelpAccess()
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 359](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L359)




### <a name="method-ajaxProcessProductManufacturers"></a>ajaxProcessProductManufacturers

```php
mixed AdminProductsControllerCore::ajaxProcessProductManufacturers()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1941](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1941)




### <a name="method-ajaxProcessProductQuantity"></a>ajaxProcessProductQuantity

```php
mixed AdminProductsControllerCore::ajaxProcessProductQuantity()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3738](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3738)




### <a name="method-ajaxProcessSearchCustomers"></a>ajaxProcessSearchCustomers

```php
mixed AdminProductsControllerCore::ajaxProcessSearchCustomers()
```

Search customers



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1197](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1197)




### <a name="method-ajaxProcessUpdateCover"></a>ajaxProcessUpdateCover

```php
mixed AdminProductsControllerCore::ajaxProcessUpdateCover()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1230](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1230)




### <a name="method-ajaxProcessUpdateImagePosition"></a>ajaxProcessUpdateImagePosition

```php
mixed AdminProductsControllerCore::ajaxProcessUpdateImagePosition()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1207](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1207)




### <a name="method-ajaxProcessUpdateProductImageShopAsso"></a>ajaxProcessUpdateProductImageShopAsso

```php
mixed AdminProductsControllerCore::ajaxProcessUpdateProductImageShopAsso()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1172](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1172)




### <a name="method-beforeAdd"></a>beforeAdd

```php
boolean AdminControllerCore::beforeAdd(object $object)
```

Called before Add



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2530](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2530)


#### Arguments
* $object **object** - Object



### <a name="method-beforeDelete"></a>beforeDelete

```php
boolean AdminControllerCore::beforeDelete(object $object)
```

Called before deletion



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2217](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2217)


#### Arguments
* $object **object** - Object



### <a name="method-beforeUpdateOptions"></a>beforeUpdateOptions

```php
mixed AdminControllerCore::beforeUpdateOptions()
```

Can be overriden



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2365](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2365)




### <a name="method-checkAccess"></a>checkAccess

```php
mixed AdminControllerCore::checkAccess()
```

Check if the token is valid, else display a warning page



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1030](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1030)




### <a name="method-checkFeatures"></a>checkFeatures

```php
mixed AdminProductsControllerCore::checkFeatures($languages, $feature_id)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 1291](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1291)


#### Arguments
* $languages **mixed**
* $feature_id **mixed**



### <a name="method-checkProduct"></a>checkProduct

```php
mixed AdminProductsControllerCore::checkProduct()
```

Check that a saved product is valid



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1540](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1540)




### <a name="method-checkToken"></a>checkToken

```php
mixed AdminControllerCore::checkToken()
```

Check for security token



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 353](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L353)




### <a name="method-copyFromPost"></a>copyFromPost

```php
mixed AdminProductsControllerCore::copyFromPost($object, $table)
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 234](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L234)


#### Arguments
* $object **mixed**
* $table **mixed**



### <a name="method-copyImage"></a>copyImage

```php
mixed AdminProductsControllerCore::copyImage(integer $id_product, integer $id_image, $method)
```

Copy a product image



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1353](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1353)


#### Arguments
* $id_product **integer** - Product Id for product image filename
* $id_image **integer** - Image Id for product image filename
* $method **mixed**



### <a name="method-deleteDownloadProduct"></a>deleteDownloadProduct

```php
mixed AdminProductsControllerCore::deleteDownloadProduct($id_product_attribute)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1778](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1778)


#### Arguments
* $id_product_attribute **mixed**



### <a name="method-display"></a>display

```php
mixed AdminControllerCore::display()
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1081](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1081)




### <a name="method-displayAjax"></a>displayAjax

```php
mixed AdminControllerCore::displayAjax()
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1063](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1063)




### <a name="method-displayFooter"></a>displayFooter

```php
mixed ControllerCore::displayFooter($display)
```





* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 191](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L191)


#### Arguments
* $display **mixed**



### <a name="method-displayHeader"></a>displayHeader

```php
mixed ControllerCore::displayHeader($display)
```





* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 186](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L186)


#### Arguments
* $display **mixed**



### <a name="method-displayInformation"></a>displayInformation

```php
mixed AdminControllerCore::displayInformation(string $msg)
```

add a info message to display at the top of the page



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1163](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1163)


#### Arguments
* $msg **string**



### <a name="method-displayNoSmarty"></a>displayNoSmarty

```php
mixed AdminControllerCore::displayNoSmarty()
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1059](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1059)




### <a name="method-displayRequiredFields"></a>displayRequiredFields

```php
mixed AdminControllerCore::displayRequiredFields()
```

prepare the view to display the required fields form



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2538](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2538)




### <a name="method-displayWarning"></a>displayWarning

```php
mixed AdminControllerCore::displayWarning(string $msg)
```

add a warning message to display at the top of the page



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1153](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1153)


#### Arguments
* $msg **string**



### <a name="method-filterToField"></a>filterToField

```php
mixed AdminControllerCore::filterToField($key, $filter)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1049](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1049)


#### Arguments
* $key **mixed**
* $filter **mixed**



### <a name="method-getAssoShop"></a>getAssoShop

```php
mixed AdminControllerCore::getAssoShop(string $table, integer $id_object)
```

Returns an array with selected shops and type (group or boutique shop)



* Visibility: **protected**
* This method is **static**.
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2293](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2293)


#### Arguments
* $table **string**
* $id_object **integer**



### <a name="method-getCarrierList"></a>getCarrierList

```php
mixed AdminProductsControllerCore::getCarrierList()
```





* Visibility: **protected**
* Source: [controllers/admin/AdminProductsController.php line 3182](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3182)




### <a name="method-getCombinationImagesJS"></a>getCombinationImagesJS

```php
mixed AdminProductsControllerCore::getCombinationImagesJS()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3792](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3792)




### <a name="method-getController"></a>getController

```php
mixed ControllerCore::getController(string $class_name, boolean $auth, boolean $ssl)
```

Get an instance of a controller



* Visibility: **public**
* This method is **static**.
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 122](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L122)


#### Arguments
* $class_name **string**
* $auth **boolean**
* $ssl **boolean**



### <a name="method-getFieldValue"></a>getFieldValue

```php
string AdminControllerCore::getFieldValue(object $obj, string $key, integer $id_lang)
```

Return field value if possible (both classical and multilingual fields)

Case 1 : Return value if present in $_POST / $_GET
Case 2 : Return object value

* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2103](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2103)


#### Arguments
* $obj **object** - Object
* $key **string** - Field name
* $id_lang **integer** - Language id (optional)



### <a name="method-getFieldsValue"></a>getFieldsValue

```php
array AdminControllerCore::getFieldsValue(object $obj)
```

Return the list of fields value



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2064](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2064)


#### Arguments
* $obj **object** - Object



### <a name="method-getL"></a>getL

```php
mixed AdminProductsControllerCore::getL($key)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3865](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3865)


#### Arguments
* $key **mixed**



### <a name="method-getList"></a>getList

```php
mixed AdminProductsControllerCore::getList($id_lang, $orderBy, $orderWay, $start, $limit, $id_lang_shop)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 264](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L264)


#### Arguments
* $id_lang **mixed**
* $orderBy **mixed**
* $orderWay **mixed**
* $start **mixed**
* $limit **mixed**
* $id_lang_shop **mixed**



### <a name="method-getPreviewUrl"></a>getPreviewUrl

```php
mixed AdminProductsControllerCore::getPreviewUrl(\Product $product)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2156](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2156)


#### Arguments
* $product **[Product](class.ProductCore.md)**



### <a name="method-getTranslationsFlags"></a>getTranslationsFlags

```php
string AdminControllerCore::getTranslationsFlags(array $languages, integer $default_language, string $ids, string $id, $return, boolean $use_vars_instead_of_ids)
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2499](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2499)


#### Arguments
* $languages **array** - All languages available
* $default_language **integer** - Default language id
* $ids **string** - Multilingual div ids in form
* $id **string** - Current div id]
* $return **mixed**
* $use_vars_instead_of_ids **boolean** - use an js vars instead of ids seperate by &quot;¤&quot;



### <a name="method-getlanguages"></a>getlanguages

```php
mixed AdminControllerCore::getlanguages()
```





* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2034](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2034)




### <a name="method-haveThisAccessory"></a>haveThisAccessory

```php
mixed AdminProductsControllerCore::haveThisAccessory($accessory_id, $accessories)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3810](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3810)


#### Arguments
* $accessory_id **mixed**
* $accessories **mixed**



### <a name="method-init"></a>init

```php
mixed AdminControllerCore::init()
```

Init context and dependencies, handles POST and GET



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1667](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1667)




### <a name="method-initContent"></a>initContent

```php
mixed AdminProductsControllerCore::initContent($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1831](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1831)


#### Arguments
* $token **mixed**



### <a name="method-initCursedPage"></a>initCursedPage

```php
void AdminControllerCore::initCursedPage()
```

initialize the invalid doom page of death



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1392](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1392)




### <a name="method-initFooter"></a>initFooter

```php
mixed AdminControllerCore::initFooter()
```

Assign smarty variables for the footer



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1400](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1400)




### <a name="method-initFormAccounting"></a>initFormAccounting

```php
mixed AdminProductsControllerCore::initFormAccounting($obj)
```

Init data for accounting



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2479](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2479)


#### Arguments
* $obj **mixed**



### <a name="method-initFormAssociations"></a>initFormAssociations

```php
mixed AdminProductsControllerCore::initFormAssociations($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2522](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2522)


#### Arguments
* $obj **mixed**



### <a name="method-initFormAttachments"></a>initFormAttachments

```php
mixed AdminProductsControllerCore::initFormAttachments($obj, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3050](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3050)


#### Arguments
* $obj **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormAttributes"></a>initFormAttributes

```php
mixed AdminProductsControllerCore::initFormAttributes($product)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3258](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3258)


#### Arguments
* $product **mixed**



### <a name="method-initFormCombinations"></a>initFormCombinations

```php
mixed AdminProductsControllerCore::initFormCombinations($obj, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3253](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3253)


#### Arguments
* $obj **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormCustomization"></a>initFormCustomization

```php
mixed AdminProductsControllerCore::initFormCustomization($obj, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3021](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3021)


#### Arguments
* $obj **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormFeatures"></a>initFormFeatures

```php
mixed AdminProductsControllerCore::initFormFeatures($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3692](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3692)


#### Arguments
* $obj **mixed**



### <a name="method-initFormImages"></a>initFormImages

```php
mixed AdminProductsControllerCore::initFormImages($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3211](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3211)


#### Arguments
* $obj **mixed**



### <a name="method-initFormInformations"></a>initFormInformations

```php
mixed AdminProductsControllerCore::initFormInformations($product)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3082](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3082)


#### Arguments
* $product **mixed**



### <a name="method-initFormPack"></a>initFormPack

```php
mixed AdminProductsControllerCore::initFormPack($product, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2682](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2682)


#### Arguments
* $product **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormPrices"></a>initFormPrices

```php
mixed AdminProductsControllerCore::initFormPrices($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2586](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2586)


#### Arguments
* $obj **mixed**



### <a name="method-initFormQuantities"></a>initFormQuantities

```php
mixed AdminProductsControllerCore::initFormQuantities($obj, $languages)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3474](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3474)


#### Arguments
* $obj **mixed**
* $languages **mixed**



### <a name="method-initFormSeo"></a>initFormSeo

```php
mixed AdminProductsControllerCore::initFormSeo($product, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2668](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2668)


#### Arguments
* $product **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormShipping"></a>initFormShipping

```php
mixed AdminProductsControllerCore::initFormShipping($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3168](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3168)


#### Arguments
* $obj **mixed**



### <a name="method-initFormSuppliers"></a>initFormSuppliers

```php
mixed AdminProductsControllerCore::initFormSuppliers($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3575](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3575)


#### Arguments
* $obj **mixed**



### <a name="method-initFormVirtualProduct"></a>initFormVirtualProduct

```php
mixed AdminProductsControllerCore::initFormVirtualProduct($product, $languages, $default_language)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2715](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2715)


#### Arguments
* $product **mixed**
* $languages **mixed**
* $default_language **mixed**



### <a name="method-initFormWarehouses"></a>initFormWarehouses

```php
mixed AdminProductsControllerCore::initFormWarehouses($obj)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3647](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3647)


#### Arguments
* $obj **mixed**



### <a name="method-initHeader"></a>initHeader

```php
mixed AdminControllerCore::initHeader()
```

Assign smarty variables for the header



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1171](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1171)




### <a name="method-initPack"></a>initPack

```php
mixed AdminProductsControllerCore::initPack(\Product $product)
```





* Visibility: **private**
* Source: [controllers/admin/AdminProductsController.php line 3818](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3818)


#### Arguments
* $product **[Product](class.ProductCore.md)**



### <a name="method-initProcess"></a>initProcess

```php
mixed AdminProductsControllerCore::initProcess()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 878](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L878)




### <a name="method-initToolbar"></a>initToolbar

```php
mixed AdminProductsControllerCore::initToolbar()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2014](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2014)




### <a name="method-initToolbarTitle"></a>initToolbarTitle

```php
mixed AdminProductsControllerCore::initToolbarTitle()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2088](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2088)




### <a name="method-l"></a>l

```php
string AdminControllerCore::l(mixed $string, string $class, \boolan $addslashes, boolean $htmlentities)
```

non-static method which uses AdminController::translate()



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1653](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1653)


#### Arguments
* $string **mixed** - term or expression in english
* $class **string** - name of the class, without &quot;Controller&quot; suffix
* $addslashes **boolan** - if set to true, the return value will pass through addslashes(). Otherwise, stripslashes().
* $htmlentities **boolean** - if set to true(default), the return value will pass through htmlentities($string, ENT_QUOTES, &#039;utf-8&#039;)



### <a name="method-loadObject"></a>loadObject

```php
object AdminControllerCore::loadObject(boolean $opt)
```

Load class object using identifier in $_GET (if possible)
otherwise return an empty object, or die



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1000](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1000)


#### Arguments
* $opt **boolean** - Return an empty object if load fail



### <a name="method-postImage"></a>postImage

```php
boolean AdminControllerCore::postImage(integer $id)
```

Overload this method for custom checking



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2375](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2375)


#### Arguments
* $id **integer** - Object id used for deleting images



### <a name="method-postProcess"></a>postProcess

```php
void AdminProductsControllerCore::postProcess(mixed $token)
```

postProcess handle every checks before saving products information



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1032](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1032)


#### Arguments
* $token **mixed**



### <a name="method-processAccounting"></a>processAccounting

```php
mixed AdminProductsControllerCore::processAccounting($token)
```

Post treatment for accounting



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2188](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2188)


#### Arguments
* $token **mixed**



### <a name="method-processAdd"></a>processAdd

```php
mixed AdminProductsControllerCore::processAdd($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1385](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1385)


#### Arguments
* $token **mixed**



### <a name="method-processAddAttachments"></a>processAddAttachments

```php
void AdminProductsControllerCore::processAddAttachments($token)
```

Upload new attachment



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 320](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L320)


#### Arguments
* $token **mixed**



### <a name="method-processAttachments"></a>processAttachments

```php
void AdminProductsControllerCore::processAttachments($token)
```

Attach an existing attachment to the product



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 401](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L401)


#### Arguments
* $token **mixed**



### <a name="method-processBulkAffectZone"></a>processBulkAffectZone

```php
mixed AdminControllerCore::processBulkAffectZone($token)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2468](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2468)


#### Arguments
* $token **mixed**



### <a name="method-processBulkDelete"></a>processBulkDelete

```php
mixed AdminProductsControllerCore::processBulkDelete($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 523](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L523)


#### Arguments
* $token **mixed**



### <a name="method-processCustomizationConfiguration"></a>processCustomizationConfiguration

```php
mixed AdminProductsControllerCore::processCustomizationConfiguration($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 825](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L825)


#### Arguments
* $token **mixed**



### <a name="method-processDelete"></a>processDelete

```php
mixed AdminProductsControllerCore::processDelete($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 452](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L452)


#### Arguments
* $token **mixed**



### <a name="method-processDeleteImage"></a>processDeleteImage

```php
mixed AdminControllerCore::processDeleteImage(string $token)
```

Object Delete images



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 507](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L507)


#### Arguments
* $token **string**



### <a name="method-processDeleteSpecificPrice"></a>processDeleteSpecificPrice

```php
mixed AdminProductsControllerCore::processDeleteSpecificPrice($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 789](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L789)


#### Arguments
* $token **mixed**



### <a name="method-processDeleteVirtualProduct"></a>processDeleteVirtualProduct

```php
mixed AdminProductsControllerCore::processDeleteVirtualProduct($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 298](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L298)


#### Arguments
* $token **mixed**



### <a name="method-processDeleteVirtualProductAttribute"></a>processDeleteVirtualProductAttribute

```php
mixed AdminProductsControllerCore::processDeleteVirtualProductAttribute($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 306](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L306)


#### Arguments
* $token **mixed**



### <a name="method-processDuplicate"></a>processDuplicate

```php
mixed AdminProductsControllerCore::processDuplicate($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 413](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L413)


#### Arguments
* $token **mixed**



### <a name="method-processFeatures"></a>processFeatures

```php
mixed AdminProductsControllerCore::processFeatures($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 671](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L671)


#### Arguments
* $token **mixed**



### <a name="method-processFilter"></a>processFilter

```php
mixed AdminControllerCore::processFilter()
```

Set the filters used for the list display



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 377](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L377)




### <a name="method-processImage"></a>processImage

```php
mixed AdminProductsControllerCore::processImage($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 480](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L480)


#### Arguments
* $token **mixed**



### <a name="method-processPosition"></a>processPosition

```php
mixed AdminProductsControllerCore::processPosition($token)
```

Overrides parent for custom redirect link



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 865](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L865)


#### Arguments
* $token **mixed**



### <a name="method-processPriceAddition"></a>processPriceAddition

```php
mixed AdminProductsControllerCore::processPriceAddition($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 752](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L752)


#### Arguments
* $token **mixed**



### <a name="method-processPricesModification"></a>processPricesModification

```php
mixed AdminProductsControllerCore::processPricesModification($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 714](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L714)


#### Arguments
* $token **mixed**



### <a name="method-processProductAttribute"></a>processProductAttribute

```php
mixed AdminProductsControllerCore::processProductAttribute($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 562](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L562)


#### Arguments
* $token **mixed**



### <a name="method-processProductCustomization"></a>processProductCustomization

```php
mixed AdminProductsControllerCore::processProductCustomization($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 845](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L845)


#### Arguments
* $token **mixed**



### <a name="method-processResetFilters"></a>processResetFilters

```php
mixed AdminControllerCore::processResetFilters()
```

Cancel all filters for this tab



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 796](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L796)




### <a name="method-processSave"></a>processSave

```php
mixed AdminControllerCore::processSave($token)
```

Call the right method for creating or updating object



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 581](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L581)


#### Arguments
* $token **mixed**



### <a name="method-processSpecificPricePriorities"></a>processSpecificPricePriorities

```php
mixed AdminProductsControllerCore::processSpecificPricePriorities($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 806](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L806)


#### Arguments
* $token **mixed**



### <a name="method-processStatus"></a>processStatus

```php
mixed AdminControllerCore::processStatus(string $token)
```

Change object status (active, inactive)



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 748](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L748)


#### Arguments
* $token **string**



### <a name="method-processSuppliers"></a>processSuppliers

```php
mixed AdminProductsControllerCore::processSuppliers($token)
```

Post treatment for suppliers



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2219](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2219)


#### Arguments
* $token **mixed**



### <a name="method-processUpdate"></a>processUpdate

```php
mixed AdminProductsControllerCore::processUpdate($token)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1454](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1454)


#### Arguments
* $token **mixed**



### <a name="method-processUpdateFields"></a>processUpdateFields

```php
mixed AdminControllerCore::processUpdateFields(string $token)
```

Change object required fields



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 729](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L729)


#### Arguments
* $token **string**



### <a name="method-processUpdateOptions"></a>processUpdateOptions

```php
mixed AdminControllerCore::processUpdateOptions(string $token)
```

Update options and preferences



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 830](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L830)


#### Arguments
* $token **string**



### <a name="method-processWarehouses"></a>processWarehouses

```php
mixed AdminProductsControllerCore::processWarehouses($token)
```

Post treatment for warehouses



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2397](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2397)


#### Arguments
* $token **mixed**



### <a name="method-recurseCategoryForInclude"></a>recurseCategoryForInclude

```php
mixed AdminProductsControllerCore::recurseCategoryForInclude($id_obj, array $indexedCategories, array $categories, array $current, integer $id_category, $id_category_default, $has_suite)
```

Build a categories tree



* Visibility: **public**
* This method is **static**.
* Source: [controllers/admin/AdminProductsController.php line 1961](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1961)


#### Arguments
* $id_obj **mixed**
* $indexedCategories **array** - Array with categories where product is indexed (in order to check checkbox)
* $categories **array** - Categories to list
* $current **array** - Current category
* $id_category **integer** - Current category id
* $id_category_default **mixed**
* $has_suite **mixed**



### <a name="method-redirect"></a>redirect

```php
mixed AdminControllerCore::redirect()
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1076](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1076)




### <a name="method-renderForm"></a>renderForm

```php
void AdminProductsControllerCore::renderForm()
```

renderForm contains all necessary initialization needed for all tabs



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 2101](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L2101)




### <a name="method-renderList"></a>renderList

```php
mixed AdminProductsControllerCore::renderList()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1930](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1930)




### <a name="method-renderListAttributes"></a>renderListAttributes

```php
mixed AdminProductsControllerCore::renderListAttributes($id_product_download, $product, $currency)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3330](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3330)


#### Arguments
* $id_product_download **mixed**
* $product **mixed**
* $currency **mixed**



### <a name="method-renderOptions"></a>renderOptions

```php
mixed AdminControllerCore::renderOptions()
```

Function used to render the options for this controller



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1499](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1499)




### <a name="method-renderView"></a>renderView

```php
mixed AdminControllerCore::renderView()
```

Override to render the view page



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1452](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1452)




### <a name="method-run"></a>run

```php
mixed ControllerCore::run()
```

Start controller process (this method shouldn't be overriden !)



* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 143](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L143)




### <a name="method-setHelperDisplay"></a>setHelperDisplay

```php
void AdminControllerCore::setHelperDisplay(\Helper $helper)
```

this function set various display option for helper list



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1523](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1523)


#### Arguments
* $helper **[Helper](class.HelperCore.md)**



### <a name="method-setMedia"></a>setMedia

```php
mixed AdminProductsControllerCore::setMedia()
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3878](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3878)




### <a name="method-setTemplate"></a>setTemplate

```php
mixed ControllerCore::setTemplate($template)
```





* Visibility: **public**
* This method is defined by [ControllerCore](class.ControllerCore.md).
* Source: [classes/Controller.php line 196](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/Controller.php#L196)


#### Arguments
* $template **mixed**



### <a name="method-translate"></a>translate

```php
string AdminControllerCore::translate(mixed $string, string $class, \boolan $addslashes, boolean $htmlentities)
```

use translations files to replace english expression.



* Visibility: **public**
* This method is **static**.
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 1596](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L1596)


#### Arguments
* $string **mixed** - term or expression in english
* $class **string** - the classname (without &quot;Controller&quot; suffix)
* $addslashes **boolan** - if set to true, the return value will pass through addslashes(). Otherwise, stripslashes().
* $htmlentities **boolean** - if set to true(default), the return value will pass through htmlentities($string, ENT_QUOTES, &#039;utf-8&#039;)



### <a name="method-updateAccessories"></a>updateAccessories

```php
mixed AdminProductsControllerCore::updateAccessories(object $product)
```

Update product accessories



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1795](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1795)


#### Arguments
* $product **object** - Product



### <a name="method-updateAssoShop"></a>updateAssoShop

```php
mixed AdminControllerCore::updateAssoShop(integer $id_object, integer $new_id_object)
```

Update the associations of shops



* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2323](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2323)


#### Arguments
* $id_object **integer**
* $new_id_object **integer**



### <a name="method-updateDownloadProduct"></a>updateDownloadProduct

```php
boolean AdminProductsControllerCore::updateDownloadProduct(object $product, $edit, $id_product_attribute)
```

Update product download



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1635](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1635)


#### Arguments
* $product **object** - Product
* $edit **mixed**
* $id_product_attribute **mixed**



### <a name="method-updatePackItems"></a>updatePackItems

```php
mixed AdminProductsControllerCore::updatePackItems($product)
```





* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 3840](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L3840)


#### Arguments
* $product **mixed**



### <a name="method-updateTags"></a>updateTags

```php
boolean AdminProductsControllerCore::updateTags($languages, object $product)
```

Update product tags



* Visibility: **public**
* Source: [controllers/admin/AdminProductsController.php line 1816](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/controllers/admin/AdminProductsController.php#L1816)


#### Arguments
* $languages **mixed**
* $product **object** - Product



### <a name="method-uploadImage"></a>uploadImage

```php
mixed AdminControllerCore::uploadImage($id, $name, $dir, $ext, $width, $height)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2386](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2386)


#### Arguments
* $id **mixed**
* $name **mixed**
* $dir **mixed**
* $ext **mixed**
* $width **mixed**
* $height **mixed**



### <a name="method-validateField"></a>validateField

```php
mixed AdminControllerCore::validateField($value, $field)
```





* Visibility: **protected**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2344](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2344)


#### Arguments
* $value **mixed**
* $field **mixed**



### <a name="method-validateRules"></a>validateRules

```php
mixed AdminControllerCore::validateRules($class_name)
```

Manage page display (form, list.

..)

* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2118](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2118)


#### Arguments
* $class_name **mixed**



### <a name="method-viewAccess"></a>viewAccess

```php
boolean AdminControllerCore::viewAccess(boolean $disable)
```

Check rights to view the current tab



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 338](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L338)


#### Arguments
* $disable **boolean**



### <a name="method-viewDetails"></a>viewDetails

```php
mixed AdminControllerCore::viewDetails()
```

Display object details



* Visibility: **public**
* This method is defined by [AdminControllerCore](class.AdminControllerCore.md).
* Source: [classes/AdminController.php line 2209](https://github.com/PrestaShop/PrestaShop/blob/1.5.0.2/classes/AdminController.php#L2209)



