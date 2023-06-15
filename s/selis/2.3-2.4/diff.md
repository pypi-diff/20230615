# Comparing `tmp/selis-2.3.tar.gz` & `tmp/selis-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.3.tar", last modified: Thu Jun 15 16:25:48 2023, max compression
+gzip compressed data, was "selis-2.4.tar", last modified: Thu Jun 15 16:32:37 2023, max compression
```

## Comparing `selis-2.3.tar` & `selis-2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:25:48.620825 selis-2.3/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:25:48.620711 selis-2.3/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:25:48.619520 selis-2.3/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.3/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4863 2023-06-15 16:17:22.000000 selis-2.3/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.3/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:25:48.620535 selis-2.3/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 16:25:48.000000 selis-2.3/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 16:25:48.620865 selis-2.3/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-15 16:25:12.000000 selis-2.3/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.514233 selis-2.4/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:32:37.514131 selis-2.4/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.512936 selis-2.4/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.4/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4863 2023-06-15 16:17:22.000000 selis-2.4/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.4/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:32:37.513940 selis-2.4/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 16:32:37.000000 selis-2.4/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 16:32:37.514271 selis-2.4/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-15 16:32:35.000000 selis-2.4/setup.py
```

### Comparing `selis-2.3/selis/client.py` & `selis-2.4/selis/client.py`

 * *Files identical despite different names*

### Comparing `selis-2.3/selis/selis.py` & `selis-2.4/selis/selis.py`

 * *Files identical despite different names*

