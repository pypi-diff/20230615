# Comparing `tmp/e-data-1.1.4.tar.gz` & `tmp/e-data-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-data-1.1.4.tar", last modified: Mon Jun 12 16:37:40 2023, max compression
+gzip compressed data, was "e-data-1.1.5.tar", last modified: Thu Jun 15 08:58:46 2023, max compression
```

## Comparing `e-data-1.1.4.tar` & `e-data-1.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.095496 e-data-1.1.4/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35149 2023-06-11 10:01:58.000000 e-data-1.1.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.4/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:37:40.095496 e-data-1.1.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.4/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.059496 e-data-1.1.4/e_data.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      507 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.071496 e-data-1.1.4/edata/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.4/edata/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.079496 e-data-1.1.4/edata/connectors/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 12:18:54.000000 e-data-1.1.4/edata/connectors/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15204 2023-06-12 15:54:38.000000 e-data-1.1.4/edata/connectors/datadis.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1990 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/connectors/redata.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3828 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/definitions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22473 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/helpers.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.091496 e-data-1.1.4/edata/processors/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.4/edata/processors/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6287 2023-06-12 16:29:42.000000 e-data-1.1.4/edata/processors/billing.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2385 2023-06-12 16:33:12.000000 e-data-1.1.4/edata/processors/consumption.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1334 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/maximeter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5155 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-06-12 16:37:40.099496 e-data-1.1.4/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4261 2023-06-12 16:36:36.000000 e-data-1.1.4/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-15 08:58:46.324172 e-data-1.1.5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    35149 2022-09-06 14:38:03.000000 e-data-1.1.5/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      193 2022-09-06 14:38:03.000000 e-data-1.1.5/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-15 08:58:46.324172 e-data-1.1.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4860 2023-02-19 09:31:45.000000 e-data-1.1.5/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-15 08:58:46.324172 e-data-1.1.5/e_data.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-15 08:58:46.000000 e-data-1.1.5/e_data.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      507 2023-06-15 08:58:46.000000 e-data-1.1.5/e_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-15 08:58:46.000000 e-data-1.1.5/e_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2023-06-15 08:58:46.000000 e-data-1.1.5/e_data.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-06-15 08:58:46.000000 e-data-1.1.5/e_data.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-15 08:58:46.324172 e-data-1.1.5/edata/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-09-06 14:38:03.000000 e-data-1.1.5/edata/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-15 08:58:46.324172 e-data-1.1.5/edata/connectors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-11-23 11:56:04.000000 e-data-1.1.5/edata/connectors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15204 2023-06-12 10:44:05.000000 e-data-1.1.5/edata/connectors/datadis.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1990 2023-02-19 10:47:16.000000 e-data-1.1.5/edata/connectors/redata.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3828 2023-02-19 10:47:16.000000 e-data-1.1.5/edata/definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22473 2023-06-12 10:44:05.000000 e-data-1.1.5/edata/helpers.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-15 08:58:46.324172 e-data-1.1.5/edata/processors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2022-11-23 11:56:04.000000 e-data-1.1.5/edata/processors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-02-19 10:47:16.000000 e-data-1.1.5/edata/processors/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6287 2023-06-15 08:53:19.000000 e-data-1.1.5/edata/processors/billing.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2385 2023-06-15 08:53:19.000000 e-data-1.1.5/edata/processors/consumption.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1334 2022-11-25 13:14:21.000000 e-data-1.1.5/edata/processors/maximeter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5155 2022-12-03 12:56:05.000000 e-data-1.1.5/edata/processors/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-06-15 08:58:46.324172 e-data-1.1.5/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4261 2023-06-15 08:55:27.000000 e-data-1.1.5/setup.py
```

### Comparing `e-data-1.1.4/LICENSE` & `e-data-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/PKG-INFO` & `e-data-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `e-data-1.1.4/README.md` & `e-data-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/e_data.egg-info/PKG-INFO` & `e-data-1.1.5/e_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `e-data-1.1.4/edata/connectors/datadis.py` & `e-data-1.1.5/edata/connectors/datadis.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/connectors/redata.py` & `e-data-1.1.5/edata/connectors/redata.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/definitions.py` & `e-data-1.1.5/edata/definitions.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/helpers.py` & `e-data-1.1.5/edata/helpers.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/processors/base.py` & `e-data-1.1.5/edata/processors/base.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/processors/billing.py` & `e-data-1.1.5/edata/processors/billing.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/processors/consumption.py` & `e-data-1.1.5/edata/processors/consumption.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/processors/maximeter.py` & `e-data-1.1.5/edata/processors/maximeter.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/edata/processors/utils.py` & `e-data-1.1.5/edata/processors/utils.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.4/setup.py` & `e-data-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 DESCRIPTION = (
     "Python library for managing spanish energy data from various web providers"
 )
 URL = "https://github.com/uvejota/python-edata"
 EMAIL = "vmayorg@outlook.es"
 AUTHOR = "VMG"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.1.4"
+VERSION = "1.1.5"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "dateparser>=1.1.2",
     "freezegun>=1.2.1",
     "holidays>=0.14.2",
-    "pandas>=2.0.2",
+    "pandas>=1.4.3",
     "pytest>=7.1.2",
     "python_dateutil>=2.8.2",
     "requests>=2.28.1",
 ]
 
 # What packages are optional?
 EXTRAS = {
```

