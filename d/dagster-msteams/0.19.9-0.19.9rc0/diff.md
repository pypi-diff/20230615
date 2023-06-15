# Comparing `tmp/dagster-msteams-0.19.9.tar.gz` & `tmp/dagster-msteams-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-msteams-0.19.9.tar", last modified: Thu Jun  8 18:53:28 2023, max compression
+gzip compressed data, was "dagster-msteams-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:39 2023, max compression
```

## Comparing `dagster-msteams-0.19.9.tar` & `dagster-msteams-0.19.9rc0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:28.980346 dagster-msteams-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-08 18:53:28.980346 dagster-msteams-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:28.980346 dagster-msteams-0.19.9/dagster_msteams/
--rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/__init__.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/card.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/client.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/py.typed
--rw-r--r--   0 root         (0) root         (0)     3553 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/resources.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/sensors.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/dagster_msteams/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:28.980346 dagster-msteams-0.19.9/dagster_msteams.egg-info/
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:53:28.000000 dagster-msteams-0.19.9/dagster_msteams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:53:28.980346 dagster-msteams-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1163 2023-06-08 18:43:17.000000 dagster-msteams-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/dagster_msteams/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/card.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/client.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3553 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/resources.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/dagster_msteams/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:28:39.000000 dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:28:39.862958 dagster-msteams-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-06-08 18:20:46.000000 dagster-msteams-0.19.9rc0/setup.py
```

### Comparing `dagster-msteams-0.19.9/LICENSE` & `dagster-msteams-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/PKG-INFO` & `dagster-msteams-0.19.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-msteams-0.19.9/dagster_msteams/card.py` & `dagster-msteams-0.19.9rc0/dagster_msteams/card.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/dagster_msteams/client.py` & `dagster-msteams-0.19.9rc0/dagster_msteams/client.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/dagster_msteams/hooks.py` & `dagster-msteams-0.19.9rc0/dagster_msteams/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/dagster_msteams/resources.py` & `dagster-msteams-0.19.9rc0/dagster_msteams/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/dagster_msteams/sensors.py` & `dagster-msteams-0.19.9rc0/dagster_msteams/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-msteams-0.19.9/dagster_msteams.egg-info/PKG-INFO` & `dagster-msteams-0.19.9rc0/dagster_msteams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-msteams
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: A Microsoft Teams client resource for posting to Microsoft Teams
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-msteams
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-msteams-0.19.9/setup.py` & `dagster-msteams-0.19.9rc0/setup.py`

 * *Files identical despite different names*

