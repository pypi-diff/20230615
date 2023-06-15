# Comparing `tmp/dagster-snowflake-0.9.9.tar.gz` & `tmp/dagster-snowflake-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-snowflake-0.9.9.tar", last modified: Thu Sep 17 21:28:37 2020, max compression
+gzip compressed data, was "dist/dagster-snowflake-0.9.9rc1.tar", last modified: Thu Sep 17 21:09:06 2020, max compression
```

## Comparing `dagster-snowflake-0.9.9.tar` & `dagster-snowflake-0.9.9rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      595 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      137 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake/
--rw-r--r--   0 bobchen    (501) staff       (20)      311 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4573 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5881 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)      504 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      595 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3080 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1215 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)      424 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/dagster_snowflake_tests/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:37.000000 dagster-snowflake-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:24:45.000000 dagster-snowflake-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      137 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/
+-rw-r--r--   0 bobchen    (501) staff       (20)      311 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4573 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5881 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      504 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       42 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3080 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1215 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      424 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:09:06.000000 dagster-snowflake-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:04:59.000000 dagster-snowflake-0.9.9rc1/setup.py
```

### Comparing `dagster-snowflake-0.9.9/LICENSE` & `dagster-snowflake-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/PKG-INFO` & `dagster-snowflake-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-snowflake
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Snowflake Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake/configs.py` & `dagster-snowflake-0.9.9rc1/dagster_snowflake/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake/resources.py` & `dagster-snowflake-0.9.9rc1/dagster_snowflake/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake.egg-info/PKG-INFO` & `dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-snowflake
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Snowflake Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake.egg-info/SOURCES.txt` & `dagster-snowflake-0.9.9rc1/dagster_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake_tests/test_resources.py` & `dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/dagster_snowflake_tests/test_solids.py` & `dagster-snowflake-0.9.9rc1/dagster_snowflake_tests/test_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-0.9.9/setup.py` & `dagster-snowflake-0.9.9rc1/setup.py`

 * *Files identical despite different names*

