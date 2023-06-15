# Comparing `tmp/multisesh-0.0.8.tar.gz` & `tmp/multisesh-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisesh-0.0.8.tar", last modified: Fri Mar  5 10:23:25 2021, max compression
+gzip compressed data, was "multisesh-0.0.9.tar", last modified: Fri Mar  5 10:26:42 2021, max compression
```

## Comparing `multisesh-0.0.8.tar` & `multisesh-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-03-05 10:23:25.248996 multisesh-0.0.8/
--rw-rw-rw-   0        0        0     1068 2021-02-27 09:53:20.000000 multisesh-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       49 2021-03-03 21:16:43.000000 multisesh-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6417 2021-03-05 10:23:25.247009 multisesh-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5409 2021-02-04 14:14:56.000000 multisesh-0.0.8/readme.md
--rw-rw-rw-   0        0        0       42 2021-03-05 10:23:25.249994 multisesh-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      958 2021-03-05 10:22:47.000000 multisesh-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-05 10:23:25.224611 multisesh-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2021-03-05 10:23:25.244308 multisesh-0.0.8/src/multisesh.egg-info/
--rw-rw-rw-   0        0        0     6417 2021-03-05 10:23:25.000000 multisesh-0.0.8/src/multisesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2021-03-05 10:23:25.000000 multisesh-0.0.8/src/multisesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-05 10:23:25.000000 multisesh-0.0.8/src/multisesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2021-03-05 10:23:25.000000 multisesh-0.0.8/src/multisesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2021-03-05 10:23:25.000000 multisesh-0.0.8/src/multisesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-05 10:26:42.303829 multisesh-0.0.9/
+-rw-rw-rw-   0        0        0     1068 2021-02-27 09:53:20.000000 multisesh-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       49 2021-03-03 21:16:43.000000 multisesh-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6417 2021-03-05 10:26:42.302832 multisesh-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5409 2021-02-04 14:14:56.000000 multisesh-0.0.9/readme.md
+-rw-rw-rw-   0        0        0       42 2021-03-05 10:26:42.303829 multisesh-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      958 2021-03-05 10:26:02.000000 multisesh-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-05 10:26:42.281196 multisesh-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-03-05 10:26:42.300836 multisesh-0.0.9/src/multisesh.egg-info/
+-rw-rw-rw-   0        0        0     6417 2021-03-05 10:26:42.000000 multisesh-0.0.9/src/multisesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2021-03-05 10:26:42.000000 multisesh-0.0.9/src/multisesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-05 10:26:42.000000 multisesh-0.0.9/src/multisesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2021-03-05 10:26:42.000000 multisesh-0.0.9/src/multisesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2021-03-05 10:26:42.000000 multisesh-0.0.9/src/multisesh.egg-info/top_level.txt
```

### Comparing `multisesh-0.0.8/LICENSE.txt` & `multisesh-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multisesh-0.0.8/PKG-INFO` & `multisesh-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisesh
-Version: 0.0.8
+Version: 0.0.9
 Summary: Handles microscope imaging data made by multiple sessions.
 Home-page: https://github.com/TomPJWyatt/MultiSesh
 Author: Tom Wyatt
 Author-email: womtyatt@gmail.com
 License: UNKNOWN
 Description: # MultiSesh
```

### Comparing `multisesh-0.0.8/readme.md` & `multisesh-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `multisesh-0.0.8/setup.py` & `multisesh-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='multisesh', 
-    version='0.0.8', 
+    version='0.0.9', 
     author='Tom Wyatt',
     author_email='womtyatt@gmail.com',
     url='https://github.com/TomPJWyatt/MultiSesh',
     license_files = 'MIT',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `multisesh-0.0.8/src/multisesh.egg-info/PKG-INFO` & `multisesh-0.0.9/src/multisesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisesh
-Version: 0.0.8
+Version: 0.0.9
 Summary: Handles microscope imaging data made by multiple sessions.
 Home-page: https://github.com/TomPJWyatt/MultiSesh
 Author: Tom Wyatt
 Author-email: womtyatt@gmail.com
 License: UNKNOWN
 Description: # MultiSesh
```

