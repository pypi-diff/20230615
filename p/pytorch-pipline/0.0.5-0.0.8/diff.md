# Comparing `tmp/pytorch-pipline-0.0.5.tar.gz` & `tmp/pytorch-pipline-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pipline-0.0.5.tar", last modified: Thu Jun 15 06:17:45 2023, max compression
+gzip compressed data, was "pytorch-pipline-0.0.8.tar", last modified: Thu Jun 15 07:10:43 2023, max compression
```

## Comparing `pytorch-pipline-0.0.5.tar` & `pytorch-pipline-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:17:45.477110 pytorch-pipline-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 06:17:45.473110 pytorch-pipline-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 06:17:35.000000 pytorch-pipline-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:17:45.473110 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 06:17:45.000000 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 06:17:45.000000 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:17:45.000000 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 06:17:45.000000 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:17:45.000000 pytorch-pipline-0.0.5/pytorch_pipline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:17:45.477110 pytorch-pipline-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 06:17:35.000000 pytorch-pipline-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:43.448771 pytorch-pipline-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:10:43.448771 pytorch-pipline-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 07:10:26.000000 pytorch-pipline-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:43.448771 pytorch-pipline-0.0.8/pytorchPipline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-15 07:10:26.000000 pytorch-pipline-0.0.8/pytorchPipline/BenchMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-15 07:10:26.000000 pytorch-pipline-0.0.8/pytorchPipline/Pipline.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 07:10:26.000000 pytorch-pipline-0.0.8/pytorchPipline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:10:43.448771 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:10:43.000000 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 07:10:43.000000 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:10:43.000000 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 07:10:43.000000 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 07:10:43.000000 pytorch-pipline-0.0.8/pytorch_pipline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:10:43.448771 pytorch-pipline-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 07:10:26.000000 pytorch-pipline-0.0.8/setup.py
```

### Comparing `pytorch-pipline-0.0.5/PKG-INFO` & `pytorch-pipline-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.0.5
+Version: 0.0.8
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.0.5/pytorch_pipline.egg-info/PKG-INFO` & `pytorch-pipline-0.0.8/pytorch_pipline.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.0.5
+Version: 0.0.8
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.0.5/setup.py` & `pytorch-pipline-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.8'
 DESCRIPTION = 'Making pytorch training easier'
 LONG_DESCRIPTION = 'A package that has functions making the training loop faster to write'
 
 # Setting up
 setup(
     name="pytorch-pipline",
     version=VERSION,
```

