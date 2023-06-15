# Comparing `tmp/test4957-0.2.1.tar.gz` & `tmp/test4957-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test4957-0.2.1.tar", last modified: Thu Jun 15 03:22:04 2023, max compression
+gzip compressed data, was "test4957-0.2.2.tar", last modified: Thu Jun 15 03:26:08 2023, max compression
```

## Comparing `test4957-0.2.1.tar` & `test4957-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:22:04.705194 test4957-0.2.1/
--rw-r--r--   0 nate       (501) staff       (20)       26 2023-06-15 03:13:23.000000 test4957-0.2.1/MANIFEST.in
--rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:22:04.705052 test4957-0.2.1/PKG-INFO
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:22:04.700991 test4957-0.2.1/pypdfe/
--rw-r--r--   0 nate       (501) staff       (20)     4049 2023-06-15 00:34:56.000000 test4957-0.2.1/pypdfe/EstimatePDFmv.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:22:04.704026 test4957-0.2.1/pypdfe/PDF-Estimator/
--rw-r--r--   0 nate       (501) staff       (20)     3056 2022-09-25 16:31:28.000000 test4957-0.2.1/pypdfe/PDF-Estimator/ChebyShev.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1586 2022-09-25 16:33:30.000000 test4957-0.2.1/pypdfe/PDF-Estimator/ChebyShev.h
--rw-r--r--   0 nate       (501) staff       (20)    10093 2022-09-29 15:35:28.000000 test4957-0.2.1/pypdfe/PDF-Estimator/InputData.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2292 2022-04-07 14:12:38.000000 test4957-0.2.1/pypdfe/PDF-Estimator/InputData.h
--rw-r--r--   0 nate       (501) staff       (20)     8394 2022-09-29 15:42:06.000000 test4957-0.2.1/pypdfe/PDF-Estimator/InputParameters.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2561 2022-04-04 18:13:02.000000 test4957-0.2.1/pypdfe/PDF-Estimator/InputParameters.h
--rw-r--r--   0 nate       (501) staff       (20)     5070 2022-07-06 18:40:54.000000 test4957-0.2.1/pypdfe/PDF-Estimator/JointProbability.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1763 2022-05-29 22:47:00.000000 test4957-0.2.1/pypdfe/PDF-Estimator/JointProbability.h
--rw-r--r--   0 nate       (501) staff       (20)    17670 2022-06-05 16:45:36.000000 test4957-0.2.1/pypdfe/PDF-Estimator/MinimizeScore.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2932 2022-06-05 16:42:44.000000 test4957-0.2.1/pypdfe/PDF-Estimator/MinimizeScore.h
--rw-r--r--   0 nate       (501) staff       (20)     4528 2022-08-10 17:22:36.000000 test4957-0.2.1/pypdfe/PDF-Estimator/OutputControl.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2094 2023-04-07 13:47:26.000000 test4957-0.2.1/pypdfe/PDF-Estimator/OutputControl.h
--rw-r--r--   0 nate       (501) staff       (20)     2024 2022-06-05 16:43:32.000000 test4957-0.2.1/pypdfe/PDF-Estimator/Score.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1912 2022-06-05 16:44:50.000000 test4957-0.2.1/pypdfe/PDF-Estimator/Score.h
--rw-r--r--   0 nate       (501) staff       (20)    16296 2022-06-05 16:45:02.000000 test4957-0.2.1/pypdfe/PDF-Estimator/ScoreQZ.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1450 2022-06-05 16:44:30.000000 test4957-0.2.1/pypdfe/PDF-Estimator/ScoreQZ.h
--rw-r--r--   0 nate       (501) staff       (20)     5635 2022-07-03 14:34:52.000000 test4957-0.2.1/pypdfe/PDF-Estimator/Variable.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2053 2022-06-05 16:42:26.000000 test4957-0.2.1/pypdfe/PDF-Estimator/Variable.h
--rw-r--r--   0 nate       (501) staff       (20)    12020 2022-07-01 16:30:00.000000 test4957-0.2.1/pypdfe/PDF-Estimator/WriteResults.cpp
--rw-r--r--   0 nate       (501) staff       (20)     2418 2022-07-01 15:46:10.000000 test4957-0.2.1/pypdfe/PDF-Estimator/WriteResults.h
--rw-r--r--   0 nate       (501) staff       (20)     2490 2022-06-05 16:44:18.000000 test4957-0.2.1/pypdfe/PDF-Estimator/callPDF.cpp
--rw-r--r--   0 nate       (501) staff       (20)     1052 2023-06-14 21:42:19.000000 test4957-0.2.1/pypdfe/PDF-Estimator/callPDF.h
--rw-r--r--   0 nate       (501) staff       (20)     1722 2022-07-15 18:21:28.000000 test4957-0.2.1/pypdfe/PDF-Estimator/mvPDFMain.cpp
--rw-r--r--   0 nate       (501) staff       (20)       41 2023-04-11 08:52:55.000000 test4957-0.2.1/pypdfe/__init__.py
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-06-15 03:22:04.705244 test4957-0.2.1/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      972 2023-06-15 03:22:04.000000 test4957-0.2.1/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:22:04.704828 test4957-0.2.1/test4957.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:22:04.000000 test4957-0.2.1/test4957.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1035 2023-06-15 03:22:04.000000 test4957-0.2.1/test4957.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-06-15 03:22:04.000000 test4957-0.2.1/test4957.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)        6 2023-06-15 03:22:04.000000 test4957-0.2.1/test4957.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        7 2023-06-15 03:22:04.000000 test4957-0.2.1/test4957.egg-info/top_level.txt
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.732785 test4957-0.2.2/
+-rw-r--r--   0 nate       (501) staff       (20)       26 2023-06-15 03:13:23.000000 test4957-0.2.2/MANIFEST.in
+-rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:26:08.732668 test4957-0.2.2/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.709756 test4957-0.2.2/pypdfe/
+-rw-r--r--   0 nate       (501) staff       (20)     4049 2023-06-15 00:34:56.000000 test4957-0.2.2/pypdfe/EstimatePDFmv.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.731770 test4957-0.2.2/pypdfe/PDF-Estimator/
+-rw-r--r--   0 nate       (501) staff       (20)     3056 2022-09-25 16:31:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1586 2022-09-25 16:33:30.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.h
+-rw-r--r--   0 nate       (501) staff       (20)    10093 2022-09-29 15:35:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputData.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2292 2022-04-07 14:12:38.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputData.h
+-rw-r--r--   0 nate       (501) staff       (20)     8394 2022-09-29 15:42:06.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2561 2022-04-04 18:13:02.000000 test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.h
+-rw-r--r--   0 nate       (501) staff       (20)     5070 2022-07-06 18:40:54.000000 test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1763 2022-05-29 22:47:00.000000 test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.h
+-rw-r--r--   0 nate       (501) staff       (20)    17670 2022-06-05 16:45:36.000000 test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2932 2022-06-05 16:42:44.000000 test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.h
+-rw-r--r--   0 nate       (501) staff       (20)     4528 2022-08-10 17:22:36.000000 test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2094 2023-04-07 13:47:26.000000 test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.h
+-rw-r--r--   0 nate       (501) staff       (20)     2024 2022-06-05 16:43:32.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Score.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1912 2022-06-05 16:44:50.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Score.h
+-rw-r--r--   0 nate       (501) staff       (20)    16296 2022-06-05 16:45:02.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1450 2022-06-05 16:44:30.000000 test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.h
+-rw-r--r--   0 nate       (501) staff       (20)     5635 2022-07-03 14:34:52.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Variable.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2053 2022-06-05 16:42:26.000000 test4957-0.2.2/pypdfe/PDF-Estimator/Variable.h
+-rw-r--r--   0 nate       (501) staff       (20)    12020 2022-07-01 16:30:00.000000 test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     2418 2022-07-01 15:46:10.000000 test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.h
+-rw-r--r--   0 nate       (501) staff       (20)     2490 2022-06-05 16:44:18.000000 test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.cpp
+-rw-r--r--   0 nate       (501) staff       (20)     1052 2023-06-14 21:42:19.000000 test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.h
+-rw-r--r--   0 nate       (501) staff       (20)     1722 2022-07-15 18:21:28.000000 test4957-0.2.2/pypdfe/PDF-Estimator/mvPDFMain.cpp
+-rw-r--r--   0 nate       (501) staff       (20)       41 2023-04-11 08:52:55.000000 test4957-0.2.2/pypdfe/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-06-15 03:26:08.732848 test4957-0.2.2/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      972 2023-06-15 03:26:08.000000 test4957-0.2.2/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-06-15 03:26:08.732470 test4957-0.2.2/test4957.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      504 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1035 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)        6 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        7 2023-06-15 03:26:08.000000 test4957-0.2.2/test4957.egg-info/top_level.txt
```

### Comparing `test4957-0.2.1/pypdfe/EstimatePDFmv.py` & `test4957-0.2.2/pypdfe/EstimatePDFmv.py`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/ChebyShev.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/ChebyShev.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/ChebyShev.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/InputData.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/InputData.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/InputData.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/InputData.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/InputParameters.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/InputParameters.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/InputParameters.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/JointProbability.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/JointProbability.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/JointProbability.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/MinimizeScore.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/MinimizeScore.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/MinimizeScore.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/OutputControl.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/OutputControl.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/OutputControl.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/Score.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/Score.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/Score.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/Score.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/ScoreQZ.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/ScoreQZ.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/ScoreQZ.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/Variable.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/Variable.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/Variable.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/Variable.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/WriteResults.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/WriteResults.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/WriteResults.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/callPDF.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/callPDF.h` & `test4957-0.2.2/pypdfe/PDF-Estimator/callPDF.h`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/pypdfe/PDF-Estimator/mvPDFMain.cpp` & `test4957-0.2.2/pypdfe/PDF-Estimator/mvPDFMain.cpp`

 * *Files identical despite different names*

### Comparing `test4957-0.2.1/setup.py` & `test4957-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 NAME = 'test4957'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'pydfe development version'
 LONG_DESCRIPTION = 'pydfe development version long description.'
 
 # Setting up
 setup(
     name=NAME,
     version=VERSION,
```

### Comparing `test4957-0.2.1/test4957.egg-info/SOURCES.txt` & `test4957-0.2.2/test4957.egg-info/SOURCES.txt`

 * *Files identical despite different names*

