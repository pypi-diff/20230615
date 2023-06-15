# Comparing `tmp/dagster-databricks-0.9.9.tar.gz` & `tmp/dagster-databricks-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-databricks-0.9.9.tar", last modified: Thu Sep 17 21:27:34 2020, max compression
+gzip compressed data, was "dist/dagster-databricks-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:32 2020, max compression
```

## Comparing `dagster-databricks-0.9.9.tar` & `dagster-databricks-0.9.9rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      193 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      626 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks/
--rw-r--r--   0 bobchen    (501) staff       (20)     1264 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    24423 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    11098 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/databricks.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14184 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/databricks_pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2241 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/databricks_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3238 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1332 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      626 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      808 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/dagster_databricks_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      293 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks_tests/test_databricks.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7543 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks_tests/test_pyspark.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3171 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/dagster_databricks_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:34.000000 dagster-databricks-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1146 2020-09-17 21:24:45.000000 dagster-databricks-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)      193 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1264 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    24423 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    11098 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    14184 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks_pyspark_step_launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2241 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/databricks_step_main.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3238 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1332 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      808 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      293 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_databricks.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7543 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_pyspark.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3171 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:32.000000 dagster-databricks-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1146 2020-09-17 21:04:59.000000 dagster-databricks-0.9.9rc1/setup.py
```

### Comparing `dagster-databricks-0.9.9/LICENSE` & `dagster-databricks-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/PKG-INFO` & `dagster-databricks-0.9.9rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-databricks
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Databricks-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-databricks
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-databricks-0.9.9/dagster_databricks/__init__.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/configs.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/databricks.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/databricks.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/databricks_pyspark_step_launcher.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/databricks_pyspark_step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/databricks_step_main.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/databricks_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/resources.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/solids.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks/types.py` & `dagster-databricks-0.9.9rc1/dagster_databricks/types.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks.egg-info/PKG-INFO` & `dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-databricks
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Databricks-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-databricks
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-databricks-0.9.9/dagster_databricks.egg-info/SOURCES.txt` & `dagster-databricks-0.9.9rc1/dagster_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks_tests/test_databricks.py` & `dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_databricks.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks_tests/test_pyspark.py` & `dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/dagster_databricks_tests/test_solids.py` & `dagster-databricks-0.9.9rc1/dagster_databricks_tests/test_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-databricks-0.9.9/setup.py` & `dagster-databricks-0.9.9rc1/setup.py`

 * *Files identical despite different names*

