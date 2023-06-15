# Comparing `tmp/dagster-celery-0.9.9.tar.gz` & `tmp/dagster-celery-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-0.9.9.tar", last modified: Thu Sep 17 21:28:16 2020, max compression
+gzip compressed data, was "dist/dagster-celery-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:14 2020, max compression
```

## Comparing `dagster-celery-0.9.9.tar` & `dagster-celery-0.9.9rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      665 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery/
--rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      346 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8673 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)      507 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7123 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/core_execution_loop.py
--rw-r--r--   0 bobchen    (501) staff       (20)      488 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/defaults.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6300 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/k8s_job_task.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1122 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/make_app.py
--rw-r--r--   0 bobchen    (501) staff       (20)      453 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2680 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/tasks.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      665 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       60 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/dagster_celery_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1317 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/empty.py
--rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/engine_config.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7683 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/repo.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5749 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1666 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12342 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_execute.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3068 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_priority.py
--rw-r--r--   0 bobchen    (501) staff       (20)      770 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_queues.py
--rw-r--r--   0 bobchen    (501) staff       (20)      289 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2773 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/dagster_celery_tests/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:16.000000 dagster-celery-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1273 2020-09-17 21:24:45.000000 dagster-celery-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      668 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery/
+-rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      346 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/app.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8673 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/cli.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      507 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/config.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7123 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/core_execution_loop.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      488 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/defaults.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6300 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/executor.py
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/k8s_job_task.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1122 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/make_app.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      453 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/tags.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2680 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/tasks.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      668 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     1079 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       60 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/entry_points.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)      106 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1317 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/empty.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/engine_config.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7683 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/repo.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5749 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_cli.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1666 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_config.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    12342 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_execute.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3068 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_priority.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      770 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_queues.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      289 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       95 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2773 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/dagster_celery_tests/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:14.000000 dagster-celery-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1273 2020-09-17 21:04:59.000000 dagster-celery-0.9.9rc1/setup.py
```

### Comparing `dagster-celery-0.9.9/LICENSE` & `dagster-celery-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/PKG-INFO` & `dagster-celery-0.9.9rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-celery
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for using Celery as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-0.9.9/dagster_celery/cli.py` & `dagster-celery-0.9.9rc1/dagster_celery/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery/core_execution_loop.py` & `dagster-celery-0.9.9rc1/dagster_celery/core_execution_loop.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery/executor.py` & `dagster-celery-0.9.9rc1/dagster_celery/executor.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery/make_app.py` & `dagster-celery-0.9.9rc1/dagster_celery/make_app.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery/tasks.py` & `dagster-celery-0.9.9rc1/dagster_celery/tasks.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery.egg-info/PKG-INFO` & `dagster-celery-0.9.9rc1/dagster_celery.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-celery
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for using Celery as Dagster's execution engine.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-0.9.9/dagster_celery.egg-info/SOURCES.txt` & `dagster-celery-0.9.9rc1/dagster_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/conftest.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/repo.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/repo.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/test_cli.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/test_config.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/test_execute.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/test_priority.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/test_queues.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/test_queues.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/dagster_celery_tests/utils.py` & `dagster-celery-0.9.9rc1/dagster_celery_tests/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-0.9.9/setup.py` & `dagster-celery-0.9.9rc1/setup.py`

 * *Files identical despite different names*

