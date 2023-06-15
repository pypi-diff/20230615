# Comparing `tmp/dagster-datadog-0.9.9.tar.gz` & `tmp/dagster-datadog-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-datadog-0.9.9.tar", last modified: Thu Sep 17 21:28:06 2020, max compression
+gzip compressed data, was "dist/dagster-datadog-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:35 2020, max compression
```

## Comparing `dagster-datadog-0.9.9.tar` & `dagster-datadog-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      589 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog/
--rw-r--r--   0 bobchen    (501) staff       (20)      230 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2800 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      589 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      476 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/dagster_datadog_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2741 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/dagster_datadog_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:06.000000 dagster-datadog-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:24:45.000000 dagster-datadog-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      592 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog/
+-rw-r--r--   0 bobchen    (501) staff       (20)      230 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2800 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      592 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      476 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2741 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/setup.py
```

### Comparing `dagster-datadog-0.9.9/LICENSE` & `dagster-datadog-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datadog-0.9.9/dagster_datadog/resources.py` & `dagster-datadog-0.9.9rc1/dagster_datadog/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datadog-0.9.9/dagster_datadog_tests/test_resources.py` & `dagster-datadog-0.9.9rc1/dagster_datadog_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datadog-0.9.9/setup.py` & `dagster-datadog-0.9.9rc1/setup.py`

 * *Files identical despite different names*

