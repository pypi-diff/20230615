# Comparing `tmp/dagster-papertrail-0.9.9.tar.gz` & `tmp/dagster-papertrail-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-papertrail-0.9.9.tar", last modified: Thu Sep 17 21:28:03 2020, max compression
+gzip compressed data, was "dist/dagster-papertrail-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:00 2020, max compression
```

## Comparing `dagster-papertrail-0.9.9.tar` & `dagster-papertrail-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail/
--rw-r--r--   0 bobchen    (501) staff       (20)      233 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2296 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail/loggers.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      598 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      508 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/dagster_papertrail_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1601 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail_tests/test_loggers.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/dagster_papertrail_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:03.000000 dagster-papertrail-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1046 2020-09-17 21:24:45.000000 dagster-papertrail-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      601 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/
+-rw-r--r--   0 bobchen    (501) staff       (20)      233 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2296 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/loggers.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      601 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      508 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1601 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/test_loggers.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1046 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/setup.py
```

### Comparing `dagster-papertrail-0.9.9/LICENSE` & `dagster-papertrail-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-papertrail-0.9.9/PKG-INFO` & `dagster-papertrail-0.9.9rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-papertrail
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for papertrail Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-papertrail
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-papertrail-0.9.9/dagster_papertrail/loggers.py` & `dagster-papertrail-0.9.9rc1/dagster_papertrail/loggers.py`

 * *Files identical despite different names*

### Comparing `dagster-papertrail-0.9.9/dagster_papertrail.egg-info/PKG-INFO` & `dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-papertrail
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for papertrail Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-papertrail
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-papertrail-0.9.9/dagster_papertrail_tests/test_loggers.py` & `dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/test_loggers.py`

 * *Files identical despite different names*

### Comparing `dagster-papertrail-0.9.9/setup.py` & `dagster-papertrail-0.9.9rc1/setup.py`

 * *Files identical despite different names*

