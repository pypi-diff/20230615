# Comparing `tmp/remlalib-1.0.2.tar.gz` & `tmp/remlalib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remlalib-1.0.2.tar", last modified: Mon Jun  5 10:14:41 2023, max compression
+gzip compressed data, was "remlalib-1.1.2.tar", last modified: Thu Jun 15 20:09:50 2023, max compression
```

## Comparing `remlalib-1.0.2.tar` & `remlalib-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-05 10:14:27.000000 remlalib-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 10:14:41.439064 remlalib-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 10:14:27.000000 remlalib-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/remlalib/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-05 10:14:27.000000 remlalib-1.0.2/remlalib/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:14:41.439064 remlalib-1.0.2/remlalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 10:14:41.000000 remlalib-1.0.2/remlalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 10:14:41.439064 remlalib-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 10:14:27.000000 remlalib-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:09:50.619627 remlalib-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 20:09:32.000000 remlalib-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 20:09:50.619627 remlalib-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 20:09:32.000000 remlalib-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:09:50.619627 remlalib-1.1.2/remlalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:09:32.000000 remlalib-1.1.2/remlalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 20:09:33.000000 remlalib-1.1.2/remlalib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-15 20:09:32.000000 remlalib-1.1.2/remlalib/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 20:09:32.000000 remlalib-1.1.2/remlalib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:09:50.619627 remlalib-1.1.2/remlalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 20:09:50.000000 remlalib-1.1.2/remlalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 20:09:50.000000 remlalib-1.1.2/remlalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:09:50.000000 remlalib-1.1.2/remlalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 20:09:50.000000 remlalib-1.1.2/remlalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 20:09:50.000000 remlalib-1.1.2/remlalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 20:09:50.623628 remlalib-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 20:09:32.000000 remlalib-1.1.2/setup.py
```

### Comparing `remlalib-1.0.2/LICENSE.txt` & `remlalib-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remlalib-1.0.2/PKG-INFO` & `remlalib-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.0.2
+Version: 1.1.2
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.0.2/remlalib.egg-info/PKG-INFO` & `remlalib-1.1.2/remlalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.0.2
+Version: 1.1.2
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.0.2/setup.py` & `remlalib-1.1.2/setup.py`

 * *Files identical despite different names*

