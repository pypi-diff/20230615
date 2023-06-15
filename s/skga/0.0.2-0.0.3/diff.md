# Comparing `tmp/skga-0.0.2.tar.gz` & `tmp/skga-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.2.tar", last modified: Thu Jun  1 19:44:22 2023, max compression
+gzip compressed data, was "skga-0.0.3.tar", last modified: Thu Jun 15 11:44:32 2023, max compression
```

## Comparing `skga-0.0.2.tar` & `skga-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.774374 skga-0.0.2/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.2/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:44:22.774173 skga-0.0.2/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.2/README.md
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.771528 skga-0.0.2/hbrkga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       69 2023-06-01 19:42:30.000000 skga-0.0.2/hbrkga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/data_utils.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7569 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     7803 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_BO_only_elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     3929 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_random_search.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2866 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-BO-only-elites.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2550 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-BO.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2560 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-randomwalk.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     1306 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/nn_decoder_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     5043 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/nn_instance_PT.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.2/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-01 19:44:22.774454 skga-0.0.2/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2392 2023-06-01 19:44:16.000000 skga-0.0.2/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.772549 skga-0.0.2/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       43 2023-06-01 19:21:11.000000 skga-0.0.2/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8183 2023-05-07 22:04:48.000000 skga-0.0.2/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.2/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.773812 skga-0.0.2/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      511 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)       12 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.461080 skga-0.0.3/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.3/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 11:44:32.460910 skga-0.0.3/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.3/README.md
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.458829 skga-0.0.3/hbrkga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:53:29.000000 skga-0.0.3/hbrkga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/data_utils.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7569 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7803 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_BO_only_elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3929 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/exploitation_method_random_search.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2866 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-BO-only-elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2550 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2560 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/main-randomwalk.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1306 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/nn_decoder_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5043 2023-05-07 22:04:48.000000 skga-0.0.3/hbrkga/nn_instance_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-01 19:48:13.000000 skga-0.0.3/hbrkga/test.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.3/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 11:44:32.461140 skga-0.0.3/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2392 2023-06-15 11:43:56.000000 skga-0.0.3/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.459693 skga-0.0.3/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       43 2023-06-01 19:55:19.000000 skga-0.0.3/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8879 2023-06-15 11:40:44.000000 skga-0.0.3/skga/adaptee.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.3/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 11:44:32.460675 skga-0.0.3/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      526 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)       12 2023-06-15 11:44:32.000000 skga-0.0.3/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.2/LICENSE` & `skga-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/PKG-INFO` & `skga-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.2
+Version: 0.0.3
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.2/README.md` & `skga-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/data_utils.py` & `skga-0.0.3/hbrkga/data_utils.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/exploitation_method_BO.py` & `skga-0.0.3/hbrkga/exploitation_method_BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/exploitation_method_BO_only_elites.py` & `skga-0.0.3/hbrkga/exploitation_method_BO_only_elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/exploitation_method_random_search.py` & `skga-0.0.3/hbrkga/exploitation_method_random_search.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/main-BO-only-elites.py` & `skga-0.0.3/hbrkga/main-BO-only-elites.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/main-BO.py` & `skga-0.0.3/hbrkga/main-BO.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/main-randomwalk.py` & `skga-0.0.3/hbrkga/main-randomwalk.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/nn_decoder_PT.py` & `skga-0.0.3/hbrkga/nn_decoder_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/hbrkga/nn_instance_PT.py` & `skga-0.0.3/hbrkga/nn_instance_PT.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/pyproject.toml` & `skga-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/setup.py` & `skga-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.2",
+    version="0.0.3",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
```

### Comparing `skga-0.0.2/skga/adaptee.py` & `skga-0.0.3/skga/adaptee.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sklearn.model_selection._validation import cross_val_score
 from sklearn.utils import indexable
 from sklearn.utils.validation import _check_fit_params
 
 from hbrkga.brkga_mp_ipr.algorithm import BrkgaMpIpr
 from hbrkga.brkga_mp_ipr.enums import Sense
 from hbrkga.brkga_mp_ipr.types import BaseChromosome
-from hbrkga.brkga_mp_ipr.types_io import load_configuration
+from hbrkga.brkga_mp_ipr.types_io import load_configuration, load_configuration_from_dict
 from hbrkga.exploitation_method_BO_only_elites import BayesianOptimizerElites
 
 
 class Decoder:
 
     def __init__(self, parameters, estimator, X, y, cv):
         self._parameters = parameters
@@ -99,16 +99,32 @@
             pre_dispatch=pre_dispatch,
             error_score=error_score,
             return_train_score=return_train_score,
         )
         if brkga_params is not None:
             self.brkga_config, _ = brkga_params
         else:
-            self.brkga_config, _ = load_configuration("../../hbrkga/config.conf")
-
+            self.brkga_config , _ = load_configuration_from_dict({
+                'population_size': 10,
+                'elite_percentage': 0.3,
+                'mutants_percentage': 0.3,
+                'num_elite_parents': 1,
+                'total_parents': 2,
+                'bias_type': 'LOGINVERSE',
+                'num_independent_populations': 1,
+                'pr_number_pairs': 0,
+                'pr_minimum_distance': 0.15,
+                'pr_type': 'PERMUTATION',
+                'pr_selection': 'BESTSOLUTION',
+                'alpha_block_size': 1.0,
+                'pr_percentage': 1.0,
+                'exchange_interval': 0,
+                'num_exchange_indivuduals': 0,
+                'reset_interval': 0
+            })
         self._parameters = parameters
 
         self.decoder = Decoder(self._parameters, estimator, data, target, cv)
         elite_number = int(self.brkga_config.elite_percentage * self.brkga_config.population_size)
 
         if exploit_method is not None:
             self.em = exploit_method(self.decoder, percentage=0.6, eliteNumber=elite_number)
```

### Comparing `skga-0.0.2/skga/main.py` & `skga-0.0.3/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.2/skga.egg-info/PKG-INFO` & `skga-0.0.3/skga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.2
+Version: 0.0.3
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.2/skga.egg-info/requires.txt` & `skga-0.0.3/skga.egg-info/requires.txt`

 * *Files identical despite different names*

