# Comparing `tmp/enum_tools-0.9.0.tar.gz` & `tmp/enum_tools-0.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_tools-0.9.0.tar", last modified: Mon Jan 31 15:00:16 2022, max compression
+gzip compressed data, was "enum_tools-0.9.0.post1.tar", last modified: Thu Feb 10 07:52:00 2022, max compression
```

## Comparing `enum_tools-0.9.0.tar` & `enum_tools-0.9.0.post1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (121)     7936 2022-01-31 15:00:16.515481 enum_tools-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-31 15:00:16.471480 enum_tools-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5953 2022-01-31 15:00:16.471480 enum_tools-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-01-31 15:00:16.463480 enum_tools-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5367 2022-01-31 15:00:16.471480 enum_tools-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-01-31 14:59:38.738970 enum_tools-0.9.0/enum_tools/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6805 2022-01-31 14:59:38.738970 enum_tools-0.9.0/enum_tools/custom_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-01-31 14:59:38.742970 enum_tools-0.9.0/enum_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-31 14:59:38.738970 enum_tools-0.9.0/enum_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19348 2022-01-31 14:59:38.738970 enum_tools-0.9.0/enum_tools/autoenum.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-31 14:59:38.742970 enum_tools-0.9.0/enum_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10949 2022-01-31 14:59:38.742970 enum_tools-0.9.0/enum_tools/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-02-10 07:52:00.467005 enum_tools-0.9.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-10 07:52:00.475005 enum_tools-0.9.0.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-02-10 07:52:00.475005 enum_tools-0.9.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     7948 2022-02-10 07:52:00.619009 enum_tools-0.9.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-02-10 07:52:00.475005 enum_tools-0.9.0.post1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10949 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6805 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/custom_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19348 2022-02-10 07:51:10.925738 enum_tools-0.9.0.post1/enum_tools/autoenum.py
```

### Comparing `enum_tools-0.9.0/PKG-INFO` & `enum_tools-0.9.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-tools
-Version: 0.9.0
+Version: 0.9.0.post1
 Summary: Tools to expand Python's enum module.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: LGPL-3.0-or-later
 Keywords: documentation,enum,sphinx,sphinx-extension
 Home-page: https://github.com/domdfcoding/enum_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/enum_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/enum_tools
@@ -143,15 +143,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/enum_tools
 	:target: https://github.com/domdfcoding/enum_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/enum_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/enum_tools/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/enum_tools/v0.9.0.post1
 	:target: https://github.com/domdfcoding/enum_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/enum_tools
 	:target: https://github.com/domdfcoding/enum_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `enum_tools-0.9.0/README.rst` & `enum_tools-0.9.0.post1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/enum_tools
 	:target: https://github.com/domdfcoding/enum_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/enum_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/enum_tools/v0.9.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/enum_tools/v0.9.0.post1
 	:target: https://github.com/domdfcoding/enum_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/enum_tools
 	:target: https://github.com/domdfcoding/enum_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `enum_tools-0.9.0/LICENSE` & `enum_tools-0.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_tools-0.9.0/pyproject.toml` & `enum_tools-0.9.0.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "enum_tools"
-version = "0.9.0"
+version = "0.9.0.post1"
 description = "Tools to expand Python's enum module."
 readme = "README.rst"
 keywords = [ "documentation", "enum", "sphinx", "sphinx-extension",]
 dynamic = []
 dependencies = [ "pygments>=2.6.1", "typing-extensions>=3.7.4.3",]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `enum_tools-0.9.0/enum_tools/demo.py` & `enum_tools-0.9.0.post1/enum_tools/demo.py`

 * *Files identical despite different names*

### Comparing `enum_tools-0.9.0/enum_tools/custom_enums.py` & `enum_tools-0.9.0.post1/enum_tools/custom_enums.py`

 * *Files identical despite different names*

### Comparing `enum_tools-0.9.0/enum_tools/utils.py` & `enum_tools-0.9.0.post1/enum_tools/utils.py`

 * *Files identical despite different names*

### Comparing `enum_tools-0.9.0/enum_tools/__init__.py` & `enum_tools-0.9.0.post1/enum_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # this package
 from enum_tools.custom_enums import AutoNumberEnum, DuplicateFreeEnum, IntEnum, OrderedEnum, StrEnum
 from enum_tools.documentation import DocumentedEnum, document_enum, document_member
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "GNU Lesser General Public License v3 or later (LGPLv3+)"
-__version__: str = "0.9.0"
+__version__: str = "0.9.0.post1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"Enum",
 		"IntEnum",
 		"StrEnum",
 		"AutoNumberEnum",
```

### Comparing `enum_tools-0.9.0/enum_tools/autoenum.py` & `enum_tools-0.9.0.post1/enum_tools/autoenum.py`

 * *Files identical despite different names*

### Comparing `enum_tools-0.9.0/enum_tools/documentation.py` & `enum_tools-0.9.0.post1/enum_tools/documentation.py`

 * *Files identical despite different names*

