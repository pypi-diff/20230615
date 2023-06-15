# Comparing `tmp/hdlib-0.1.5.tar.gz` & `tmp/hdlib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.5.tar", last modified: Fri Jun  9 04:36:59 2023, max compression
+gzip compressed data, was "hdlib-0.1.6.tar", last modified: Thu Jun 15 14:41:32 2023, max compression
```

## Comparing `hdlib-0.1.5.tar` & `hdlib-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.328309 hdlib-0.1.5/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.5/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     1713 2023-06-09 04:36:59.327566 hdlib-0.1.5/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     1079 2023-06-09 01:35:38.000000 hdlib-0.1.5/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.279552 hdlib-0.1.5/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      101 2023-06-07 18:33:03.000000 hdlib-0.1.5/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.5/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    14629 2023-06-09 01:49:03.000000 hdlib-0.1.5/hdlib/model.py
--rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.5/hdlib/parser.py
--rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.5/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.293772 hdlib-0.1.5/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     1713 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       14 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-09 04:36:59.000000 hdlib-0.1.5/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-09 04:36:59.328498 hdlib-0.1.5/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.5/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-09 04:36:59.325661 hdlib-0.1.5/test/
--rw-r--r--   0 fabio      (501) staff       (20)     6580 2023-06-08 21:35:23.000000 hdlib-0.1.5/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.697124 hdlib-0.1.6/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.6/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 14:41:32.694494 hdlib-0.1.6/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.6/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.445307 hdlib-0.1.6/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-14 21:23:08.000000 hdlib-0.1.6/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.6/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    29764 2023-06-15 01:29:07.000000 hdlib-0.1.6/hdlib/model.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.6/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.6/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.644790 hdlib-0.1.6/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-15 14:41:32.697545 hdlib-0.1.6/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.6/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.648478 hdlib-0.1.6/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     8033 2023-06-13 01:24:19.000000 hdlib-0.1.6/test/test.py
```

### Comparing `hdlib-0.1.5/LICENSE` & `hdlib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.5/hdlib/arithmetic.py` & `hdlib-0.1.6/hdlib/arithmetic.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.5/hdlib/parser.py` & `hdlib-0.1.6/hdlib/parser.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.5/hdlib/space.py` & `hdlib-0.1.6/hdlib/space.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.5/setup.py` & `hdlib-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,19 +15,28 @@
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
     ],
     description="Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python",
-    install_requires=["numpy>=1.22.3"],
+    install_requires=[
+        "numpy>=1.22.3",
+        "scikit-learn>=1.2.2",
+        "tabulate>=0.9.0"
+    ],
     license="MIT",
     license_files=["LICENSE"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     name="hdlib",
     packages=setuptools.find_packages(include=["hdlib"], exclude=["test"]),
+    project_urls={
+        "Issues": "https://github.com/cumbof/hdlib/issues",
+        "Source": "https://github.com/cumbof/hdlib",
+        "Wiki": "https://github.com/cumbof/hdlib/wiki",
+    },
     python_requires=">=3",
     url="http://github.com/cumbof/hdlib",
     version=__version__,
     zip_safe=False
 )
```

### Comparing `hdlib-0.1.5/test/test.py` & `hdlib-0.1.6/test/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 import errno
 import os
 import sys
 import tempfile
 import unittest
 
 import numpy as np
+from sklearn import datasets
+from sklearn.metrics import accuracy_score
 
 # Define the test root directory
 TESTS_DIR = os.path.dirname(os.path.realpath(__file__))
 
 # Define the hdlib root directory
 HDLIB_DIR = os.path.join(os.path.dirname(TESTS_DIR), "hdlib")
 
 # This is required to import the functions we need to test
 sys.path.append(HDLIB_DIR)
 
 # Finally import the space, vector, and arithmetic operators
 from space import Space, Vector
 from arithmetic import bundle, bind, permute
+from model import Model
 
 
 class TestHDLib(unittest.TestCase):
     """
     Unit tests for hdlib
     """
 
@@ -129,14 +132,54 @@
 
             # Load the pickle file
             pickle_space = Space(from_file=pkl_filepath)
 
             with self.subTest():
                 self.assertEqual(len(space), len(pickle_space))
 
+    def test_model(self):
+        """
+        Unit tests for hdlib/model.py:Model class
+        """
+
+        # Create a model with vector dimensionality 10000, vector type bipolar, and 10 levels
+        model = Model(size=10000, levels=10, vtype="bipolar")
+
+        # Use the IRIS dataset from sklearn
+        iris = datasets.load_iris()
+
+        # Get data points and classes
+        points = iris.data.tolist()
+        classes = iris.target.tolist()
+
+        # Fit the model
+        model.fit(points, classes)
+
+        with self.subTest():
+            # There should be N data points plus 10 level vectors in the space
+            self.assertEqual(len(model.space.memory()), len(points) + 10)
+
+        # 5-folds cross-validation
+        # 10 retraining iterations
+        predictions = model.cross_val_predict(points, classes, cv=5, retrain=10)
+
+        with self.subTest():
+            # There should be a prediction for each fold
+            self.assertEqual(len(predictions), 5)
+
+        # Collect the accuracy scores computed on each fold
+        scores = list()
+
+        for y_indices, y_pred in predictions:
+            y_true = [label for position, label in enumerate(classes) if position in y_indices]
+            accuracy = accuracy_score(y_true, y_pred)
+        
+            with self.subTest():
+                self.assertTrue(accuracy > 0.0)
+
     def test_dollar_of_mexico(self):
         """
         Reproduce the "What is the Dollar of Mexico?"
 
         Credits:
         Kanerva, P., 2010, November. 
         What we mean when we say "What's the dollar of Mexico?": Prototypes and mapping in concept space.
```

