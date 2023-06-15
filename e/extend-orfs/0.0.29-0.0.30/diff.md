# Comparing `tmp/extend_orfs-0.0.29.tar.gz` & `tmp/extend_orfs-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend_orfs-0.0.29.tar", last modified: Thu Jun 15 14:24:52 2023, max compression
+gzip compressed data, was "extend_orfs-0.0.30.tar", last modified: Thu Jun 15 14:37:07 2023, max compression
```

## Comparing `extend_orfs-0.0.29.tar` & `extend_orfs-0.0.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/
--rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/PKG-INFO
--rw-rw-r--   0 joan      (1000) joan      (1000)       14 2022-11-24 14:56:36.000000 extend_orfs-0.0.29/README.md
--rw-rw-r--   0 joan      (1000) joan      (1000)      104 2021-06-11 14:00:42.000000 extend_orfs-0.0.29/pyproject.toml
--rw-rw-r--   0 joan      (1000) joan      (1000)      774 2023-06-15 14:24:52.149291 extend_orfs-0.0.29/setup.cfg
--rw-rw-r--   0 joan      (1000) joan      (1000)       69 2021-06-14 10:13:07.000000 extend_orfs-0.0.29/setup.py
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.141291 extend_orfs-0.0.29/src/
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/src/extend_orfs/
--rw-rw-r--   0 joan      (1000) joan      (1000)       27 2022-12-01 15:21:34.000000 extend_orfs-0.0.29/src/extend_orfs/__init__.py
--rwxrw-r--   0 joan      (1000) joan      (1000)    25595 2023-06-15 14:24:03.000000 extend_orfs-0.0.29/src/extend_orfs/extend_orfs.py
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/src/extend_orfs.egg-info/
--rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/PKG-INFO
--rw-rw-r--   0 joan      (1000) joan      (1000)      296 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/SOURCES.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)        1 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/dependency_links.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)       56 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/requires.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)       12 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/top_level.txt
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:37:07.966076 extend_orfs-0.0.30/
+-rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:37:07.966076 extend_orfs-0.0.30/PKG-INFO
+-rw-rw-r--   0 joan      (1000) joan      (1000)       14 2022-11-24 14:56:36.000000 extend_orfs-0.0.30/README.md
+-rw-rw-r--   0 joan      (1000) joan      (1000)      104 2021-06-11 14:00:42.000000 extend_orfs-0.0.30/pyproject.toml
+-rw-rw-r--   0 joan      (1000) joan      (1000)      774 2023-06-15 14:37:07.966076 extend_orfs-0.0.30/setup.cfg
+-rw-rw-r--   0 joan      (1000) joan      (1000)       69 2021-06-14 10:13:07.000000 extend_orfs-0.0.30/setup.py
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:37:07.962076 extend_orfs-0.0.30/src/
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:37:07.962076 extend_orfs-0.0.30/src/extend_orfs/
+-rw-rw-r--   0 joan      (1000) joan      (1000)       27 2022-12-01 15:21:34.000000 extend_orfs-0.0.30/src/extend_orfs/__init__.py
+-rwxrw-r--   0 joan      (1000) joan      (1000)    25595 2023-06-15 14:36:22.000000 extend_orfs-0.0.30/src/extend_orfs/extend_orfs.py
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:37:07.966076 extend_orfs-0.0.30/src/extend_orfs.egg-info/
+-rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:37:07.000000 extend_orfs-0.0.30/src/extend_orfs.egg-info/PKG-INFO
+-rw-rw-r--   0 joan      (1000) joan      (1000)      296 2023-06-15 14:37:07.000000 extend_orfs-0.0.30/src/extend_orfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)        1 2023-06-15 14:37:07.000000 extend_orfs-0.0.30/src/extend_orfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)       56 2023-06-15 14:37:07.000000 extend_orfs-0.0.30/src/extend_orfs.egg-info/requires.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)       12 2023-06-15 14:37:07.000000 extend_orfs-0.0.30/src/extend_orfs.egg-info/top_level.txt
```

### Comparing `extend_orfs-0.0.29/setup.cfg` & `extend_orfs-0.0.30/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = extend_orfs
-version = 0.0.29
+version = 0.0.30
 author = Joan Pallarès-Albanell
 author_email = joan.pallares.albanell@gmail.com
 description = MModule description
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JoanPAAL/extend_orfs/
 project_urls =
```

### Comparing `extend_orfs-0.0.29/src/extend_orfs/extend_orfs.py` & `extend_orfs-0.0.30/src/extend_orfs/extend_orfs.py`

 * *Files identical despite different names*

