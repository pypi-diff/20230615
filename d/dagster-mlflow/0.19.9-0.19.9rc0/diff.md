# Comparing `tmp/dagster-mlflow-0.19.9.tar.gz` & `tmp/dagster-mlflow-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.19.9.tar", last modified: Thu Jun  8 18:51:46 2023, max compression
+gzip compressed data, was "dagster-mlflow-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:31 2023, max compression
```

## Comparing `dagster-mlflow-0.19.9.tar` & `dagster-mlflow-0.19.9rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:46.182918 dagster-mlflow-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-08 18:51:46.182918 dagster-mlflow-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:46.178918 dagster-mlflow-0.19.9/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10800 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:46.182918 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:51:46.000000 dagster-mlflow-0.19.9/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:51:46.182918 dagster-mlflow-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-08 18:43:17.000000 dagster-mlflow-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.982865 dagster-mlflow-0.19.9rc0/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10800 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:31.982865 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:28:31.000000 dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:28:31.986865 dagster-mlflow-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-08 18:20:46.000000 dagster-mlflow-0.19.9rc0/setup.py
```

### Comparing `dagster-mlflow-0.19.9/LICENSE` & `dagster-mlflow-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.19.9/PKG-INFO` & `dagster-mlflow-0.19.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mlflow-0.19.9/dagster_mlflow/hooks.py` & `dagster-mlflow-0.19.9rc0/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.19.9/dagster_mlflow/resources.py` & `dagster-mlflow-0.19.9rc0/dagster_mlflow/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.19.9/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.19.9rc0/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mlflow-0.19.9/setup.py` & `dagster-mlflow-0.19.9rc0/setup.py`

 * *Files identical despite different names*

