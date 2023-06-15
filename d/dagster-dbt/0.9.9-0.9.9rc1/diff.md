# Comparing `tmp/dagster-dbt-0.9.9.tar.gz` & `tmp/dagster-dbt-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-dbt-0.9.9.tar", last modified: Thu Sep 17 21:27:18 2020, max compression
+gzip compressed data, was "dist/dagster-dbt-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:46 2020, max compression
```

## Comparing `dagster-dbt-0.9.9.tar` & `dagster-dbt-0.9.9rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)      511 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      118 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/dagster_dbt/
--rw-r--r--   0 bobchen    (501) staff       (20)     1134 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8550 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)    28581 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3950 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3720 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      511 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      595 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:27:17.000000 dagster-dbt-0.9.9/dagster_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/dagster_dbt_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    10353 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3661 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4771 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/test_solids_i.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9315 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/test_solids_ii.py
--rw-r--r--   0 bobchen    (501) staff       (20)      458 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/dagster_dbt_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:27:18.000000 dagster-dbt-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1100 2020-09-17 21:24:45.000000 dagster-dbt-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)      514 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      118 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1134 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8550 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    28581 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3950 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3720 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      514 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      595 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    10353 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3661 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4771 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_i.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     9315 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_ii.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      458 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:07:46.000000 dagster-dbt-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1100 2020-09-17 21:04:59.000000 dagster-dbt-0.9.9rc1/setup.py
```

### Comparing `dagster-dbt-0.9.9/dagster_dbt/__init__.py` & `dagster-dbt-0.9.9rc1/dagster_dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt/resources.py` & `dagster-dbt-0.9.9rc1/dagster_dbt/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt/solids.py` & `dagster-dbt-0.9.9rc1/dagster_dbt/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt/types.py` & `dagster-dbt-0.9.9rc1/dagster_dbt/types.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt/utils.py` & `dagster-dbt-0.9.9rc1/dagster_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt.egg-info/SOURCES.txt` & `dagster-dbt-0.9.9rc1/dagster_dbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt_tests/conftest.py` & `dagster-dbt-0.9.9rc1/dagster_dbt_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt_tests/test_resources.py` & `dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt_tests/test_solids_i.py` & `dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_i.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/dagster_dbt_tests/test_solids_ii.py` & `dagster-dbt-0.9.9rc1/dagster_dbt_tests/test_solids_ii.py`

 * *Files identical despite different names*

### Comparing `dagster-dbt-0.9.9/setup.py` & `dagster-dbt-0.9.9rc1/setup.py`

 * *Files identical despite different names*

