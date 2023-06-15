# Comparing `tmp/http_helper-0.0.1.tar.gz` & `tmp/http_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_helper-0.0.1.tar", last modified: Thu Jun 15 17:40:28 2023, max compression
+gzip compressed data, was "http_helper-0.0.2.tar", last modified: Thu Jun 15 18:33:58 2023, max compression
```

## Comparing `http_helper-0.0.1.tar` & `http_helper-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 17:40:28.279236 http_helper-0.0.1/
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      208 2023-06-15 17:40:28.279306 http_helper-0.0.1/PKG-INFO
-drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 17:40:28.277318 http_helper-0.0.1/http_helper/
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)        0 2022-04-18 08:52:30.000000 http_helper-0.0.1/http_helper/__init__.py
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)     1297 2023-06-15 15:57:20.000000 http_helper-0.0.1/http_helper/http_helper.py
-drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 17:40:28.279073 http_helper-0.0.1/http_helper.egg-info/
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      208 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/PKG-INFO
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      281 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/SOURCES.txt
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)        1 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/dependency_links.txt
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       62 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/entry_points.txt
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       15 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/requires.txt
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       12 2023-06-15 17:40:28.000000 http_helper-0.0.1/http_helper.egg-info/top_level.txt
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       38 2023-06-15 17:40:28.279569 http_helper-0.0.1/setup.cfg
--rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      417 2023-06-15 17:18:48.000000 http_helper-0.0.1/setup.py
+drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 18:33:58.024228 http_helper-0.0.2/
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      165 2023-06-15 18:33:58.024313 http_helper-0.0.2/PKG-INFO
+drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 18:33:58.022623 http_helper-0.0.2/http_helper/
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)        0 2022-04-18 08:52:30.000000 http_helper-0.0.2/http_helper/__init__.py
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)     1297 2023-06-15 15:57:20.000000 http_helper-0.0.2/http_helper/http_helper.py
+drwxr-xr-x   0 bonam.vamsikrishna   (503) staff       (20)        0 2023-06-15 18:33:58.024044 http_helper-0.0.2/http_helper.egg-info/
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      165 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/PKG-INFO
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      281 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)        1 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       62 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/entry_points.txt
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       15 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/requires.txt
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       12 2023-06-15 18:33:58.000000 http_helper-0.0.2/http_helper.egg-info/top_level.txt
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)       38 2023-06-15 18:33:58.024753 http_helper-0.0.2/setup.cfg
+-rw-r--r--   0 bonam.vamsikrishna   (503) staff       (20)      374 2023-06-15 18:33:43.000000 http_helper-0.0.2/setup.py
```

### Comparing `http_helper-0.0.1/http_helper/http_helper.py` & `http_helper-0.0.2/http_helper/http_helper.py`

 * *Files identical despite different names*

