# Comparing `tmp/dagster-prometheus-0.9.9.tar.gz` & `tmp/dagster-prometheus-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-prometheus-0.9.9.tar", last modified: Thu Sep 17 21:28:13 2020, max compression
+gzip compressed data, was "dist/dagster-prometheus-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:59 2020, max compression
```

## Comparing `dagster-prometheus-0.9.9.tar` & `dagster-prometheus-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      582 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/dagster_prometheus/
--rw-r--r--   0 bobchen    (501) staff       (20)      239 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5524 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      582 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      502 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:28:12.000000 dagster-prometheus-0.9.9/dagster_prometheus.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/dagster_prometheus_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4529 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/dagster_prometheus_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:28:13.000000 dagster-prometheus-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1051 2020-09-17 21:24:45.000000 dagster-prometheus-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      585 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/
+-rw-r--r--   0 bobchen    (501) staff       (20)      239 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5524 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      585 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      502 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4529 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1051 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/setup.py
```

### Comparing `dagster-prometheus-0.9.9/LICENSE` & `dagster-prometheus-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-prometheus-0.9.9/PKG-INFO` & `dagster-prometheus-0.9.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-prometheus
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for prometheus
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-prometheus
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-prometheus-0.9.9/dagster_prometheus/resources.py` & `dagster-prometheus-0.9.9rc1/dagster_prometheus/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-prometheus-0.9.9/dagster_prometheus.egg-info/PKG-INFO` & `dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-prometheus
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for prometheus
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-prometheus
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-prometheus-0.9.9/dagster_prometheus_tests/test_resources.py` & `dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-prometheus-0.9.9/setup.py` & `dagster-prometheus-0.9.9rc1/setup.py`

 * *Files identical despite different names*

