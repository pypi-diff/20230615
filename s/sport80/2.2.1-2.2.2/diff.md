# Comparing `tmp/sport80-2.2.1.tar.gz` & `tmp/sport80-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sport80-2.2.1.tar", last modified: Wed May 25 18:54:22 2022, max compression
+gzip compressed data, was "sport80-2.2.2.tar", last modified: Wed Jun 14 22:17:38 2023, max compression
```

## Comparing `sport80-2.2.1.tar` & `sport80-2.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 18:54:22.668584 sport80-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-05-25 18:54:09.000000 sport80-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-05-25 18:54:22.668584 sport80-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-25 18:54:09.000000 sport80-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-25 18:54:22.668584 sport80-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-25 18:54:09.000000 sport80-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 18:54:22.664584 sport80-2.2.1/sport80/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6642 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/pages_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/request_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/sport80.py
--rw-r--r--   0 runner    (1001) docker     (121)     7997 2022-05-25 18:54:09.000000 sport80-2.2.1/sport80/sport80_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 18:54:22.668584 sport80-2.2.1/sport80.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-05-25 18:54:22.000000 sport80-2.2.1/sport80.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-05-25 18:54:22.000000 sport80-2.2.1/sport80.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 18:54:22.000000 sport80-2.2.1/sport80.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-25 18:54:22.000000 sport80-2.2.1/sport80.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-25 18:54:22.000000 sport80-2.2.1/sport80.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:17:38.155637 sport80-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-14 22:17:17.000000 sport80-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 22:17:38.155637 sport80-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-14 22:17:17.000000 sport80-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:17:38.155637 sport80-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 22:17:17.000000 sport80-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:17:38.155637 sport80-2.2.2/sport80/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/pages_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/request_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/sport80.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-14 22:17:17.000000 sport80-2.2.2/sport80/sport80_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:17:38.155637 sport80-2.2.2/sport80.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 22:17:38.000000 sport80-2.2.2/sport80.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-14 22:17:38.000000 sport80-2.2.2/sport80.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:17:38.000000 sport80-2.2.2/sport80.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 22:17:38.000000 sport80-2.2.2/sport80.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 22:17:38.000000 sport80-2.2.2/sport80.egg-info/top_level.txt
```

### Comparing `sport80-2.2.1/LICENSE` & `sport80-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sport80-2.2.1/setup.py` & `sport80-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Setup file for PyPi """
 from setuptools import setup
 
 setup(
     name="sport80",
-    version="2.2.1",
+    version="2.2.2",
     description="Python API interface for the Sport80 sites",
     long_description='Intentionally empty',
     url="https://github.com/euanwm/sport80_api",
     author="Euan Meston",
     author_email="euanmeston@gmail.com",
     license="BSD",
     install_requires=["requests",
```

### Comparing `sport80-2.2.1/sport80/helpers.py` & `sport80-2.2.2/sport80/helpers.py`

 * *Files identical despite different names*

### Comparing `sport80-2.2.1/sport80/pages_enum.py` & `sport80-2.2.2/sport80/pages_enum.py`

 * *Files identical despite different names*

### Comparing `sport80-2.2.1/sport80/request_dataclasses.py` & `sport80-2.2.2/sport80/request_dataclasses.py`

 * *Files identical despite different names*

### Comparing `sport80-2.2.1/sport80/sport80.py` & `sport80-2.2.2/sport80/sport80.py`

 * *Files identical despite different names*

### Comparing `sport80-2.2.1/sport80/sport80_http_client.py` & `sport80-2.2.2/sport80/sport80_http_client.py`

 * *Files identical despite different names*

