# Comparing `tmp/dagster-census-0.19.9.tar.gz` & `tmp/dagster-census-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.19.9.tar", last modified: Thu Jun  8 18:52:00 2023, max compression
+gzip compressed data, was "dagster-census-0.19.9rc0.tar", last modified: Thu Jun  8 18:27:58 2023, max compression
```

## Comparing `dagster-census-0.19.9.tar` & `dagster-census-0.19.9rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:00.063115 dagster-census-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-census-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 18:43:17.000000 dagster-census-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-08 18:52:00.063115 dagster-census-0.19.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:00.063115 dagster-census-0.19.9/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10169 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-census-0.19.9/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:00.063115 dagster-census-0.19.9/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-08 18:51:59.000000 dagster-census-0.19.9/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:52:00.000000 dagster-census-0.19.9/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:59.000000 dagster-census-0.19.9/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:59.000000 dagster-census-0.19.9/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:51:59.000000 dagster-census-0.19.9/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:51:59.000000 dagster-census-0.19.9/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:52:00.067115 dagster-census-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1248 2023-06-08 18:43:17.000000 dagster-census-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10169 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      671 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:27:58.000000 dagster-census-0.19.9rc0/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-08 18:27:58.146390 dagster-census-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-08 18:20:46.000000 dagster-census-0.19.9rc0/setup.py
```

### Comparing `dagster-census-0.19.9/LICENSE` & `dagster-census-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9/PKG-INFO` & `dagster-census-0.19.9rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-census-0.19.9/dagster_census/ops.py` & `dagster-census-0.19.9rc0/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9/dagster_census/resources.py` & `dagster-census-0.19.9rc0/dagster_census/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9/dagster_census/types.py` & `dagster-census-0.19.9rc0/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9/dagster_census/utils.py` & `dagster-census-0.19.9rc0/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.19.9/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.19.9rc0/dagster_census.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-census-0.19.9/setup.py` & `dagster-census-0.19.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
-    install_requires=["dagster==1.3.9"],
+    install_requires=["dagster==1.3.9rc0"],
     zip_safe=False,
 )
```

