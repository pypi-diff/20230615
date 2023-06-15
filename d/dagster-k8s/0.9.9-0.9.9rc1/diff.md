# Comparing `tmp/dagster-k8s-0.9.9.tar.gz` & `tmp/dagster-k8s-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-k8s-0.9.9.tar", last modified: Thu Sep 17 21:28:20 2020, max compression
+gzip compressed data, was "dist/dagster-k8s-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:18 2020, max compression
```

## Comparing `dagster-k8s-0.9.9.tar` & `dagster-k8s-0.9.9rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      561 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s/
--rw-r--r--   0 bobchen    (501) staff       (20)      337 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16154 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/client.py
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/config.py
--rw-r--r--   0 bobchen    (501) staff       (20)    22168 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/job.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14915 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9341 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/scheduler.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1558 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/test.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3253 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      561 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      751 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       69 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    17876 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1193 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_job.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2780 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_resource_tags.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8042 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:20.000000 dagster-k8s-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1202 2020-09-17 21:24:45.000000 dagster-k8s-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      564 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s/
+-rw-r--r--   0 bobchen    (501) staff       (20)      337 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    16154 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/client.py
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/config.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    22168 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/job.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    14915 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     9341 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/scheduler.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1558 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/test.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3253 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      564 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      751 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       69 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:17.000000 dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    17876 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_client.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1193 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_job.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2780 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_resource_tags.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8042 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:18.000000 dagster-k8s-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1202 2020-09-17 21:04:59.000000 dagster-k8s-0.9.9rc1/setup.py
```

### Comparing `dagster-k8s-0.9.9/LICENSE` & `dagster-k8s-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/PKG-INFO` & `dagster-k8s-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-k8s
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for k8s
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-k8s
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-k8s-0.9.9/dagster_k8s/client.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/client.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s/job.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/job.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s/launcher.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s/scheduler.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s/test.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/test.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s/utils.py` & `dagster-k8s-0.9.9rc1/dagster_k8s/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s.egg-info/PKG-INFO` & `dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-k8s
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for k8s
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-k8s
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-k8s-0.9.9/dagster_k8s.egg-info/SOURCES.txt` & `dagster-k8s-0.9.9rc1/dagster_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_client.py` & `dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_job.py` & `dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_job.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_resource_tags.py` & `dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_resource_tags.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/dagster_k8s_tests/unit_tests/test_utils.py` & `dagster-k8s-0.9.9rc1/dagster_k8s_tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-k8s-0.9.9/setup.py` & `dagster-k8s-0.9.9rc1/setup.py`

 * *Files identical despite different names*

