# Comparing `tmp/autogluon-0.7.1b20230614.tar.gz` & `tmp/autogluon-0.8.0b20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230614.tar", last modified: Wed Jun 14 09:04:24 2023, max compression
+gzip compressed data, was "autogluon-0.8.0b20230615.tar", last modified: Thu Jun 15 09:04:36 2023, max compression
```

## Comparing `autogluon-0.7.1b20230614.tar` & `autogluon-0.8.0b20230615.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:04:24.198775 autogluon-0.7.1b20230614/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-14 09:03:34.000000 autogluon-0.7.1b20230614/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:03:34.000000 autogluon-0.7.1b20230614/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:24.194775 autogluon-0.7.1b20230614/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:24.000000 autogluon-0.7.1b20230614/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.669564 autogluon-0.8.0b20230615/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:04:36.669564 autogluon-0.8.0b20230615/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-15 09:03:44.000000 autogluon-0.8.0b20230615/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:03:44.000000 autogluon-0.8.0b20230615/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:36.665564 autogluon-0.8.0b20230615/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:36.000000 autogluon-0.8.0b20230615/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230614/PKG-INFO` & `autogluon-0.8.0b20230615/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230614
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -32,15 +32,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.7.0
+        # pip install autogluon  # autogluon==0.8.0
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

### Comparing `autogluon-0.7.1b20230614/setup.py` & `autogluon-0.8.0b20230615/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230614/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.0b20230615/src/autogluon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230614
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -32,15 +32,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.7.0
+        # pip install autogluon  # autogluon==0.8.0
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

