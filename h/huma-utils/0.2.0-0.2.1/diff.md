# Comparing `tmp/huma_utils-0.2.0.tar.gz` & `tmp/huma_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_utils-0.2.0.tar", max compression
+gzip compressed data, was "huma_utils-0.2.1.tar", max compression
```

## Comparing `huma_utils-0.2.0.tar` & `huma_utils-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-15 18:17:08.936579 huma_utils-0.2.0/LICENSE
--rw-r--r--   0        0        0       35 2023-06-15 18:17:08.936579 huma_utils-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/__init__.py
--rw-r--r--   0        0        0      291 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/chain_utils.py
--rw-r--r--   0        0        0      330 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/datetime_utils.py
--rw-r--r--   0        0        0      428 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/pydantic_utils.py
--rw-r--r--   0        0        0      702 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/request_utils.py
--rw-r--r--   0        0        0     1113 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/string_utils.py
--rw-r--r--   0        0        0      543 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/address_helpers.py
--rw-r--r--   0        0        0      809 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/api_test_helpers.py
--rw-r--r--   0        0        0     2294 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/vcr_helpers.py
--rw-r--r--   0        0        0     1129 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/web3_utils.py
--rw-r--r--   0        0        0     2240 2023-06-15 18:17:08.936579 huma_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-15 18:29:22.782850 huma_utils-0.2.1/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-15 18:29:22.782850 huma_utils-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/chain_utils.py
+-rw-r--r--   0        0        0      330 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/datetime_utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/py.typed
+-rw-r--r--   0        0        0      428 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/pydantic_utils.py
+-rw-r--r--   0        0        0      702 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/request_utils.py
+-rw-r--r--   0        0        0     1113 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/string_utils.py
+-rw-r--r--   0        0        0      543 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/test_helpers/address_helpers.py
+-rw-r--r--   0        0        0      809 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/test_helpers/api_test_helpers.py
+-rw-r--r--   0        0        0     2294 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/test_helpers/vcr_helpers.py
+-rw-r--r--   0        0        0     1129 2023-06-15 18:29:22.782850 huma_utils-0.2.1/huma_utils/web3_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-15 18:29:22.786850 huma_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.2.1/PKG-INFO
```

### Comparing `huma_utils-0.2.0/LICENSE` & `huma_utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/request_utils.py` & `huma_utils-0.2.1/huma_utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/string_utils.py` & `huma_utils-0.2.1/huma_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/test_helpers/address_helpers.py` & `huma_utils-0.2.1/huma_utils/test_helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/test_helpers/api_test_helpers.py` & `huma_utils-0.2.1/huma_utils/test_helpers/api_test_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/test_helpers/vcr_helpers.py` & `huma_utils-0.2.1/huma_utils/test_helpers/vcr_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/huma_utils/web3_utils.py` & `huma_utils-0.2.1/huma_utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.0/pyproject.toml` & `huma_utils-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-utils"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["flowers-huang <flora221@stanford.edu>"]
 readme = "README.md"
 packages = [{include = "huma_utils"}]
 
 [tool.poetry.dependencies]
 python = "~3.10"
```

