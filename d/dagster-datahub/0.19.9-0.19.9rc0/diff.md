# Comparing `tmp/dagster-datahub-0.19.9.tar.gz` & `tmp/dagster-datahub-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-datahub-0.19.9.tar", last modified: Thu Jun  8 18:52:38 2023, max compression
+gzip compressed data, was "dagster-datahub-0.19.9rc0.tar", last modified: Thu Jun  8 18:30:25 2023, max compression
```

## Comparing `dagster-datahub-0.19.9.tar` & `dagster-datahub-0.19.9rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:38.159640 dagster-datahub-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-08 18:52:38.159640 dagster-datahub-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:38.159640 dagster-datahub-0.19.9/dagster_datahub/
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/dagster_datahub/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/dagster_datahub/py.typed
--rw-r--r--   0 root         (0) root         (0)     3932 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/dagster_datahub/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/dagster_datahub/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:38.159640 dagster-datahub-0.19.9/dagster_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:52:38.000000 dagster-datahub-0.19.9/dagster_datahub.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:52:38.163640 dagster-datahub-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 18:43:17.000000 dagster-datahub-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/resources.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/dagster_datahub/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:30:25.000000 dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-08 18:30:25.800431 dagster-datahub-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 18:20:46.000000 dagster-datahub-0.19.9rc0/setup.py
```

### Comparing `dagster-datahub-0.19.9/LICENSE` & `dagster-datahub-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.19.9/PKG-INFO` & `dagster-datahub-0.19.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-datahub-0.19.9/dagster_datahub/resources.py` & `dagster-datahub-0.19.9rc0/dagster_datahub/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-datahub-0.19.9/dagster_datahub.egg-info/PKG-INFO` & `dagster-datahub-0.19.9rc0/dagster_datahub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-datahub
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for Datahub-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datahub
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-datahub-0.19.9/setup.py` & `dagster-datahub-0.19.9rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,14 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_datahub_tests*"]),
     include_package_data=True,
     install_requires=[
         "acryl-datahub[datahub-rest, datahub-kafka]<=0.10.2",
-        "dagster==1.3.9",
+        "dagster==1.3.9rc0",
         "packaging",
         "requests",
     ],
     extras_require={},
     zip_safe=False,
 )
```

