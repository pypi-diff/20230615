# Comparing `tmp/cdktf-cdktf-provider-null-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-null-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-null-6.0.1.tar", last modified: Thu Jun  1 14:26:56 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-null-7.0.0.tar", last modified: Thu Jun 15 11:29:12 2023, max compression
```

## Comparing `cdktf-cdktf-provider-null-6.0.1.tar` & `cdktf-cdktf-provider-null-7.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.406397 cdktf-cdktf-provider-null-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.406397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23456 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:56.410397 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:26:56.000000 cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.477673 cdktf-cdktf-provider-null-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.477673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/_jsii/provider-null@7.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.481673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-15 11:28:50.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:29:12.477673 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:29:12.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-15 11:29:12.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:29:12.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:29:12.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 11:29:12.000000 cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-null-6.0.1/LICENSE` & `cdktf-cdktf-provider-null-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-null-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-null-6.0.1/README.md` & `cdktf-cdktf-provider-null-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/setup.py` & `cdktf-cdktf-provider-null-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-null",
-    "version": "6.0.1",
+    "version": "7.0.0",
     "description": "Prebuilt null Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-null.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_null._jsii",
         "cdktf_cdktf_provider_null.data_null_data_source",
         "cdktf_cdktf_provider_null.provider",
         "cdktf_cdktf_provider_null.resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_null._jsii": [
-            "provider-null@6.0.1.jsii.tgz"
+            "provider-null@7.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_null": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.3, <0.17.0",
+        "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/__init__.py` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/provider/__init__.py` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null/resource/__init__.py` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-null
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt null Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-null.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-null.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-null-6.0.1/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-null-7.0.0/src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_null/py.typed
 src/cdktf_cdktf_provider_null.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_null.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_null.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_null.egg-info/requires.txt
 src/cdktf_cdktf_provider_null.egg-info/top_level.txt
 src/cdktf_cdktf_provider_null/_jsii/__init__.py
-src/cdktf_cdktf_provider_null/_jsii/provider-null@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_null/_jsii/provider-null@7.0.0.jsii.tgz
 src/cdktf_cdktf_provider_null/data_null_data_source/__init__.py
 src/cdktf_cdktf_provider_null/provider/__init__.py
 src/cdktf_cdktf_provider_null/resource/__init__.py
```

