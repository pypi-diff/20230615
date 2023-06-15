# Comparing `tmp/odoo14_addon_crm_rest_api-14.0.1.0.1.dev1-py3-none-any.whl.zip` & `tmp/odoo14_addon_crm_rest_api-14.0.1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 3637 bytes, number of entries: 10
+Zip file size: 4195 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      648 b- defN 23-Jun-15 16:56 odoo/addons/crm_rest_api/CHANGELOG.md
 -rw-r--r--  2.0 unx       96 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/README.rst
 -rw-r--r--  2.0 unx       23 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/__init__.py
--rw-r--r--  2.0 unx      516 b- defN 23-May-03 13:36 odoo/addons/crm_rest_api/__manifest__.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Jun-15 16:56 odoo/addons/crm_rest_api/__manifest__.py
 -rw-r--r--  2.0 unx       32 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/__init__.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/crm_lead_services.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Jun-15 16:56 odoo/addons/crm_rest_api/services/crm_lead_services.py
 -rw-r--r--  2.0 unx      235 b- defN 23-May-08 14:04 odoo/addons/crm_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      605 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      995 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
-10 files, 3551 bytes uncompressed, 1867 bytes compressed:  47.4%
+-rw-r--r--  2.0 unx      600 b- defN 23-Jun-15 16:56 odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 16:56 odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-15 16:56 odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1068 b- defN 23-Jun-15 16:56 odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/RECORD
+11 files, 4308 bytes uncompressed, 2315 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: odoo/addons/crm_rest_api/CHANGELOG.md
+Comment: 
+
 Filename: odoo/addons/crm_rest_api/README.rst
 Comment: 
 
 Filename: odoo/addons/crm_rest_api/__init__.py
 Comment: 
 
 Filename: odoo/addons/crm_rest_api/__manifest__.py
@@ -12,20 +15,20 @@
 
 Filename: odoo/addons/crm_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM Lead on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '14.0.1.0.0',
+    'version': '14.0.1.0.2',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'base_rest',
         'base_rest_base_structure',
         'crm',
```

## odoo/addons/crm_rest_api/services/crm_lead_services.py

```diff
@@ -9,15 +9,15 @@
     _inherit = "base.rest.private_abstract_service"
     _name = "crm.lead.service"
     _usage = "crm-lead"
     _description = """
         Crm Lead Services
     """
 
-    def create(self, **params):
+    def create(self, params):
         create_dict = self._prepare_create(params)
         crm_lead = self.env['crm.lead'].create(create_dict)
         return Response(
             json.dumps({
                 'message': _("Creation ok"),
                 'id': crm_lead.id
             }),
@@ -25,11 +25,13 @@
             content_type="application/json"
         )
 
     def _validator_create(self):
         return schemas.S_CRM_LEAD_CREATE
 
     def _prepare_create(self, params):
-        create_dict = {}
+        create_dict = {
+            'type': 'opportunity'
+        }
         for key in params:
             create_dict[key] = params[key]
         return create_dict
```

## Comparing `odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA` & `odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-crm-rest-api
-Version: 14.0.1.0.1.dev1
+Version: 14.0.1.0.2
 Summary: Expose CRM Lead on the Rest API
 Home-page: UNKNOWN
 Author: Coopdevs Treball SCCL
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD` & `odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+odoo/addons/crm_rest_api/CHANGELOG.md,sha256=RUlc8jZv_tYB-yaV2-eyJYThEz_1IhIRADQIuepe138,648
 odoo/addons/crm_rest_api/README.rst,sha256=PNgi4-SbJwOD445Gn_oNPQvrgB5v7OprI92qr8Ctmsw,96
 odoo/addons/crm_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_rest_api/__manifest__.py,sha256=sbRDSV3rSGeEn-gf7HKlCMZBQiP28iv8z4JamUFBRTY,516
+odoo/addons/crm_rest_api/__manifest__.py,sha256=b0ZgRyxXnNQlAehb8sDl_LEHvE_kGsESMZkp5XRlUVU,516
 odoo/addons/crm_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
-odoo/addons/crm_rest_api/services/crm_lead_services.py,sha256=IeoJAFjcXUVJbwxGZqaYiVBsFLmz_dDmxyUq-wWGU18,952
+odoo/addons/crm_rest_api/services/crm_lead_services.py,sha256=b8KEkCuipUP0wT_1CBz__BXLYUt0j_P6JspSGuAUxkk,993
 odoo/addons/crm_rest_api/services/schemas.py,sha256=ePXpp9hilOM7h4JjvAelE7hDzuax10WAN1CU1WlWaeE,235
-odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA,sha256=yEJj1ZI1weOWimpncJ3X7aWJx7YWaIO-JBjWX9SQDUQ,605
-odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD,,
+odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/METADATA,sha256=i_NVlolc4PTUgbZNfoUNhHmtBiMZXlD0EO9Qpargqck,600
+odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_crm_rest_api-14.0.1.0.2.dist-info/RECORD,,
```

