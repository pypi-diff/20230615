# Comparing `tmp/AlgDiff-2.0.tar.gz` & `tmp/AlgDiff-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-2.0.tar", last modified: Thu Jun 15 15:15:18 2023, max compression
+gzip compressed data, was "AlgDiff-2.0.1.tar", last modified: Thu Jun 15 15:48:02 2023, max compression
```

## Comparing `AlgDiff-2.0.tar` & `AlgDiff-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:15:18.091909 AlgDiff-2.0/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:15:18.091909 AlgDiff-2.0/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.438138 AlgDiff-2.0/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41426 2023-06-15 14:57:11.442138 AlgDiff-2.0/AlgDiff/algebraicDifferentiator.py
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      717 2023-06-15 15:15:18.091909 AlgDiff-2.0/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 14:57:11.482138 AlgDiff-2.0/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      923 2023-06-15 15:08:37.704701 AlgDiff-2.0/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:48:02.447700 AlgDiff-2.0.1/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:48:02.447700 AlgDiff-2.0.1/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.438138 AlgDiff-2.0.1/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41426 2023-06-15 14:57:11.442138 AlgDiff-2.0.1/AlgDiff/algebraicDifferentiator.py
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      726 2023-06-15 15:48:02.447700 AlgDiff-2.0.1/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 14:57:11.482138 AlgDiff-2.0.1/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1014 2023-06-15 15:47:55.043721 AlgDiff-2.0.1/setup.py
```

### Comparing `AlgDiff-2.0/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.0.1/AlgDiff/algebraicDifferentiator.py`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.0/PKG-INFO` & `AlgDiff-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: AlgDiff
-Version: 2.0
+Version: 2.0.1
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
 Author: Amine Othmane
 Author-email: amine.othmane@uni-saarland.de
 License: bsd-3-clause
 Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.0
-Description: UNKNOWN
+Description: dosc/index.rst
 Keywords: numerical-differentiation ,fir-filters,orthogonal-polynomials,numerical-methods 
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgDiff-2.0/setup.py` & `AlgDiff-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '2.0',
+  version = '2.0.1',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
+  
+  long_description='dosc/index.rst',
+  long_description_content_type='text/x-rst',
+  
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
   download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.0',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[            # I get to this in a second
           'scipy',
```

