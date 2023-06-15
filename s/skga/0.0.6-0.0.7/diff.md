# Comparing `tmp/skga-0.0.6.tar.gz` & `tmp/skga-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.6.tar", last modified: Thu Jun 15 13:31:10 2023, max compression
+gzip compressed data, was "skga-0.0.7.tar", last modified: Thu Jun 15 16:12:26 2023, max compression
```

## Comparing `skga-0.0.6.tar` & `skga-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.373540 skga-0.0.6/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.6/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:31:10.373335 skga-0.0.6/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.6/README.md
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.6/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 13:31:10.373613 skga-0.0.6/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2382 2023-06-15 13:31:06.000000 skga-0.0.6/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.371994 skga-0.0.6/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.6/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8663 2023-06-15 13:13:31.000000 skga-0.0.6/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.6/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.373048 skga-0.0.6/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.978668 skga-0.0.7/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.7/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:12:26.978490 skga-0.0.7/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.7/README.md
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.7/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 16:12:26.978750 skga-0.0.7/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2382 2023-06-15 16:12:09.000000 skga-0.0.7/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.977173 skga-0.0.7/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.7/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8659 2023-06-15 16:10:12.000000 skga-0.0.7/skga/adaptee.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.7/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.978217 skga-0.0.7/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.6/LICENSE` & `skga-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.6/PKG-INFO` & `skga-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.6
+Version: 0.0.7
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.6/README.md` & `skga-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.6/pyproject.toml` & `skga-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.6/setup.py` & `skga-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.6",
+    version="0.0.7",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
```

### Comparing `skga-0.0.6/skga/adaptee.py` & `skga-0.0.7/skga/adaptee.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sklearn.metrics._scorer import _check_multimetric_scoring
 from sklearn.model_selection import check_cv
 from sklearn.model_selection._search import BaseSearchCV, ParameterGrid
 from sklearn.model_selection._validation import cross_val_score
 from sklearn.utils import indexable
 from sklearn.utils.validation import _check_fit_params
 
-from skga.hbrkga import BrkgaMpIpr, Sense, BaseChromosome, load_configuration_from_dict, BayesianOptimizerElites
+from .hbrkga import BrkgaMpIpr, Sense, BaseChromosome, load_configuration_from_dict, BayesianOptimizerElites
 
 class Decoder:
 
     def __init__(self, parameters, estimator, X, y, cv):
         self._parameters = parameters
         self._estimator = estimator
         self._X = X
```

### Comparing `skga-0.0.6/skga/main.py` & `skga-0.0.7/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.6/skga.egg-info/PKG-INFO` & `skga-0.0.7/skga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.6
+Version: 0.0.7
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.6/skga.egg-info/requires.txt` & `skga-0.0.7/skga.egg-info/requires.txt`

 * *Files identical despite different names*

