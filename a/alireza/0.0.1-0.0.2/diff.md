# Comparing `tmp/alireza-0.0.1.tar.gz` & `tmp/alireza-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alireza-0.0.1.tar", last modified: Thu Jun 15 15:50:26 2023, max compression
+gzip compressed data, was "alireza-0.0.2.tar", last modified: Thu Jun 15 16:20:59 2023, max compression
```

## Comparing `alireza-0.0.1.tar` & `alireza-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 15:50:26.730762 alireza-0.0.1/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 15:50:26.730762 alireza-0.0.1/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.1/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 15:50:26.730762 alireza-0.0.1/alireza/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       46 2023-06-14 12:30:53.000000 alireza-0.0.1/alireza/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2076 2023-06-14 14:14:09.000000 alireza-0.0.1/alireza/django_tools.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 15:50:26.730762 alireza-0.0.1/alireza.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 15:50:26.000000 alireza-0.0.1/alireza.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      186 2023-06-15 15:50:26.000000 alireza-0.0.1/alireza.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-06-15 15:50:26.000000 alireza-0.0.1/alireza.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-06-15 15:50:26.000000 alireza-0.0.1/alireza.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-06-15 15:50:26.730762 alireza-0.0.1/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      934 2023-06-15 15:50:24.000000 alireza-0.0.1/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.942122 alireza-0.0.2/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 16:20:59.942122 alireza-0.0.2/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.2/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.938122 alireza-0.0.2/alireza/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       54 2023-06-15 16:11:41.000000 alireza-0.0.2/alireza/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2076 2023-06-14 14:14:09.000000 alireza-0.0.2/alireza/django_tools.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.938122 alireza-0.0.2/alireza.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      186 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-06-15 16:20:59.942122 alireza-0.0.2/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      934 2023-06-15 16:20:12.000000 alireza-0.0.2/setup.py
```

### Comparing `alireza-0.0.1/PKG-INFO` & `alireza-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful tools for python frameworks
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
```

### Comparing `alireza-0.0.1/alireza/django_tools.py` & `alireza-0.0.2/alireza/django_tools.py`

 * *Files identical despite different names*

### Comparing `alireza-0.0.1/alireza.egg-info/PKG-INFO` & `alireza-0.0.2/alireza.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful tools for python frameworks
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
```

### Comparing `alireza-0.0.1/setup.py` & `alireza-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Useful tools for python frameworks'
 LONG_DESCRIPTION = 'The purpose of starting this project is to make useful tools for all Python frameworks and make the life of programmers easier :)'
 
 # Setting up
 setup(
     name="alireza",
     version=VERSION,
```

