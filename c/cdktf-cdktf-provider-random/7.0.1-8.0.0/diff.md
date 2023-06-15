# Comparing `tmp/cdktf-cdktf-provider-random-7.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-random-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-random-7.0.1.tar", last modified: Thu Jun  1 14:29:27 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-random-8.0.0.tar", last modified: Thu Jun 15 11:33:09 2023, max compression
```

## Comparing `cdktf-cdktf-provider-random-7.0.1.tar` & `cdktf-cdktf-provider-random-8.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.565065 cdktf-cdktf-provider-random-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:29:27.565065 cdktf-cdktf-provider-random-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46458 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/_jsii/provider-random@7.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/id/
--rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/id/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/integer/
--rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/integer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/password/
--rw-r--r--   0 runner    (1001) docker     (123)    47501 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/pet/
--rw-r--r--   0 runner    (1001) docker     (123)    22780 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/pet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)    24679 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/shuffle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/string_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    47512 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/string_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/uuid/
--rw-r--r--   0 runner    (1001) docker     (123)    15895 2023-06-01 14:29:15.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/uuid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:29:27.561065 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-01 14:29:27.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-01 14:29:27.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:29:27.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:29:27.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 14:29:27.000000 cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.480606 cdktf-cdktf-provider-random-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46457 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/_jsii/provider-random@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/id/
+-rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/id/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/integer/
+-rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/password/
+-rw-r--r--   0 runner    (1001) docker     (123)    47501 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/pet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22780 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)    24679 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/string_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    47512 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/uuid/
+-rw-r--r--   0 runner    (1001) docker     (123)    15895 2023-06-15 11:32:52.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:33:09.484606 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-15 11:33:09.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 11:33:09.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:33:09.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:33:09.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 11:33:09.000000 cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-random-7.0.1/LICENSE` & `cdktf-cdktf-provider-random-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/PKG-INFO` & `cdktf-cdktf-provider-random-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-random
-Version: 7.0.1
+Version: 8.0.0
 Summary: Prebuilt random Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-random.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-random.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-random-7.0.1/README.md` & `cdktf-cdktf-provider-random-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/setup.py` & `cdktf-cdktf-provider-random-8.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-random",
-    "version": "7.0.1",
+    "version": "8.0.0",
     "description": "Prebuilt random Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-random.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -30,25 +30,25 @@
         "cdktf_cdktf_provider_random.provider",
         "cdktf_cdktf_provider_random.shuffle",
         "cdktf_cdktf_provider_random.string_resource",
         "cdktf_cdktf_provider_random.uuid"
     ],
     "package_data": {
         "cdktf_cdktf_provider_random._jsii": [
-            "provider-random@7.0.1.jsii.tgz"
+            "provider-random@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_random": [
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

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/id/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/id/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/integer/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/password/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/pet/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/provider/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/shuffle/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/string_resource/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random/uuid/__init__.py` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-random
-Version: 7.0.1
+Version: 8.0.0
 Summary: Prebuilt random Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-random.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-random.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-random-7.0.1/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-random-8.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_random/py.typed
 src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_random.egg-info/requires.txt
 src/cdktf_cdktf_provider_random.egg-info/top_level.txt
 src/cdktf_cdktf_provider_random/_jsii/__init__.py
-src/cdktf_cdktf_provider_random/_jsii/provider-random@7.0.1.jsii.tgz
+src/cdktf_cdktf_provider_random/_jsii/provider-random@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_random/id/__init__.py
 src/cdktf_cdktf_provider_random/integer/__init__.py
 src/cdktf_cdktf_provider_random/password/__init__.py
 src/cdktf_cdktf_provider_random/pet/__init__.py
 src/cdktf_cdktf_provider_random/provider/__init__.py
 src/cdktf_cdktf_provider_random/shuffle/__init__.py
 src/cdktf_cdktf_provider_random/string_resource/__init__.py
```

