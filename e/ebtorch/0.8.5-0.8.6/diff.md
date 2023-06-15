# Comparing `tmp/ebtorch-0.8.5.tar.gz` & `tmp/ebtorch-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.8.5.tar", last modified: Sun May 14 01:11:26 2023, max compression
+gzip compressed data, was "ebtorch-0.8.6.tar", last modified: Thu Jun 15 14:37:30 2023, max compression
```

## Comparing `ebtorch-0.8.5.tar` & `ebtorch-0.8.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-14 01:11:15.000000 ebtorch-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-14 01:11:26.580222 ebtorch-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-14 01:11:15.000000 ebtorch-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/lmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:11:26.580222 ebtorch-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-14 01:11:15.000000 ebtorch-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.452027 ebtorch-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-15 14:37:15.000000 ebtorch-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 14:37:30.452027 ebtorch-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-15 14:37:15.000000 ebtorch-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.440027 ebtorch-0.8.6/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.444027 ebtorch-0.8.6/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/lmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.448027 ebtorch-0.8.6/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-15 14:37:15.000000 ebtorch-0.8.6/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:37:30.444027 ebtorch-0.8.6/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 14:37:30.000000 ebtorch-0.8.6/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:37:30.452027 ebtorch-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 14:37:15.000000 ebtorch-0.8.6/setup.py
```

### Comparing `ebtorch-0.8.5/LICENSE` & `ebtorch-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/PKG-INFO` & `ebtorch-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.5
+Version: 0.8.6
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.5 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.8.6 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.5/ebtorch/__init__.py` & `ebtorch-0.8.6/ebtorch/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,11 +73,12 @@
 del AdaHessian
 del Adan
 del Lion
 del Lookahead
 del RAdam
 del SAM
 del ralah_optim
+del wfneal
 
 # Deletions (from .logging)
 del AverageMeter
 del LogCSV
```

### Comparing `ebtorch-0.8.5/ebtorch/logging/__init__.py` & `ebtorch-0.8.6/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/logging/avgmeter.py` & `ebtorch-0.8.6/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/logging/logcsv.py` & `ebtorch-0.8.6/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/__init__.py` & `ebtorch-0.8.6/ebtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/architectures.py` & `ebtorch-0.8.6/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/conv2drp.py` & `ebtorch-0.8.6/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.8.6/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/coordconv.py` & `ebtorch-0.8.6/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/debuglayers.py` & `ebtorch-0.8.6/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/fieldtransform.py` & `ebtorch-0.8.6/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/functional/__init__.py` & `ebtorch-0.8.6/ebtorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.8.6/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/kwta.py` & `ebtorch-0.8.6/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/laplacenet.py` & `ebtorch-0.8.6/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/lmu.py` & `ebtorch-0.8.6/ebtorch/nn/lmu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/mish.py` & `ebtorch-0.8.6/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/nnsemble.py` & `ebtorch-0.8.6/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/reshapelayers.py` & `ebtorch-0.8.6/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/serf.py` & `ebtorch-0.8.6/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/serlu.py` & `ebtorch-0.8.6/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/sinlu.py` & `ebtorch-0.8.6/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/smelu.py` & `ebtorch-0.8.6/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/__init__.py` & `ebtorch-0.8.6/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.8.6/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.8.6/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.8.6/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/patches.py` & `ebtorch-0.8.6/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.8.6/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/__init__.py` & `ebtorch-0.8.6/ebtorch/optim/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 # Imports (specific)
 from .adahessian import AdaHessian
 from .adan import Adan
 from .custom import ralah_optim
+from .custom import wfneal
 from .lion import Lion
 from .lookahead import Lookahead
 from .radam import RAdam
 from .sam import SAM
 
 # Deletions (from .)
 del adahessian
```

### Comparing `ebtorch-0.8.5/ebtorch/optim/adahessian.py` & `ebtorch-0.8.6/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/adan.py` & `ebtorch-0.8.6/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/lion.py` & `ebtorch-0.8.6/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/lookahead.py` & `ebtorch-0.8.6/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/radam.py` & `ebtorch-0.8.6/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch/optim/sam.py` & `ebtorch-0.8.6/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.8.6/ebtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.5
+Version: 0.8.6
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.5 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.8.6 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.5/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.8.6/ebtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.5/setup.py` & `ebtorch-0.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 
 check_dependencies()
 
 
 setup(
     name="ebtorch",
-    version="0.8.5",
+    version="0.8.6",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
```

