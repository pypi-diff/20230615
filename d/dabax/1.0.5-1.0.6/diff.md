# Comparing `tmp/dabax-1.0.5.tar.gz` & `tmp/dabax-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dabax-1.0.5.tar", last modified: Mon May  9 13:48:14 2022, max compression
+gzip compressed data, was "dist/dabax-1.0.6.tar", last modified: Thu Jun 15 07:41:43 2023, max compression
```

## Comparing `dabax-1.0.5.tar` & `dabax-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-05-09 13:48:14.000000 dabax-1.0.5/
--rw-r--r--   0 srio      (4230) soft      (3401)     1096 2021-10-22 09:05:26.000000 dabax-1.0.5/LICENSE
--rw-r--r--   0 srio      (4230) soft      (3401)      254 2022-05-09 13:48:14.000000 dabax-1.0.5/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)       88 2021-10-22 09:05:26.000000 dabax-1.0.5/README.md
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-05-09 13:48:14.000000 dabax-1.0.5/dabax/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-10-22 09:06:12.000000 dabax-1.0.5/dabax/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    55193 2022-01-28 08:37:57.000000 dabax-1.0.5/dabax/common_tools.py
--rw-r--r--   0 srio      (4230) soft      (3401)    26872 2022-05-06 07:32:11.000000 dabax-1.0.5/dabax/dabax_base.py
--rw-r--r--   0 srio      (4230) soft      (3401)      846 2022-05-06 07:33:59.000000 dabax-1.0.5/dabax/dabax_files.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8837 2022-05-09 10:49:18.000000 dabax-1.0.5/dabax/dabax_xraylib.py
--rw-r--r--   0 srio      (4230) soft      (3401)    19881 2022-05-09 10:39:21.000000 dabax-1.0.5/dabax/dabax_xraylib_decorator.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-05-09 13:48:14.000000 dabax-1.0.5/dabax.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)      254 2022-05-09 13:48:13.000000 dabax-1.0.5/dabax.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)      307 2022-05-09 13:48:13.000000 dabax-1.0.5/dabax.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-05-09 13:48:13.000000 dabax-1.0.5/dabax.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       17 2022-05-09 13:48:13.000000 dabax-1.0.5/dabax.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        6 2022-05-09 13:48:13.000000 dabax-1.0.5/dabax.egg-info/top_level.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-05-09 13:48:14.000000 dabax-1.0.5/setup.cfg
--rw-r--r--   0 srio      (4230) soft      (3401)     1835 2022-05-09 13:48:01.000000 dabax-1.0.5/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-06-15 07:41:43.000000 dabax-1.0.6/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1096 2021-10-22 09:05:26.000000 dabax-1.0.6/LICENSE
+-rw-r--r--   0 srio      (4230) soft      (3401)      254 2023-06-15 07:41:43.000000 dabax-1.0.6/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)      137 2023-03-09 08:48:25.000000 dabax-1.0.6/README.md
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-10-22 09:06:12.000000 dabax-1.0.6/dabax/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    55193 2022-01-28 08:37:57.000000 dabax-1.0.6/dabax/common_tools.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    26837 2023-06-15 07:26:54.000000 dabax-1.0.6/dabax/dabax_base.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      846 2022-05-06 07:33:59.000000 dabax-1.0.6/dabax/dabax_files.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8837 2022-05-10 11:07:50.000000 dabax-1.0.6/dabax/dabax_xraylib.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    19881 2022-05-09 10:39:21.000000 dabax-1.0.6/dabax/dabax_xraylib_decorator.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)      254 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)      307 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       17 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        6 2023-06-15 07:41:43.000000 dabax-1.0.6/dabax.egg-info/top_level.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2023-06-15 07:41:43.000000 dabax-1.0.6/setup.cfg
+-rw-r--r--   0 srio      (4230) soft      (3401)     1835 2023-06-15 07:27:46.000000 dabax-1.0.6/setup.py
```

### Comparing `dabax-1.0.5/LICENSE` & `dabax-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dabax-1.0.5/dabax/common_tools.py` & `dabax-1.0.6/dabax/common_tools.py`

 * *Files identical despite different names*

### Comparing `dabax-1.0.5/dabax/dabax_base.py` & `dabax-1.0.6/dabax/dabax_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 dabax: python module for processing remote files containing dabax
 
 """
 
 import numpy
 import os
-import socket
 from urllib.request import urlretrieve
 from silx.io.specfile import SpecFile
 
 from dabax.common_tools import calculate_f0_from_f0coeff, f0_interpolate_coefficients
 from dabax.common_tools import atomic_symbols, atomic_names, atomic_number
 from dabax.common_tools import parse_formula
 
@@ -33,18 +32,15 @@
 
         if dabax_repository is None:
             self._dabax_repository = self.get_dabax_default_repository()
         else:
             self._dabax_repository = dabax_repository
 
     def get_dabax_default_repository(self):
-        if socket.getfqdn().find("esrf") >= 0:
-            return "http://ftp.esrf.fr/pub/scisoft/DabaxFiles/"
-        else:
-            return "http://ftp.esrf.eu/pub/scisoft/DabaxFiles/"
+        return "https://raw.githubusercontent.com/oasys-kit/DabaxFiles/main/"
 
     def set_dabax_repository(self, repo):
         self._dabax_repository = repo
 
     def get_dabax_repository(self):
         return self._dabax_repository
 
@@ -616,15 +612,16 @@
             "nAtoms" :fatomic,
             "molarMass": mweight,
         }
 
         return new_dict
 
 if __name__ == '__main__':
-    dx = DabaxBase()
+    dx = DabaxBase(dabax_repository="https://gitlab.esrf.fr/srio/dabaxfiles/-/raw/main/")
+    print(dx.info())
     #
     # f0
     #
     if False:
         #
         # test f0 data for B3+
         #
```

### Comparing `dabax-1.0.5/dabax/dabax_files.py` & `dabax-1.0.6/dabax/dabax_files.py`

 * *Files identical despite different names*

### Comparing `dabax-1.0.5/dabax/dabax_xraylib.py` & `dabax-1.0.6/dabax/dabax_xraylib.py`

 * *Files identical despite different names*

### Comparing `dabax-1.0.5/dabax/dabax_xraylib_decorator.py` & `dabax-1.0.6/dabax/dabax_xraylib_decorator.py`

 * *Files identical despite different names*

### Comparing `dabax-1.0.5/setup.py` & `dabax-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 __authors__ = ["M Sanchez del Rio - ESRF"]
 __license__ = "MIT"
 __date__ = "22/10/2021"
 
 from setuptools import setup, find_packages
 
 setup(name='dabax',
-    version='1.0.5',
+    version='1.0.6',
     description='python access to DABAX files',
     author='M Sanchez del Rio',
     author_email='srio@esrf.eu',
     url='https://github.com/oasys-kit/dabax/',
     packages=find_packages(include=['dabax', 'dabax.*']),
     install_requires=[
         'numpy',
```

