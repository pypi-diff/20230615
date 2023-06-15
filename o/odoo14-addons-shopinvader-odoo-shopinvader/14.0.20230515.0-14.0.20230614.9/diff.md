# Comparing `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2046 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4585 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      477 b- defN 23-May-16 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/RECORD
-4 files, 5155 bytes uncompressed, 1104 bytes compressed:  78.6%
+Zip file size: 2138 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5227 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      477 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/RECORD
+4 files, 5797 bytes uncompressed, 1196 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/WHEEL
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/top_level.txt
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/RECORD
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230515.0.dist-info/METADATA` & `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-shopinvader-odoo-shopinvader
-Version: 14.0.20230515.0
+Version: 14.0.20230614.9
 Summary: Meta package for shopinvader-odoo-shopinvader Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -15,23 +15,25 @@
 Requires-Dist: odoo14-addon-shopinvader-auth-api-key
 Requires-Dist: odoo14-addon-shopinvader-auth-jwt
 Requires-Dist: odoo14-addon-shopinvader-backend-image-proxy
 Requires-Dist: odoo14-addon-shopinvader-cart-expiry
 Requires-Dist: odoo14-addon-shopinvader-category-image-for-product
 Requires-Dist: odoo14-addon-shopinvader-contact-address-default
 Requires-Dist: odoo14-addon-shopinvader-customer-activity
+Requires-Dist: odoo14-addon-shopinvader-customer-autobind
 Requires-Dist: odoo14-addon-shopinvader-customer-invoicing-mode
 Requires-Dist: odoo14-addon-shopinvader-customer-multi-user
 Requires-Dist: odoo14-addon-shopinvader-customer-multi-user-company-group
 Requires-Dist: odoo14-addon-shopinvader-customer-multi-user-validate
 Requires-Dist: odoo14-addon-shopinvader-customer-multi-user-wishlist
 Requires-Dist: odoo14-addon-shopinvader-customer-price
 Requires-Dist: odoo14-addon-shopinvader-customer-price-wishlist
 Requires-Dist: odoo14-addon-shopinvader-customer-validate
 Requires-Dist: odoo14-addon-shopinvader-delivery-carrier
+Requires-Dist: odoo14-addon-shopinvader-delivery-carrier-category-keep-carrier
 Requires-Dist: odoo14-addon-shopinvader-delivery-instruction
 Requires-Dist: odoo14-addon-shopinvader-delivery-state
 Requires-Dist: odoo14-addon-shopinvader-easy-binding
 Requires-Dist: odoo14-addon-shopinvader-elasticsearch
 Requires-Dist: odoo14-addon-shopinvader-guest-mode
 Requires-Dist: odoo14-addon-shopinvader-image
 Requires-Dist: odoo14-addon-shopinvader-import-image
@@ -39,14 +41,15 @@
 Requires-Dist: odoo14-addon-shopinvader-lead
 Requires-Dist: odoo14-addon-shopinvader-locomotive
 Requires-Dist: odoo14-addon-shopinvader-locomotive-algolia
 Requires-Dist: odoo14-addon-shopinvader-locomotive-guest-mode
 Requires-Dist: odoo14-addon-shopinvader-locomotive-reset-password
 Requires-Dist: odoo14-addon-shopinvader-locomotive-sale-profile
 Requires-Dist: odoo14-addon-shopinvader-locomotive-wishlist
+Requires-Dist: odoo14-addon-shopinvader-mass-mailing-company-newsletter
 Requires-Dist: odoo14-addon-shopinvader-membership
 Requires-Dist: odoo14-addon-shopinvader-multi-cart
 Requires-Dist: odoo14-addon-shopinvader-multi-category
 Requires-Dist: odoo14-addon-shopinvader-notification-default
 Requires-Dist: odoo14-addon-shopinvader-partner-firstname
 Requires-Dist: odoo14-addon-shopinvader-partner-vat
 Requires-Dist: odoo14-addon-shopinvader-pending-cart-reminder
@@ -69,19 +72,26 @@
 Requires-Dist: odoo14-addon-shopinvader-product-stock-state
 Requires-Dist: odoo14-addon-shopinvader-product-template-multi-link
 Requires-Dist: odoo14-addon-shopinvader-product-template-multi-link-date-span
 Requires-Dist: odoo14-addon-shopinvader-product-template-tags
 Requires-Dist: odoo14-addon-shopinvader-product-variant-multi-link
 Requires-Dist: odoo14-addon-shopinvader-product-variant-selector
 Requires-Dist: odoo14-addon-shopinvader-product-video-link
+Requires-Dist: odoo14-addon-shopinvader-promotion-rule
 Requires-Dist: odoo14-addon-shopinvader-quotation
+Requires-Dist: odoo14-addon-shopinvader-quotation-portal-mode
 Requires-Dist: odoo14-addon-shopinvader-sale-amount-by-group
 Requires-Dist: odoo14-addon-shopinvader-sale-automatic-workflow
 Requires-Dist: odoo14-addon-shopinvader-sale-coupon
+Requires-Dist: odoo14-addon-shopinvader-sale-order-report-without-price
 Requires-Dist: odoo14-addon-shopinvader-sale-packaging
 Requires-Dist: odoo14-addon-shopinvader-sale-packaging-wishlist
 Requires-Dist: odoo14-addon-shopinvader-sale-profile
+Requires-Dist: odoo14-addon-shopinvader-sale-profile-update-price
+Requires-Dist: odoo14-addon-shopinvader-sale-update-price
 Requires-Dist: odoo14-addon-shopinvader-search-engine
+Requires-Dist: odoo14-addon-shopinvader-validation-token
+Requires-Dist: odoo14-addon-shopinvader-validation-token-guest
 Requires-Dist: odoo14-addon-shopinvader-wishlist
 
 UNKNOWN
```

