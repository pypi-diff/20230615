# Comparing `tmp/mafese-0.1.4.tar.gz` & `tmp/mafese-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.4.tar", last modified: Thu Jun  1 14:58:30 2023, max compression
+gzip compressed data, was "mafese-0.1.5.tar", last modified: Thu Jun 15 09:52:38 2023, max compression
```

## Comparing `mafese-0.1.4.tar` & `mafese-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-01 14:57:37.000000 mafese-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 14:57:37.000000 mafese-0.1.4/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 14:57:37.000000 mafese-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 14:57:37.000000 mafese-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-01 14:58:30.515283 mafese-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-06-01 14:57:37.000000 mafese-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-01 14:57:37.000000 mafese-0.1.4/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 14:58:30.000000 mafese-0.1.4/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:58:30.515283 mafese-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-01 14:57:37.000000 mafese-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:58:30.515283 mafese-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-01 14:57:37.000000 mafese-0.1.4/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.781912 mafese-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-15 09:51:23.000000 mafese-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-15 09:51:23.000000 mafese-0.1.5/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 09:51:23.000000 mafese-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 09:51:23.000000 mafese-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-15 09:52:38.781912 mafese-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-15 09:51:23.000000 mafese-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.773912 mafese-0.1.5/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-15 09:51:23.000000 mafese-0.1.5/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:52:38.781912 mafese-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-15 09:51:24.000000 mafese-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_wrapper.py
```

### Comparing `mafese-0.1.4/CODE_OF_CONDUCT.md` & `mafese-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/ChangeLog.md` & `mafese-0.1.5/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+# Version 0.1.5
+
++ Add more regression and classification datasets
++ Update documents, examples, test
++ Remove matplotlib dependency
+
+---------------------------------------------------------------------
+
 # Version 0.1.4
 
-+ Relocate regression and classification datasets
 + Add Unsupervised-based methods:
   - "VAR": Variance Threshold method
   - "MAD": Mean Absolute Difference
   - "DR": Dispersion Ratio
   - "MCL": Multicollinearity method based on Variance Inflation Factor (VIF) value
 + Update documents, examples, test
 + Remove matplotlib dependency
```

### Comparing `mafese-0.1.4/LICENSE` & `mafese-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/PKG-INFO` & `mafese-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.4
+Version: 0.1.5
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.5-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -60,37 +60,37 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 3 datasets
+* **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.4
+$ pip install mafese==0.1.5
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -255,16 +255,15 @@
 ```
 
 
 Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
 
 ```python
 from mafese.wrapper.mha import MhaSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
 # define mafese feature selection method
@@ -292,16 +291,15 @@
 ```
 
 
 Or, use Lasso-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.lasso import LassoSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -328,16 +326,15 @@
 ```
 
 
 Or, use Tree-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.tree import TreeSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -367,15 +364,15 @@
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
-from mafese import Data, get_dataset
+from mafese import Data, get_dataset, evaluator
 from mafese import FilterSelector
 from mafese import SequentialSelector, RecursiveSelector, MhaSelector
 from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
@@ -422,9 +419,12 @@
 
 ```code 
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-```
+6.  https://elki-project.github.io/
+7. https://sci2s.ugr.es/keel/index.php
+8. https://archive.ics.uci.edu/datasets
 
+```
```

### Comparing `mafese-0.1.4/README.md` & `mafese-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.5-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -17,37 +17,37 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 3 datasets
+* **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.4
+$ pip install mafese==0.1.5
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -212,16 +212,15 @@
 ```
 
 
 Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
 
 ```python
 from mafese.wrapper.mha import MhaSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
 # define mafese feature selection method
@@ -249,16 +248,15 @@
 ```
 
 
 Or, use Lasso-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.lasso import LassoSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -285,16 +283,15 @@
 ```
 
 
 Or, use Tree-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.tree import TreeSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -324,15 +321,15 @@
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
-from mafese import Data, get_dataset
+from mafese import Data, get_dataset, evaluator
 from mafese import FilterSelector
 from mafese import SequentialSelector, RecursiveSelector, MhaSelector
 from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
