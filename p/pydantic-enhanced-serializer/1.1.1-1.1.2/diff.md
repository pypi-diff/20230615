# Comparing `tmp/pydantic_enhanced_serializer-1.1.1-py3-none-any.whl.zip` & `tmp/pydantic_enhanced_serializer-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15782 bytes, number of entries: 15
+Zip file size: 15805 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      309 b- defN 23-Mar-08 23:12 pydantic_enhanced_serializer/__init__.py
 -rw-r--r--  2.0 unx     9424 b- defN 23-Apr-27 05:29 pydantic_enhanced_serializer/fieldsets.py
 -rw-r--r--  2.0 unx     2724 b- defN 23-Mar-08 23:35 pydantic_enhanced_serializer/models.py
 -rw-r--r--  2.0 unx     3960 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/path_put.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/py.typed
 -rw-r--r--  2.0 unx     4222 b- defN 23-Mar-08 23:32 pydantic_enhanced_serializer/render.py
--rw-r--r--  2.0 unx     6996 b- defN 23-Apr-13 21:29 pydantic_enhanced_serializer/schema.py
+-rw-r--r--  2.0 unx     7136 b- defN 23-Jun-15 20:42 pydantic_enhanced_serializer/schema.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/integrations/__init__.py
 -rw-r--r--  2.0 unx     1401 b- defN 23-Mar-08 23:47 pydantic_enhanced_serializer/integrations/django_ninja.py
 -rw-r--r--  2.0 unx     6078 b- defN 23-Mar-08 23:14 pydantic_enhanced_serializer/integrations/fastapi.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6021 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       29 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-27 05:34 pydantic_enhanced_serializer-1.1.1.dist-info/RECORD
-15 files, 43817 bytes uncompressed, 13224 bytes compressed:  69.8%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-15 20:53 pydantic_enhanced_serializer-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6021 b- defN 23-Jun-15 20:53 pydantic_enhanced_serializer-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 20:53 pydantic_enhanced_serializer-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-15 20:53 pydantic_enhanced_serializer-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1488 b- defN 23-Jun-15 20:53 pydantic_enhanced_serializer-1.1.2.dist-info/RECORD
+15 files, 43957 bytes uncompressed, 13247 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pydantic_enhanced_serializer/integrations/django_ninja.py
 Comment: 
 
 Filename: pydantic_enhanced_serializer/integrations/fastapi.py
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE
+Filename: pydantic_enhanced_serializer-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.1.dist-info/METADATA
+Filename: pydantic_enhanced_serializer-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL
+Filename: pydantic_enhanced_serializer-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt
+Filename: pydantic_enhanced_serializer-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.1.1.dist-info/RECORD
+Filename: pydantic_enhanced_serializer-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydantic_enhanced_serializer/schema.py

```diff
@@ -84,20 +84,22 @@
 
             if inspect.isclass(response_model) and issubclass(
                 response_model, BaseModel
             ):
                 model_name = normalize_name(response_model.__name__)
                 schema["properties"][fieldset_name][
                     "$ref"
-                ] = f"#/definitions/{model_name}"
+                ] = f"#/components/schemas/{model_name}"
 
                 augment_schema_with_fieldsets(response_model)
-                if "definitions" not in schema:
-                    schema["definitions"] = {}
-                schema["definitions"][model_name] = model_schema(response_model)
+                if "components" not in schema:
+                    schema["components"] = {"schemas": {}}
+                schema["components"]["schemas"][model_name] = model_schema(
+                    response_model
+                )
 
             else:
                 add_field_type_to_schema(
                     get_origin(response_model) or response_model,
                     schema["properties"][fieldset_name],
                 )
 
@@ -106,21 +108,23 @@
                 if (
                     list_models
                     and inspect.isclass(list_models[0])
                     and issubclass(list_models[0], BaseModel)
                 ):
                     model_name = normalize_name(list_models[0].__name__)
                     schema["properties"][fieldset_name]["items"] = {
-                        "$ref": f"#/definitions/{model_name}"
+                        "$ref": f"#/components/schemas/{model_name}"
                     }
 
                     augment_schema_with_fieldsets(list_models[0])
-                    if "definitions" not in schema:
-                        schema["definitions"] = {}
-                    schema["definitions"][model_name] = model_schema(list_models[0])
+                    if "components" not in schema:
+                        schema["components"] = {"schemas": {}}
+                    schema["components"]["schemas"][model_name] = model_schema(
+                        list_models[0]
+                    )
 
                 elif list_models:
                     # add_field_type_to_schema is not copy-safe on subdicts
                     schema["properties"][fieldset_name]["items"] = {}
                     add_field_type_to_schema(
                         list_models[0], schema["properties"][fieldset_name]["items"]
                     )
```

