# Comparing `tmp/dagster-spark-0.9.9.tar.gz` & `tmp/dagster-spark-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-spark-0.9.9.tar", last modified: Thu Sep 17 21:27:42 2020, max compression
+gzip compressed data, was "dist/dagster-spark-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:39 2020, max compression
```

## Comparing `dagster-spark-0.9.9.tar` & `dagster-spark-0.9.9rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/dagster_spark/
--rw-r--r--   0 bobchen    (501) staff       (20)      508 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2631 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)   145666 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/configs_spark.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1961 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)      967 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)      286 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2482 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/dagster_spark.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:27:41.000000 dagster-spark-0.9.9/dagster_spark.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      643 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/dagster_spark.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:41.000000 dagster-spark-0.9.9/dagster_spark.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:41.000000 dagster-spark-0.9.9/dagster_spark.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:27:41.000000 dagster-spark-0.9.9/dagster_spark.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:27:41.000000 dagster-spark-0.9.9/dagster_spark.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/dagster_spark_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2076 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark_tests/test_error.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1636 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2740 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       83 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/dagster_spark_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:42.000000 dagster-spark-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1026 2020-09-17 21:24:45.000000 dagster-spark-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      586 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark/
+-rw-r--r--   0 bobchen    (501) staff       (20)      508 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2631 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)   145666 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/configs_spark.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1961 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      967 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      286 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2482 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      586 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      643 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2076 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/test_error.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1636 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/test_solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2740 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       83 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/dagster_spark_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:39.000000 dagster-spark-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1026 2020-09-17 21:04:59.000000 dagster-spark-0.9.9rc1/setup.py
```

### Comparing `dagster-spark-0.9.9/LICENSE` & `dagster-spark-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/PKG-INFO` & `dagster-spark-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-spark
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Spark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-spark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-spark-0.9.9/dagster_spark/configs.py` & `dagster-spark-0.9.9rc1/dagster_spark/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark/configs_spark.py` & `dagster-spark-0.9.9rc1/dagster_spark/configs_spark.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark/resources.py` & `dagster-spark-0.9.9rc1/dagster_spark/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark/solids.py` & `dagster-spark-0.9.9rc1/dagster_spark/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark/utils.py` & `dagster-spark-0.9.9rc1/dagster_spark/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark.egg-info/PKG-INFO` & `dagster-spark-0.9.9rc1/dagster_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-spark
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Spark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-spark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-spark-0.9.9/dagster_spark.egg-info/SOURCES.txt` & `dagster-spark-0.9.9rc1/dagster_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark_tests/test_error.py` & `dagster-spark-0.9.9rc1/dagster_spark_tests/test_error.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark_tests/test_solids.py` & `dagster-spark-0.9.9rc1/dagster_spark_tests/test_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/dagster_spark_tests/test_utils.py` & `dagster-spark-0.9.9rc1/dagster_spark_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-spark-0.9.9/setup.py` & `dagster-spark-0.9.9rc1/setup.py`

 * *Files identical despite different names*