@@ -379,9 +376,12 @@
 
 ```code 
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-```
+6.  https://elki-project.github.io/
+7. https://sci2s.ugr.es/keel/index.php
+8. https://archive.ics.uci.edu/datasets
 
+```
```

### Comparing `mafese-0.1.4/mafese/__init__.py` & `mafese-0.1.5/mafese/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
 from mafese.wrapper.mha import MhaSelector
 from mafese.embedded.lasso import LassoSelector
```

### Comparing `mafese-0.1.4/mafese/embedded/lasso.py` & `mafese-0.1.5/mafese/embedded/lasso.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/embedded/tree.py` & `mafese-0.1.5/mafese/embedded/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     Defines a TreeSelector class that hold all Tree-based Feature Selection methods for feature selection problems
 
     Parameters
     ----------
     problem: str, default = "classification"
         The problem you are trying to solve (or type of dataset), "classification" or "regression"
 
-    estimator: str, default = 'lasso'
+    estimator: str, default = 'tree'
         We are currently support:
-            - lasso: lasso estimator (both regression and classification)
-            - lr: Logistic Regression (classification)
-            - svm: LinearSVC, support vector machine (classification)
+            - rf: random forest
+            - adaboost: AdaBoost
+            - xgb: Gradient Boosting
+            - tree: Extra Trees
 
     estimator_paras: None or dict, default = None
         The parameters of the estimator, please see the official document of scikit-learn to selected estimator.
         If None, we use the best parameter for selected estimator
 
     threshold : str or float, default=None
         The threshold value to use for feature selection. Features whose absolute importance value is greater or equal
@@ -78,14 +79,15 @@
     """
 
     SUPPORTED_ESTIMATORS = ["rf", "adaboost", "xgb", "tree"]
 
     def __init__(self, problem="classification", estimator="tree", estimator_paras=None, threshold=None, norm_order=1, max_features=None):
         super().__init__(problem)
         self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator_paras = estimator_paras
         self.threshold = threshold
         self.norm_order = norm_order
         self.max_features = max_features
         self.selector = SelectFromModel(estimator=self.estimator, threshold=self.threshold, prefit=False,
                                         norm_order=self.norm_order, max_features=self.max_features)
 
     def set_estimator(self, estimator=None, paras=None):
```

### Comparing `mafese-0.1.4/mafese/evaluator.py` & `mafese-0.1.5/mafese/evaluator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/filter.py` & `mafese-0.1.5/mafese/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # Created by "Thieu" at 22:14, 24/05/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mafese.selector import Selector
-from mafese.utils import validator
-from mafese.utils import correlation
+from mafese.utils import validator, correlation
 
 
 class FilterSelector(Selector):
     """
     Defines a FilterSelector class that hold all filter methods for feature selection problems
 
     Parameters
```

### Comparing `mafese-0.1.4/mafese/selector.py` & `mafese-0.1.5/mafese/selector.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/unsupervised.py` & `mafese-0.1.5/mafese/unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/correlation.py` & `mafese-0.1.5/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/data_loader.py` & `mafese-0.1.5/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/encoder.py` & `mafese-0.1.5/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/estimator.py` & `mafese-0.1.5/mafese/utils/estimator.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,60 +2,94 @@
 # Created by "Thieu" at 15:43, 24/05/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 from sklearn.svm import SVC, SVR, LinearSVC
 from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
-from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
-from sklearn.linear_model import Lasso, LogisticRegression, LinearRegression
+from sklearn.neural_network import MLPRegressor, MLPClassifier
+from sklearn.linear_model import Lasso, LogisticRegression, LinearRegression, BayesianRidge, Perceptron
+from sklearn.ensemble import ExtraTreesRegressor, RandomForestRegressor, AdaBoostRegressor, GradientBoostingRegressor
+from sklearn.ensemble import ExtraTreesClassifier, RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier
 
 
-def get_classifier(name):
-    name = name.lower()
-    if name == 'knn':
-        return KNeighborsClassifier()
-    elif name == 'rf':
-        return RandomForestClassifier()
-    elif name == 'svm':
-        return SVC()
-    else:
-        raise ValueError(f"Currently, MAFESE doesn't support: {name} classifier. You can define your own scikit-learn model.")
-
-
-def get_regressor(name):
-    name = name.lower()
-    if name == "knn":
-        return KNeighborsRegressor()
-    elif name == "rf":
-        return RandomForestRegressor()
-    elif name == "svm":
-        return SVR()
-    else:
-        raise ValueError(f"Currently, we don't support: {name} regressor. You can define your own scikit-learn model.")
-
-
-def get_classifier_for_recursive(name):
+def get_general_estimator(problem, name, paras=None):
+    if paras is None:
+        paras = {}
     name = name.lower()
