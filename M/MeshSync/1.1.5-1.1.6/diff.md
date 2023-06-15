# Comparing `tmp/MeshSync-1.1.5.tar.gz` & `tmp/MeshSync-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeshSync-1.1.5.tar", last modified: Thu Jun 15 19:57:19 2023, max compression
+gzip compressed data, was "MeshSync-1.1.6.tar", last modified: Thu Jun 15 19:58:40 2023, max compression
```

## Comparing `MeshSync-1.1.5.tar` & `MeshSync-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:57:19.561356 MeshSync-1.1.5/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      136 2022-06-01 04:54:00.000000 MeshSync-1.1.5/LICENSE
--rw-r--r--   0 rawandahmad   (501) staff       (20)       15 2022-06-01 04:54:00.000000 MeshSync-1.1.5/MANIFEST.in
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:57:19.560087 MeshSync-1.1.5/MeshSync.egg-info/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)      315 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/SOURCES.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/dependency_links.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)       54 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/entry_points.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        6 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/requires.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-15 19:57:19.000000 MeshSync-1.1.5/MeshSync.egg-info/top_level.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:57:19.561155 MeshSync-1.1.5/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)       99 2022-07-05 16:20:52.000000 MeshSync-1.1.5/README.rst
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:57:19.560747 MeshSync-1.1.5/meshsync/
--rw-r--r--   0 rawandahmad   (501) staff       (20)        0 2022-06-01 04:54:00.000000 MeshSync-1.1.5/meshsync/__init__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)      142 2023-06-15 19:56:20.000000 MeshSync-1.1.5/meshsync/__main__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)    13973 2023-06-15 19:56:55.000000 MeshSync-1.1.5/meshsync/mesh_sync.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)      818 2023-06-15 19:36:09.000000 MeshSync-1.1.5/meshsync/vault.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-15 19:57:19.561429 MeshSync-1.1.5/setup.cfg
--rw-r--r--   0 rawandahmad   (501) staff       (20)      700 2023-06-15 19:55:08.000000 MeshSync-1.1.5/setup.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:58:40.064453 MeshSync-1.1.6/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      136 2022-06-01 04:54:00.000000 MeshSync-1.1.6/LICENSE
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       15 2022-06-01 04:54:00.000000 MeshSync-1.1.6/MANIFEST.in
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:58:40.063516 MeshSync-1.1.6/MeshSync.egg-info/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      315 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/SOURCES.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/dependency_links.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       54 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/entry_points.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        6 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/requires.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-15 19:58:40.000000 MeshSync-1.1.6/MeshSync.egg-info/top_level.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      355 2023-06-15 19:58:40.064347 MeshSync-1.1.6/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       99 2022-07-05 16:20:52.000000 MeshSync-1.1.6/README.rst
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-15 19:58:40.064067 MeshSync-1.1.6/meshsync/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        0 2022-06-01 04:54:00.000000 MeshSync-1.1.6/meshsync/__init__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      142 2023-06-15 19:56:20.000000 MeshSync-1.1.6/meshsync/__main__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)    14019 2023-06-15 19:58:39.000000 MeshSync-1.1.6/meshsync/mesh_sync.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      818 2023-06-15 19:36:09.000000 MeshSync-1.1.6/meshsync/vault.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-15 19:58:40.064490 MeshSync-1.1.6/setup.cfg
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      700 2023-06-15 19:55:08.000000 MeshSync-1.1.6/setup.py
```

### Comparing `MeshSync-1.1.5/meshsync/mesh_sync.py` & `MeshSync-1.1.6/meshsync/mesh_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 """mesh_sync provides entry point main()."""
 
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 
 import argparse
 import asyncio
 import base64
 import re
 import sys
 import os
@@ -248,15 +248,15 @@
             # Check if 'project' is in the UPDATE_FILE
             with open('UPDATE_FILE', 'r') as f:
                 content = f.read()
                 if 'project' in content:
                     # Get the project name using regex
                     project_name = re.search(r'project:(.*)', content).group(1)
                     print(">> Project name: %s" % project_name)
-                    github_token = get_token_from_env()
+                    github_token = master_token if master_token is not None else get_token_from_env()
                     if not args.t and github_token is None and master_token is None:
                         token = input("Enter your GitHub token: ")
                     elif github_token is not None or master_token is None:
                         token = github_token or master_token
                     else:
                         token = args.t
```

### Comparing `MeshSync-1.1.5/meshsync/vault.py` & `MeshSync-1.1.6/meshsync/vault.py`

 * *Files identical despite different names*

### Comparing `MeshSync-1.1.5/setup.py` & `MeshSync-1.1.6/setup.py`

 * *Files identical despite different names*

