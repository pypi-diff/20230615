# Comparing `tmp/embarrassing_qwertyuu-0.0.1.tar.gz` & `tmp/embarrassing_qwertyuu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embarrassing_qwertyuu-0.0.1.tar", last modified: Thu Jun 15 02:08:46 2023, max compression
+gzip compressed data, was "embarrassing_qwertyuu-0.0.2.tar", last modified: Thu Jun 15 02:09:45 2023, max compression
```

## Comparing `embarrassing_qwertyuu-0.0.1.tar` & `embarrassing_qwertyuu-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:08:46.278920 embarrassing_qwertyuu-0.0.1/
--rw-rw-rw-   0        0        0      405 2023-06-15 02:08:46.277920 embarrassing_qwertyuu-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 02:08:46.268920 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/
--rw-rw-rw-   0        0        0      405 2023-06-15 02:08:46.000000 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-15 02:08:46.000000 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:08:46.000000 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 02:08:46.000000 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-15 02:08:46.000000 embarrassing_qwertyuu-0.0.1/embarrassing_qwertyuu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:08:46.278920 embarrassing_qwertyuu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-06-15 02:07:44.000000 embarrassing_qwertyuu-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:08:46.270944 embarrassing_qwertyuu-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-15 02:05:53.000000 embarrassing_qwertyuu-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:08:46.274918 embarrassing_qwertyuu-0.0.1/src/embarrassing_qwertyuu/
--rw-rw-rw-   0        0        0        0 2023-06-15 02:05:43.000000 embarrassing_qwertyuu-0.0.1/src/embarrassing_qwertyuu/__init__.py
--rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing_qwertyuu-0.0.1/src/embarrassing_qwertyuu/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:09:45.507984 embarrassing_qwertyuu-0.0.2/
+-rw-rw-rw-   0        0        0      405 2023-06-15 02:09:45.506985 embarrassing_qwertyuu-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 02:09:45.497983 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-06-15 02:09:45.000000 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-15 02:09:45.000000 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:09:45.000000 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 02:09:45.000000 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-15 02:09:45.000000 embarrassing_qwertyuu-0.0.2/embarrassing_qwertyuu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:09:45.508987 embarrassing_qwertyuu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-06-15 02:09:40.000000 embarrassing_qwertyuu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:09:45.500013 embarrassing_qwertyuu-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-15 02:05:53.000000 embarrassing_qwertyuu-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:09:45.504014 embarrassing_qwertyuu-0.0.2/src/embarrassing_qwertyuu/
+-rw-rw-rw-   0        0        0        0 2023-06-15 02:05:43.000000 embarrassing_qwertyuu-0.0.2/src/embarrassing_qwertyuu/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing_qwertyuu-0.0.2/src/embarrassing_qwertyuu/main.py
```

### Comparing `embarrassing_qwertyuu-0.0.1/setup.py` & `embarrassing_qwertyuu-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="embarrassing_qwertyuu",
-    version="0.0.1",
+    version="0.0.2",
     description="A package to embarrassingly parallelize your code",
     author="Raphaël Côté",
     author_email="cotlarrc@gmail.com",
     # url="<package-url>",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

