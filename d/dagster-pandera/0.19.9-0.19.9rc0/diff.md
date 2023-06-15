# Comparing `tmp/dagster-pandera-0.19.9.tar.gz` & `tmp/dagster-pandera-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pandera-0.19.9.tar", last modified: Thu Jun  8 18:50:54 2023, max compression
+gzip compressed data, was "dagster-pandera-0.19.9rc0.tar", last modified: Thu Jun  8 18:31:06 2023, max compression
```

## Comparing `dagster-pandera-0.19.9.tar` & `dagster-pandera-0.19.9rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:54.990192 dagster-pandera-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-08 18:50:54.990192 dagster-pandera-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:54.990192 dagster-pandera-0.19.9/dagster_pandera/
--rw-r--r--   0 root         (0) root         (0)     9258 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/dagster_pandera/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/dagster_pandera/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/dagster_pandera/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:54.990192 dagster-pandera-0.19.9/dagster_pandera.egg-info/
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-08 18:50:54.000000 dagster-pandera-0.19.9/dagster_pandera.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-08 18:50:54.000000 dagster-pandera-0.19.9/dagster_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:50:54.000000 dagster-pandera-0.19.9/dagster_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-08 18:50:54.000000 dagster-pandera-0.19.9/dagster_pandera.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:50:54.000000 dagster-pandera-0.19.9/dagster_pandera.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:50:54.994192 dagster-pandera-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1316 2023-06-08 18:43:18.000000 dagster-pandera-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/dagster_pandera/
+-rw-r--r--   0 root         (0) root         (0)     9258 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/dagster_pandera/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 18:31:06.000000 dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:31:06.229002 dagster-pandera-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-06-08 18:20:46.000000 dagster-pandera-0.19.9rc0/setup.py
```

### Comparing `dagster-pandera-0.19.9/LICENSE` & `dagster-pandera-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.19.9/PKG-INFO` & `dagster-pandera-0.19.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-pandera-0.19.9/dagster_pandera/__init__.py` & `dagster-pandera-0.19.9rc0/dagster_pandera/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.19.9/dagster_pandera.egg-info/PKG-INFO` & `dagster-pandera-0.19.9rc0/dagster_pandera.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-pandera-0.19.9/setup.py` & `dagster-pandera-0.19.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_pandera_tests*"]),
     include_package_data=True,
-    install_requires=["dagster==1.3.9", "pandas", "pandera>=0.14.2"],
+    install_requires=["dagster==1.3.9rc0", "pandas", "pandera>=0.14.2"],
     extras_require={
         "test": [
             "pytest",
         ],
     },
 )
```

