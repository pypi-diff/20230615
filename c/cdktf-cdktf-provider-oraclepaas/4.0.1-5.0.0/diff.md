# Comparing `tmp/cdktf-cdktf-provider-oraclepaas-4.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-oraclepaas-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-oraclepaas-4.0.1.tar", last modified: Thu Jun  1 14:30:31 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-oraclepaas-5.0.0.tar", last modified: Thu Jun 15 11:31:29 2023, max compression
```

## Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1.tar` & `cdktf-cdktf-provider-oraclepaas-5.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.203182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.203182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.203182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   206444 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/_jsii/provider-oraclepaas@4.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/application_container/
--rw-r--r--   0 runner    (1001) docker     (123)   159933 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/application_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/
--rw-r--r--   0 runner    (1001) docker     (123)    23224 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    42341 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/
--rw-r--r--   0 runner    (1001) docker     (123)   235385 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    43957 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/
--rw-r--r--   0 runner    (1001) docker     (123)   334882 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    44496 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/
--rw-r--r--   0 runner    (1001) docker     (123)   122384 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.207182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:30:19.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:31.203182 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-01 14:30:31.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-01 14:30:31.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:30:31.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:30:31.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 14:30:31.000000 cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   206443 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/_jsii/provider-oraclepaas@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/application_container/
+-rw-r--r--   0 runner    (1001) docker     (123)   159933 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/application_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)    23224 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    42341 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)   235385 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    43957 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)   334882 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    44496 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/
+-rw-r--r--   0 runner    (1001) docker     (123)   122384 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.584193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:31:10.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:29.580193 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:31:29.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 11:31:29.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:31:29.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:31:29.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 11:31:29.000000 cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/LICENSE` & `cdktf-cdktf-provider-oraclepaas-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/PKG-INFO` & `cdktf-cdktf-provider-oraclepaas-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-oraclepaas
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt oraclepaas Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-oraclepaas.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-oraclepaas.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/README.md` & `cdktf-cdktf-provider-oraclepaas-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/setup.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-oraclepaas",
-    "version": "4.0.1",
+    "version": "5.0.0",
     "description": "Prebuilt oraclepaas Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-oraclepaas.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -31,25 +31,25 @@
         "cdktf_cdktf_provider_oraclepaas.java_service_instance",
         "cdktf_cdktf_provider_oraclepaas.mysql_access_rule",
         "cdktf_cdktf_provider_oraclepaas.mysql_service_instance",
         "cdktf_cdktf_provider_oraclepaas.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_oraclepaas._jsii": [
-            "provider-oraclepaas@4.0.1.jsii.tgz"
+            "provider-oraclepaas@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_oraclepaas": [
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

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/application_container/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/application_container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_access_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/database_service_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_access_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/java_service_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/mysql_service_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas/provider/__init__.py` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/PKG-INFO` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-oraclepaas
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt oraclepaas Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-oraclepaas.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-oraclepaas.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-oraclepaas-4.0.1/src/cdktf_cdktf_provider_oraclepaas.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-oraclepaas-5.0.0/src/cdktf_cdktf_provider_oraclepaas.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_oraclepaas/py.typed
 src/cdktf_cdktf_provider_oraclepaas.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_oraclepaas.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_oraclepaas.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_oraclepaas.egg-info/requires.txt
 src/cdktf_cdktf_provider_oraclepaas.egg-info/top_level.txt
 src/cdktf_cdktf_provider_oraclepaas/_jsii/__init__.py
-src/cdktf_cdktf_provider_oraclepaas/_jsii/provider-oraclepaas@4.0.1.jsii.tgz
+src/cdktf_cdktf_provider_oraclepaas/_jsii/provider-oraclepaas@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_oraclepaas/application_container/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/data_oraclepaas_database_service_instance/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/database_access_rule/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/database_service_instance/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/java_access_rule/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/java_service_instance/__init__.py
 src/cdktf_cdktf_provider_oraclepaas/mysql_access_rule/__init__.py
```

