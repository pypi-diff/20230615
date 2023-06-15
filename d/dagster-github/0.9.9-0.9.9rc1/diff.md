# Comparing `tmp/dagster-github-0.9.9.tar.gz` & `tmp/dagster-github-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-github-0.9.9.tar", last modified: Thu Sep 17 21:28:30 2020, max compression
+gzip compressed data, was "dist/dagster-github-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:43 2020, max compression
```

## Comparing `dagster-github-0.9.9.tar` & `dagster-github-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:30.000000 dagster-github-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-github-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-github-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      616 2020-09-17 21:28:30.000000 dagster-github-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:24:45.000000 dagster-github-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github/
--rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5922 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      616 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      464 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       31 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:30.000000 dagster-github-0.9.9/dagster_github_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6489 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:24:45.000000 dagster-github-0.9.9/dagster_github_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:30.000000 dagster-github-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1367 2020-09-17 21:24:45.000000 dagster-github-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      619 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github/
+-rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5922 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      619 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      464 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       31 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/dagster_github_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6489 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/dagster_github_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:43.000000 dagster-github-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1367 2020-09-17 21:04:59.000000 dagster-github-0.9.9rc1/setup.py
```

### Comparing `dagster-github-0.9.9/LICENSE` & `dagster-github-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-github-0.9.9/PKG-INFO` & `dagster-github-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-github
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Github client resource for interacting with the github API with a github App
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-github
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-github-0.9.9/dagster_github/resources.py` & `dagster-github-0.9.9rc1/dagster_github/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-github-0.9.9/dagster_github.egg-info/PKG-INFO` & `dagster-github-0.9.9rc1/dagster_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-github
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Github client resource for interacting with the github API with a github App
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-github
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-github-0.9.9/dagster_github_tests/test_resources.py` & `dagster-github-0.9.9rc1/dagster_github_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-github-0.9.9/setup.py` & `dagster-github-0.9.9rc1/setup.py`

 * *Files identical despite different names*

