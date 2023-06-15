# Comparing `tmp/dagster-snowflake-pyspark-0.19.9.tar.gz` & `tmp/dagster-snowflake-pyspark-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pyspark-0.19.9.tar", last modified: Thu Jun  8 18:52:12 2023, max compression
+gzip compressed data, was "dagster-snowflake-pyspark-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:06 2023, max compression
```

## Comparing `dagster-snowflake-pyspark-0.19.9.tar` & `dagster-snowflake-pyspark-0.19.9rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:12.211286 dagster-snowflake-pyspark-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:52:12.211286 dagster-snowflake-pyspark-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:12.211286 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)     9162 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:12.211286 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:52:12.000000 dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:52:12.215287 dagster-snowflake-pyspark-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 18:43:18.000000 dagster-snowflake-pyspark-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9162 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:29:06.000000 dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 18:29:06.655329 dagster-snowflake-pyspark-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-08 18:20:46.000000 dagster-snowflake-pyspark-0.19.9rc0/setup.py
```

### Comparing `dagster-snowflake-pyspark-0.19.9/LICENSE` & `dagster-snowflake-pyspark-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.19.9/PKG-INFO` & `dagster-snowflake-pyspark-0.19.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py` & `dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.19.9/dagster_snowflake_pyspark.egg-info/PKG-INFO` & `dagster-snowflake-pyspark-0.19.9rc0/dagster_snowflake_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-snowflake-pyspark-0.19.9/setup.py` & `dagster-snowflake-pyspark-0.19.9rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.9",
-        "dagster-snowflake==0.19.9",
+        "dagster==1.3.9rc0",
+        "dagster-snowflake==0.19.9rc0",
         "pyspark",
         "requests",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
 )
```

