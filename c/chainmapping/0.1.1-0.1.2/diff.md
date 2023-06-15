# Comparing `tmp/chainmapping-0.1.1.tar.gz` & `tmp/chainmapping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmapping-0.1.1.tar", max compression
+gzip compressed data, was "chainmapping-0.1.2.tar", max compression
```

## Comparing `chainmapping-0.1.1.tar` & `chainmapping-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-06-08 10:24:34.838542 chainmapping-0.1.1/LICENSE
--rw-r--r--   0        0        0       80 2023-06-08 10:24:34.838542 chainmapping-0.1.1/README.md
--rw-r--r--   0        0        0     2183 2023-06-08 10:24:34.838542 chainmapping-0.1.1/chainmapping/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 10:24:34.838542 chainmapping-0.1.1/chainmapping/py.typed
--rw-r--r--   0        0        0      630 2023-06-08 10:24:34.838542 chainmapping-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 chainmapping-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-15 11:06:34.673850 chainmapping-0.1.2/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-15 11:06:34.673850 chainmapping-0.1.2/README.md
+-rw-r--r--   0        0        0     2183 2023-06-15 11:06:34.673850 chainmapping-0.1.2/chainmapping/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:06:34.673850 chainmapping-0.1.2/chainmapping/py.typed
+-rw-r--r--   0        0        0      589 2023-06-15 11:06:34.673850 chainmapping-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 chainmapping-0.1.2/PKG-INFO
```

### Comparing `chainmapping-0.1.1/LICENSE` & `chainmapping-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmapping-0.1.1/chainmapping/__init__.py` & `chainmapping-0.1.2/chainmapping/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmapping-0.1.1/pyproject.toml` & `chainmapping-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [tool.poetry]
 name = "chainmapping"
-version = "0.1.1"
-description = "Simple class to create readonly ChainMaps that support typing,Mapping"
+version = "0.1.2"
+description = "Simple class to create readonly ChainMaps that support typing.Mapping"
 authors = ["Kalle M. Aagaard <km@conscia.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 
-[tool.poetry.group.test]
-optional = true
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 
 
+
 [tool.pytest.ini_options]
 addopts = "-v --cov=chainmapping --cov-report=xml --cov-report=term"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainmapping-0.1.1/PKG-INFO` & `chainmapping-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chainmapping
-Version: 0.1.1
-Summary: Simple class to create readonly ChainMaps that support typing,Mapping
+Version: 0.1.2
+Summary: Simple class to create readonly ChainMaps that support typing.Mapping
 Author: Kalle M. Aagaard
 Author-email: km@conscia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

