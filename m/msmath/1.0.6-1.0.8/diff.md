# Comparing `tmp/msmath-1.0.6.tar.gz` & `tmp/msmath-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmath-1.0.6.tar", last modified: Tue Jul 12 00:51:59 2022, max compression
+gzip compressed data, was "msmath-1.0.8.tar", last modified: Sat Jul 23 01:58:00 2022, max compression
```

## Comparing `msmath-1.0.6.tar` & `msmath-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-12 00:51:59.687510 msmath-1.0.6/
--rwxr-xr-x   0 ms        (1001) None       (513)    35795 2022-07-10 15:40:40.000000 msmath-1.0.6/LICENSE
--rw-r--r--   0 ms        (1001) None       (513)    42427 2022-07-12 00:51:59.679302 msmath-1.0.6/PKG-INFO
--rwxr-xr-x   0 ms        (1001) None       (513)     1247 2022-07-12 00:48:27.000000 msmath-1.0.6/README.md
--rwxr-xr-x   0 ms        (1001) None       (513)      800 2022-07-12 00:21:58.000000 msmath-1.0.6/pyproject.toml
--rw-r--r--   0 ms        (1001) None       (513)       38 2022-07-12 00:51:59.689687 msmath-1.0.6/setup.cfg
-drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-12 00:51:58.812551 msmath-1.0.6/src/
-drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-12 00:51:59.523513 msmath-1.0.6/src/msmath/
--rw-r--r--   0 ms        (1001) None       (513)        0 2022-06-04 23:32:08.000000 msmath-1.0.6/src/msmath/__init__.py
--rwxr-x---   0 ms        (1001) None       (513)     2962 2022-07-12 00:29:14.000000 msmath-1.0.6/src/msmath/bch.py
--rwxr-x---   0 ms        (1001) None       (513)    28881 2022-06-05 00:40:12.000000 msmath-1.0.6/src/msmath/bitstring.py
--rwxr-x---   0 ms        (1001) None       (513)     4607 2022-03-11 16:23:04.000000 msmath-1.0.6/src/msmath/conversions.py
--rwxr-x---   0 ms        (1001) None       (513)    47216 2022-06-05 00:37:42.000000 msmath-1.0.6/src/msmath/ffield.py
--rwxr-x---   0 ms        (1001) None       (513)      846 2022-06-05 00:42:46.000000 msmath-1.0.6/src/msmath/ffpoly.py
--rwxr-xr-x   0 ms        (1001) None       (513)     7936 2022-07-12 00:45:03.000000 msmath-1.0.6/src/msmath/fring.py
--rwxr-x---   0 ms        (1001) None       (513)    12840 2022-06-05 00:39:50.000000 msmath-1.0.6/src/msmath/graph.py
--rwxr-x---   0 ms        (1001) None       (513)    61294 2022-06-05 00:34:26.000000 msmath-1.0.6/src/msmath/matrix.py
--rwxr-x---   0 ms        (1001) None       (513)    21039 2022-06-05 00:32:56.000000 msmath-1.0.6/src/msmath/numfuns.py
--rwxr-xr-x   0 ms        (1001) None       (513)     1844 2022-07-12 00:36:56.000000 msmath-1.0.6/src/msmath/optable.py
--rwxr-x---   0 ms        (1001) None       (513)    32364 2022-06-05 00:36:33.000000 msmath-1.0.6/src/msmath/poly.py
--rwxr-x---   0 ms        (1001) None       (513)    11845 2022-06-05 00:35:47.000000 msmath-1.0.6/src/msmath/quaternion.py
--rwxr-x---   0 ms        (1001) None       (513)    82981 2022-06-05 00:35:20.000000 msmath-1.0.6/src/msmath/rational.py
--rwxr-x---   0 ms        (1001) None       (513)     3889 2022-07-12 00:28:27.000000 msmath-1.0.6/src/msmath/share.py
-drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-12 00:51:59.658470 msmath-1.0.6/src/msmath.egg-info/
--rw-r--r--   0 ms        (1001) None       (513)    42427 2022-07-12 00:51:58.000000 msmath-1.0.6/src/msmath.egg-info/PKG-INFO
--rw-r--r--   0 ms        (1001) None       (513)      493 2022-07-12 00:51:58.000000 msmath-1.0.6/src/msmath.egg-info/SOURCES.txt
--rw-r--r--   0 ms        (1001) None       (513)        1 2022-07-12 00:51:58.000000 msmath-1.0.6/src/msmath.egg-info/dependency_links.txt
--rw-r--r--   0 ms        (1001) None       (513)        7 2022-07-12 00:51:58.000000 msmath-1.0.6/src/msmath.egg-info/top_level.txt
+drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-23 01:58:00.637126 msmath-1.0.8/
+-rwxr-xr-x   0 ms        (1001) None       (513)    35795 2022-07-10 15:40:40.000000 msmath-1.0.8/LICENSE
+-rw-r--r--   0 ms        (1001) None       (513)    42490 2022-07-23 01:58:00.792003 msmath-1.0.8/PKG-INFO
+-rwxr-xr-x   0 ms        (1001) None       (513)     1247 2022-07-12 00:48:27.000000 msmath-1.0.8/README.md
+-rwxr-xr-x   0 ms        (1001) None       (513)      810 2022-07-23 01:53:13.000000 msmath-1.0.8/pyproject.toml
+-rwxr-xr-x   0 ms        (1001) None       (513)       74 2022-07-23 01:58:00.802286 msmath-1.0.8/setup.cfg
+-rwxr-xr-x   0 ms        (1001) None       (513)      909 2022-07-23 01:52:49.000000 msmath-1.0.8/setup.py
+drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-23 01:57:58.821385 msmath-1.0.8/src/
+drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-23 01:58:00.369113 msmath-1.0.8/src/msmath/
+-rw-r--r--   0 ms        (1001) None       (513)        0 2022-06-04 23:32:08.000000 msmath-1.0.8/src/msmath/__init__.py
+-rwxr-x---   0 ms        (1001) None       (513)     2962 2022-07-12 00:29:14.000000 msmath-1.0.8/src/msmath/bch.py
+-rwxr-x---   0 ms        (1001) None       (513)    28881 2022-06-05 00:40:12.000000 msmath-1.0.8/src/msmath/bitstring.py
+-rwxr-x---   0 ms        (1001) None       (513)     4607 2022-03-11 16:23:04.000000 msmath-1.0.8/src/msmath/conversions.py
+-rwxr-x---   0 ms        (1001) None       (513)    47216 2022-06-05 00:37:42.000000 msmath-1.0.8/src/msmath/ffield.py
+-rwxr-x---   0 ms        (1001) None       (513)      846 2022-06-05 00:42:46.000000 msmath-1.0.8/src/msmath/ffpoly.py
+-rwxr-xr-x   0 ms        (1001) None       (513)     7936 2022-07-12 00:45:03.000000 msmath-1.0.8/src/msmath/fring.py
+-rwxr-x---   0 ms        (1001) None       (513)    12840 2022-06-05 00:39:50.000000 msmath-1.0.8/src/msmath/graph.py
+-rwxr-x---   0 ms        (1001) None       (513)    61294 2022-06-05 00:34:26.000000 msmath-1.0.8/src/msmath/matrix.py
+-rwxr-x---   0 ms        (1001) None       (513)    21039 2022-06-05 00:32:56.000000 msmath-1.0.8/src/msmath/numfuns.py
+-rwxr-xr-x   0 ms        (1001) None       (513)     1844 2022-07-12 00:36:56.000000 msmath-1.0.8/src/msmath/optable.py
+-rwxr-x---   0 ms        (1001) None       (513)    32364 2022-06-05 00:36:33.000000 msmath-1.0.8/src/msmath/poly.py
+-rwxr-x---   0 ms        (1001) None       (513)    11845 2022-06-05 00:35:47.000000 msmath-1.0.8/src/msmath/quaternion.py
+-rwxr-x---   0 ms        (1001) None       (513)    82981 2022-06-05 00:35:20.000000 msmath-1.0.8/src/msmath/rational.py
+-rwxr-x---   0 ms        (1001) None       (513)     3889 2022-07-12 00:28:27.000000 msmath-1.0.8/src/msmath/share.py
+drwxr-xr-x   0 ms        (1001) None       (513)        0 2022-07-23 01:58:00.626774 msmath-1.0.8/src/msmath.egg-info/
+-rw-r--r--   0 ms        (1001) None       (513)    42490 2022-07-23 01:57:58.000000 msmath-1.0.8/src/msmath.egg-info/PKG-INFO
+-rw-r--r--   0 ms        (1001) None       (513)      512 2022-07-23 01:57:58.000000 msmath-1.0.8/src/msmath.egg-info/SOURCES.txt
+-rw-r--r--   0 ms        (1001) None       (513)        1 2022-07-23 01:57:58.000000 msmath-1.0.8/src/msmath.egg-info/dependency_links.txt
+-rw-r--r--   0 ms        (1001) None       (513)        7 2022-07-23 01:57:58.000000 msmath-1.0.8/src/msmath.egg-info/top_level.txt
```

### Comparing `msmath-1.0.6/LICENSE` & `msmath-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/PKG-INFO` & `msmath-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: msmath
-Version: 1.0.6
+Version: 1.0.8
 Summary: mathematical Python classes: finite fields, rationals, quaternions, matrices, polynomials, graphs, bitstrings
