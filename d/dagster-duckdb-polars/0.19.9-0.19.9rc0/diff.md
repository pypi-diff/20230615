# Comparing `tmp/dagster-duckdb-polars-0.19.9.tar.gz` & `tmp/dagster-duckdb-polars-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.19.9.tar", last modified: Thu Jun  8 18:52:41 2023, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.19.9rc0.tar", last modified: Thu Jun  8 18:29:01 2023, max compression
```

## Comparing `dagster-duckdb-polars-0.19.9.tar` & `dagster-duckdb-polars-0.19.9rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:41.699681 dagster-duckdb-polars-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-08 18:52:41.699681 dagster-duckdb-polars-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:41.699681 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:41.699681 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:52:41.000000 dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:52:41.699681 dagster-duckdb-polars-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-08 18:43:17.000000 dagster-duckdb-polars-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.871264 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:29:01.000000 dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-08 18:29:01.875264 dagster-duckdb-polars-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-06-08 18:20:46.000000 dagster-duckdb-polars-0.19.9rc0/setup.py
```

### Comparing `dagster-duckdb-polars-0.19.9/LICENSE` & `dagster-duckdb-polars-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.19.9/PKG-INFO` & `dagster-duckdb-polars-0.19.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.19.9/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.19.9/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.19.9rc0/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.19.9/setup.py` & `dagster-duckdb-polars-0.19.9rc0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9",
-        "dagster-duckdb==0.19.9",
+        "dagster==1.3.9rc0",
+        "dagster-duckdb==0.19.9rc0",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

