# Comparing `tmp/rongdavbaaddins-0.0.2.0.tar.gz` & `tmp/rongdavbaaddins-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.2.0.tar", last modified: Wed Jun 14 01:33:02 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.2.1.tar", last modified: Thu Jun 15 05:59:15 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.2.0.tar` & `rongdavbaaddins-0.0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.316204 rongdavbaaddins-0.0.2.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      417 2023-06-14 01:33:02.317204 rongdavbaaddins-0.0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.185196 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.223196 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   111558 2023-06-13 01:27:20.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.244204 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   141312 2023-06-14 01:32:05.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/rongdavbaaddins.pyd
--rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27954 2023-06-13 01:27:19.000000 rongdavbaaddins-0.0.2.0/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-14 01:33:02.304206 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      417 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 01:33:01.000000 rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-14 01:33:02.322204 rongdavbaaddins-0.0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-06-14 01:32:33.000000 rongdavbaaddins-0.0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:59:15.057628 rongdavbaaddins-0.0.2.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-06-15 05:59:15.057628 rongdavbaaddins-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 05:59:15.044632 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-15 05:59:15.049628 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   111222 2023-06-15 05:43:44.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-15 05:59:15.051628 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   141312 2023-06-15 05:56:32.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/rongdavbaaddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27954 2023-06-15 05:43:44.000000 rongdavbaaddins-0.0.2.1/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-15 05:59:15.055628 rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-06-15 05:59:14.000000 rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-15 05:59:15.000000 rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 05:59:14.000000 rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 05:59:14.000000 rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-15 05:59:15.059638 rongdavbaaddins-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-06-15 05:58:33.000000 rongdavbaaddins-0.0.2.1/setup.py
```

### Comparing `rongdavbaaddins-0.0.2.0/LICENSE.txt` & `rongdavbaaddins-0.0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.2.1/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.2.1/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.2.1/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.2.0/setup.py` & `rongdavbaaddins-0.0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 2
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.0"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

