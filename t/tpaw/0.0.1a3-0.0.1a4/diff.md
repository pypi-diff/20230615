# Comparing `tmp/tpaw-0.0.1a3.tar.gz` & `tmp/tpaw-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpaw-0.0.1a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tpaw-0.0.1a4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tpaw-0.0.1a3.tar` & `tpaw-0.0.1a4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      149 2023-06-14 07:58:32.698840 tpaw-0.0.1a3/.flake8
--rw-r--r--   0        0        0      993 2023-06-14 08:04:29.469030 tpaw-0.0.1a3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     3078 2023-06-14 03:45:27.697084 tpaw-0.0.1a3/.gitignore
--rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a3/LICENSE
--rw-r--r--   0        0        0      524 2023-06-14 08:15:37.593983 tpaw-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 03:27:30.402948 tpaw-0.0.1a3/tests/__init__.py
--rw-r--r--   0        0        0    17029 2023-06-14 04:07:11.683947 tpaw-0.0.1a3/tests/data/groups.html
--rw-r--r--   0        0        0    35218 2023-06-14 06:34:57.679137 tpaw-0.0.1a3/tests/data/slash_new.html
--rw-r--r--   0        0        0     1767 2023-06-14 07:41:59.421902 tpaw-0.0.1a3/tests/test_tpaw.py
--rw-r--r--   0        0        0     6358 2023-06-14 08:16:01.054736 tpaw-0.0.1a3/tpaw.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 tpaw-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      149 2023-06-14 07:58:32.698840 tpaw-0.0.1a4/.flake8
+-rw-r--r--   0        0        0      993 2023-06-14 08:04:29.469030 tpaw-0.0.1a4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     3078 2023-06-14 03:45:27.697084 tpaw-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0      524 2023-06-14 08:15:37.593983 tpaw-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 03:27:30.402948 tpaw-0.0.1a4/tests/__init__.py
+-rw-r--r--   0        0        0    17029 2023-06-14 04:07:11.683947 tpaw-0.0.1a4/tests/data/groups.html
+-rw-r--r--   0        0        0    35218 2023-06-14 06:34:57.679137 tpaw-0.0.1a4/tests/data/slash_new.html
+-rw-r--r--   0        0        0     1767 2023-06-14 07:41:59.421902 tpaw-0.0.1a4/tests/test_tpaw.py
+-rw-r--r--   0        0        0     6358 2023-06-15 02:14:04.424547 tpaw-0.0.1a4/tpaw/__init__.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 tpaw-0.0.1a4/PKG-INFO
```

### Comparing `tpaw-0.0.1a3/.github/workflows/python-package.yml` & `tpaw-0.0.1a4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/.gitignore` & `tpaw-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/LICENSE` & `tpaw-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/pyproject.toml` & `tpaw-0.0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/tests/data/groups.html` & `tpaw-0.0.1a4/tests/data/groups.html`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/tests/data/slash_new.html` & `tpaw-0.0.1a4/tests/data/slash_new.html`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/tests/test_tpaw.py` & `tpaw-0.0.1a4/tests/test_tpaw.py`

 * *Files identical despite different names*

### Comparing `tpaw-0.0.1a3/tpaw.py` & `tpaw-0.0.1a4/tpaw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tildes Python API Wrapper."""
 
 from datetime import datetime, timedelta
 
 import lxml.html
 import requests
 
-__version__ = "0.0.1a3"
+__version__ = "0.0.1a4"
 
 
 def one_class(element, class_selector, /):
     collection = element.find_class(class_selector)
     if len(collection) != 1:
         raise TPAWError(
             "Expected to find exactly 1 element", collection=collection, element=element
```