-    if name == 'rf':
-        return RandomForestClassifier()
-    elif name == 'svm':
-        return SVC(kernel="linear")
+    if problem == "regression":
+        if name == "knn":
+            return KNeighborsRegressor(**paras)
+        elif name == "svm":
+            return SVR(**paras)
+        elif name == "rf":
+            return RandomForestRegressor(**paras)
+        elif name == "adaboost":
+            return AdaBoostRegressor(**paras)
+        elif name == "xgb":
+            return GradientBoostingRegressor(**paras)
+        elif name == "tree":
+            return ExtraTreesRegressor(**paras)
+        elif name == "ann":
+            return MLPRegressor(**paras)
+        else:
+            raise ValueError(f"For Regression problem, we don't support: {name} regressor as string. \n"
+                             f"You can define your own scikit-learn model.")
     else:
-        raise ValueError(f"Currently, MAFESE doesn't support: {name} classifier. You can define your own scikit-learn model.")
+        if name == 'knn':
+            return KNeighborsClassifier(**paras)
+        elif name == 'svm':
+            return SVC(**paras)
+        elif name == 'rf':
+            return RandomForestClassifier(**paras)
+        elif name == "adaboost":
+            return AdaBoostClassifier(**paras)
+        elif name == "xgb":
+            return GradientBoostingClassifier(**paras)
+        elif name == "tree":
+            return ExtraTreesClassifier(**paras)
+        elif name == "ann":
+            return MLPClassifier(**paras)
+        else:
+            raise ValueError(f"For Classification problem, we don't support: {name} classifier as string. \n"
+                             f"You can define your own scikit-learn model.")
 
 
-def get_regressor_for_recursive(name):
+def get_recursive_estimator(problem, name, paras=None):
+    if paras is None:
+        paras = {}
     name = name.lower()
-    if name == "rf":
-        return RandomForestRegressor()
-    elif name == "svm":
-        return SVR(kernel="linear")
+    if problem == "regression":
+        if name == "rf":
+            return RandomForestRegressor(**paras)
+        elif name == "svm":
+            return SVR(**paras, kernel="linear")
+        elif name == "adaboost":
+            return AdaBoostRegressor(**paras)
+        elif name == "xgb":
+            return GradientBoostingRegressor(**paras)
+        elif name == "tree":
+            return ExtraTreesRegressor(**paras)
+        else:
+            raise ValueError(f"For Regression problem, with Recursive method, you can't use: {name} regressor as base estimator.")
     else:
-        raise ValueError(f"Currently, we don't support: {name} regressor. You can define your own scikit-learn model.")
+        if name == 'rf':
+            return RandomForestClassifier(**paras)
+        elif name == 'svm':
+            est = SVC(**paras)
+            est.set_params(**{"kernel": "linear"})
+            return est
+        elif name == "adaboost":
+            return AdaBoostClassifier(**paras)
+        elif name == "xgb":
+            return GradientBoostingClassifier(**paras)
+        elif name == "tree":
+            return ExtraTreesClassifier(**paras)
+        else:
+            raise ValueError(f"For Classification problem, with Recursive method, you can't use: {name} classifier as base estimator.")
 
 
 def get_lasso_based_estimator(problem, name, paras=None):
     if paras is None:
         paras = {}
     name = name.lower()
     if problem == "regression":
@@ -73,17 +107,14 @@
         elif name == "svm":
             return LinearSVC(**paras)
         else:
             raise ValueError(f"For Classification problem, lasso-based method supports: 'lasso', 'lr', and 'svm' estimator.")
 
 
 def get_tree_based_estimator(problem, name, paras=None):
