# Comparing `tmp/dagster-duckdb-pyspark-0.19.9.tar.gz` & `tmp/dagster-duckdb-pyspark-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.19.9.tar", last modified: Thu Jun  8 18:53:25 2023, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:36 2023, max compression
```

## Comparing `dagster-duckdb-pyspark-0.19.9.tar` & `dagster-duckdb-pyspark-0.19.9rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:25.356295 dagster-duckdb-pyspark-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      637 2023-06-08 18:53:25.356295 dagster-duckdb-pyspark-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:25.352295 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7500 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:53:25.356295 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      637 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:53:25.000000 dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-08 18:53:25.356295 dagster-duckdb-pyspark-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1549 2023-06-08 18:43:17.000000 dagster-duckdb-pyspark-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.246923 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:36.254923 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:28:36.000000 dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-08 18:28:36.258923 dagster-duckdb-pyspark-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-08 18:20:46.000000 dagster-duckdb-pyspark-0.19.9rc0/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.19.9/LICENSE` & `dagster-duckdb-pyspark-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.19.9/PKG-INFO` & `dagster-duckdb-pyspark-0.19.9rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.19.9/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.19.9rc0/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pyspark-0.19.9/setup.py` & `dagster-duckdb-pyspark-0.19.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9",
-        "dagster-duckdb==0.19.9",
+        "dagster==1.3.9rc0",
+        "dagster-duckdb==0.19.9rc0",
         # Pyspark 2.x is incompatible with Python 3.8+
         'pyspark>=3.0.0; python_version >= "3.8"',
         'pyspark>=2.0.2; python_version < "3.8"',
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     zip_safe=False,
 )
```

