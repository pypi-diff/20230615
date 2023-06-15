# Comparing `tmp/logging_utils_cli-1.0.0.tar.gz` & `tmp/logging_utils_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_utils_cli-1.0.0.tar", max compression
+gzip compressed data, was "logging_utils_cli-1.0.1.tar", max compression
```

## Comparing `logging_utils_cli-1.0.0.tar` & `logging_utils_cli-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-06-12 09:20:56.654387 logging_utils_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0      156 2023-06-12 11:42:12.042098 logging_utils_cli-1.0.0/README.md
--rw-r--r--   0        0        0       94 2023-06-12 09:14:13.011825 logging_utils_cli-1.0.0/logging_utils_cli/__init__.py
--rw-r--r--   0        0        0      985 2023-06-12 09:18:22.044683 logging_utils_cli-1.0.0/logging_utils_cli/formatter.py
--rw-r--r--   0        0        0     2158 2023-06-12 09:18:10.284705 logging_utils_cli-1.0.0/logging_utils_cli/utils.py
--rw-r--r--   0        0        0      518 2023-06-12 11:39:41.735971 logging_utils_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 logging_utils_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-12 09:20:56.654387 logging_utils_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0      156 2023-06-12 11:42:12.042098 logging_utils_cli-1.0.1/README.md
+-rw-r--r--   0        0        0      385 2023-06-15 08:42:23.322314 logging_utils_cli-1.0.1/logging_utils_cli/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-12 09:18:22.044683 logging_utils_cli-1.0.1/logging_utils_cli/formatter.py
+-rw-r--r--   0        0        0     2158 2023-06-12 09:18:10.284705 logging_utils_cli-1.0.1/logging_utils_cli/utils.py
+-rw-r--r--   0        0        0      518 2023-06-15 08:30:41.005350 logging_utils_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 logging_utils_cli-1.0.1/PKG-INFO
```

### Comparing `logging_utils_cli-1.0.0/LICENSE` & `logging_utils_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_utils_cli-1.0.0/logging_utils_cli/formatter.py` & `logging_utils_cli-1.0.1/logging_utils_cli/formatter.py`

 * *Files identical despite different names*

### Comparing `logging_utils_cli-1.0.0/logging_utils_cli/utils.py` & `logging_utils_cli-1.0.1/logging_utils_cli/utils.py`

 * *Files identical despite different names*

### Comparing `logging_utils_cli-1.0.0/pyproject.toml` & `logging_utils_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logging-utils-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "Useful extensions to python logging"
 authors = ["Sebastian Endres <dev@sedrubal.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "logging_utils_cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `logging_utils_cli-1.0.0/PKG-INFO` & `logging_utils_cli-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-utils-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Useful extensions to python logging
 License: MIT
 Author: Sebastian Endres
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