-    from sklearn.ensemble import ExtraTreesRegressor, RandomForestRegressor, AdaBoostRegressor, GradientBoostingRegressor
-    from sklearn.ensemble import ExtraTreesClassifier, RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier
-
     if paras is None:
         paras = {}
     name = name.lower()
     if problem == "regression":
         if name == "rf":
             return RandomForestRegressor(**paras)
         elif name == "adaboost":
```

### Comparing `mafese-0.1.4/mafese/utils/mealpy_util.py` & `mafese-0.1.5/mafese/utils/mealpy_util.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/transfer.py` & `mafese-0.1.5/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/utils/validator.py` & `mafese-0.1.5/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/mafese/wrapper/mha.py` & `mafese-0.1.5/mafese/wrapper/mha.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mafese.selector import Selector
 from mafese.utils import validator
-from mafese.utils.estimator import get_classifier, get_regressor
+from mafese.utils.estimator import get_general_estimator
 from mafese.utils.mealpy_util import get_optimizer_by_name, get_all_optimizers, FeatureSelectionProblem, Optimizer
 from mafese.utils import transfer
 from mafese.utils.data_loader import Data
 from permetrics.regression import RegressionMetric
 from permetrics.classification import ClassificationMetric
 
 
@@ -22,20 +22,27 @@
     Parameters
     ----------
     problem: str, default = "classification"
         The problem you are trying to solve (or type of dataset), "classification" or "regression"
 
     estimator: str or Estimator instance (from scikit-learn or custom)
         If estimator is str, we are currently support:
-            - knn: K-Nearest Neighbors
-            - rf: random forest
+            - knn: k-nearest neighbors
             - svm: support vector machine
-
-        If estimator is Estimator instance: you need to make sure it is has a ``fit`` method that provides
-        information about feature importance (e.g. `coef_`, `feature_importances_`).
+            - rf: random forest
+            - adaboost: AdaBoost
+            - xgb: Gradient Boosting
+            - tree: Extra Trees
+            - ann: Artificial Neural Network (Multi-Layer Perceptron)
+
+        If estimator is Estimator instance: you need to make sure that it has `fit` and `predict` methods
+
+    estimator_paras: None or dict, default = None
+        The parameters of the estimator, please see the official document of scikit-learn to selected estimator.
+        If None, we use the default parameter for selected estimator
 
     optimizer : str or instance of Optimizer class (from Mealpy library), default = "BaseGA"
         The Metaheuristic Algorithm that use to solve the feature selection problem.
         Current supported list, please check it here: https://github.com/thieu1995/mealpy.
         If a custom optimizer is passed, make sure it is an instance of `Optimizer` class.
 
     optimizer_paras : None or dict of parameter, default=None
@@ -77,38 +84,36 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["knn", "rf", "svm"]
+    SUPPORTED_ESTIMATORS = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
     SUPPORTED_TRANSFER_FUNCS = ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04", "rtf"]
     SUPPORTED_REG_METRICS = {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
                              "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
                              "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"}
     SUPPORTED_CLS_METRICS = {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
                              "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"}
     SUPPORTED_OPTIMIZERS = list(get_all_optimizers().keys())
 
-    def __init__(self, problem="classification", estimator="knn", optimizer="BaseGA", optimizer_paras=None,
-                 transfer_func="vstf_01", obj_name=None):
+    def __init__(self, problem="classification", estimator="knn", estimator_paras=None,
+                 optimizer="BaseGA", optimizer_paras=None, transfer_func="vstf_01", obj_name=None):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator)
+        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.optimizer_paras = estimator_paras
         self.optimizer = self.set_optimizer(optimizer, optimizer_paras)
         self.transfer_func_ = self.set_transfer_func(transfer_func)
         self.obj_name = obj_name
 
-    def set_estimator(self, estimator=None):
+    def set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
             estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
-            if self.problem == "classification":
-                return get_classifier(estimator_name)
-            else:
-                return get_regressor(estimator_name)
+            return get_general_estimator(self.problem, estimator_name, paras)
         elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and \
                 (callable(estimator.fit) and callable(estimator.predict)):
             return estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
 
     def set_optimizer(self, optimizer=None, optimizer_paras=None):
