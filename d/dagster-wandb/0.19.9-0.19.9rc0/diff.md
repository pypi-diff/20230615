# Comparing `tmp/dagster-wandb-0.19.9.tar.gz` & `tmp/dagster-wandb-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.19.9.tar", last modified: Thu Jun  8 18:51:17 2023, max compression
+gzip compressed data, was "dagster-wandb-0.19.9rc0.tar", last modified: Thu Jun  8 18:31:09 2023, max compression
```

## Comparing `dagster-wandb-0.19.9.tar` & `dagster-wandb-0.19.9rc0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      679 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33673 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/types.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      679 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:51:17.000000 dagster-wandb-0.19.9/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-08 18:51:17.886520 dagster-wandb-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-08 18:43:18.000000 dagster-wandb-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33673 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/types.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:09.849053 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:31:09.000000 dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-08 18:31:09.853053 dagster-wandb-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-06-08 18:20:46.000000 dagster-wandb-0.19.9rc0/setup.py
```

### Comparing `dagster-wandb-0.19.9/LICENSE` & `dagster-wandb-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/PKG-INFO` & `dagster-wandb-0.19.9rc0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.19.9/dagster_wandb/__init__.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb/io_manager.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb/launch/configs.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb/launch/ops.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb/resources.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb/types.py` & `dagster-wandb-0.19.9rc0/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-wandb-0.19.9/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.19.9rc0/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.19.9/setup.py` & `dagster-wandb-0.19.9rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     install_requires=[
-        "dagster==1.3.9",
+        "dagster==1.3.9rc0",
         "wandb>=0.13.5,<0.15.4",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

