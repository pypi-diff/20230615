# Comparing `tmp/cdktf-cdktf-provider-http-4.0.2.tar.gz` & `tmp/cdktf-cdktf-provider-http-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-http-4.0.2.tar", last modified: Thu Jun  1 14:26:40 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-http-5.0.0.tar", last modified: Thu Jun 15 11:28:08 2023, max compression
```

## Comparing `cdktf-cdktf-provider-http-4.0.2.tar` & `cdktf-cdktf-provider-http-5.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.341862 cdktf-cdktf-provider-http-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/data_http/
--rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/data_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:28.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:26:40.345862 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 14:26:40.000000 cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/
+-rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-http-4.0.2/LICENSE` & `cdktf-cdktf-provider-http-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.2/PKG-INFO` & `cdktf-cdktf-provider-http-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 4.0.2
+Version: 5.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-4.0.2/README.md` & `cdktf-cdktf-provider-http-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.2/setup.py` & `cdktf-cdktf-provider-http-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-http",
-    "version": "4.0.2",
+    "version": "5.0.0",
     "description": "Prebuilt http Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-http.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,25 +24,25 @@
         "cdktf_cdktf_provider_http",
         "cdktf_cdktf_provider_http._jsii",
         "cdktf_cdktf_provider_http.data_http",
         "cdktf_cdktf_provider_http.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_http._jsii": [
-            "provider-http@4.0.2.jsii.tgz"
+            "provider-http@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_http": [
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

### Comparing `cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/__init__.py` & `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/data_http/__init__.py` & `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http/provider/__init__.py` & `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO` & `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 4.0.2
+Version: 5.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-4.0.2/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_http/py.typed
 src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_http.egg-info/requires.txt
 src/cdktf_cdktf_provider_http.egg-info/top_level.txt
 src/cdktf_cdktf_provider_http/_jsii/__init__.py
-src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.2.jsii.tgz
+src/cdktf_cdktf_provider_http/_jsii/provider-http@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_http/data_http/__init__.py
 src/cdktf_cdktf_provider_http/provider/__init__.py
```

