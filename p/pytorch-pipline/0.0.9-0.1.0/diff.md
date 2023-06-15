# Comparing `tmp/pytorch-pipline-0.0.9.tar.gz` & `tmp/pytorch-pipline-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pipline-0.0.9.tar", last modified: Thu Jun 15 07:17:59 2023, max compression
+gzip compressed data, was "pytorch-pipline-0.1.0.tar", last modified: Thu Jun 15 07:57:13 2023, max compression
```

## Comparing `pytorch-pipline-0.0.9.tar` & `pytorch-pipline-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:17:59.204885 pytorch-pipline-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:17:59.204885 pytorch-pipline-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 07:17:47.000000 pytorch-pipline-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:17:59.200885 pytorch-pipline-0.0.9/pytorchPipline/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-15 07:17:47.000000 pytorch-pipline-0.0.9/pytorchPipline/BenchMark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-15 07:17:47.000000 pytorch-pipline-0.0.9/pytorchPipline/Pipline.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 07:17:47.000000 pytorch-pipline-0.0.9/pytorchPipline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:17:59.204885 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:17:59.000000 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 07:17:59.000000 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:17:59.000000 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 07:17:59.000000 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 07:17:59.000000 pytorch-pipline-0.0.9/pytorch_pipline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:17:59.204885 pytorch-pipline-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 07:17:47.000000 pytorch-pipline-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:13.863031 pytorch-pipline-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:57:13.863031 pytorch-pipline-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 07:57:04.000000 pytorch-pipline-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:13.863031 pytorch-pipline-0.1.0/pytorchPipline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-15 07:57:04.000000 pytorch-pipline-0.1.0/pytorchPipline/BenchMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-15 07:57:04.000000 pytorch-pipline-0.1.0/pytorchPipline/Pipline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 07:57:04.000000 pytorch-pipline-0.1.0/pytorchPipline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:57:13.863031 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 07:57:13.000000 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 07:57:13.000000 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:57:13.000000 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 07:57:13.000000 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 07:57:13.000000 pytorch-pipline-0.1.0/pytorch_pipline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:57:13.863031 pytorch-pipline-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 07:57:04.000000 pytorch-pipline-0.1.0/setup.py
```

### Comparing `pytorch-pipline-0.0.9/PKG-INFO` & `pytorch-pipline-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.0.9
+Version: 0.1.0
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.0.9/pytorchPipline/BenchMark.py` & `pytorch-pipline-0.1.0/pytorchPipline/BenchMark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from torch.utils.data import Dataset, DataLoader
 from torchvision import datasets
 import torch.nn as nn
 import torch.optim as optim
 from torchvision import transforms
-from Pipline import TrainModel, TestModel, FitModel
+from pytorchPipline.Pipline import TrainModel, TestModel, FitModel
 from timeit import default_timer as timer
 
 def BenchMark(epoch=10):
     start = timer()
     trainLoader = datasets.MNIST(
         root="./",
         train=True,
```

### Comparing `pytorch-pipline-0.0.9/pytorchPipline/Pipline.py` & `pytorch-pipline-0.1.0/pytorchPipline/Pipline.py`

 * *Files identical despite different names*

### Comparing `pytorch-pipline-0.0.9/pytorch_pipline.egg-info/PKG-INFO` & `pytorch-pipline-0.1.0/pytorch_pipline.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.0.9
+Version: 0.1.0
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.0.9/setup.py` & `pytorch-pipline-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Making pytorch training easier'
 LONG_DESCRIPTION = 'A package that has functions making the training loop faster to write'
 
 # Setting up
 setup(
     name="pytorch-pipline",
     version=VERSION,
```

