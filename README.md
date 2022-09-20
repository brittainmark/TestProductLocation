For testing against 1.5.8
- Install files in zc_install
- login to admin
- goto Admin>modules>Plugin Manager
- install module
- goto Admin>Catalogue>Categories/Products
- goto page with products
- you will see a new column called location (it will be blank at this stage)
- edit an existing product
- add in a text string to the product location box
- save the change

this will show you the warning
```
[20-Sep-2022 12:16:13 UTC] Request URI: /Test158/Horse-ENN-qUill/index.php?cmd=product&cPath=67&pID=205&action=new_product_preview, IP address: 127.0.0.1
#0 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/includes/classes/object_info.php(735): zen_debug_error_handler()
#1 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/includes/classes/object_info.php(724): objectInfo->__set()
#2 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/includes/classes/object_info.php(700): objectInfo->updateObjectInfo()
#3 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/includes/modules/product/preview_info.php(17): objectInfo->__construct()
#4 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/product.php(106): require('...')
#5 /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/index.php(11): require('...')
--> PHP Deprecated: Creation of dynamic property objectInfo::$vs_products_location is deprecated in /home/lotus/public_html/innerlightcrystals/Test158/Horse-ENN-qUill/includes/classes/object_info.php on line 735.
```


