# Comparing `tmp/embarrassing-0.0.6.tar.gz` & `tmp/embarrassing-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embarrassing-0.0.6.tar", last modified: Thu Jun 15 02:36:23 2023, max compression
+gzip compressed data, was "embarrassing-0.0.7.tar", last modified: Thu Jun 15 02:40:04 2023, max compression
```

## Comparing `embarrassing-0.0.6.tar` & `embarrassing-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:36:23.172138 embarrassing-0.0.6/
--rw-rw-rw-   0        0        0      396 2023-06-15 02:36:23.171138 embarrassing-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 02:36:23.157439 embarrassing-0.0.6/embarrassing/
--rw-rw-rw-   0        0        0       59 2023-06-15 02:35:10.000000 embarrassing-0.0.6/embarrassing/__init__.py
--rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.6/embarrassing/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:36:23.169129 embarrassing-0.0.6/embarrassing.egg-info/
--rw-rw-rw-   0        0        0      396 2023-06-15 02:36:23.000000 embarrassing-0.0.6/embarrassing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 02:36:23.000000 embarrassing-0.0.6/embarrassing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:36:23.000000 embarrassing-0.0.6/embarrassing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 02:36:23.000000 embarrassing-0.0.6/embarrassing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 02:36:23.000000 embarrassing-0.0.6/embarrassing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:36:23.172138 embarrassing-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-06-15 02:35:54.000000 embarrassing-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.207524 embarrassing-0.0.7/
+-rw-rw-rw-   0        0        0      396 2023-06-15 02:40:04.206513 embarrassing-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.193494 embarrassing-0.0.7/embarrassing/
+-rw-rw-rw-   0        0        0       60 2023-06-15 02:39:01.000000 embarrassing-0.0.7/embarrassing/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.7/embarrassing/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.204494 embarrassing-0.0.7/embarrassing.egg-info/
+-rw-rw-rw-   0        0        0      396 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:40:04.207524 embarrassing-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-06-15 02:40:02.000000 embarrassing-0.0.7/setup.py
```

### Comparing `embarrassing-0.0.6/setup.py` & `embarrassing-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="embarrassing",
-    version="0.0.6",
+    version="0.0.7",
     description="A package to embarrassingly parallelize your code",
     author="Raphaël Côté",
     author_email="cotlarrc@gmail.com",
     # url="<package-url>",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

