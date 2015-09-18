Adapter_AddressFactory
===============

2007-2015 PrestaShop

NOTICE OF LICENSE

This source file is subject to the Open Software License (OSL 3.0)
that is bundled with this package in the file LICENSE.txt.
It is also available through the world-wide-web at this URL:
http://opensource.org/licenses/osl-3.0.php
If you did not receive a copy of the license and are unable to
obtain it through the world-wide-web, please send an email
to license@prestashop.com so we can send you a copy immediately.

DISCLAIMER

Do not edit or add to this file if you wish to upgrade PrestaShop to newer
versions in the future. If you wish to customize PrestaShop for your
needs please refer to http://www.prestashop.com for more information.


* Class name: Adapter_AddressFactory
* Namespace: 







Methods
-------


### findOrCreate

    \Address Adapter_AddressFactory::findOrCreate(null $id_address, boolean $with_geoloc)

Initilize an address corresponding to the specified id address or if empty to the
default shop configuration



* Visibility: **public**


#### Arguments
* $id_address **null**
* $with_geoloc **boolean**



### addressExists

    boolean Adapter_AddressFactory::addressExists($id_address)

Check if an address exists depending on given $id_address



* Visibility: **public**


#### Arguments
* $id_address **mixed**

