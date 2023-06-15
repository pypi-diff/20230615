# Comparing `tmp/fudan_utils-0.1.7.tar.gz` & `tmp/fudan_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudan_utils-0.1.7.tar", max compression
+gzip compressed data, was "fudan_utils-0.1.8.tar", max compression
```

## Comparing `fudan_utils-0.1.7.tar` & `fudan_utils-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1771 2023-06-15 06:53:43.292562 fudan_utils-0.1.7/README.md
--rw-r--r--   0        0        0       21 2023-06-15 07:29:47.603999 fudan_utils-0.1.7/fudan_utils/__init__.py
--rw-r--r--   0        0        0       77 2023-06-15 06:07:40.832259 fudan_utils-0.1.7/fudan_utils/config.py
--rw-r--r--   0        0        0     7703 2023-06-15 06:26:16.496167 fudan_utils-0.1.7/fudan_utils/fudan.py
--rwxr-xr-x   0        0        0     1594 2023-06-15 06:51:44.415471 fudan_utils-0.1.7/fudan_utils/fudan_grades.py
--rw-r--r--   0        0        0      682 2023-06-15 06:50:32.231301 fudan_utils-0.1.7/fudan_utils/utils.py
--rw-r--r--   0        0        0      970 2023-06-15 07:29:47.603552 fudan_utils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 fudan_utils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1771 2023-06-15 06:53:43.292562 fudan_utils-0.1.8/README.md
+-rw-r--r--   0        0        0       21 2023-06-15 07:34:34.945116 fudan_utils-0.1.8/fudan_utils/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-15 06:07:40.832259 fudan_utils-0.1.8/fudan_utils/config.py
+-rw-r--r--   0        0        0     7703 2023-06-15 06:26:16.496167 fudan_utils-0.1.8/fudan_utils/fudan.py
+-rwxr-xr-x   0        0        0     1594 2023-06-15 06:51:44.415471 fudan_utils-0.1.8/fudan_utils/fudan_grades.py
+-rw-r--r--   0        0        0      682 2023-06-15 06:50:32.231301 fudan_utils-0.1.8/fudan_utils/utils.py
+-rw-r--r--   0        0        0      969 2023-06-15 07:34:34.944440 fudan_utils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 fudan_utils-0.1.8/PKG-INFO
```

### Comparing `fudan_utils-0.1.7/README.md` & `fudan_utils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.7/fudan_utils/fudan.py` & `fudan_utils-0.1.8/fudan_utils/fudan.py`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.7/fudan_utils/fudan_grades.py` & `fudan_utils-0.1.8/fudan_utils/fudan_grades.py`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.7/fudan_utils/utils.py` & `fudan_utils-0.1.8/fudan_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fudan_utils-0.1.7/pyproject.toml` & `fudan_utils-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fudan-utils"
-version = "0.1.7"
+version = "0.1.8"
 description = "Fudan UIS Login Utilities and More"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "fudan_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/fudan-utils"
 repository = "https://github.com/tddschn/fudan-utils"
@@ -13,15 +13,15 @@
 [tool.poetry.scripts]
 fudan-grades = "fudan_utils.fudan_grades:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/fudan-utils/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <4.0"
+python = ">=3.8, <4.0"
 bs4 = { version = "^0.0.1", extras = ["jwfw"] }
 requests = "^2.31.0"
 tabulate = { version = "^0.9.0", extras = ["jwfw"] }
 wcwidth = { version = "^0.2.6", extras = ["jwfw"] }  # cjk support
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fudan_utils-0.1.7/PKG-INFO` & `fudan_utils-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: fudan-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Fudan UIS Login Utilities and More
 Home-page: https://github.com/tddschn/fudan-utils
 License: MIT
 Keywords: Fudan University
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: bs4[jwfw] (>=0.0.1,<0.0.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate[jwfw] (>=0.9.0,<0.10.0)
 Requires-Dist: wcwidth[jwfw] (>=0.2.6,<0.3.0)
```

