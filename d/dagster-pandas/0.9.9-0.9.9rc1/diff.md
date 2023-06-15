# Comparing `tmp/dagster-pandas-0.9.9.tar.gz` & `tmp/dagster-pandas-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-pandas-0.9.9.tar", last modified: Thu Sep 17 21:28:47 2020, max compression
+gzip compressed data, was "dist/dagster-pandas-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:25 2020, max compression
```

## Comparing `dagster-pandas-0.9.9.tar` & `dagster-pandas-0.9.9rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       56 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      843 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas/
--rw-r--r--   0 bobchen    (501) staff       (20)     1464 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    49516 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/constraints.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13352 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/data_frame.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas/examples/
--rw-r--r--   0 bobchen    (501) staff       (20)     1727 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/env.yaml
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/environments/
--rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_prod.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       88 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_test.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)      111 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_prod.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)     1543 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/pipeline.py
--rw-r--r--   0 bobchen    (501) staff       (20)      124 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/solids.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)       77 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/examples/repository.yaml
--rw-r--r--   0 bobchen    (501) staff       (20)    18338 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/validation.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      843 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1198 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas_tests/
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/dagster_pandas_tests/pandas_hello_world/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas_tests/pandas_hello_world/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2830 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:47.000000 dagster-pandas-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1462 2020-09-17 21:24:45.000000 dagster-pandas-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       56 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      846 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1464 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    49516 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/constraints.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    13352 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/data_frame.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1727 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/env.yaml
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/
+-rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_prod.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)       88 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/pandas_hello_world_test.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)      111 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_prod.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/environments/papermill_pandas_hello_world_test.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)     1543 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/pipeline.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      124 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/solids.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)       77 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/examples/repository.yaml
+-rw-r--r--   0 bobchen    (501) staff       (20)    18338 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/validation.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      846 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     1198 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2830 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:25.000000 dagster-pandas-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1462 2020-09-17 21:04:59.000000 dagster-pandas-0.9.9rc1/setup.py
```

### Comparing `dagster-pandas-0.9.9/LICENSE` & `dagster-pandas-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/PKG-INFO` & `dagster-pandas-0.9.9rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandas
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Utilities and examples for working with pandas and dagster, an opinionated framework for expressing data pipelines
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: # dagster-pandas
```

### Comparing `dagster-pandas-0.9.9/dagster_pandas/__init__.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas/constraints.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/constraints.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas/data_frame.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/data_frame.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas/examples/__init__.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas/examples/pandas_hello_world/pipeline.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/examples/pandas_hello_world/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas/validation.py` & `dagster-pandas-0.9.9rc1/dagster_pandas/validation.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas.egg-info/PKG-INFO` & `dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandas
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Utilities and examples for working with pandas and dagster, an opinionated framework for expressing data pipelines
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: # dagster-pandas
```

### Comparing `dagster-pandas-0.9.9/dagster_pandas.egg-info/SOURCES.txt` & `dagster-pandas-0.9.9rc1/dagster_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py` & `dagster-pandas-0.9.9rc1/dagster_pandas_tests/pandas_hello_world/test_pandas_hello_world.py`

 * *Files identical despite different names*

### Comparing `dagster-pandas-0.9.9/setup.py` & `dagster-pandas-0.9.9rc1/setup.py`

 * *Files identical despite different names*

