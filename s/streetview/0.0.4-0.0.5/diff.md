# Comparing `tmp/streetview-0.0.4.tar.gz` & `tmp/streetview-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetview-0.0.4.tar", last modified: Tue Jun 13 16:39:43 2023, max compression
+gzip compressed data, was "streetview-0.0.5.tar", last modified: Thu Jun 15 07:46:16 2023, max compression
```

## Comparing `streetview-0.0.4.tar` & `streetview-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 16:39:26.000000 streetview-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-13 16:39:43.483541 streetview-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-13 16:39:26.000000 streetview-0.0.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:39:43.483541 streetview-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:39:26.000000 streetview-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.479541 streetview-0.0.4/streetview/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/streetview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 16:39:26.000000 streetview-0.0.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:46:16.427043 streetview-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 07:45:56.000000 streetview-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-15 07:46:16.427043 streetview-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-15 07:45:56.000000 streetview-0.0.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:46:16.427043 streetview-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-15 07:45:56.000000 streetview-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:46:16.427043 streetview-0.0.5/streetview/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 07:45:56.000000 streetview-0.0.5/streetview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-15 07:45:56.000000 streetview-0.0.5/streetview/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-15 07:45:56.000000 streetview-0.0.5/streetview/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-15 07:45:56.000000 streetview-0.0.5/streetview/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:46:16.427043 streetview-0.0.5/streetview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 07:46:16.000000 streetview-0.0.5/streetview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:46:16.427043 streetview-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-15 07:45:56.000000 streetview-0.0.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-15 07:45:56.000000 streetview-0.0.5/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-15 07:45:56.000000 streetview-0.0.5/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 07:45:56.000000 streetview-0.0.5/version.py
```

### Comparing `streetview-0.0.4/PKG-INFO` & `streetview-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.4
+Version: 0.0.5
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `streetview-0.0.4/readme.md` & `streetview-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `streetview-0.0.4/setup.py` & `streetview-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.4/streetview/api.py` & `streetview-0.0.5/streetview/api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.4/streetview/search.py` & `streetview-0.0.5/streetview/search.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.4/streetview.egg-info/PKG-INFO` & `streetview-0.0.5/streetview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.4
+Version: 0.0.5
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `streetview-0.0.4/tests/test_api.py` & `streetview-0.0.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.4/tests/test_search.py` & `streetview-0.0.5/tests/test_search.py`

 * *Files identical despite different names*

