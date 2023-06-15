# Comparing `tmp/odoo14_addons_oca_sale_workflow-14.0.20230612.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_sale_workflow-14.0.20230614.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2405 bytes, number of entries: 4
--rw-r--r--  2.0 unx     6501 b- defN 23-Jun-13 05:18 odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:18 odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 05:18 odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      433 b- defN 23-Jun-13 05:18 odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/RECORD
-4 files, 7027 bytes uncompressed, 1551 bytes compressed:  77.9%
+Zip file size: 2428 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     6675 b- defN 23-Jun-15 05:02 odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 05:02 odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-15 05:02 odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      433 b- defN 23-Jun-15 05:02 odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/RECORD
+4 files, 7201 bytes uncompressed, 1574 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/METADATA
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/RECORD
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_sale_workflow-14.0.20230612.0.dist-info/METADATA` & `odoo14_addons_oca_sale_workflow-14.0.20230614.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-sale-workflow
-Version: 14.0.20230612.0
+Version: 14.0.20230614.2
 Summary: Meta package for oca-sale-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -36,14 +36,15 @@
 Requires-Dist: odoo14-addon-sale-delivery-state
 Requires-Dist: odoo14-addon-sale-discount-display-amount
 Requires-Dist: odoo14-addon-sale-elaboration
 Requires-Dist: odoo14-addon-sale-exception
 Requires-Dist: odoo14-addon-sale-fixed-discount
 Requires-Dist: odoo14-addon-sale-force-invoiced
 Requires-Dist: odoo14-addon-sale-global-discount
+Requires-Dist: odoo14-addon-sale-invoice-auto-deliver
 Requires-Dist: odoo14-addon-sale-invoice-blocking
 Requires-Dist: odoo14-addon-sale-invoice-no-mail
 Requires-Dist: odoo14-addon-sale-invoice-plan
 Requires-Dist: odoo14-addon-sale-invoice-policy
 Requires-Dist: odoo14-addon-sale-isolated-quotation
 Requires-Dist: odoo14-addon-sale-last-price-info
 Requires-Dist: odoo14-addon-sale-mail-autosubscribe
@@ -97,14 +98,16 @@
 Requires-Dist: odoo14-addon-sale-product-category-menu
 Requires-Dist: odoo14-addon-sale-product-multi-add
 Requires-Dist: odoo14-addon-sale-product-rating-verified
 Requires-Dist: odoo14-addon-sale-product-seasonality
 Requires-Dist: odoo14-addon-sale-product-set
 Requires-Dist: odoo14-addon-sale-product-set-packaging-qty
 Requires-Dist: odoo14-addon-sale-product-set-sale-by-packaging
+Requires-Dist: odoo14-addon-sale-promotion-rule
+Requires-Dist: odoo14-addon-sale-promotion-rule-display-discount-amount
 Requires-Dist: odoo14-addon-sale-purchase-requisition
 Requires-Dist: odoo14-addon-sale-quick
 Requires-Dist: odoo14-addon-sale-quick-seasonality
 Requires-Dist: odoo14-addon-sale-quotation-number
 Requires-Dist: odoo14-addon-sale-quotation-template-product-multi-add
 Requires-Dist: odoo14-addon-sale-rental
 Requires-Dist: odoo14-addon-sale-restricted-qty
```

