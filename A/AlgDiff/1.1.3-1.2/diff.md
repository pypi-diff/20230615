# Comparing `tmp/AlgDiff-1.1.3.tar.gz` & `tmp/AlgDiff-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-1.1.3.tar", last modified: Thu Jun 15 13:27:18 2023, max compression
+gzip compressed data, was "AlgDiff-1.2.tar", last modified: Thu Jun 15 13:39:43 2023, max compression
```

## Comparing `AlgDiff-1.1.3.tar` & `AlgDiff-1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:27:18.524099 AlgDiff-1.1.3/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:27:18.524099 AlgDiff-1.1.3/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 13:13:15.397151 AlgDiff-1.1.3/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41410 2023-06-06 12:55:23.439375 AlgDiff-1.1.3/AlgDiff/algebraicDifferentiator.py
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      721 2023-06-15 13:27:18.524099 AlgDiff-1.1.3/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 13:24:16.656184 AlgDiff-1.1.3/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      944 2023-06-15 13:23:38.456239 AlgDiff-1.1.3/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:39:43.851899 AlgDiff-1.2/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 13:39:43.851899 AlgDiff-1.2/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 13:13:15.397151 AlgDiff-1.2/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41410 2023-06-06 12:55:23.439375 AlgDiff-1.2/AlgDiff/algebraicDifferentiator.py
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      719 2023-06-15 13:39:43.851899 AlgDiff-1.2/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 13:24:16.656184 AlgDiff-1.2/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      925 2023-06-15 13:39:40.351901 AlgDiff-1.2/setup.py
```

### Comparing `AlgDiff-1.1.3/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-1.2/AlgDiff/algebraicDifferentiator.py`

 * *Files identical despite different names*

### Comparing `AlgDiff-1.1.3/PKG-INFO` & `AlgDiff-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: AlgDiff
-Version: 1.1.3
+Version: 1.2
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
 Author: Amine Othmane
 Author-email: amine.othmane@uni-saarland.de
 License: bsd-3-clause
 Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v1.1.3
 Description: UNKNOWN
```

### Comparing `AlgDiff-1.1.3/setup.py` & `AlgDiff-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from distutils.core import setup
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '1.1.3',
+  version = '1.2',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
   download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v1.1.3',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[            # I get to this in a second
           'scipy',
           'mpmath',
           'numpy',
-          'math'
       ],
   classifiers=[
     'License :: OSI Approved :: BSD License',
     'Programming Language :: Python :: 3',
   ],
 )
```

