# Comparing `tmp/AlgDiff-1.2.tar.gz` & `tmp/AlgDiff-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-1.2.tar", last modified: Thu Jun 15 13:39:43 2023, max compression
+gzip compressed data, was "AlgDiff-2.0.tar", last modified: Thu Jun 15 15:15:18 2023, max compression
```

## Comparing `AlgDiff-1.2.tar` & `AlgDiff-2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:39:43.851899 AlgDiff-1.2/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:39:43.851899 AlgDiff-1.2/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 13:13:15.397151 AlgDiff-1.2/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41410 2023-06-06 12:55:23.439375 AlgDiff-1.2/AlgDiff/algebraicDifferentiator.py
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      719 2023-06-15 13:39:43.851899 AlgDiff-1.2/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 13:24:16.656184 AlgDiff-1.2/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      925 2023-06-15 13:39:40.351901 AlgDiff-1.2/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:15:18.091909 AlgDiff-2.0/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 15:15:18.091909 AlgDiff-2.0/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.438138 AlgDiff-2.0/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41426 2023-06-15 14:57:11.442138 AlgDiff-2.0/AlgDiff/algebraicDifferentiator.py
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      717 2023-06-15 15:15:18.091909 AlgDiff-2.0/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 14:57:11.482138 AlgDiff-2.0/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      923 2023-06-15 15:08:37.704701 AlgDiff-2.0/setup.py
```

### Comparing `AlgDiff-1.2/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.0/AlgDiff/algebraicDifferentiator.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         the new window such that the truncation is performed symmetrically.
         If this is enabled, the functions also returns the times at which
         the filter was truncated.
 
         :param der: Order of the derivative to be estimated.
         :type der: int
         :param method: Discretization scheme: "mid-point", "trapezoidal",\
-            "analytic".
+            "analytic", "simpson rule".
         :type method: string
         :param reduceFilLength: Reduce or not the filter window length.
         :type reduceFilLength: Bool
         :param redTol: Tolerance to be used when the filter length is reduced.
         :type redTol: float.
         :param discreteSpectrum: If it is set, then the parameter \
             :math:`\\theta` used in the discretization is returned. See survey paper
```

### Comparing `AlgDiff-1.2/PKG-INFO` & `AlgDiff-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: AlgDiff
-Version: 1.2
+Version: 2.0
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
 Author: Amine Othmane
 Author-email: amine.othmane@uni-saarland.de
 License: bsd-3-clause
-Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v1.1.3
+Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.0
 Description: UNKNOWN
 Keywords: numerical-differentiation ,fir-filters,orthogonal-polynomials,numerical-methods 
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgDiff-1.2/setup.py` & `AlgDiff-2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '1.2',
+  version = '2.0',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
-  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v1.1.3',
+  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.0',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[            # I get to this in a second
           'scipy',
           'mpmath',
           'numpy',
       ],
   classifiers=[
```

