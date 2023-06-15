# Comparing `tmp/gerk-0.0.1.tar.gz` & `tmp/gerk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerk-0.0.1.tar", last modified: Thu Jun 15 19:12:14 2023, max compression
+gzip compressed data, was "gerk-0.0.2.tar", last modified: Thu Jun 15 19:29:13 2023, max compression
```

## Comparing `gerk-0.0.1.tar` & `gerk-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:12:14.674770 gerk-0.0.1/
--rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.1/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)      420 2023-06-15 19:12:14.674345 gerk-0.0.1/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)    14441 2023-06-15 19:03:01.000000 gerk-0.0.1/README.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:12:14.670143 gerk-0.0.1/gerk/
--rw-r--r--   0 yasser     (501) staff       (20)      195 2023-06-15 18:49:34.000000 gerk-0.0.1/gerk/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.1/gerk/_gerk_error.py
--rw-r--r--   0 yasser     (501) staff       (20)    10256 2023-01-15 23:24:42.000000 gerk-0.0.1/gerk/gerk.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:12:14.673705 gerk-0.0.1/gerk.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)      420 2023-06-15 19:12:14.000000 gerk-0.0.1/gerk.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 19:12:14.000000 gerk-0.0.1/gerk.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 19:12:14.000000 gerk-0.0.1/gerk.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)       11 2023-06-15 19:12:14.000000 gerk-0.0.1/gerk.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 19:12:14.000000 gerk-0.0.1/gerk.egg-info/top_level.txt
--rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 19:12:14.674982 gerk-0.0.1/setup.cfg
--rw-r--r--   0 yasser     (501) staff       (20)      642 2023-06-15 19:09:21.000000 gerk-0.0.1/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:29:13.684227 gerk-0.0.2/
+-rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.2/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)      420 2023-06-15 19:29:13.683265 gerk-0.0.2/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)    14441 2023-06-15 19:03:01.000000 gerk-0.0.2/README.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:29:13.677517 gerk-0.0.2/gerk/
+-rw-r--r--   0 yasser     (501) staff       (20)      195 2023-06-15 18:49:34.000000 gerk-0.0.2/gerk/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.2/gerk/_gerk_error.py
+-rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.2/gerk/gerk.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 19:29:13.682410 gerk-0.0.2/gerk.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)      420 2023-06-15 19:29:13.000000 gerk-0.0.2/gerk.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 19:29:13.000000 gerk-0.0.2/gerk.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 19:29:13.000000 gerk-0.0.2/gerk.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2023-06-15 19:29:13.000000 gerk-0.0.2/gerk.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 19:29:13.000000 gerk-0.0.2/gerk.egg-info/top_level.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 19:29:13.684773 gerk-0.0.2/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)      651 2023-06-15 19:28:21.000000 gerk-0.0.2/setup.py
```

### Comparing `gerk-0.0.1/LICENSE` & `gerk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gerk-0.0.1/README.md` & `gerk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gerk-0.0.1/gerk/_gerk_error.py` & `gerk-0.0.2/gerk/_gerk_error.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.1/gerk/gerk.py` & `gerk-0.0.2/gerk/gerk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import math
 import decimal
-from _gerk_error import (
+from ._gerk_error import (
     GerkArrayError,
     GerkFunctionError, 
     GerkAdaptiveError,
     GerkArrayErrorEnum,
     GerkFunctionErrorEnum,
     GerkAdaptiveErrorEnum,
 )
```

### Comparing `gerk-0.0.1/setup.py` & `gerk-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Generalized Explicit Runge-Kutta"
 
 setup(
     name="gerk",
     version=VERSION,
     author="Yasser Naji",
     author_email="yfnaji@gmail.com",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=["matplotlib"],
+    install_requires=["matplotlib", "numpy"],
     keywords=["runge-kutta", "runge", "kutta", "numerical", "integration", "approximation"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

