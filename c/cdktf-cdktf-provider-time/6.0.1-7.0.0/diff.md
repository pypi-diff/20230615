# Comparing `tmp/cdktf-cdktf-provider-time-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-time-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-time-6.0.1.tar", last modified: Fri Jun  2 14:17:52 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-time-7.0.0.tar", last modified: Thu Jun 15 11:35:26 2023, max compression
```

## Comparing `cdktf-cdktf-provider-time-6.0.1.tar` & `cdktf-cdktf-provider-time-7.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36435 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/_jsii/provider-time@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/offset/
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/offset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/rotating/
--rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/rotating/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/sleep/
--rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/sleep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/static_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-02 14:17:38.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/static_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:52.359815 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-02 14:17:52.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-02 14:17:52.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:17:52.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:17:52.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:17:52.000000 cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36433 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/_jsii/provider-time@7.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/offset/
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/rotating/
+-rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/sleep/
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/static_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-15 11:35:09.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:26.406701 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:35:26.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 11:35:26.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:26.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:35:26.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 11:35:26.000000 cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-time-6.0.1/LICENSE` & `cdktf-cdktf-provider-time-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-time-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-time-6.0.1/README.md` & `cdktf-cdktf-provider-time-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/setup.py` & `cdktf-cdktf-provider-time-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-time",
-    "version": "6.0.1",
+    "version": "7.0.0",
     "description": "Prebuilt time Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-time.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "cdktf_cdktf_provider_time.provider",
         "cdktf_cdktf_provider_time.rotating",
         "cdktf_cdktf_provider_time.sleep",
         "cdktf_cdktf_provider_time.static_resource"
     ],
     "package_data": {
         "cdktf_cdktf_provider_time._jsii": [
-            "provider-time@6.0.1.jsii.tgz"
+            "provider-time@7.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_time": [
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

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/offset/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/offset/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/provider/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/rotating/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/rotating/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/sleep/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time/static_resource/__init__.py` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time/static_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-time
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt time Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-time.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-time.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-time-6.0.1/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-time-7.0.0/src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_time/py.typed
 src/cdktf_cdktf_provider_time.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_time.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_time.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_time.egg-info/requires.txt
 src/cdktf_cdktf_provider_time.egg-info/top_level.txt
 src/cdktf_cdktf_provider_time/_jsii/__init__.py
-src/cdktf_cdktf_provider_time/_jsii/provider-time@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_time/_jsii/provider-time@7.0.0.jsii.tgz
 src/cdktf_cdktf_provider_time/offset/__init__.py
 src/cdktf_cdktf_provider_time/provider/__init__.py
 src/cdktf_cdktf_provider_time/rotating/__init__.py
 src/cdktf_cdktf_provider_time/sleep/__init__.py
 src/cdktf_cdktf_provider_time/static_resource/__init__.py
```

