# Comparing `tmp/eodc_faas_sen2like-2023.5.1rc0.tar.gz` & `tmp/eodc_faas_sen2like-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.5.1rc0.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.6.1.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.5.1rc0.tar` & `eodc_faas_sen2like-2023.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2023-04-03 14:47:47.787253 eodc_faas_sen2like-2023.5.1rc0/README.md
--rw-r--r--   0        0        0      689 2023-06-12 08:38:17.799253 eodc_faas_sen2like-2023.5.1rc0/pyproject.toml
--rw-r--r--   0        0        0      193 2023-06-12 08:38:17.799253 eodc_faas_sen2like-2023.5.1rc0/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.1rc0/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.031253 eodc_faas_sen2like-2023.5.1rc0/sen2like_processor_bindings/workflows.py
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.5.1rc0/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.1/README.md
+-rw-r--r--   0        0        0      684 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2057 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.1/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.5.1rc0/pyproject.toml` & `eodc_faas_sen2like-2023.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.05.1-rc.0"
+version = "2023.06.1"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_sen2like-2023.5.1rc0/sen2like_processor_bindings/model.py` & `eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
 class Sen2LikeParameters(BaseModel):
     """Pydantic model of sen2like supported parameters."""
 
     spatial_extent: BoundingBox
     temporal_extent: list
     user_workspace: Path
-    target_resolution: Optional[int] = 10
+    target_resolution: Optional[int] = None
     target_product: Optional[str] = Field(regex=r"L2F|L2H|l2f|l2h", default="L2F")
     options: Optional[sen2like_options] = None
 
     @validator("target_resolution")
     def check_resolution(cls, v):
-        if v not in [10, 20, 60]:
+        if v not in [None, 10, 20, 60]:
             raise ValueError("Resolution must be set to 10, 20 or 60.")
         return v
```

### Comparing `eodc_faas_sen2like-2023.5.1rc0/sen2like_processor_bindings/workflows.py` & `eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/workflows.py`

 * *Files identical despite different names*

