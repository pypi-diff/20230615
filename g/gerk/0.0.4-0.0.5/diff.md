# Comparing `tmp/gerk-0.0.4.tar.gz` & `tmp/gerk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerk-0.0.4.tar", last modified: Thu Jun 15 20:33:53 2023, max compression
+gzip compressed data, was "gerk-0.0.5.tar", last modified: Thu Jun 15 21:13:08 2023, max compression
```

## Comparing `gerk-0.0.4.tar` & `gerk-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.859611 gerk-0.0.4/
--rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.4/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 20:33:53.858801 gerk-0.0.4/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)    14974 2023-06-15 20:32:47.000000 gerk-0.0.4/README.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.854754 gerk-0.0.4/gerk/
--rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.4/gerk/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.4/gerk/_gerk_error.py
--rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.4/gerk/gerk.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 20:33:53.858209 gerk-0.0.4/gerk.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)       22 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 20:33:53.000000 gerk-0.0.4/gerk.egg-info/top_level.txt
--rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 20:33:53.859776 gerk-0.0.4/setup.cfg
--rw-r--r--   0 yasser     (501) staff       (20)      852 2023-06-15 20:33:46.000000 gerk-0.0.4/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 21:13:08.779394 gerk-0.0.5/
+-rw-r--r--   0 yasser     (501) staff       (20)     1093 2023-06-15 19:06:49.000000 gerk-0.0.5/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 21:13:08.778674 gerk-0.0.5/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)    14974 2023-06-15 20:32:47.000000 gerk-0.0.5/README.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 21:13:08.773892 gerk-0.0.5/gerk/
+-rw-r--r--   0 yasser     (501) staff       (20)       23 2023-06-15 20:05:46.000000 gerk-0.0.5/gerk/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)     3277 2023-01-04 23:34:49.000000 gerk-0.0.5/gerk/_gerk_error.py
+-rw-r--r--   0 yasser     (501) staff       (20)    10257 2023-06-15 19:26:27.000000 gerk-0.0.5/gerk/gerk.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-06-15 21:13:08.777926 gerk-0.0.5/gerk.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)    15435 2023-06-15 21:13:08.000000 gerk-0.0.5/gerk.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)      215 2023-06-15 21:13:08.000000 gerk-0.0.5/gerk.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2023-06-15 21:13:08.000000 gerk-0.0.5/gerk.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2023-06-15 21:13:08.000000 gerk-0.0.5/gerk.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        5 2023-06-15 21:13:08.000000 gerk-0.0.5/gerk.egg-info/top_level.txt
+-rw-r--r--   0 yasser     (501) staff       (20)       38 2023-06-15 21:13:08.779618 gerk-0.0.5/setup.cfg
+-rw-r--r--   0 yasser     (501) staff       (20)      868 2023-06-15 21:12:17.000000 gerk-0.0.5/setup.py
```

### Comparing `gerk-0.0.4/LICENSE` & `gerk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gerk-0.0.4/PKG-INFO` & `gerk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `gerk-0.0.4/README.md` & `gerk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gerk-0.0.4/gerk/_gerk_error.py` & `gerk-0.0.5/gerk/_gerk_error.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.4/gerk/gerk.py` & `gerk-0.0.5/gerk/gerk.py`

 * *Files identical despite different names*

### Comparing `gerk-0.0.4/gerk.egg-info/PKG-INFO` & `gerk-0.0.5/gerk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generalized Explicit Runge-Kutta
 Author: Yasser Naji
 Author-email: yfnaji@gmail.com
 Keywords: runge-kutta,runge,kutta,numerical,integration,approximation
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `gerk-0.0.4/setup.py` & `gerk-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 from pathlib import Path
+import codecs
+import os
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Generalized Explicit Runge-Kutta"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="gerk",
     version=VERSION,
     author="Yasser Naji",
     author_email="yfnaji@gmail.com",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["matplotlib", "numpy", "math"],
+    install_requires=["matplotlib", "numpy"],
     keywords=["runge-kutta", "runge", "kutta", "numerical", "integration", "approximation"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

