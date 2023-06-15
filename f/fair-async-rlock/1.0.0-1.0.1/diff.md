# Comparing `tmp/fair_async_rlock-1.0.0.tar.gz` & `tmp/fair_async_rlock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_async_rlock-1.0.0.tar", last modified: Wed Jun 14 23:29:06 2023, max compression
+gzip compressed data, was "fair_async_rlock-1.0.1.tar", last modified: Thu Jun 15 00:13:40 2023, max compression
```

## Comparing `fair_async_rlock-1.0.0.tar` & `fair_async_rlock-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.0/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)      927 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      405 2023-06-14 23:07:24.000000 fair_async_rlock-1.0.0/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/fair_async_rlock/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.0/fair_async_rlock/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1969 2023-06-14 11:44:15.000000 fair_async_rlock-1.0.0/fair_async_rlock/fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/fair_async_rlock/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.0/fair_async_rlock/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12069 2023-06-14 11:51:23.000000 fair_async_rlock-1.0.0/fair_async_rlock/tests/test_fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/fair_async_rlock.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)      927 2023-06-14 23:29:06.000000 fair_async_rlock-1.0.0/fair_async_rlock.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-14 23:29:06.000000 fair_async_rlock-1.0.0/fair_async_rlock.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-14 23:29:06.000000 fair_async_rlock-1.0.0/fair_async_rlock.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-14 23:29:06.000000 fair_async_rlock-1.0.0/fair_async_rlock.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.0/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-14 23:29:06.403895 fair_async_rlock-1.0.0/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-14 11:46:46.000000 fair_async_rlock-1.0.0/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.1/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4862 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4340 2023-06-15 00:12:42.000000 fair_async_rlock-1.0.1/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.994697 fair_async_rlock-1.0.1/fair_async_rlock/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.1/fair_async_rlock/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1969 2023-06-14 11:44:15.000000 fair_async_rlock-1.0.1/fair_async_rlock/fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/fair_async_rlock/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.1/fair_async_rlock/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12069 2023-06-14 11:51:23.000000 fair_async_rlock-1.0.1/fair_async_rlock/tests/test_fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.994697 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4862 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.1/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-14 23:58:07.000000 fair_async_rlock-1.0.1/setup.py
```

### Comparing `fair_async_rlock-1.0.0/LICENSE` & `fair_async_rlock-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.0/fair_async_rlock/fair_async_rlock.py` & `fair_async_rlock-1.0.1/fair_async_rlock/fair_async_rlock.py`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.0/fair_async_rlock/tests/test_fair_async_rlock.py` & `fair_async_rlock-1.0.1/fair_async_rlock/tests/test_fair_async_rlock.py`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.0/setup.py` & `fair_async_rlock-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='fair_async_rlock',
-      version='1.0.0',
+      version='1.0.1',
       description='A well-tested implementation of a fair asynchronous RLock for concurrent programming.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/Joshuaalbert/FairAsyncRLock",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=[],
@@ -22,9 +22,9 @@
       package_dir={'': './'},
       packages=find_packages('./'),
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
       ],
-      python_requires='>=3.6',
+      python_requires='>=3.7',
       )
```

