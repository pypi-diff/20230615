# Comparing `tmp/MeshSync-1.1.3.tar.gz` & `tmp/MeshSync-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeshSync-1.1.3.tar", last modified: Thu Jun 15 19:44:59 2023, max compression
+gzip compressed data, was "MeshSync-1.1.4.tar", last modified: Thu Jun 15 19:46:28 2023, max compression
```

## Comparing `MeshSync-1.1.3.tar` & `MeshSync-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:44:59.298195 MeshSync-1.1.3/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      136 2022-06-01 04:54:00.000000 MeshSync-1.1.3/LICENSE
--rw-r--r--   0 rawandahmad   (501) staff       (20)       15 2022-06-01 04:54:00.000000 MeshSync-1.1.3/MANIFEST.in
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:44:59.297215 MeshSync-1.1.3/MeshSync.egg-info/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)      315 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/SOURCES.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/dependency_links.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)       54 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/entry_points.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        6 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/requires.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-15 19:44:59.000000 MeshSync-1.1.3/MeshSync.egg-info/top_level.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:44:59.298074 MeshSync-1.1.3/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)       99 2022-07-05 16:20:52.000000 MeshSync-1.1.3/README.rst
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:44:59.297803 MeshSync-1.1.3/meshsync/
--rw-r--r--   0 rawandahmad   (501) staff       (20)        0 2022-06-01 04:54:00.000000 MeshSync-1.1.3/meshsync/__init__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)      142 2022-06-25 13:44:38.000000 MeshSync-1.1.3/meshsync/__main__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)    13939 2023-06-15 19:44:58.000000 MeshSync-1.1.3/meshsync/mesh_sync.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)      818 2023-06-15 19:36:09.000000 MeshSync-1.1.3/meshsync/vault.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-15 19:44:59.298232 MeshSync-1.1.3/setup.cfg
--rw-r--r--   0 rawandahmad   (501) staff       (20)      700 2023-06-15 17:18:34.000000 MeshSync-1.1.3/setup.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:46:28.052051 MeshSync-1.1.4/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      136 2022-06-01 04:54:00.000000 MeshSync-1.1.4/LICENSE
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       15 2022-06-01 04:54:00.000000 MeshSync-1.1.4/MANIFEST.in
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:46:28.051079 MeshSync-1.1.4/MeshSync.egg-info/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      315 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/SOURCES.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/dependency_links.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       54 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/entry_points.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        6 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/requires.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-15 19:46:28.000000 MeshSync-1.1.4/MeshSync.egg-info/top_level.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:46:28.051939 MeshSync-1.1.4/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       99 2022-07-05 16:20:52.000000 MeshSync-1.1.4/README.rst
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:46:28.051569 MeshSync-1.1.4/meshsync/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        0 2022-06-01 04:54:00.000000 MeshSync-1.1.4/meshsync/__init__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      171 2023-06-15 19:46:09.000000 MeshSync-1.1.4/meshsync/__main__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)    13939 2023-06-15 19:46:09.000000 MeshSync-1.1.4/meshsync/mesh_sync.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      818 2023-06-15 19:36:09.000000 MeshSync-1.1.4/meshsync/vault.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-15 19:46:28.052084 MeshSync-1.1.4/setup.cfg
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      700 2023-06-15 17:18:34.000000 MeshSync-1.1.4/setup.py
```

### Comparing `MeshSync-1.1.3/meshsync/mesh_sync.py` & `MeshSync-1.1.4/meshsync/mesh_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 """mesh_sync provides entry point main()."""
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 import argparse
 import base64
 import re
 import sys
 import os
 import httpx
```

### Comparing `MeshSync-1.1.3/meshsync/vault.py` & `MeshSync-1.1.4/meshsync/vault.py`

 * *Files identical despite different names*

### Comparing `MeshSync-1.1.3/setup.py` & `MeshSync-1.1.4/setup.py`

 * *Files identical despite different names*