```

### Comparing `mafese-0.1.4/mafese/wrapper/recursive.py` & `mafese-0.1.5/mafese/wrapper/recursive.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,41 @@
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from sklearn.feature_selection import RFE
 from mafese.selector import Selector
 from mafese.utils import validator
-from mafese.utils.estimator import get_classifier_for_recursive, get_regressor_for_recursive
+from mafese.utils.estimator import get_recursive_estimator
 
 
 class RecursiveSelector(Selector):
     """
     Defines a RecursiveSelector class that hold all RecursiveSelector Feature Selection methods for feature selection problems
 
     Parameters
     ----------
     problem: str, default = "classification"
         The problem you are trying to solve (or type of dataset), "classification" or "regression"
 
     estimator: str or Estimator instance (from scikit-learn or custom)
         If estimator is str, we are currently support:
-            - rf: random forest
             - svm: support vector machine with kernel = 'linear'
+            - rf: random forest
+            - adaboost: AdaBoost
+            - xgb: Gradient Boosting
+            - tree: Extra Trees
 
         If estimator is Estimator instance: you need to make sure it is has a ``fit`` method that provides
         information about feature importance (e.g. `coef_`, `feature_importances_`).
 
+    estimator_paras: None or dict, default = None
+        The parameters of the estimator, please see the official document of scikit-learn to selected estimator.
+        If None, we use the best parameter for selected estimator
+
     n_features : int or float, default=3
         The number of features to select. If `None`, half of the features are selected.
         If integer, the parameter is the absolute number of features to select.
         If float between 0 and 1, it is the fraction of features to  select.
 
     step : int or float, default=1
         If greater than or equal to 1, then ``step`` corresponds to the (integer) number of features to remove at each iteration.
@@ -71,33 +78,31 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["rf", "svm"]
+    SUPPORTED_ESTIMATORS = ["svm", "rf", "adaboost", "xgb", "tree"]
 
-    def __init__(self, problem="classification", estimator="knn", n_features=3, step=1, verbose=0, importance_getter="auto"):
+    def __init__(self, problem="classification", estimator="knn", estimator_paras=None, n_features=3, step=1, verbose=0, importance_getter="auto"):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator)
+        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator_paras = estimator_paras
         self.n_features = n_features
         self.step = step
         self.verbose = verbose
         self.importance_getter = importance_getter
         self.selector = RFE(estimator=self.estimator, n_features_to_select=self.n_features,
                             step=self.step, verbose=self.verbose, importance_getter=self.importance_getter)
 
-    def set_estimator(self, estimator=None):
+    def set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
             estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
-            if self.problem == "classification":
-                return get_classifier_for_recursive(estimator_name)
-            else:
-                return get_regressor_for_recursive(estimator_name)
+            return get_recursive_estimator(self.problem, estimator_name, paras)
         elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and \
                 (callable(estimator.fit) and callable(estimator.predict)):
             return estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
 
     def fit(self, X, y=None):
```

### Comparing `mafese-0.1.4/mafese/wrapper/sequential.py` & `mafese-0.1.5/mafese/wrapper/sequential.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,43 @@
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from sklearn.feature_selection import SequentialFeatureSelector as SFS
 from mafese.selector import Selector
 from mafese.utils import validator
-from mafese.utils.estimator import get_classifier, get_regressor
+from mafese.utils.estimator import get_general_estimator
 
 
 class SequentialSelector(Selector):
     """
     Defines a SequentialSelector class that hold all Forward or Backward Feature Selection methods for feature selection problems
 
     Parameters
     ----------
     problem: str, default = "classification"
         The problem you are trying to solve (or type of dataset), "classification" or "regression"
 
     estimator: str or Estimator instance (from scikit-learn or custom)
         If estimator is str, we are currently support:
             - knn: k-nearest neighbors
-            - rf: random forest
             - svm: support vector machine
+            - rf: random forest
+            - adaboost: AdaBoost
+            - xgb: Gradient Boosting
+            - tree: Extra Trees
+            - ann: Artificial Neural Network (Multi-Layer Perceptron)
 
         If estimator is Estimator instance: you need to make sure it is has a ``fit`` method that provides
         information about feature importance (e.g. `coef_`, `feature_importances_`).
 
