# Comparing `tmp/eodc_faas_sen2like-2023.6.1.tar.gz` & `tmp/eodc_faas_sen2like-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_sen2like-2023.6.1.tar", max compression
+gzip compressed data, was "eodc_faas_sen2like-2023.6.2.tar", max compression
```

## Comparing `eodc_faas_sen2like-2023.6.1.tar` & `eodc_faas_sen2like-2023.6.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.1/README.md
--rw-r--r--   0        0        0      684 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0      188 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2057 2023-06-15 07:17:59.175253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-05-08 06:47:08.055253 eodc_faas_sen2like-2023.6.1/sen2like_processor_bindings/workflows.py
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-04-04 13:05:37.511253 eodc_faas_sen2like-2023.6.2/README.md
+-rw-r--r--   0        0        0      619 2023-06-15 13:43:14.072000 eodc_faas_sen2like-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-15 13:43:14.072000 eodc_faas_sen2like-2023.6.2/sen2like_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2970 2023-06-15 13:35:28.568000 eodc_faas_sen2like-2023.6.2/sen2like_processor_bindings/model.py
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 eodc_faas_sen2like-2023.6.2/PKG-INFO
```

### Comparing `eodc_faas_sen2like-2023.6.1/pyproject.toml` & `eodc_faas_sen2like-2023.6.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 [tool.poetry]
 name = "eodc-faas-sen2like"
-version = "2023.06.1"
+version = "2023.6.2"
 description = "Bindings for the sen2like processor exposed at EODC"
 authors = ["Valentina Hutter <valentina.hutter@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "sen2like_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.7"
-requests = "^2.28.2"
-pyproj = "^3.5.0"
-argo-workflows = "6.3.9"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 pytest = "^7.2.2"
 ruff = "^0.0.259"
 ipykernel = "^6.22.0"
```

