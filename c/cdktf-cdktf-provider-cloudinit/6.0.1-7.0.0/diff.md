# Comparing `tmp/cdktf-cdktf-provider-cloudinit-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-cloudinit-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-cloudinit-6.0.1.tar", last modified: Thu Jun  1 14:29:33 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-cloudinit-7.0.0.tar", last modified: Thu Jun 15 11:17:18 2023, max compression
```

## Comparing `cdktf-cdktf-provider-cloudinit-6.0.1.tar` & `cdktf-cdktf-provider-cloudinit-7.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36818 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/config/
--rw-r--r--   0 runner    (1001) docker     (123)    43369 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/
--rw-r--r--   0 runner    (1001) docker     (123)    44298 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:29:20.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:33.805780 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-01 14:29:33.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 14:29:33.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:29:33.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:29:33.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 14:29:33.000000 cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.919366 cdktf-cdktf-provider-cloudinit-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@7.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    43369 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    44298 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:16:53.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:18.923366 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-15 11:17:18.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 11:17:18.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:17:18.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:17:18.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 11:17:18.000000 cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/LICENSE` & `cdktf-cdktf-provider-cloudinit-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-cloudinit-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-cloudinit
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt cloudinit Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-cloudinit.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-cloudinit.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/README.md` & `cdktf-cdktf-provider-cloudinit-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/setup.py` & `cdktf-cdktf-provider-cloudinit-7.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-cloudinit",
-    "version": "6.0.1",
+    "version": "7.0.0",
     "description": "Prebuilt cloudinit Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-cloudinit.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_cloudinit._jsii",
         "cdktf_cdktf_provider_cloudinit.config",
         "cdktf_cdktf_provider_cloudinit.data_cloudinit_config",
         "cdktf_cdktf_provider_cloudinit.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_cloudinit._jsii": [
-            "provider-cloudinit@6.0.1.jsii.tgz"
+            "provider-cloudinit@7.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_cloudinit": [
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

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/__init__.py` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/config/__init__.py` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-cloudinit
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt cloudinit Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-cloudinit.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-cloudinit.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-cloudinit-6.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-cloudinit-7.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_cloudinit/py.typed
 src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
 src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
-src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@7.0.0.jsii.tgz
 src/cdktf_cdktf_provider_cloudinit/config/__init__.py
 src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
 src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
```

