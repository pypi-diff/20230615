# Comparing `tmp/huma_utils-0.1.0.tar.gz` & `tmp/huma_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_utils-0.1.0.tar", max compression
+gzip compressed data, was "huma_utils-0.2.0.tar", max compression
```

## Comparing `huma_utils-0.1.0.tar` & `huma_utils-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-06-14 23:34:15.702626 huma_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2023-06-14 23:34:15.702626 huma_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/__init__.py
--rw-r--r--   0        0        0      291 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/chain_utils.py
--rw-r--r--   0        0        0      330 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/datetime_utils.py
--rw-r--r--   0        0        0      428 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/pydantic_utils.py
--rw-r--r--   0        0        0      702 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/request_utils.py
--rw-r--r--   0        0        0     1113 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/string_utils.py
--rw-r--r--   0        0        0     1129 2023-06-14 23:34:15.702626 huma_utils-0.1.0/huma_utils/web3_utils.py
--rw-r--r--   0        0        0     2171 2023-06-14 23:34:15.706626 huma_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-15 18:17:08.936579 huma_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-15 18:17:08.936579 huma_utils-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/chain_utils.py
+-rw-r--r--   0        0        0      330 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/datetime_utils.py
+-rw-r--r--   0        0        0      428 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/pydantic_utils.py
+-rw-r--r--   0        0        0      702 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/request_utils.py
+-rw-r--r--   0        0        0     1113 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/string_utils.py
+-rw-r--r--   0        0        0      543 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/address_helpers.py
+-rw-r--r--   0        0        0      809 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/api_test_helpers.py
+-rw-r--r--   0        0        0     2294 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/test_helpers/vcr_helpers.py
+-rw-r--r--   0        0        0     1129 2023-06-15 18:17:08.936579 huma_utils-0.2.0/huma_utils/web3_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-15 18:17:08.936579 huma_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.2.0/PKG-INFO
```

### Comparing `huma_utils-0.1.0/LICENSE` & `huma_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_utils-0.1.0/huma_utils/request_utils.py` & `huma_utils-0.2.0/huma_utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.1.0/huma_utils/string_utils.py` & `huma_utils-0.2.0/huma_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.1.0/huma_utils/web3_utils.py` & `huma_utils-0.2.0/huma_utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.1.0/pyproject.toml` & `huma_utils-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-utils"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["flowers-huang <flora221@stanford.edu>"]
 readme = "README.md"
 packages = [{include = "huma_utils"}]
 
 [tool.poetry.dependencies]
 python = "~3.10"
@@ -25,14 +25,17 @@
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 pylint-google-style-guide-imports-enforcing = "^1.3.0"
 pytest-spec = "^3.2.0"
 pylint-pydantic = "^0.1.8"
 pre-commit = "^3.3.3"
 pytest-cov = "^4.1.0"
+types-factory-boy = "^0.4.1"
+vcrpy = "^4.3.1"
+factory-boy = "^3.2.1"
 
 [tool.pytest.ini_options]
 describe_prefixes = ["describe", "if", "when", "with", "without"]
 pythonfunctions = ["it", "its_"]
 asyncio_mode = "auto"
 
 [tool.isort]
```

