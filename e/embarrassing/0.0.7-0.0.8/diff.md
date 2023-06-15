# Comparing `tmp/embarrassing-0.0.7.tar.gz` & `tmp/embarrassing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embarrassing-0.0.7.tar", last modified: Thu Jun 15 02:40:04 2023, max compression
+gzip compressed data, was "embarrassing-0.0.8.tar", last modified: Thu Jun 15 02:58:52 2023, max compression
```

## Comparing `embarrassing-0.0.7.tar` & `embarrassing-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.207524 embarrassing-0.0.7/
--rw-rw-rw-   0        0        0      396 2023-06-15 02:40:04.206513 embarrassing-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.193494 embarrassing-0.0.7/embarrassing/
--rw-rw-rw-   0        0        0       60 2023-06-15 02:39:01.000000 embarrassing-0.0.7/embarrassing/__init__.py
--rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.7/embarrassing/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:40:04.204494 embarrassing-0.0.7/embarrassing.egg-info/
--rw-rw-rw-   0        0        0      396 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 02:40:04.000000 embarrassing-0.0.7/embarrassing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:40:04.207524 embarrassing-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-06-15 02:40:02.000000 embarrassing-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.512090 embarrassing-0.0.8/
+-rw-rw-rw-   0        0        0     2006 2023-06-15 02:58:52.511136 embarrassing-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1567 2023-06-15 02:58:14.000000 embarrassing-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.498134 embarrassing-0.0.8/embarrassing/
+-rw-rw-rw-   0        0        0       60 2023-06-15 02:39:01.000000 embarrassing-0.0.8/embarrassing/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.8/embarrassing/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.509144 embarrassing-0.0.8/embarrassing.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:58:52.513094 embarrassing-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-06-15 02:58:21.000000 embarrassing-0.0.8/setup.py
```

### Comparing `embarrassing-0.0.7/setup.py` & `embarrassing-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from setuptools import setup, find_packages
 
+
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name="embarrassing",
-    version="0.0.7",
+    version="0.0.8",
     description="A package to embarrassingly parallelize your code",
     author="Raphaël Côté",
     author_email="cotlarrc@gmail.com",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     # url="<package-url>",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