## Comparing `pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE` & `pydantic_enhanced_serializer-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydantic_enhanced_serializer-1.1.1.dist-info/METADATA` & `pydantic_enhanced_serializer-1.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-enhanced-serializer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Pydantic extension that allows user selection of object fields or expansions inline when serializing models
 Home-page: https://github.com/adamsussman/pydantic-enhanced-serializer
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
```

## Comparing `pydantic_enhanced_serializer-1.1.1.dist-info/RECORD` & `pydantic_enhanced_serializer-1.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pydantic_enhanced_serializer/__init__.py,sha256=YDA4Ntaq4mBBR0nDyHFXlvqE_OWJ6mzsCHlxjX71nYc,309
 pydantic_enhanced_serializer/fieldsets.py,sha256=YU94v7aW5dDNkGmhZXkWYlCKb2up1iXKsYaoPPKApNc,9424
 pydantic_enhanced_serializer/models.py,sha256=ZGoQZ9cHTT9icObGvfWFkeBYRSQUKYYbligdsiDvX94,2724
 pydantic_enhanced_serializer/path_put.py,sha256=CPqpjErHgzvipU6B326A-XpSbhTtWJzGeV9UODzMUjY,3960
 pydantic_enhanced_serializer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/render.py,sha256=OsnGmTjDr93Xi1vYWcM5YgNDpsZbpsAa5Ct724-BxBw,4222
-pydantic_enhanced_serializer/schema.py,sha256=p3kUgONZMZ3qMdoCw7qMYgQHjHL39I2kh39fT_gwaks,6996
+pydantic_enhanced_serializer/schema.py,sha256=XRayqeqtFvCjTmx_mMY-4ob7_VUo6F_1x2nfUS2i_AM,7136
 pydantic_enhanced_serializer/integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/integrations/django_ninja.py,sha256=Z60LR0vfM4wbpvWo_qfEhcsUn4ufXU80xwD4zbPGIdI,1401
 pydantic_enhanced_serializer/integrations/fastapi.py,sha256=6qBNdbafvEAmVDBVS0h_AedDnevh_Ilv3bztF3pcYHY,6078
-pydantic_enhanced_serializer-1.1.1.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-pydantic_enhanced_serializer-1.1.1.dist-info/METADATA,sha256=D0ceLYIqy6OSFWziAzHZj2VmLb4g6JIM4dVOM3uj_kw,6021
-pydantic_enhanced_serializer-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pydantic_enhanced_serializer-1.1.1.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
-pydantic_enhanced_serializer-1.1.1.dist-info/RECORD,,
+pydantic_enhanced_serializer-1.1.2.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+pydantic_enhanced_serializer-1.1.2.dist-info/METADATA,sha256=UZEM8ZdCQmsYYLggFoqjNE3k1edXijrpte0M_fslGOk,6021
+pydantic_enhanced_serializer-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pydantic_enhanced_serializer-1.1.2.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
+pydantic_enhanced_serializer-1.1.2.dist-info/RECORD,,
```

