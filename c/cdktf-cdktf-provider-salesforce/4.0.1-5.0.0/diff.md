# Comparing `tmp/cdktf-cdktf-provider-salesforce-4.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-salesforce-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-salesforce-4.0.1.tar", last modified: Fri Jun  2 14:13:47 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-salesforce-5.0.0.tar", last modified: Thu Jun 15 11:34:00 2023, max compression
```

## Comparing `cdktf-cdktf-provider-salesforce-4.0.1.tar` & `cdktf-cdktf-provider-salesforce-5.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.589915 cdktf-cdktf-provider-salesforce-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:13:47.589915 cdktf-cdktf-provider-salesforce-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.581915 cdktf-cdktf-provider-salesforce-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40895 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@4.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/
--rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/profile/
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user/
--rw-r--r--   0 runner    (1001) docker     (123)    44505 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user_role/
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-02 14:13:32.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.585915 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-02 14:13:47.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-02 14:13:47.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:47.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:13:47.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:13:47.000000 cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.750518 cdktf-cdktf-provider-salesforce-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.750518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    44505 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-15 11:33:43.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:00.754518 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:34:00.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 11:34:00.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:34:00.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:34:00.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 11:34:00.000000 cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/LICENSE` & `cdktf-cdktf-provider-salesforce-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/PKG-INFO` & `cdktf-cdktf-provider-salesforce-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-salesforce
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt salesforce Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-salesforce.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-salesforce.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/README.md` & `cdktf-cdktf-provider-salesforce-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/setup.py` & `cdktf-cdktf-provider-salesforce-5.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-salesforce",
-    "version": "4.0.1",
+    "version": "5.0.0",
     "description": "Prebuilt salesforce Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-salesforce.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -28,25 +28,25 @@
         "cdktf_cdktf_provider_salesforce.profile",
         "cdktf_cdktf_provider_salesforce.provider",
         "cdktf_cdktf_provider_salesforce.user",
         "cdktf_cdktf_provider_salesforce.user_role"
     ],
     "package_data": {
         "cdktf_cdktf_provider_salesforce._jsii": [
-            "provider-salesforce@4.0.1.jsii.tgz"
+            "provider-salesforce@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_salesforce": [
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

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/profile/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/provider/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce/user_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-salesforce
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt salesforce Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-salesforce.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-salesforce.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-salesforce-4.0.1/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-salesforce-5.0.0/src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdktf_cdktf_provider_salesforce/py.typed
 src/cdktf_cdktf_provider_salesforce.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_salesforce.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/requires.txt
 src/cdktf_cdktf_provider_salesforce.egg-info/top_level.txt
 src/cdktf_cdktf_provider_salesforce/_jsii/__init__.py
-src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@4.0.1.jsii.tgz
+src/cdktf_cdktf_provider_salesforce/_jsii/provider-salesforce@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_salesforce/data_salesforce_profile/__init__.py
 src/cdktf_cdktf_provider_salesforce/data_salesforce_user_license/__init__.py
 src/cdktf_cdktf_provider_salesforce/profile/__init__.py
 src/cdktf_cdktf_provider_salesforce/provider/__init__.py
 src/cdktf_cdktf_provider_salesforce/user/__init__.py
 src/cdktf_cdktf_provider_salesforce/user_role/__init__.py
```

