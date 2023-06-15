# Comparing `tmp/dagster-pyspark-0.9.9.tar.gz` & `tmp/dagster-pyspark-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-pyspark-0.9.9.tar", last modified: Thu Sep 17 21:27:52 2020, max compression
+gzip compressed data, was "dist/dagster-pyspark-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:36 2020, max compression
```

## Comparing `dagster-pyspark-0.9.9.tar` & `dagster-pyspark-0.9.9rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      539 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark/
--rw-r--r--   0 bobchen    (501) staff       (20)      283 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1151 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)    50077 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      539 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      562 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      107 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/dagster_pyspark_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      960 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4166 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark_tests/test_types.py
--rw-r--r--   0 bobchen    (501) staff       (20)       85 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/dagster_pyspark_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:52.000000 dagster-pyspark-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1201 2020-09-17 21:24:45.000000 dagster-pyspark-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      542 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/
+-rw-r--r--   0 bobchen    (501) staff       (20)      283 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1151 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    50077 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      542 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      562 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)      107 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      960 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4166 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       85 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:36.000000 dagster-pyspark-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1201 2020-09-17 21:04:59.000000 dagster-pyspark-0.9.9rc1/setup.py
```

### Comparing `dagster-pyspark-0.9.9/LICENSE` & `dagster-pyspark-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/PKG-INFO` & `dagster-pyspark-0.9.9rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-pyspark
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for PySpark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-framework/pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark/resources.py` & `dagster-pyspark-0.9.9rc1/dagster_pyspark/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark/types.py` & `dagster-pyspark-0.9.9rc1/dagster_pyspark/types.py`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark/utils.py` & `dagster-pyspark-0.9.9rc1/dagster_pyspark/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark.egg-info/PKG-INFO` & `dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-pyspark
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for PySpark Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-framework/pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark.egg-info/SOURCES.txt` & `dagster-pyspark-0.9.9rc1/dagster_pyspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark_tests/test_resources.py` & `dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/dagster_pyspark_tests/test_types.py` & `dagster-pyspark-0.9.9rc1/dagster_pyspark_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dagster-pyspark-0.9.9/setup.py` & `dagster-pyspark-0.9.9rc1/setup.py`

 * *Files identical despite different names*

