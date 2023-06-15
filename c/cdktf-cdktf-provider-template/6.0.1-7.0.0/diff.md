# Comparing `tmp/cdktf-cdktf-provider-template-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-template-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-template-6.0.1.tar", last modified: Fri Jun  2 14:16:27 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-template-7.0.0.tar", last modified: Thu Jun 15 11:34:54 2023, max compression
```

## Comparing `cdktf-cdktf-provider-template-6.0.1.tar` & `cdktf-cdktf-provider-template-7.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.595690 cdktf-cdktf-provider-template-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-02 14:16:27.595690 cdktf-cdktf-provider-template-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:16:27.595690 cdktf-cdktf-provider-template-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.587689 cdktf-cdktf-provider-template-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/_jsii/provider-template@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/cloudinit_config/
--rw-r--r--   0 runner    (1001) docker     (123)    42871 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/cloudinit_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/
--rw-r--r--   0 runner    (1001) docker     (123)    43758 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_file/
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/dir/
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/dir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/file/
--rw-r--r--   0 runner    (1001) docker     (123)    22770 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.595690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:16:12.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:27.591690 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-02 14:16:27.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-02 14:16:27.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:16:27.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:16:27.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:16:27.000000 cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.033335 cdktf-cdktf-provider-template-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42492 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/_jsii/provider-template@7.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/cloudinit_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    42871 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/cloudinit_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    43758 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/dir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    22770 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:34:40.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:34:54.037335 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 11:34:54.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 11:34:54.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:34:54.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:34:54.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 11:34:54.000000 cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-template-6.0.1/LICENSE` & `cdktf-cdktf-provider-template-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-template-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-template
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt template Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-template.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-template.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-template-6.0.1/README.md` & `cdktf-cdktf-provider-template-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/setup.py` & `cdktf-cdktf-provider-template-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-template",
-    "version": "6.0.1",
+    "version": "7.0.0",
     "description": "Prebuilt template Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-template.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -28,25 +28,25 @@
         "cdktf_cdktf_provider_template.data_template_file",
         "cdktf_cdktf_provider_template.dir",
         "cdktf_cdktf_provider_template.file",
         "cdktf_cdktf_provider_template.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_template._jsii": [
-            "provider-template@6.0.1.jsii.tgz"
+            "provider-template@7.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_template": [
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

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/cloudinit_config/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/cloudinit_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_cloudinit_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/data_template_file/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/data_template_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/dir/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/dir/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/file/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template/provider/__init__.py` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/PKG-INFO` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-template
-Version: 6.0.1
+Version: 7.0.0
 Summary: Prebuilt template Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-template.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-template.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-template-6.0.1/src/cdktf_cdktf_provider_template.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-template-7.0.0/src/cdktf_cdktf_provider_template.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdktf_cdktf_provider_template/py.typed
 src/cdktf_cdktf_provider_template.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_template.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_template.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_template.egg-info/requires.txt
 src/cdktf_cdktf_provider_template.egg-info/top_level.txt
 src/cdktf_cdktf_provider_template/_jsii/__init__.py
-src/cdktf_cdktf_provider_template/_jsii/provider-template@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_template/_jsii/provider-template@7.0.0.jsii.tgz
 src/cdktf_cdktf_provider_template/cloudinit_config/__init__.py
 src/cdktf_cdktf_provider_template/data_template_cloudinit_config/__init__.py
 src/cdktf_cdktf_provider_template/data_template_file/__init__.py
 src/cdktf_cdktf_provider_template/dir/__init__.py
 src/cdktf_cdktf_provider_template/file/__init__.py
 src/cdktf_cdktf_provider_template/provider/__init__.py
```

