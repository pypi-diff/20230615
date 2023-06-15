# Comparing `tmp/eodc-2023.5.3.tar.gz` & `tmp/eodc-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.5.3.tar", max compression
+gzip compressed data, was "eodc-2023.6.0.tar", max compression
```

## Comparing `eodc-2023.5.3.tar` & `eodc-2023.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-05-31 06:57:59.894315 eodc-2023.5.3/README.md
--rw-r--r--   0        0        0      213 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/dask.py
--rw-r--r--   0        0        0      757 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-05-31 06:57:59.894315 eodc-2023.5.3/eodc/settings.py
--rw-r--r--   0        0        0     1114 2023-05-31 06:57:59.894315 eodc-2023.5.3/pyproject.toml
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 eodc-2023.5.3/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-15 14:23:04.217737 eodc-2023.6.0/README.md
+-rw-r--r--   0        0        0      213 2023-06-15 14:23:04.217737 eodc-2023.6.0/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-15 14:23:04.217737 eodc-2023.6.0/eodc/dask.py
+-rw-r--r--   0        0        0     6828 2023-06-15 14:23:04.217737 eodc-2023.6.0/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-15 14:23:04.217737 eodc-2023.6.0/eodc/settings.py
+-rw-r--r--   0        0        0     1143 2023-06-15 14:23:04.217737 eodc-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1641 1970-01-01 00:00:00.000000 eodc-2023.6.0/PKG-INFO
```

### Comparing `eodc-2023.5.3/README.md` & `eodc-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.3/eodc/dask.py` & `eodc-2023.6.0/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.5.3/pyproject.toml` & `eodc-2023.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.5.3"
+version = "2023.6.0"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -21,16 +21,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
-eodc-faas-force = "^2023.5.3"
-eodc-faas-sen2like = "^2023.5.0rc0"
+eodc-faas-force = "2023.6.2"
+eodc-faas-sen2like = "2023.6.2"
+eodc-faas-openeo = "^2023.6.5rc1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
```

