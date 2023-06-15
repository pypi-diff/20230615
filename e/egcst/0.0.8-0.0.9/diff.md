# Comparing `tmp/egcst-0.0.8.tar.gz` & `tmp/egcst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.8.tar", last modified: Thu Jun 15 15:49:50 2023, max compression
+gzip compressed data, was "egcst-0.0.9.tar", last modified: Thu Jun 15 17:30:52 2023, max compression
```

## Comparing `egcst-0.0.8.tar` & `egcst-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:49:50.337054 egcst-0.0.8/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 15:49:50.337243 egcst-0.0.8/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.8/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:49:50.333867 egcst-0.0.8/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.8/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    12561 2023-06-15 15:47:16.000000 egcst-0.0.8/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:49:50.336610 egcst-0.0.8/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 15:49:50.000000 egcst-0.0.8/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-15 15:49:50.000000 egcst-0.0.8/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-15 15:49:50.000000 egcst-0.0.8/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-15 15:49:50.000000 egcst-0.0.8/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-15 15:49:50.000000 egcst-0.0.8/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-15 15:49:50.338332 egcst-0.0.8/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-15 15:48:02.000000 egcst-0.0.8/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 17:30:52.787952 egcst-0.0.9/
+-rw-r--r--   0 sasha      (502) staff       (20)     2624 2023-06-15 17:30:52.788174 egcst-0.0.9/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.9/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 17:30:52.782974 egcst-0.0.9/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.9/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    12561 2023-06-15 15:47:16.000000 egcst-0.0.9/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 17:30:52.787457 egcst-0.0.9/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)     2624 2023-06-15 17:30:52.000000 egcst-0.0.9/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-15 17:30:52.000000 egcst-0.0.9/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-15 17:30:52.000000 egcst-0.0.9/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-15 17:30:52.000000 egcst-0.0.9/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-15 17:30:52.000000 egcst-0.0.9/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-15 17:30:52.788953 egcst-0.0.9/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      783 2023-06-15 17:30:28.000000 egcst-0.0.9/setup.py
```

### Comparing `egcst-0.0.8/README.md` & `egcst-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `egcst-0.0.8/egcst/core.py` & `egcst-0.0.9/egcst/core.py`

 * *Files identical despite different names*

