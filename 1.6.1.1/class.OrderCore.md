Class OrderCore
=====================





* Class name: OrderCore
* Parent class: [ObjectModel](class.ObjectModelCore.md)
* Source: [classes/order/Order.php line 27](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L27)

Constants
----------

* [ROUND_ITEM](#constant-ROUND_ITEM)
* [ROUND_LINE](#constant-ROUND_LINE)
* [ROUND_TOTAL](#constant-ROUND_TOTAL)

Properties
----------

* [$_historyCache](#property-$_historyCache)
* [$_taxCalculationMethod](#property-$_taxCalculationMethod)
* [$cacheCustomer](#property-$cacheCustomer)
* [$carrier_tax_rate](#property-$carrier_tax_rate)
* [$conversion_rate](#property-$conversion_rate)
* [$current_state](#property-$current_state)
* [$date_add](#property-$date_add)
* [$date_upd](#property-$date_upd)
* [$definition](#property-$definition)
* [$delivery_date](#property-$delivery_date)
* [$delivery_number](#property-$delivery_number)
* [$gift](#property-$gift)
* [$gift_message](#property-$gift_message)
* [$id_address_delivery](#property-$id_address_delivery)
* [$id_address_invoice](#property-$id_address_invoice)
* [$id_carrier](#property-$id_carrier)
* [$id_cart](#property-$id_cart)
* [$id_currency](#property-$id_currency)
* [$id_customer](#property-$id_customer)
* [$id_lang](#property-$id_lang)
* [$id_shop](#property-$id_shop)
* [$id_shop_group](#property-$id_shop_group)
* [$invoice_date](#property-$invoice_date)
* [$invoice_number](#property-$invoice_number)
* [$mobile_theme](#property-$mobile_theme)
* [$module](#property-$module)
* [$payment](#property-$payment)
* [$recyclable](#property-$recyclable)
* [$reference](#property-$reference)
* [$round_mode](#property-$round_mode)
* [$round_type](#property-$round_type)
* [$secure_key](#property-$secure_key)
* [$shipping_number](#property-$shipping_number)
* [$total_discounts](#property-$total_discounts)
* [$total_discounts_tax_excl](#property-$total_discounts_tax_excl)
* [$total_discounts_tax_incl](#property-$total_discounts_tax_incl)
* [$total_paid](#property-$total_paid)
* [$total_paid_real](#property-$total_paid_real)
* [$total_paid_tax_excl](#property-$total_paid_tax_excl)
* [$total_paid_tax_incl](#property-$total_paid_tax_incl)
* [$total_products](#property-$total_products)
* [$total_products_wt](#property-$total_products_wt)
* [$total_shipping](#property-$total_shipping)
* [$total_shipping_tax_excl](#property-$total_shipping_tax_excl)
* [$total_shipping_tax_incl](#property-$total_shipping_tax_incl)
* [$total_wrapping](#property-$total_wrapping)
* [$total_wrapping_tax_excl](#property-$total_wrapping_tax_excl)
* [$total_wrapping_tax_incl](#property-$total_wrapping_tax_incl)
* [$valid](#property-$valid)
* [$webserviceParameters](#property-$webserviceParameters)

Methods
-------
* [__construct](#method-__construct)
* [_deleteProduct](#method-_deleteProduct)
* [add](#method-add)
* [addCartRule](#method-addCartRule)
* [addDiscount](#method-addDiscount)
* [addOrderPayment](#method-addOrderPayment)
* [addWs](#method-addWs)
* [deleteAssociations](#method-deleteAssociations)
* [deleteCustomization](#method-deleteCustomization)
* [deleteProduct](#method-deleteProduct)
* [generateReference](#method-generateReference)
* [getBrother](#method-getBrother)
* [getByDelivery](#method-getByDelivery)
* [getByReference](#method-getByReference)
* [getCartIdStatic](#method-getCartIdStatic)
* [getCartProducts](#method-getCartProducts)
* [getCartRules](#method-getCartRules)
* [getCurrentOrderState](#method-getCurrentOrderState)
* [getCurrentState](#method-getCurrentState)
* [getCurrentStateFull](#method-getCurrentStateFull)
* [getCustomer](#method-getCustomer)
* [getCustomerNbOrders](#method-getCustomerNbOrders)
* [getCustomerOrders](#method-getCustomerOrders)
* [getDeliveryNumber](#method-getDeliveryNumber)
* [getDeliverySlipsCollection](#method-getDeliverySlipsCollection)
* [getDiscounts](#method-getDiscounts)
* [getDiscountsCustomer](#method-getDiscountsCustomer)
* [getDocuments](#method-getDocuments)
* [getEcoTaxTaxesBreakdown](#method-getEcoTaxTaxesBreakdown)
* [getFields](#method-getFields)
* [getFirstMessage](#method-getFirstMessage)
* [getHistory](#method-getHistory)
* [getIdOrderCarrier](#method-getIdOrderCarrier)
* [getIdOrderProduct](#method-getIdOrderProduct)
* [getInvoice](#method-getInvoice)
* [getInvoiceNumber](#method-getInvoiceNumber)
* [getInvoicesCollection](#method-getInvoicesCollection)
* [getLastInvoiceNumber](#method-getLastInvoiceNumber)
* [getNextOrderId](#method-getNextOrderId)
* [getNotPaidInvoicesCollection](#method-getNotPaidInvoicesCollection)
* [getNumberOfDays](#method-getNumberOfDays)
* [getOrderByCartId](#method-getOrderByCartId)
* [getOrderDetailList](#method-getOrderDetailList)
* [getOrderDetailTaxes](#method-getOrderDetailTaxes)
* [getOrderIdsByStatus](#method-getOrderIdsByStatus)
* [getOrderPaymentCollection](#method-getOrderPaymentCollection)
* [getOrderPayments](#method-getOrderPayments)
* [getOrderSlipsCollection](#method-getOrderSlipsCollection)
* [getOrdersIdByDate](#method-getOrdersIdByDate)
* [getOrdersIdInvoiceByDate](#method-getOrdersIdInvoiceByDate)
* [getOrdersTotalPaid](#method-getOrdersTotalPaid)
* [getOrdersWithInformations](#method-getOrdersWithInformations)
* [getPreviousOrderId](#method-getPreviousOrderId)
* [getProductTaxesBreakdown](#method-getProductTaxesBreakdown)
* [getProductTaxesDetails](#method-getProductTaxesDetails)
* [getProducts](#method-getProducts)
* [getProductsDetail](#method-getProductsDetail)
* [getReturn](#method-getReturn)
* [getShipping](#method-getShipping)
* [getShippingTaxesBreakdown](#method-getShippingTaxesBreakdown)
* [getTaxCalculationMethod](#method-getTaxCalculationMethod)
* [getTaxesAverageUsed](#method-getTaxesAverageUsed)
* [getTotalPaid](#method-getTotalPaid)
* [getTotalProductsWithTaxes](#method-getTotalProductsWithTaxes)
* [getTotalProductsWithoutTaxes](#method-getTotalProductsWithoutTaxes)
* [getTotalWeight](#method-getTotalWeight)
* [getUniqReference](#method-getUniqReference)
* [getUniqReferenceOf](#method-getUniqReferenceOf)
* [getVirtualProducts](#method-getVirtualProducts)
* [getWarehouseList](#method-getWarehouseList)
* [getWebserviceObjectList](#method-getWebserviceObjectList)
* [getWrappingTaxesBreakdown](#method-getWrappingTaxesBreakdown)
* [getWsCurrentState](#method-getWsCurrentState)
* [getWsOrderRows](#method-getWsOrderRows)
* [getWsShippingNumber](#method-getWsShippingNumber)
* [hasBeenDelivered](#method-hasBeenDelivered)
* [hasBeenPaid](#method-hasBeenPaid)
* [hasBeenShipped](#method-hasBeenShipped)
* [hasDelivery](#method-hasDelivery)
* [hasInvoice](#method-hasInvoice)
* [hasProductReturned](#method-hasProductReturned)
* [isAssociatedAtGuest](#method-isAssociatedAtGuest)
* [isInPreparation](#method-isInPreparation)
* [isPaidAndShipped](#method-isPaidAndShipped)
* [isReturnable](#method-isReturnable)
* [isVirtual](#method-isVirtual)
* [orderContainProduct](#method-orderContainProduct)
* [setCurrentState](#method-setCurrentState)
* [setDelivery](#method-setDelivery)
* [setDeliveryNumber](#method-setDeliveryNumber)
* [setDeliverySlip](#method-setDeliverySlip)
* [setInvoice](#method-setInvoice)
* [setInvoiceDetails](#method-setInvoiceDetails)
* [setLastInvoiceNumber](#method-setLastInvoiceNumber)
* [setProductCurrentStock](#method-setProductCurrentStock)
* [setProductCustomizedDatas](#method-setProductCustomizedDatas)
* [setProductImageInformations](#method-setProductImageInformations)
* [setProductPrices](#method-setProductPrices)
* [setWsCurrentState](#method-setWsCurrentState)
* [setWsShippingNumber](#method-setWsShippingNumber)
* [sortDocuments](#method-sortDocuments)
* [updateOrderDetailTax](#method-updateOrderDetailTax)
* [updateShippingCost](#method-updateShippingCost)
* [useOneAfterAnotherTaxComputationMethod](#method-useOneAfterAnotherTaxComputationMethod)


Constants
----------


### <a name="constant-ROUND_ITEM"></a>ROUND_ITEM

    const ROUND_ITEM = 1





* Source: [classes/order/Order.php line 29](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L29).


### <a name="constant-ROUND_LINE"></a>ROUND_LINE

    const ROUND_LINE = 2





* Source: [classes/order/Order.php line 30](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L30).


### <a name="constant-ROUND_TOTAL"></a>ROUND_TOTAL

    const ROUND_TOTAL = 3





* Source: [classes/order/Order.php line 31](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L31).


Properties
----------


### <a name="property-$_historyCache"></a>$_historyCache

    protected mixed $_historyCache = array()





* Visibility: **protected**
* This property is **static**.
* Source: [classes/order/Order.php line 279](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L279).


### <a name="property-$_taxCalculationMethod"></a>$_taxCalculationMethod

    protected mixed $_taxCalculationMethod = PS_TAX_EXC





* Visibility: **protected**
* Source: [classes/order/Order.php line 277](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L277).


### <a name="property-$cacheCustomer"></a>$cacheCustomer

    protected mixed $cacheCustomer = null

used to cache order customer



* Visibility: **protected**
* Source: [classes/order/Order.php line 1048](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1048).


### <a name="property-$carrier_tax_rate"></a>$carrier_tax_rate

    public float $carrier_tax_rate





* Visibility: **public**
* Source: [classes/order/Order.php line 127](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L127).


### <a name="property-$conversion_rate"></a>$conversion_rate

    public float $conversion_rate





* Visibility: **public**
* Source: [classes/order/Order.php line 72](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L72).


### <a name="property-$current_state"></a>$current_state

    public integer $current_state





* Visibility: **public**
* Source: [classes/order/Order.php line 60](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L60).


### <a name="property-$date_add"></a>$date_add

    public string $date_add





* Visibility: **public**
* Source: [classes/order/Order.php line 154](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L154).


### <a name="property-$date_upd"></a>$date_upd

    public string $date_upd





* Visibility: **public**
* Source: [classes/order/Order.php line 157](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L157).


### <a name="property-$definition"></a>$definition

    public mixed $definition = array('table' => 'orders', 'primary' => 'id_order', 'fields' => array('id_address_delivery' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_address_invoice' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_cart' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_currency' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_shop_group' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_shop' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'id_lang' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_customer' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'id_carrier' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId', 'required' => true), 'current_state' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'secure_key' => array('type' => self::TYPE_STRING, 'validate' => 'isMd5'), 'payment' => array('type' => self::TYPE_STRING, 'validate' => 'isGenericName', 'required' => true), 'module' => array('type' => self::TYPE_STRING, 'validate' => 'isModuleName', 'required' => true), 'recyclable' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'gift_message' => array('type' => self::TYPE_STRING, 'validate' => 'isMessage'), 'mobile_theme' => array('type' => self::TYPE_BOOL, 'validate' => 'isBool'), 'total_discounts' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_discounts_tax_incl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_discounts_tax_excl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_paid' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'total_paid_tax_incl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_paid_tax_excl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_paid_real' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'total_products' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'total_products_wt' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice', 'required' => true), 'total_shipping' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_shipping_tax_incl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_shipping_tax_excl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'carrier_tax_rate' => array('type' => self::TYPE_FLOAT, 'validate' => 'isFloat'), 'total_wrapping' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_wrapping_tax_incl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'total_wrapping_tax_excl' => array('type' => self::TYPE_FLOAT, 'validate' => 'isPrice'), 'round_mode' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'round_type' => array('type' => self::TYPE_INT, 'validate' => 'isUnsignedId'), 'shipping_number' => array('type' => self::TYPE_STRING, 'validate' => 'isTrackingNumber'), 'conversion_rate' => array('type' => self::TYPE_FLOAT, 'validate' => 'isFloat', 'required' => true), 'invoice_number' => array('type' => self::TYPE_INT), 'delivery_number' => array('type' => self::TYPE_INT), 'invoice_date' => array('type' => self::TYPE_DATE), 'delivery_date' => array('type' => self::TYPE_DATE), 'valid' => array('type' => self::TYPE_BOOL), 'reference' => array('type' => self::TYPE_STRING), 'date_add' => array('type' => self::TYPE_DATE, 'validate' => 'isDate'), 'date_upd' => array('type' => self::TYPE_DATE, 'validate' => 'isDate')))





* Visibility: **public**
* This property is **static**.
* Source: [classes/order/Order.php line 177](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L177).


### <a name="property-$delivery_date"></a>$delivery_date

    public string $delivery_date





* Visibility: **public**
* Source: [classes/order/Order.php line 148](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L148).


### <a name="property-$delivery_number"></a>$delivery_number

    public integer $delivery_number





* Visibility: **public**
* Source: [classes/order/Order.php line 142](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L142).


### <a name="property-$gift"></a>$gift

    public boolean $gift





* Visibility: **public**
* Source: [classes/order/Order.php line 78](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L78).


### <a name="property-$gift_message"></a>$gift_message

    public string $gift_message





* Visibility: **public**
* Source: [classes/order/Order.php line 81](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L81).


### <a name="property-$id_address_delivery"></a>$id_address_delivery

    public integer $id_address_delivery





* Visibility: **public**
* Source: [classes/order/Order.php line 35](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L35).


### <a name="property-$id_address_invoice"></a>$id_address_invoice

    public integer $id_address_invoice





* Visibility: **public**
* Source: [classes/order/Order.php line 38](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L38).


### <a name="property-$id_carrier"></a>$id_carrier

    public integer $id_carrier





* Visibility: **public**
* Source: [classes/order/Order.php line 57](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L57).


### <a name="property-$id_cart"></a>$id_cart

    public integer $id_cart





* Visibility: **public**
* Source: [classes/order/Order.php line 45](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L45).


### <a name="property-$id_currency"></a>$id_currency

    public integer $id_currency





* Visibility: **public**
* Source: [classes/order/Order.php line 48](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L48).


### <a name="property-$id_customer"></a>$id_customer

    public integer $id_customer





* Visibility: **public**
* Source: [classes/order/Order.php line 54](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L54).


### <a name="property-$id_lang"></a>$id_lang

    public integer $id_lang





* Visibility: **public**
* Source: [classes/order/Order.php line 51](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L51).


### <a name="property-$id_shop"></a>$id_shop

    public mixed $id_shop





* Visibility: **public**
* Source: [classes/order/Order.php line 42](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L42).


### <a name="property-$id_shop_group"></a>$id_shop_group

    public mixed $id_shop_group





* Visibility: **public**
* Source: [classes/order/Order.php line 40](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L40).


### <a name="property-$invoice_date"></a>$invoice_date

    public string $invoice_date





* Visibility: **public**
* Source: [classes/order/Order.php line 145](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L145).


### <a name="property-$invoice_number"></a>$invoice_number

    public integer $invoice_number





* Visibility: **public**
* Source: [classes/order/Order.php line 139](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L139).


### <a name="property-$mobile_theme"></a>$mobile_theme

    public boolean $mobile_theme





* Visibility: **public**
* Source: [classes/order/Order.php line 84](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L84).


### <a name="property-$module"></a>$module

    public string $module





* Visibility: **public**
* Source: [classes/order/Order.php line 69](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L69).


### <a name="property-$payment"></a>$payment

    public string $payment





* Visibility: **public**
* Source: [classes/order/Order.php line 66](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L66).


### <a name="property-$recyclable"></a>$recyclable

    public boolean $recyclable = 1





* Visibility: **public**
* Source: [classes/order/Order.php line 75](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L75).


### <a name="property-$reference"></a>$reference

    public string $reference





* Visibility: **public**
* Source: [classes/order/Order.php line 162](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L162).


### <a name="property-$round_mode"></a>$round_mode

    public integer $round_mode





* Visibility: **public**
* Source: [classes/order/Order.php line 167](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L167).


### <a name="property-$round_type"></a>$round_type

    public integer $round_type





* Visibility: **public**
* Source: [classes/order/Order.php line 172](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L172).


### <a name="property-$secure_key"></a>$secure_key

    public string $secure_key





* Visibility: **public**
* Source: [classes/order/Order.php line 63](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L63).


### <a name="property-$shipping_number"></a>$shipping_number

    public string $shipping_number





* Visibility: **public**
* Source: [classes/order/Order.php line 91](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L91).


### <a name="property-$total_discounts"></a>$total_discounts

    public float $total_discounts





* Visibility: **public**
* Source: [classes/order/Order.php line 94](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L94).


### <a name="property-$total_discounts_tax_excl"></a>$total_discounts_tax_excl

    public mixed $total_discounts_tax_excl





* Visibility: **public**
* Source: [classes/order/Order.php line 97](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L97).


### <a name="property-$total_discounts_tax_incl"></a>$total_discounts_tax_incl

    public mixed $total_discounts_tax_incl





* Visibility: **public**
* Source: [classes/order/Order.php line 96](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L96).


### <a name="property-$total_paid"></a>$total_paid

    public float $total_paid





* Visibility: **public**
* Source: [classes/order/Order.php line 100](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L100).


### <a name="property-$total_paid_real"></a>$total_paid_real

    public float $total_paid_real





* Visibility: **public**
* Source: [classes/order/Order.php line 109](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L109).


### <a name="property-$total_paid_tax_excl"></a>$total_paid_tax_excl

    public float $total_paid_tax_excl





* Visibility: **public**
* Source: [classes/order/Order.php line 106](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L106).


### <a name="property-$total_paid_tax_incl"></a>$total_paid_tax_incl

    public float $total_paid_tax_incl





* Visibility: **public**
* Source: [classes/order/Order.php line 103](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L103).


### <a name="property-$total_products"></a>$total_products

    public float $total_products





* Visibility: **public**
* Source: [classes/order/Order.php line 112](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L112).


### <a name="property-$total_products_wt"></a>$total_products_wt

    public float $total_products_wt





* Visibility: **public**
* Source: [classes/order/Order.php line 115](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L115).


### <a name="property-$total_shipping"></a>$total_shipping

    public float $total_shipping





* Visibility: **public**
* Source: [classes/order/Order.php line 118](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L118).


### <a name="property-$total_shipping_tax_excl"></a>$total_shipping_tax_excl

    public float $total_shipping_tax_excl





* Visibility: **public**
* Source: [classes/order/Order.php line 124](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L124).


### <a name="property-$total_shipping_tax_incl"></a>$total_shipping_tax_incl

    public float $total_shipping_tax_incl





* Visibility: **public**
* Source: [classes/order/Order.php line 121](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L121).


### <a name="property-$total_wrapping"></a>$total_wrapping

    public float $total_wrapping





* Visibility: **public**
* Source: [classes/order/Order.php line 130](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L130).


### <a name="property-$total_wrapping_tax_excl"></a>$total_wrapping_tax_excl

    public float $total_wrapping_tax_excl





* Visibility: **public**
* Source: [classes/order/Order.php line 136](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L136).


### <a name="property-$total_wrapping_tax_incl"></a>$total_wrapping_tax_incl

    public float $total_wrapping_tax_incl





* Visibility: **public**
* Source: [classes/order/Order.php line 133](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L133).


### <a name="property-$valid"></a>$valid

    public boolean $valid





* Visibility: **public**
* Source: [classes/order/Order.php line 151](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L151).


### <a name="property-$webserviceParameters"></a>$webserviceParameters

    protected mixed $webserviceParameters = array('objectMethods' => array('add' => 'addWs'), 'objectNodeName' => 'order', 'objectsNodeName' => 'orders', 'fields' => array('id_address_delivery' => array('xlink_resource' => 'addresses'), 'id_address_invoice' => array('xlink_resource' => 'addresses'), 'id_cart' => array('xlink_resource' => 'carts'), 'id_currency' => array('xlink_resource' => 'currencies'), 'id_lang' => array('xlink_resource' => 'languages'), 'id_customer' => array('xlink_resource' => 'customers'), 'id_carrier' => array('xlink_resource' => 'carriers'), 'current_state' => array('xlink_resource' => 'order_states', 'setter' => 'setWsCurrentState'), 'module' => array('required' => true), 'invoice_number' => array(), 'invoice_date' => array(), 'delivery_number' => array(), 'delivery_date' => array(), 'valid' => array(), 'date_add' => array(), 'date_upd' => array(), 'shipping_number' => array('getter' => 'getWsShippingNumber', 'setter' => 'setWsShippingNumber')), 'associations' => array('order_rows' => array('resource' => 'order_row', 'setter' => false, 'virtual_entity' => true, 'fields' => array('id' => array(), 'product_id' => array('required' => true), 'product_attribute_id' => array('required' => true), 'product_quantity' => array('required' => true), 'product_name' => array('setter' => false), 'product_reference' => array('setter' => false), 'product_ean13' => array('setter' => false), 'product_upc' => array('setter' => false), 'product_price' => array('setter' => false), 'unit_price_tax_incl' => array('setter' => false), 'unit_price_tax_excl' => array('setter' => false)))))





* Visibility: **protected**
* Source: [classes/order/Order.php line 229](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L229).


Methods
-------


### <a name="method-__construct"></a>__construct

    mixed OrderCore::__construct($id, $id_lang)





* Visibility: **public**
* Source: [classes/order/Order.php line 281](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L281)


#### Arguments
* $id **mixed**
* $id_lang **mixed**



### <a name="method-_deleteProduct"></a>_deleteProduct

    boolean OrderCore::_deleteProduct(\OrderDetail $order_detail, integer $quantity)

DOES delete the product



* Visibility: **protected**
* Source: [classes/order/Order.php line 390](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L390)


#### Arguments
* $order_detail **[OrderDetail](class.OrderDetailCore.md)**
* $quantity **integer**



### <a name="method-add"></a>add

    mixed OrderCore::add($autodate, $null_values)





* Visibility: **public**
* Source: [classes/order/Order.php line 307](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L307)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-addCartRule"></a>addCartRule

    boolean OrderCore::addCartRule(integer $id_cart_rule, string $name, array $values, integer $id_order_invoice, $free_shipping)





* Visibility: **public**
* Source: [classes/order/Order.php line 1120](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1120)


#### Arguments
* $id_cart_rule **integer**
* $name **string**
* $values **array**
* $id_order_invoice **integer**
* $free_shipping **mixed**



### <a name="method-addDiscount"></a>addDiscount

    boolean OrderCore::addDiscount(integer $id_cart_rule, string $name, float $value)





* Visibility: **public**
* Source: [classes/order/Order.php line 1106](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1106)


#### Arguments
* $id_cart_rule **integer**
* $name **string**
* $value **float**



### <a name="method-addOrderPayment"></a>addOrderPayment

    boolean OrderCore::addOrderPayment(float $amount_paid, string $payment_method, string $payment_transaction_id, \Currency $currency, string $date, \OrderInvoice $order_invoice)

This method allows to add a payment to the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1687](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1687)


#### Arguments
* $amount_paid **float**
* $payment_method **string**
* $payment_transaction_id **string**
* $currency **[Currency](class.CurrencyCore.md)**
* $date **string**
* $order_invoice **[OrderInvoice](class.OrderInvoiceCore.md)**



### <a name="method-addWs"></a>addWs

    mixed OrderCore::addWs($autodate, $null_values)





* Visibility: **public**
* Source: [classes/order/Order.php line 1567](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1567)


#### Arguments
* $autodate **mixed**
* $null_values **mixed**



### <a name="method-deleteAssociations"></a>deleteAssociations

    mixed OrderCore::deleteAssociations()





* Visibility: **public**
* Source: [classes/order/Order.php line 1577](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1577)




### <a name="method-deleteCustomization"></a>deleteCustomization

    mixed OrderCore::deleteCustomization($id_customization, $quantity, $order_detail)





* Visibility: **public**
* Source: [classes/order/Order.php line 461](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L461)


#### Arguments
* $id_customization **mixed**
* $quantity **mixed**
* $order_detail **mixed**



### <a name="method-deleteProduct"></a>deleteProduct

    boolean OrderCore::deleteProduct($order, \OrderDetail $order_detail, integer $quantity)

Does NOT delete a product but "cancel" it (which means return/refund/delete it depending of the case)



* Visibility: **public**
* Source: [classes/order/Order.php line 329](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L329)


#### Arguments
* $order **mixed**
* $order_detail **[OrderDetail](class.OrderDetailCore.md)**
* $quantity **integer**



### <a name="method-generateReference"></a>generateReference

    String OrderCore::generateReference()

Gennerate a unique reference for orders generated with the same cart id
This references, is usefull for check payment



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1629](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1629)




### <a name="method-getBrother"></a>getBrother

    mixed OrderCore::getBrother()

Get all other orders with the same reference



* Visibility: **public**
* Source: [classes/order/Order.php line 2107](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2107)




### <a name="method-getByDelivery"></a>getByDelivery

    mixed OrderCore::getByDelivery($id_delivery)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1442](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1442)


#### Arguments
* $id_delivery **mixed**



### <a name="method-getByReference"></a>getByReference

    \PrestaShopCollection OrderCore::getByReference(string $reference)

Get a collection of orders using reference



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1460](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1460)


#### Arguments
* $reference **string**



### <a name="method-getCartIdStatic"></a>getCartIdStatic

    integer OrderCore::getCartIdStatic(integer $id_order, integer $id_customer)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1510](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1510)


#### Arguments
* $id_order **integer**
* $id_customer **integer** - optionnal



### <a name="method-getCartProducts"></a>getCartProducts

    array OrderCore::getCartProducts()

This function return products of the orders
It's similar to Order::getProducts but with similar outputs of Cart::getProducts



* Visibility: **public**
* Source: [classes/order/Order.php line 354](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L354)




### <a name="method-getCartRules"></a>getCartRules

    mixed OrderCore::getCartRules()





* Visibility: **public**
* Source: [classes/order/Order.php line 780](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L780)




### <a name="method-getCurrentOrderState"></a>getCurrentOrderState

    \OrderState OrderCore::getCurrentOrderState()





* Visibility: **public**
* Source: [classes/order/Order.php line 2085](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2085)




### <a name="method-getCurrentState"></a>getCurrentState

    integer OrderCore::getCurrentState()

Get current order status (eg. Awaiting payment, Delivered.

..)

* Visibility: **public**
* Source: [classes/order/Order.php line 808](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L808)




### <a name="method-getCurrentStateFull"></a>getCurrentStateFull

    array OrderCore::getCurrentStateFull($id_lang)

Get current order status name (eg. Awaiting payment, Delivered.

..)

* Visibility: **public**
* Source: [classes/order/Order.php line 818](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L818)


#### Arguments
* $id_lang **mixed**



### <a name="method-getCustomer"></a>getCustomer

    \Customer OrderCore::getCustomer()

Get order customer



* Visibility: **public**
* Source: [classes/order/Order.php line 1055](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1055)




### <a name="method-getCustomerNbOrders"></a>getCustomerNbOrders

    array OrderCore::getCustomerNbOrders(integer $id_customer)

Get customer orders number



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1070](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1070)


#### Arguments
* $id_customer **integer** - Customer id



### <a name="method-getCustomerOrders"></a>getCustomerOrders

    array OrderCore::getCustomerOrders(integer $id_customer, boolean $show_hidden_status, \Context $context)

Get customer orders



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 883](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L883)


#### Arguments
* $id_customer **integer** - Customer id
* $show_hidden_status **boolean** - Display or not hidden order statuses
* $context **[Context](class.ContextCore.md)**



### <a name="method-getDeliveryNumber"></a>getDeliveryNumber

    mixed OrderCore::getDeliveryNumber($order_invoice_id)





* Visibility: **public**
* Source: [classes/order/Order.php line 1403](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1403)


#### Arguments
* $order_invoice_id **mixed**



### <a name="method-getDeliverySlipsCollection"></a>getDeliverySlipsCollection

    \PrestaShopCollection OrderCore::getDeliverySlipsCollection()

Get all delivery slips for the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1823](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1823)




### <a name="method-getDiscounts"></a>getDiscounts

    mixed OrderCore::getDiscounts($details)





* Visibility: **public**
* Source: [classes/order/Order.php line 774](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L774)


#### Arguments
* $details **mixed**



### <a name="method-getDiscountsCustomer"></a>getDiscountsCustomer

    mixed OrderCore::getDiscountsCustomer($id_customer, $id_cart_rule)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 788](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L788)


#### Arguments
* $id_customer **mixed**
* $id_cart_rule **mixed**



### <a name="method-getDocuments"></a>getDocuments

    array OrderCore::getDocuments()

Returns the correct product taxes breakdown.

Get all documents linked to the current order

* Visibility: **public**
* Source: [classes/order/Order.php line 1739](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1739)




### <a name="method-getEcoTaxTaxesBreakdown"></a>getEcoTaxTaxesBreakdown

    array OrderCore::getEcoTaxTaxesBreakdown()

Returns the ecotax taxes breakdown



* Visibility: **public**
* Source: [classes/order/Order.php line 2018](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2018)




### <a name="method-getFields"></a>getFields

    array OrderCore::getFields()





* Visibility: **public**
* Source: [classes/order/Order.php line 298](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L298)




### <a name="method-getFirstMessage"></a>getFirstMessage

    mixed OrderCore::getFirstMessage()





* Visibility: **public**
* Source: [classes/order/Order.php line 554](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L554)




### <a name="method-getHistory"></a>getHistory

    array OrderCore::getHistory(integer $id_lang, integer $id_order_state, integer $no_hidden, integer $filters)

Get order history



* Visibility: **public**
* Source: [classes/order/Order.php line 491](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L491)


#### Arguments
* $id_lang **integer** - Language id
* $id_order_state **integer** - Filter a specific order status
* $no_hidden **integer** - Filter no hidden status
* $filters **integer** - Flag to use specific field filter



### <a name="method-getIdOrderCarrier"></a>getIdOrderCarrier

    mixed OrderCore::getIdOrderCarrier()

Return id of carrier

Get id of the carrier used in order

* Visibility: **public**
* Source: [classes/order/Order.php line 2170](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2170)




### <a name="method-getIdOrderProduct"></a>getIdOrderProduct

    mixed OrderCore::getIdOrderProduct($id_customer, $id_product)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 648](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L648)


#### Arguments
* $id_customer **mixed**
* $id_product **mixed**



### <a name="method-getInvoice"></a>getInvoice

    mixed OrderCore::getInvoice(integer $id_invoice)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1481](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1481)


#### Arguments
* $id_invoice **integer**



### <a name="method-getInvoiceNumber"></a>getInvoiceNumber

    mixed OrderCore::getInvoiceNumber($order_invoice_id)





* Visibility: **public**
* Source: [classes/order/Order.php line 1200](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1200)


#### Arguments
* $order_invoice_id **mixed**



### <a name="method-getInvoicesCollection"></a>getInvoicesCollection

    \PrestaShopCollection OrderCore::getInvoicesCollection()

Get all invoices for the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1810](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1810)




### <a name="method-getLastInvoiceNumber"></a>getLastInvoiceNumber

    mixed OrderCore::getLastInvoiceNumber()





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1166](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1166)




### <a name="method-getNextOrderId"></a>getNextOrderId

    integer OrderCore::getNextOrderId()

This method return the ID of the next order



* Visibility: **public**
* Source: [classes/order/Order.php line 1604](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1604)




### <a name="method-getNotPaidInvoicesCollection"></a>getNotPaidInvoicesCollection

    \PrestaShopCollection OrderCore::getNotPaidInvoicesCollection()

Get all not paid invoices for the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1836](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1836)




### <a name="method-getNumberOfDays"></a>getNumberOfDays

    mixed OrderCore::getNumberOfDays()





* Visibility: **public**
* Source: [classes/order/Order.php line 1137](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1137)




### <a name="method-getOrderByCartId"></a>getOrderByCartId

    array OrderCore::getOrderByCartId(integer $id_cart)

Get an order by its cart id



* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1087](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1087)


#### Arguments
* $id_cart **integer** - Cart id



### <a name="method-getOrderDetailList"></a>getOrderDetailList

    array OrderCore::getOrderDetailList()

Get the an order detail list of the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1618](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1618)




### <a name="method-getOrderDetailTaxes"></a>getOrderDetailTaxes

    mixed OrderCore::getOrderDetailTaxes()





* Visibility: **public**
* Source: [classes/order/Order.php line 2419](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2419)




### <a name="method-getOrderIdsByStatus"></a>getOrderIdsByStatus

    array OrderCore::getOrderIdsByStatus($id_order_state)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 990](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L990)


#### Arguments
* $id_order_state **mixed**



### <a name="method-getOrderPaymentCollection"></a>getOrderPaymentCollection

    \PrestaShopCollection OrderCore::getOrderPaymentCollection()

This method allows to get all Order Payment for the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1668](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1668)




### <a name="method-getOrderPayments"></a>getOrderPayments

    mixed OrderCore::getOrderPayments()

Get a collection of order payments



* Visibility: **public**
* Source: [classes/order/Order.php line 2120](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2120)




### <a name="method-getOrderSlipsCollection"></a>getOrderSlipsCollection

    \PrestaShopCollection OrderCore::getOrderSlipsCollection()

Get all order_slips for the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1797](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1797)




### <a name="method-getOrdersIdByDate"></a>getOrdersIdByDate

    mixed OrderCore::getOrdersIdByDate($date_from, $date_to, $id_customer, $type)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 916](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L916)


#### Arguments
* $date_from **mixed**
* $date_to **mixed**
* $id_customer **mixed**
* $type **mixed**



### <a name="method-getOrdersIdInvoiceByDate"></a>getOrdersIdInvoiceByDate

    array OrderCore::getOrdersIdInvoiceByDate($date_from, $date_to, $id_customer, $type)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 965](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L965)


#### Arguments
* $date_from **mixed**
* $date_to **mixed**
* $id_customer **mixed**
* $type **mixed**



### <a name="method-getOrdersTotalPaid"></a>getOrdersTotalPaid

    float OrderCore::getOrdersTotalPaid()

Get the sum of total_paid_tax_incl of the orders with similar reference



* Visibility: **public**
* Source: [classes/order/Order.php line 1888](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1888)




### <a name="method-getOrdersWithInformations"></a>getOrdersWithInformations

    mixed OrderCore::getOrdersWithInformations($limit, \Context $context)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 933](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L933)


#### Arguments
* $limit **mixed**
* $context **[Context](class.ContextCore.md)**



### <a name="method-getPreviousOrderId"></a>getPreviousOrderId

    integer OrderCore::getPreviousOrderId()

This method return the ID of the previous order



* Visibility: **public**
* Source: [classes/order/Order.php line 1589](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1589)




### <a name="method-getProductTaxesBreakdown"></a>getProductTaxesBreakdown

    array OrderCore::getProductTaxesBreakdown()

Returns the correct product taxes breakdown.



* Visibility: **public**
* Source: [classes/order/Order.php line 1928](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1928)




### <a name="method-getProductTaxesDetails"></a>getProductTaxesDetails

    array OrderCore::getProductTaxesDetails($limitToOrderDetails)

By default this function was made for invoice, to compute tax amounts and balance delta (because of computation made on round values).

If you provide $limitToOrderDetails, only these item will be taken into account. This option is usefull for order slip for example,
where only sublist of the order is refunded.

* Visibility: **public**
* Source: [classes/order/Order.php line 2240](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2240)


#### Arguments
* $limitToOrderDetails **mixed** - Optional array of OrderDetails to take into account. False by default to take all OrderDetails from the current Order.



### <a name="method-getProducts"></a>getProducts

    array OrderCore::getProducts($products, $selected_products, $selected_qty)

Get order products



* Visibility: **public**
* Source: [classes/order/Order.php line 597](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L597)


#### Arguments
* $products **mixed**
* $selected_products **mixed**
* $selected_qty **mixed**



### <a name="method-getProductsDetail"></a>getProductsDetail

    mixed OrderCore::getProductsDetail()





* Visibility: **public**
* Source: [classes/order/Order.php line 544](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L544)




### <a name="method-getReturn"></a>getReturn

    mixed OrderCore::getReturn()





* Visibility: **public**
* Source: [classes/order/Order.php line 1764](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1764)




### <a name="method-getShipping"></a>getShipping

    array OrderCore::getShipping()





* Visibility: **public**
* Source: [classes/order/Order.php line 1773](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1773)




### <a name="method-getShippingTaxesBreakdown"></a>getShippingTaxesBreakdown

    array OrderCore::getShippingTaxesBreakdown()

Returns the shipping taxes breakdown



* Visibility: **public**
* Source: [classes/order/Order.php line 1983](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1983)




### <a name="method-getTaxCalculationMethod"></a>getTaxCalculationMethod

    mixed OrderCore::getTaxCalculationMethod()





* Visibility: **public**
* Source: [classes/order/Order.php line 315](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L315)




### <a name="method-getTaxesAverageUsed"></a>getTaxesAverageUsed

    mixed OrderCore::getTaxesAverageUsed()





* Visibility: **public**
* Source: [classes/order/Order.php line 724](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L724)




### <a name="method-getTotalPaid"></a>getTotalPaid

    float OrderCore::getTotalPaid(\Currency $currency)

Get total paid



* Visibility: **public**
* Source: [classes/order/Order.php line 1856](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1856)


#### Arguments
* $currency **[Currency](class.CurrencyCore.md)** - currency used for the total paid of the current order



### <a name="method-getTotalProductsWithTaxes"></a>getTotalProductsWithTaxes

    \Product OrderCore::getTotalProductsWithTaxes($products)

Get product total with taxes



* Visibility: **public**
* Source: [classes/order/Order.php line 1022](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1022)


#### Arguments
* $products **mixed**



### <a name="method-getTotalProductsWithoutTaxes"></a>getTotalProductsWithoutTaxes

    \Product OrderCore::getTotalProductsWithoutTaxes($products)

Get product total without taxes



* Visibility: **public**
* Source: [classes/order/Order.php line 1012](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1012)


#### Arguments
* $products **mixed**



### <a name="method-getTotalWeight"></a>getTotalWeight

    mixed OrderCore::getTotalWeight()





* Visibility: **public**
* Source: [classes/order/Order.php line 1467](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1467)




### <a name="method-getUniqReference"></a>getUniqReference

    mixed OrderCore::getUniqReference()

Return a unique reference like : GWJTHMZUN#2

With multishipping, order reference are the same for all orders made with the same cart
in this case this method suffix the order reference by a # and the order number

* Visibility: **public**
* Source: [classes/order/Order.php line 2133](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2133)




### <a name="method-getUniqReferenceOf"></a>getUniqReferenceOf

    mixed OrderCore::getUniqReferenceOf($id_order)

Return a unique reference like : GWJTHMZUN#2

With multishipping, order reference are the same for all orders made with the same cart
in this case this method suffix the order reference by a # and the order number

* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 2157](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2157)


#### Arguments
* $id_order **mixed**



### <a name="method-getVirtualProducts"></a>getVirtualProducts

    integer OrderCore::getVirtualProducts()

Count virtual products in order



* Visibility: **public**
* Source: [classes/order/Order.php line 734](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L734)




### <a name="method-getWarehouseList"></a>getWarehouseList

    mixed OrderCore::getWarehouseList()

Get warehouse associated to the order

return array List of warehouse

* Visibility: **public**
* Source: [classes/order/Order.php line 2062](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2062)




### <a name="method-getWebserviceObjectList"></a>getWebserviceObjectList

    mixed OrderCore::getWebserviceObjectList($sql_join, $sql_filter, $sql_sort, $sql_limit)





* Visibility: **public**
* Source: [classes/order/Order.php line 2096](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2096)


#### Arguments
* $sql_join **mixed**
* $sql_filter **mixed**
* $sql_sort **mixed**
* $sql_limit **mixed**



### <a name="method-getWrappingTaxesBreakdown"></a>getWrappingTaxesBreakdown

    array OrderCore::getWrappingTaxesBreakdown()

Returns the wrapping taxes breakdown



* Visibility: **public**
* Source: [classes/order/Order.php line 2006](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2006)




### <a name="method-getWsCurrentState"></a>getWsCurrentState

    mixed OrderCore::getWsCurrentState()





* Visibility: **public**
* Source: [classes/order/Order.php line 2218](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2218)




### <a name="method-getWsOrderRows"></a>getWsOrderRows

    mixed OrderCore::getWsOrderRows()





* Visibility: **public**
* Source: [classes/order/Order.php line 1519](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1519)




### <a name="method-getWsShippingNumber"></a>getWsShippingNumber

    mixed OrderCore::getWsShippingNumber()





* Visibility: **public**
* Source: [classes/order/Order.php line 2186](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2186)




### <a name="method-hasBeenDelivered"></a>hasBeenDelivered

    mixed OrderCore::hasBeenDelivered()





* Visibility: **public**
* Source: [classes/order/Order.php line 827](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L827)




### <a name="method-hasBeenPaid"></a>hasBeenPaid

    mixed OrderCore::hasBeenPaid()





* Visibility: **public**
* Source: [classes/order/Order.php line 847](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L847)




### <a name="method-hasBeenShipped"></a>hasBeenShipped

    mixed OrderCore::hasBeenShipped()





* Visibility: **public**
* Source: [classes/order/Order.php line 852](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L852)




### <a name="method-hasDelivery"></a>hasDelivery

    boolean OrderCore::hasDelivery()

Has Delivery return true if this order has already a delivery slip



* Visibility: **public**
* Source: [classes/order/Order.php line 2047](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2047)




### <a name="method-hasInvoice"></a>hasInvoice

    boolean OrderCore::hasInvoice()

Has invoice return true if this order has already an invoice



* Visibility: **public**
* Source: [classes/order/Order.php line 2032](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2032)




### <a name="method-hasProductReturned"></a>hasProductReturned

    mixed OrderCore::hasProductReturned()

Has products returned by the merchant or by the customer?



* Visibility: **public**
* Source: [classes/order/Order.php line 835](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L835)




### <a name="method-isAssociatedAtGuest"></a>isAssociatedAtGuest

    mixed OrderCore::isAssociatedAtGuest($email)





* Visibility: **public**
* Source: [classes/order/Order.php line 1490](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1490)


#### Arguments
* $email **mixed**



### <a name="method-isInPreparation"></a>isInPreparation

    mixed OrderCore::isInPreparation()





* Visibility: **public**
* Source: [classes/order/Order.php line 857](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L857)




### <a name="method-isPaidAndShipped"></a>isPaidAndShipped

    boolean OrderCore::isPaidAndShipped()

Checks if the current order status is paid and shipped



* Visibility: **public**
* Source: [classes/order/Order.php line 867](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L867)




### <a name="method-isReturnable"></a>isReturnable

    boolean OrderCore::isReturnable()

Can this order be returned by the client?



* Visibility: **public**
* Source: [classes/order/Order.php line 1157](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1157)




### <a name="method-isVirtual"></a>isVirtual

    boolean OrderCore::isVirtual(boolean $strict)

Check if order contains (only) virtual products



* Visibility: **public**
* Source: [classes/order/Order.php line 751](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L751)


#### Arguments
* $strict **boolean** - If false return true if there are at least one product virtual



### <a name="method-orderContainProduct"></a>orderContainProduct

    mixed OrderCore::orderContainProduct($id_product)





* Visibility: **public**
* Source: [classes/order/Order.php line 1634](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1634)


#### Arguments
* $id_product **mixed**



### <a name="method-setCurrentState"></a>setCurrentState

    mixed OrderCore::setCurrentState(integer $id_order_state, integer $id_employee)

Set current order status



* Visibility: **public**
* Source: [classes/order/Order.php line 1545](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1545)


#### Arguments
* $id_order_state **integer**
* $id_employee **integer** - (/!\ not optional except for Webservice.



### <a name="method-setDelivery"></a>setDelivery

    mixed OrderCore::setDelivery()





* Visibility: **public**
* Source: [classes/order/Order.php line 1416](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1416)




### <a name="method-setDeliveryNumber"></a>setDeliveryNumber

    mixed OrderCore::setDeliveryNumber($order_invoice_id, $id_shop)





* Visibility: **public**
* Source: [classes/order/Order.php line 1375](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1375)


#### Arguments
* $order_invoice_id **mixed**
* $id_shop **mixed**



### <a name="method-setDeliverySlip"></a>setDeliverySlip

    mixed OrderCore::setDeliverySlip()

This method allows to generate first delivery slip of the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1362](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1362)




### <a name="method-setInvoice"></a>setInvoice

    mixed OrderCore::setInvoice($use_existing_payment)

This method allows to generate first invoice of the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1216](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1216)


#### Arguments
* $use_existing_payment **mixed**



### <a name="method-setInvoiceDetails"></a>setInvoiceDetails

    mixed OrderCore::setInvoiceDetails($order_invoice)

This method allows to fulfill the object order_invoice with sales figures



* Visibility: **protected**
* Source: [classes/order/Order.php line 1312](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1312)


#### Arguments
* $order_invoice **mixed**



### <a name="method-setLastInvoiceNumber"></a>setLastInvoiceNumber

    mixed OrderCore::setLastInvoiceNumber($order_invoice_id, $id_shop)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 1174](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1174)


#### Arguments
* $order_invoice_id **mixed**
* $id_shop **mixed**



### <a name="method-setProductCurrentStock"></a>setProductCurrentStock

    mixed OrderCore::setProductCurrentStock($product)

This method allow to add stock information on a product detail

If advanced stock management is active, get physical stock of this product in the warehouse associated to the ptoduct for the current order
Else get the available quantity of the product in fucntion of the shop associated to the order

* Visibility: **protected**
* Source: [classes/order/Order.php line 680](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L680)


#### Arguments
* $product **mixed**



### <a name="method-setProductCustomizedDatas"></a>setProductCustomizedDatas

    mixed OrderCore::setProductCustomizedDatas($product, $customized_datas)





* Visibility: **protected**
* Source: [classes/order/Order.php line 661](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L661)


#### Arguments
* $product **mixed**
* $customized_datas **mixed**



### <a name="method-setProductImageInformations"></a>setProductImageInformations

    mixed OrderCore::setProductImageInformations($product)

This method allow to add image information on a product detail



* Visibility: **protected**
* Source: [classes/order/Order.php line 696](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L696)


#### Arguments
* $product **mixed**



### <a name="method-setProductPrices"></a>setProductPrices

    mixed OrderCore::setProductPrices($row)

Marked as deprecated but should not throw any "deprecated" message
This function is used in order to keep front office backward compatibility 14 -> 1.5
(Order History)



* Visibility: **public**
* Source: [classes/order/Order.php line 571](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L571)


#### Arguments
* $row **mixed**



### <a name="method-setWsCurrentState"></a>setWsCurrentState

    mixed OrderCore::setWsCurrentState($state)





* Visibility: **public**
* Source: [classes/order/Order.php line 2223](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2223)


#### Arguments
* $state **mixed**



### <a name="method-setWsShippingNumber"></a>setWsShippingNumber

    mixed OrderCore::setWsShippingNumber($shipping_number)





* Visibility: **public**
* Source: [classes/order/Order.php line 2199](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2199)


#### Arguments
* $shipping_number **mixed**



### <a name="method-sortDocuments"></a>sortDocuments

    mixed OrderCore::sortDocuments($a, $b)





* Visibility: **public**
* This method is **static**.
* Source: [classes/order/Order.php line 2178](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2178)


#### Arguments
* $a **mixed**
* $b **mixed**



### <a name="method-updateOrderDetailTax"></a>updateOrderDetailTax

    mixed OrderCore::updateOrderDetailTax()

The primary purpose of this method is to be
called at the end of the generation of each order
in PaymentModule::validateOrder, to fill in
the order_detail_tax table with taxes
that will add up in such a way that
the sum of the tax amounts in the product tax breakdown
is equal to the difference between products with tax and
products without tax.



* Visibility: **public**
* Source: [classes/order/Order.php line 2393](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L2393)




### <a name="method-updateShippingCost"></a>updateShippingCost

    boolean OrderCore::updateShippingCost(float $amount)

This method allows to change the shipping cost of the current order



* Visibility: **public**
* Source: [classes/order/Order.php line 1905](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1905)


#### Arguments
* $amount **float**



### <a name="method-useOneAfterAnotherTaxComputationMethod"></a>useOneAfterAnotherTaxComputationMethod

    boolean OrderCore::useOneAfterAnotherTaxComputationMethod()

This method returns true if at least one order details uses the
One After Another tax computation method.



* Visibility: **public**
* Source: [classes/order/Order.php line 1651](https://github.com/PrestaShop/PrestaShop/blob/1.6.1.1/classes/order/Order.php#L1651)


