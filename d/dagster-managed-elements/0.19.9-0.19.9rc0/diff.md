# Comparing `tmp/dagster-managed-elements-0.19.9.tar.gz` & `tmp/dagster-managed-elements-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.19.9.tar", last modified: Thu Jun  8 18:50:25 2023, max compression
+gzip compressed data, was "dagster-managed-elements-0.19.9rc0.tar", last modified: Thu Jun  8 18:30:57 2023, max compression
```

## Comparing `dagster-managed-elements-0.19.9.tar` & `dagster-managed-elements-0.19.9rc0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:25.005763 dagster-managed-elements-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 18:50:25.005763 dagster-managed-elements-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:25.005763 dagster-managed-elements-0.19.9/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:50:25.005763 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:50:24.000000 dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 18:50:25.005763 dagster-managed-elements-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1518 2023-06-08 18:43:17.000000 dagster-managed-elements-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:57.252877 dagster-managed-elements-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 18:30:57.252877 dagster-managed-elements-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:57.248877 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:30:57.252877 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:30:57.000000 dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-08 18:30:57.252877 dagster-managed-elements-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 18:20:46.000000 dagster-managed-elements-0.19.9rc0/setup.py
```

### Comparing `dagster-managed-elements-0.19.9/LICENSE` & `dagster-managed-elements-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.9/PKG-INFO` & `dagster-managed-elements-0.19.9rc0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.9/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.19.9rc0/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.9/dagster_managed_elements/types.py` & `dagster-managed-elements-0.19.9rc0/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.9/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.19.9rc0/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.9/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.19.9rc0/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.9/setup.py` & `dagster-managed-elements-0.19.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
-    install_requires=["dagster==1.3.9", "requests", "click_spinner"],
+    install_requires=["dagster==1.3.9rc0", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

