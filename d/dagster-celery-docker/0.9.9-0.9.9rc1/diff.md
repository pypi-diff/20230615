# Comparing `tmp/dagster-celery-docker-0.9.9.tar.gz` & `tmp/dagster-celery-docker-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-celery-docker-0.9.9.tar", last modified: Thu Sep 17 21:27:38 2020, max compression
+gzip compressed data, was "dist/dagster-celery-docker-0.9.9rc1.tar", last modified: Thu Sep 17 21:09:03 2020, max compression
```

## Comparing `dagster-celery-docker-0.9.9.tar` & `dagster-celery-docker-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      149 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker/
--rw-r--r--   0 bobchen    (501) staff       (20)      209 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      312 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker/app.py
--rw-r--r--   0 bobchen    (501) staff       (20)    13029 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker/executor.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      597 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       46 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       50 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/dagster_celery_docker_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2702 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker_tests/test_execute_docker.py
--rw-r--r--   0 bobchen    (501) staff       (20)      207 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker_tests/test_inclusion.py
--rw-r--r--   0 bobchen    (501) staff       (20)       99 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/dagster_celery_docker_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:27:38.000000 dagster-celery-docker-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1072 2020-09-17 21:24:45.000000 dagster-celery-docker-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      149 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/
+-rw-r--r--   0 bobchen    (501) staff       (20)      209 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      312 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/app.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    13029 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/executor.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      597 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       46 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       50 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2702 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_execute_docker.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      207 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_inclusion.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       99 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:09:03.000000 dagster-celery-docker-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1072 2020-09-17 21:04:59.000000 dagster-celery-docker-0.9.9rc1/setup.py
```

### Comparing `dagster-celery-docker-0.9.9/PKG-INFO` & `dagster-celery-docker-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-celery-docker
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for celery-docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-docker
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-docker-0.9.9/dagster_celery_docker/executor.py` & `dagster-celery-docker-0.9.9rc1/dagster_celery_docker/executor.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/PKG-INFO` & `dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-celery-docker
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for celery-docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-celery-docker
 Author: Elementl
 Author-email: UNKNOWN
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-celery-docker-0.9.9/dagster_celery_docker.egg-info/SOURCES.txt` & `dagster-celery-docker-0.9.9rc1/dagster_celery_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-celery-docker-0.9.9/dagster_celery_docker_tests/test_execute_docker.py` & `dagster-celery-docker-0.9.9rc1/dagster_celery_docker_tests/test_execute_docker.py`

 * *Files identical despite different names*

### Comparing `dagster-celery-docker-0.9.9/setup.py` & `dagster-celery-docker-0.9.9rc1/setup.py`

 * *Files identical despite different names*

