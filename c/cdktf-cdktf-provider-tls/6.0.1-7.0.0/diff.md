# Comparing `tmp/cdktf-cdktf-provider-tls-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-tls-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-tls-6.0.1.tar", last modified: Fri Jun  2 14:17:24 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-tls-7.0.0.tar", last modified: Thu Jun 15 11:36:36 2023, max compression
```

## Comparing `cdktf-cdktf-provider-tls-6.0.1.tar` & `cdktf-cdktf-provider-tls-7.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.036701 cdktf-cdktf-provider-tls-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71455 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/_jsii/provider-tls@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/cert_request/
--rw-r--r--   0 runner    (1001) docker     (123)    52342 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/cert_request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_public_key/
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/locally_signed_cert/
--rw-r--r--   0 runner    (1001) docker     (123)    41062 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/private_key/
--rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/private_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/self_signed_cert/
--rw-r--r--   0 runner    (1001) docker     (123)    76711 2023-06-02 14:17:12.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:17:24.040701 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-02 14:17:24.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 14:17:24.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:17:24.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:17:24.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 14:17:24.000000 cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.655755 cdktf-cdktf-provider-tls-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-15 11:36:36.655755 cdktf-cdktf-provider-tls-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:36:36.655755 cdktf-cdktf-provider-tls-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.647755 cdktf-cdktf-provider-tls-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71454 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/_jsii/provider-tls@7.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/cert_request/
+-rw-r--r--   0 runner    (1001) docker     (123)    52342 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)    41062 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/private_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.655755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)    76711 2023-06-15 11:36:18.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:36:36.651755 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-06-15 11:36:36.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-15 11:36:36.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:36:36.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:36:36.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 11:36:36.000000 cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-tls-6.0.1/LICENSE` & `cdktf-cdktf-provider-tls-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-tls-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tls
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt tls Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tls.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tls.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-tls-6.0.1/README.md` & `cdktf-cdktf-provider-tls-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/setup.py` & `cdktf-cdktf-provider-tls-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-tls",
-    "version": "6.0.1",
+    "version": "7.0.0",
     "description": "Prebuilt tls Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-tls.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -29,25 +29,25 @@
         "cdktf_cdktf_provider_tls.locally_signed_cert",
         "cdktf_cdktf_provider_tls.private_key",
         "cdktf_cdktf_provider_tls.provider",
         "cdktf_cdktf_provider_tls.self_signed_cert"
     ],
     "package_data": {
         "cdktf_cdktf_provider_tls._jsii": [
-            "provider-tls@6.0.1.jsii.tgz"
+            "provider-tls@7.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_tls": [
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

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/cert_request/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/cert_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/private_key/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/private_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/provider/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-tls
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt tls Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-tls.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-tls.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-tls-6.0.1/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-tls-7.0.0/src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_tls/py.typed
 src/cdktf_cdktf_provider_tls.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_tls.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_tls.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_tls.egg-info/requires.txt
 src/cdktf_cdktf_provider_tls.egg-info/top_level.txt
 src/cdktf_cdktf_provider_tls/_jsii/__init__.py
-src/cdktf_cdktf_provider_tls/_jsii/provider-tls@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_tls/_jsii/provider-tls@7.0.0.jsii.tgz
 src/cdktf_cdktf_provider_tls/cert_request/__init__.py
 src/cdktf_cdktf_provider_tls/data_tls_certificate/__init__.py
 src/cdktf_cdktf_provider_tls/data_tls_public_key/__init__.py
 src/cdktf_cdktf_provider_tls/locally_signed_cert/__init__.py
 src/cdktf_cdktf_provider_tls/private_key/__init__.py
 src/cdktf_cdktf_provider_tls/provider/__init__.py
 src/cdktf_cdktf_provider_tls/self_signed_cert/__init__.py
```

