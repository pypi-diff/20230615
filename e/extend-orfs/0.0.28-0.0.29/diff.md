# Comparing `tmp/extend_orfs-0.0.28.tar.gz` & `tmp/extend_orfs-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend_orfs-0.0.28.tar", last modified: Thu Jun 15 13:27:15 2023, max compression
+gzip compressed data, was "extend_orfs-0.0.29.tar", last modified: Thu Jun 15 14:24:52 2023, max compression
```

## Comparing `extend_orfs-0.0.28.tar` & `extend_orfs-0.0.29.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 13:27:15.831645 extend_orfs-0.0.28/
--rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 13:27:15.831645 extend_orfs-0.0.28/PKG-INFO
--rw-rw-r--   0 joan      (1000) joan      (1000)       14 2022-11-24 14:56:36.000000 extend_orfs-0.0.28/README.md
--rw-rw-r--   0 joan      (1000) joan      (1000)      104 2021-06-11 14:00:42.000000 extend_orfs-0.0.28/pyproject.toml
--rw-rw-r--   0 joan      (1000) joan      (1000)      774 2023-06-15 13:27:15.835645 extend_orfs-0.0.28/setup.cfg
--rw-rw-r--   0 joan      (1000) joan      (1000)       69 2021-06-14 10:13:07.000000 extend_orfs-0.0.28/setup.py
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 13:27:15.827645 extend_orfs-0.0.28/src/
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 13:27:15.831645 extend_orfs-0.0.28/src/extend_orfs/
--rw-rw-r--   0 joan      (1000) joan      (1000)       27 2022-12-01 15:21:34.000000 extend_orfs-0.0.28/src/extend_orfs/__init__.py
--rwxrw-r--   0 joan      (1000) joan      (1000)    25600 2023-06-15 13:24:51.000000 extend_orfs-0.0.28/src/extend_orfs/extend_orfs.py
-drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 13:27:15.831645 extend_orfs-0.0.28/src/extend_orfs.egg-info/
--rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 13:27:15.000000 extend_orfs-0.0.28/src/extend_orfs.egg-info/PKG-INFO
--rw-rw-r--   0 joan      (1000) joan      (1000)      296 2023-06-15 13:27:15.000000 extend_orfs-0.0.28/src/extend_orfs.egg-info/SOURCES.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)        1 2023-06-15 13:27:15.000000 extend_orfs-0.0.28/src/extend_orfs.egg-info/dependency_links.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)       56 2023-06-15 13:27:15.000000 extend_orfs-0.0.28/src/extend_orfs.egg-info/requires.txt
--rw-rw-r--   0 joan      (1000) joan      (1000)       12 2023-06-15 13:27:15.000000 extend_orfs-0.0.28/src/extend_orfs.egg-info/top_level.txt
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/
+-rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/PKG-INFO
+-rw-rw-r--   0 joan      (1000) joan      (1000)       14 2022-11-24 14:56:36.000000 extend_orfs-0.0.29/README.md
+-rw-rw-r--   0 joan      (1000) joan      (1000)      104 2021-06-11 14:00:42.000000 extend_orfs-0.0.29/pyproject.toml
+-rw-rw-r--   0 joan      (1000) joan      (1000)      774 2023-06-15 14:24:52.149291 extend_orfs-0.0.29/setup.cfg
+-rw-rw-r--   0 joan      (1000) joan      (1000)       69 2021-06-14 10:13:07.000000 extend_orfs-0.0.29/setup.py
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.141291 extend_orfs-0.0.29/src/
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/src/extend_orfs/
+-rw-rw-r--   0 joan      (1000) joan      (1000)       27 2022-12-01 15:21:34.000000 extend_orfs-0.0.29/src/extend_orfs/__init__.py
+-rwxrw-r--   0 joan      (1000) joan      (1000)    25595 2023-06-15 14:24:03.000000 extend_orfs-0.0.29/src/extend_orfs/extend_orfs.py
+drwxrwxr-x   0 joan      (1000) joan      (1000)        0 2023-06-15 14:24:52.145291 extend_orfs-0.0.29/src/extend_orfs.egg-info/
+-rw-rw-r--   0 joan      (1000) joan      (1000)      443 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/PKG-INFO
+-rw-rw-r--   0 joan      (1000) joan      (1000)      296 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)        1 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)       56 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/requires.txt
+-rw-rw-r--   0 joan      (1000) joan      (1000)       12 2023-06-15 14:24:52.000000 extend_orfs-0.0.29/src/extend_orfs.egg-info/top_level.txt
```

### Comparing `extend_orfs-0.0.28/setup.cfg` & `extend_orfs-0.0.29/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = extend_orfs
-version = 0.0.28
+version = 0.0.29
 author = Joan Pallarès-Albanell
 author_email = joan.pallares.albanell@gmail.com
 description = MModule description
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JoanPAAL/extend_orfs/
 project_urls =
```

### Comparing `extend_orfs-0.0.28/src/extend_orfs/extend_orfs.py` & `extend_orfs-0.0.29/src/extend_orfs/extend_orfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,19 +521,19 @@
 
 
 def mod_extend(p, group_by):
     """Modified version of PyRanges extend()
     The modifications allow for a specific 'chunk' extension for each group.
     """
 
-    kwargs = pr.pyranges.fill_kwargs({"strand": p.stranded})
+    kwargs = pr.pyranges_main.fill_kwargs({"strand": p.stranded})
           
     kwargs['group_by']=group_by
     prg = pr.PyRanges(
-                      pr.multithreaded.pyrange_apply_single(_extend_grp_j, p, **kwargs))            
+                      pr.multithreaded.pyrange_apply_single(_extend_grp_j, p, **kwargs))  
 
     return prg
 
 
 def _extend_grp_j(df, **kwargs):
     """Modified version of Pyranges multithreaded._extend_grp
     """
```