+    estimator_paras: None or dict, default = None
+        The parameters of the estimator, please see the official document of scikit-learn to selected estimator.
+        If None, we use the default parameter for selected estimator
+
     n_features : int or float, default=3
         The number of features to select. If `None`, half of the features are selected.
         If integer, the parameter is the absolute number of features to select.
         If float between 0 and 1, it is the fraction of features to  select.
 
     direction : {'forward', 'backward'}, default='forward'
         Whether to perform forward selection or backward selection.
@@ -85,35 +93,33 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["knn", "rf", "svm"]
+    SUPPORTED_ESTIMATORS = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
 
-    def __init__(self, problem="classification", estimator="knn", n_features=3,
+    def __init__(self, problem="classification", estimator="knn", estimator_paras=None, n_features=3,
                  direction="forward", tol=None, scoring=None, cv=5, n_jobs=None):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator)
+        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator_paras = estimator_paras
         self.n_features = n_features
         self.direction = direction
         self.tol = tol
         self.scoring = scoring
         self.cv = cv
         self.n_jobs = n_jobs
         self.selector = SFS(estimator=self.estimator, n_features_to_select=self.n_features, direction=self.direction)
 
-    def set_estimator(self, estimator=None):
+    def set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
             estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
-            if self.problem == "classification":
-                return get_classifier(estimator_name)
-            else:
-                return get_regressor(estimator_name)
+            return get_general_estimator(self.problem, estimator_name, paras)
         elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and \
                 (callable(estimator.fit) and callable(estimator.predict)):
             return estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
 
     def fit(self, X, y=None):
```

### Comparing `mafese-0.1.4/mafese.egg-info/PKG-INFO` & `mafese-0.1.5/mafese.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.4
+Version: 0.1.5
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.4-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.5-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -60,37 +60,37 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library focused on feature selection 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
 * **Total Filter-based (Statistical-based)**: > 12 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 3 datasets
+* **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
 
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.4
+$ pip install mafese==0.1.5
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -255,16 +255,15 @@
 ```
 
 
 Or, use Metaheuristic-based feature selection with different metaheuristic algorithms:
 
 ```python
 from mafese.wrapper.mha import MhaSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
 # define mafese feature selection method
@@ -292,16 +291,15 @@
 ```
 
 
 Or, use Lasso-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.lasso import LassoSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -328,16 +326,15 @@
 ```
 
 
 Or, use Tree-based feature selection with different estimator:
 
 ```python
 from mafese.embedded.tree import TreeSelector
-from mafese import get_dataset
-from mafese import evaluator
+from mafese import get_dataset, evaluator
 from sklearn.svm import SVC
 
 
 data = get_dataset("Arrhythmia")
 data.split_train_test(test_size=0.2)
 print(data.X_train.shape, data.X_test.shape)            # (361, 279) (91, 279)
 
@@ -367,15 +364,15 @@
 
 For more usage examples please look at [examples](/examples) folder.
 
 ### Shortcut 
 To call the class
 
 ```code 
-from mafese import Data, get_dataset
+from mafese import Data, get_dataset, evaluator
 from mafese import FilterSelector
 from mafese import SequentialSelector, RecursiveSelector, MhaSelector
 from mafese import LassoSelector, TreeSelector
 ```
 
 
 # Get helps (questions, problems)
@@ -422,9 +419,12 @@
 
 ```code 
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-```
+6.  https://elki-project.github.io/
+7. https://sci2s.ugr.es/keel/index.php
+8. https://archive.ics.uci.edu/datasets
 
+```
```

### Comparing `mafese-0.1.4/mafese.egg-info/SOURCES.txt` & `mafese-0.1.5/mafese.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/setup.py` & `mafese-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.4",
+    version="0.1.5",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
```

### Comparing `mafese-0.1.4/tests/test_embedded.py` & `mafese-0.1.5/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/tests/test_filter.py` & `mafese-0.1.5/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/tests/test_unsupervised.py` & `mafese-0.1.5/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.4/tests/test_wrapper.py` & `mafese-0.1.5/tests/test_wrapper.py`

 * *Files identical despite different names*

