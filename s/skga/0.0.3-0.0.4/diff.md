# Comparing `tmp/skga-0.0.3.tar.gz` & `tmp/skga-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.3.tar", last modified: Thu Jun 15 11:44:32 2023, max compression
+gzip compressed data, was "skga-0.0.4.tar", last modified: Thu Jun 15 12:13:54 2023, max compression
```

## Comparing `skga-0.0.3.tar` & `skga-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.461080 skga-0.0.3/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.3/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 11:44:32.460910 skga-0.0.3/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.3/README.md
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.458829 skga-0.0.3/hbrkga/
--rw-r--r--   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:53:29.000000 skga-0.0.3/hbrkga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/data_utils.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7569 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7803 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_BO_only_elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     3929 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_random_search.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2866 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-BO-only-elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2550 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2560 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-randomwalk.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     1306 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/nn_decoder_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     5043 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/nn_instance_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-01 19:48:13.000000 skga-0.0.3/hbrkga/test.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.3/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 11:44:32.461140 skga-0.0.3/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2392 2023-06-15 11:43:56.000000 skga-0.0.3/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.459693 skga-0.0.3/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       43 2023-06-01 19:55:19.000000 skga-0.0.3/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8879 2023-06-15 11:40:44.000000 skga-0.0.3/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.3/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.460675 skga-0.0.3/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      526 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)       12 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 12:13:54.778425 skga-0.0.4/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.4/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 12:13:54.778230 skga-0.0.4/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.4/README.md
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 12:13:54.775959 skga-0.0.4/hbrkga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)      337 2023-06-15 12:06:49.000000 skga-0.0.4/hbrkga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/data_utils.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7569 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/exploitation_method_BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7803 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/exploitation_method_BO_only_elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3929 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/exploitation_method_random_search.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2866 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/main-BO-only-elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2550 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/main-BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2560 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/main-randomwalk.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1306 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/nn_decoder_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5043 2023-05-07 22:04:48.000000 skga-0.0.4/hbrkga/nn_instance_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-01 19:48:13.000000 skga-0.0.4/hbrkga/test.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.4/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 12:13:54.778493 skga-0.0.4/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2392 2023-06-15 12:13:47.000000 skga-0.0.4/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 12:13:54.776926 skga-0.0.4/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.4/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8668 2023-06-15 12:08:02.000000 skga-0.0.4/skga/adaptee.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.4/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 12:13:54.777961 skga-0.0.4/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 12:13:54.000000 skga-0.0.4/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      526 2023-06-15 12:13:54.000000 skga-0.0.4/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 12:13:54.000000 skga-0.0.4/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 12:13:54.000000 skga-0.0.4/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)       12 2023-06-15 12:13:54.000000 skga-0.0.4/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.3/LICENSE` & `skga-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/PKG-INFO` & `skga-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.3
+Version: 0.0.4
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.3/README.md` & `skga-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/data_utils.py` & `skga-0.0.4/hbrkga/data_utils.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/exploitation_method_BO.py` & `skga-0.0.4/hbrkga/exploitation_method_BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/exploitation_method_BO_only_elites.py` & `skga-0.0.4/hbrkga/exploitation_method_BO_only_elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/exploitation_method_random_search.py` & `skga-0.0.4/hbrkga/exploitation_method_random_search.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/main-BO-only-elites.py` & `skga-0.0.4/hbrkga/main-BO-only-elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/main-BO.py` & `skga-0.0.4/hbrkga/main-BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/main-randomwalk.py` & `skga-0.0.4/hbrkga/main-randomwalk.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/nn_decoder_PT.py` & `skga-0.0.4/hbrkga/nn_decoder_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/hbrkga/nn_instance_PT.py` & `skga-0.0.4/hbrkga/nn_instance_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/pyproject.toml` & `skga-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/setup.py` & `skga-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.3",
+    version="0.0.4",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
```

### Comparing `skga-0.0.3/skga/adaptee.py` & `skga-0.0.4/skga/adaptee.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 from sklearn.metrics._scorer import _check_multimetric_scoring
 from sklearn.model_selection import check_cv
 from sklearn.model_selection._search import BaseSearchCV, ParameterGrid
 from sklearn.model_selection._validation import cross_val_score
 from sklearn.utils import indexable
 from sklearn.utils.validation import _check_fit_params
 
-from hbrkga.brkga_mp_ipr.algorithm import BrkgaMpIpr
-from hbrkga.brkga_mp_ipr.enums import Sense
-from hbrkga.brkga_mp_ipr.types import BaseChromosome
-from hbrkga.brkga_mp_ipr.types_io import load_configuration, load_configuration_from_dict
-from hbrkga.exploitation_method_BO_only_elites import BayesianOptimizerElites
-
+from hbrkga import BrkgaMpIpr, Sense, BaseChromosome, load_configuration_from_dict, BayesianOptimizerElites
 
 class Decoder:
 
     def __init__(self, parameters, estimator, X, y, cv):
         self._parameters = parameters
         self._estimator = estimator
         self._X = X
```

### Comparing `skga-0.0.3/skga/main.py` & `skga-0.0.4/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/skga.egg-info/PKG-INFO` & `skga-0.0.4/skga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.3
+Version: 0.0.4
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.3/skga.egg-info/SOURCES.txt` & `skga-0.0.4/skga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skga-0.0.3/skga.egg-info/requires.txt` & `skga-0.0.4/skga.egg-info/requires.txt`

 * *Files identical despite different names*