+Home-page: https://github.com/ms0/msmath
+Author: Mike Speciner
 Author-email: Mike Speciner <ms@alum.mit.edu>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `msmath-1.0.6/README.md` & `msmath-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/pyproject.toml` & `msmath-1.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["setuptools>=44"]
+requires = ["setuptools>=44","pathlib"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "msmath"
-version = "1.0.6"
+version = "1.0.8"
 authors = [
   { name="Mike Speciner", email="ms@alum.mit.edu" },
 ]
 description = "mathematical Python classes: finite fields, rationals, quaternions, matrices, polynomials, graphs, bitstrings"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=2.7"
```

### Comparing `msmath-1.0.6/src/msmath/bch.py` & `msmath-1.0.8/src/msmath/bch.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/bitstring.py` & `msmath-1.0.8/src/msmath/bitstring.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/conversions.py` & `msmath-1.0.8/src/msmath/conversions.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/ffield.py` & `msmath-1.0.8/src/msmath/ffield.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/ffpoly.py` & `msmath-1.0.8/src/msmath/ffpoly.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/fring.py` & `msmath-1.0.8/src/msmath/fring.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/graph.py` & `msmath-1.0.8/src/msmath/graph.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/matrix.py` & `msmath-1.0.8/src/msmath/matrix.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/numfuns.py` & `msmath-1.0.8/src/msmath/numfuns.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/optable.py` & `msmath-1.0.8/src/msmath/optable.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/poly.py` & `msmath-1.0.8/src/msmath/poly.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/quaternion.py` & `msmath-1.0.8/src/msmath/quaternion.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/rational.py` & `msmath-1.0.8/src/msmath/rational.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath/share.py` & `msmath-1.0.8/src/msmath/share.py`

 * *Files identical despite different names*

### Comparing `msmath-1.0.6/src/msmath.egg-info/PKG-INFO` & `msmath-1.0.8/src/msmath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: msmath
-Version: 1.0.6
+Version: 1.0.8
 Summary: mathematical Python classes: finite fields, rationals, quaternions, matrices, polynomials, graphs, bitstrings
+Home-page: https://github.com/ms0/msmath
+Author: Mike Speciner
 Author-email: Mike Speciner <ms@alum.mit.edu>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

