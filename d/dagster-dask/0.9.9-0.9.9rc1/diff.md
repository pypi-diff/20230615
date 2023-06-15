# Comparing `tmp/dagster-dask-0.9.9.tar.gz` & `tmp/dagster-dask-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-dask-0.9.9.tar", last modified: Thu Sep 17 21:28:34 2020, max compression
+gzip compressed data, was "dist/dagster-dask-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:46 2020, max compression
```

## Comparing `dagster-dask-0.9.9.tar` & `dagster-dask-0.9.9rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      649 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      122 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/dagster_dask/
--rw-r--r--   0 bobchen    (501) staff       (20)      278 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    18787 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask/data_frame.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12368 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/dagster_dask.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      649 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      578 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      136 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       32 2020-09-17 21:28:33.000000 dagster-dask-0.9.9/dagster_dask.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/dagster_dask_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2962 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/test_data_frame.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3429 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/test_execute.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2373 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/test_graphql.py
--rw-r--r--   0 bobchen    (501) staff       (20)      350 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/test_resource_tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)       90 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/dagster_dask_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:34.000000 dagster-dask-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1327 2020-09-17 21:24:45.000000 dagster-dask-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      652 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      122 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask/
+-rw-r--r--   0 bobchen    (501) staff       (20)      278 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    18787 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/data_frame.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    12368 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/executor.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      652 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      578 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)      136 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       32 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2962 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_data_frame.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3429 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_execute.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2373 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_graphql.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      350 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_resource_tags.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       90 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/dagster_dask_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:46.000000 dagster-dask-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1327 2020-09-17 21:04:59.000000 dagster-dask-0.9.9rc1/setup.py
```

### Comparing `dagster-dask-0.9.9/LICENSE` & `dagster-dask-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/PKG-INFO` & `dagster-dask-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-dask
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for using Dask as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dask
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: yarn
 Provides-Extra: kube
+Provides-Extra: yarn
 Provides-Extra: pbs
```

### Comparing `dagster-dask-0.9.9/dagster_dask/data_frame.py` & `dagster-dask-0.9.9rc1/dagster_dask/data_frame.py`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/dagster_dask/executor.py` & `dagster-dask-0.9.9rc1/dagster_dask/executor.py`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/dagster_dask.egg-info/PKG-INFO` & `dagster-dask-0.9.9rc1/dagster_dask.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dagster-dask
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for using Dask as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-dask
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Provides-Extra: yarn
 Provides-Extra: kube
+Provides-Extra: yarn
 Provides-Extra: pbs
```

### Comparing `dagster-dask-0.9.9/dagster_dask.egg-info/SOURCES.txt` & `dagster-dask-0.9.9rc1/dagster_dask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/dagster_dask_tests/test_data_frame.py` & `dagster-dask-0.9.9rc1/dagster_dask_tests/test_data_frame.py`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/dagster_dask_tests/test_execute.py` & `dagster-dask-0.9.9rc1/dagster_dask_tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/dagster_dask_tests/test_graphql.py` & `dagster-dask-0.9.9rc1/dagster_dask_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `dagster-dask-0.9.9/setup.py` & `dagster-dask-0.9.9rc1/setup.py`

 * *Files identical despite different names*

