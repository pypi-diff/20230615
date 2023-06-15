# Comparing `tmp/sam_ml-py-0.4.0.tar.gz` & `tmp/sam_ml-py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.4.0.tar", last modified: Thu Jun 15 11:46:24 2023, max compression
+gzip compressed data, was "sam_ml-py-0.4.1.tar", last modified: Thu Jun 15 11:54:26 2023, max compression
```

## Comparing `sam_ml-py-0.4.0.tar` & `sam_ml-py-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.642055 sam_ml-py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 11:46:24.642055 sam_ml-py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.634055 sam_ml-py-0.4.0/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.634055 sam_ml-py-0.4.0/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.634055 sam_ml-py-0.4.0/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.642055 sam_ml-py-0.4.0/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:46:24.642055 sam_ml-py-0.4.0/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 11:46:24.000000 sam_ml-py-0.4.0/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-15 11:46:24.000000 sam_ml-py-0.4.0/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:46:24.000000 sam_ml-py-0.4.0/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 11:46:24.000000 sam_ml-py-0.4.0/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 11:46:24.000000 sam_ml-py-0.4.0/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:46:24.642055 sam_ml-py-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 11:46:10.000000 sam_ml-py-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.204165 sam_ml-py-0.4.1/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.204165 sam_ml-py-0.4.1/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.208165 sam_ml-py-0.4.1/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 11:54:26.000000 sam_ml-py-0.4.1/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:54:26.216165 sam_ml-py-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 11:54:15.000000 sam_ml-py-0.4.1/setup.py
```

### Comparing `sam_ml-py-0.4.0/LICENSE` & `sam_ml-py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/PKG-INFO` & `sam_ml-py-0.4.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # SAM_ML
-a library created by Samuel Brinkmann
-
-## getting started
 
-1. clone this repository into your current working directory
-
-```
-git clone https://github.com/Priapos1004/SAM_ML
-```
+[![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
-2. go into the `SAM_ML` folder
+a library created by Samuel Brinkmann
 
-```
-cd SAM_ML/
-```
+## getting started
 
-3. install the package to your activated virtual environment
+1. install the package to your activated virtual environment
 
 ```
-pip install -e .
+pip install sam-ml-py
 ```
 
-4. now you can import the package, e.g.:
+2. now you can import the package, e.g.:
 
 ```
 from sam_ml.models import RFC
 
 RandomForestClassifier = RFC()
 ```
```

### Comparing `sam_ml-py-0.4.0/sam_ml/config/logging.py` & `sam_ml-py-0.4.1/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/data/embeddings.py` & `sam_ml-py-0.4.1/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/data/feature_selection.py` & `sam_ml-py-0.4.1/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/data/sampling.py` & `sam_ml-py-0.4.1/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/data/scaler.py` & `sam_ml-py-0.4.1/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.4.1/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.4.1/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.4.1/sam_ml/models/ClassifierTest.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.4.1/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.4.1/sam_ml/models/GradientBoostingMachine.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.4.1/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.4.1/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.4.1/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.4.1/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/__init__.py` & `sam_ml-py-0.4.1/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/main_classifier.py` & `sam_ml-py-0.4.1/sam_ml/models/main_classifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/main_model.py` & `sam_ml-py-0.4.1/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.4.1/sam_ml/models/main_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml/models/scorer.py` & `sam_ml-py-0.4.1/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.4.1/sam_ml_py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # SAM_ML
-a library created by Samuel Brinkmann
-
-## getting started
 
-1. clone this repository into your current working directory
-
-```
-git clone https://github.com/Priapos1004/SAM_ML
-```
+[![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
-2. go into the `SAM_ML` folder
+a library created by Samuel Brinkmann
 
-```
-cd SAM_ML/
-```
+## getting started
 
-3. install the package to your activated virtual environment
+1. install the package to your activated virtual environment
 
 ```
-pip install -e .
+pip install sam-ml-py
 ```
 
-4. now you can import the package, e.g.:
+2. now you can import the package, e.g.:
 
 ```
 from sam_ml.models import RFC
 
 RandomForestClassifier = RFC()
 ```
```

### Comparing `sam_ml-py-0.4.0/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.4.1/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.0/setup.py` & `sam_ml-py-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.4.0",
+    version="0.4.1",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

