# Comparing `tmp/projen-0.71.96.tar.gz` & `tmp/projen-0.71.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.71.96.tar", last modified: Wed Jun 14 12:46:54 2023, max compression
+gzip compressed data, was "projen-0.71.97.tar", last modified: Thu Jun 15 12:34:29 2023, max compression
```

## Comparing `projen-0.71.96.tar` & `projen-0.71.97.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.312811 projen-0.71.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 12:46:42.000000 projen-0.71.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 12:46:42.000000 projen-0.71.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-14 12:46:54.308811 projen-0.71.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-14 12:46:42.000000 projen-0.71.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 12:46:42.000000 projen-0.71.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:46:54.312811 projen-0.71.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-14 12:46:42.000000 projen-0.71.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.296811 projen-0.71.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.300811 projen-0.71.96/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.300811 projen-0.71.96/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  2715416 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/_jsii/projen@0.71.96.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.304811 projen-0.71.96/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.308811 projen-0.71.96/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-14 12:46:42.000000 projen-0.71.96/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:46:54.300811 projen-0.71.96/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-14 12:46:54.000000 projen-0.71.96/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 12:46:54.000000 projen-0.71.96/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:46:54.000000 projen-0.71.96/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 12:46:54.000000 projen-0.71.96/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 12:46:54.000000 projen-0.71.96/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.747825 projen-0.71.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-15 12:34:16.000000 projen-0.71.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 12:34:16.000000 projen-0.71.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-15 12:34:29.747825 projen-0.71.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-15 12:34:16.000000 projen-0.71.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 12:34:16.000000 projen-0.71.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:34:29.747825 projen-0.71.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-15 12:34:16.000000 projen-0.71.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.731825 projen-0.71.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.735825 projen-0.71.97/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.735825 projen-0.71.97/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.739825 projen-0.71.97/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  2731613 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/_jsii/projen@0.71.97.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.739825 projen-0.71.97/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.739825 projen-0.71.97/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.739825 projen-0.71.97/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.739825 projen-0.71.97/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.743825 projen-0.71.97/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.747825 projen-0.71.97/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-15 12:34:16.000000 projen-0.71.97/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:34:29.735825 projen-0.71.97/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-15 12:34:29.000000 projen-0.71.97/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-15 12:34:29.000000 projen-0.71.97/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:34:29.000000 projen-0.71.97/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 12:34:29.000000 projen-0.71.97/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 12:34:29.000000 projen-0.71.97/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.71.96/LICENSE` & `projen-0.71.97/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/PKG-INFO` & `projen-0.71.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.96
+Version: 0.71.97
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.96/README.md` & `projen-0.71.97/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/setup.py` & `projen-0.71.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.71.96",
+    "version": "0.71.97",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.71.96.jsii.tgz"
+            "projen@0.71.97.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.71.96/src/projen/__init__.py` & `projen-0.71.97/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/awscdk/__init__.py` & `projen-0.71.97/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/build/__init__.py` & `projen-0.71.97/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/cdk/__init__.py` & `projen-0.71.97/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/cdk8s/__init__.py` & `projen-0.71.97/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/cdktf/__init__.py` & `projen-0.71.97/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/circleci/__init__.py` & `projen-0.71.97/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/github/__init__.py` & `projen-0.71.97/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/github/workflows/__init__.py` & `projen-0.71.97/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/gitlab/__init__.py` & `projen-0.71.97/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/java/__init__.py` & `projen-0.71.97/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/javascript/__init__.py` & `projen-0.71.97/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/python/__init__.py` & `projen-0.71.97/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/release/__init__.py` & `projen-0.71.97/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/typescript/__init__.py` & `projen-0.71.97/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/vscode/__init__.py` & `projen-0.71.97/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen/web/__init__.py` & `projen-0.71.97/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.96/src/projen.egg-info/PKG-INFO` & `projen-0.71.97/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.96
+Version: 0.71.97
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.96/src/projen.egg-info/SOURCES.txt` & `projen-0.71.97/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.71.96.jsii.tgz
+src/projen/_jsii/projen@0.71.97.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

