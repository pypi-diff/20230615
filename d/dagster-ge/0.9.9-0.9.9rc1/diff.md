# Comparing `tmp/dagster-ge-0.9.9.tar.gz` & `tmp/dagster-ge-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-ge-0.9.9.tar", last modified: Thu Sep 17 21:28:50 2020, max compression
+gzip compressed data, was "dist/dagster-ge-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:11 2020, max compression
```

## Comparing `dagster-ge-0.9.9.tar` & `dagster-ge-0.9.9rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      541 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      115 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge/
--rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/dagster_ge/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3835 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/dagster_ge/factory.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/dagster_ge/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      541 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      317 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       11 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/dagster_ge.egg-info/top_level.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:50.000000 dagster-ge-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:24:45.000000 dagster-ge-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      544 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      115 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/dagster_ge/
+-rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3835 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/factory.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      544 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      317 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       11 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/top_level.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/setup.py
```

### Comparing `dagster-ge-0.9.9/LICENSE` & `dagster-ge-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-ge-0.9.9/PKG-INFO` & `dagster-ge-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-ge
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for GE-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ge
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-ge-0.9.9/dagster_ge/factory.py` & `dagster-ge-0.9.9rc1/dagster_ge/factory.py`

 * *Files identical despite different names*

### Comparing `dagster-ge-0.9.9/dagster_ge.egg-info/PKG-INFO` & `dagster-ge-0.9.9rc1/dagster_ge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-ge
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for GE-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ge
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-ge-0.9.9/setup.py` & `dagster-ge-0.9.9rc1/setup.py`

 * *Files identical despite different names*

