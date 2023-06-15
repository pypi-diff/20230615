# Comparing `tmp/dagster-celery-k8s-0.9.9.tar.gz` & `tmp/dagster-celery-k8s-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-k8s-0.9.9.tar", last modified: Thu Sep 17 21:27:55 2020, max compression
+gzip compressed data, was "dist/dagster-celery-k8s-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:50 2020, max compression
```

## Comparing `dagster-celery-k8s-0.9.9.tar` & `dagster-celery-k8s-0.9.9rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/
--rw-r--r--   0 bobchen    (501) staff       (20)      250 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      351 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3003 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    21066 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13303 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      671 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       35 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      270 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/example_celery_mode_def.py
--rw-r--r--   0 bobchen    (501) staff       (20)      448 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/test_inclusion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4906 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/test_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:55.000000 dagster-celery-k8s-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1055 2020-09-17 21:24:45.000000 dagster-celery-k8s-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/
+-rw-r--r--   0 bobchen    (501) staff       (20)      250 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      351 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/app.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3003 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/config.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    21066 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/executor.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    13303 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      671 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       35 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      270 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/example_celery_mode_def.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      448 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_inclusion.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4906 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:50.000000 dagster-celery-k8s-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1055 2020-09-17 21:04:59.000000 dagster-celery-k8s-0.9.9rc1/setup.py
```

### Comparing `dagster-celery-k8s-0.9.9/PKG-INFO` & `dagster-celery-k8s-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-celery-k8s
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for celery-k8s-executor
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-k8s
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s/config.py` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/config.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s/executor.py` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/executor.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s/launcher.py` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/PKG-INFO` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-celery-k8s
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for celery-k8s-executor
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-k8s
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s.egg-info/SOURCES.txt` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-celery-k8s-0.9.9/dagster_celery_k8s_tests/test_launcher.py` & `dagster-celery-k8s-0.9.9rc1/dagster_celery_k8s_tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-k8s-0.9.9/setup.py` & `dagster-celery-k8s-0.9.9rc1/setup.py`

 * *Files identical despite different names*

