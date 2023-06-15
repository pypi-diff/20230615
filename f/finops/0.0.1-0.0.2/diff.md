# Comparing `tmp/finops-0.0.1.tar.gz` & `tmp/finops-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.0.1.tar", last modified: Thu Jun 15 16:19:10 2023, max compression
+gzip compressed data, was "finops-0.0.2.tar", last modified: Thu Jun 15 16:25:59 2023, max compression
```

## Comparing `finops-0.0.1.tar` & `finops-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 16:19:10.409982 finops-0.0.1/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)     1073 2023-06-05 21:44:45.000000 finops-0.0.1/LICENSE
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      499 2023-06-15 16:19:10.409982 finops-0.0.1/PKG-INFO
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       32 2023-06-05 21:44:29.000000 finops-0.0.1/README.md
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      542 2023-06-15 16:18:23.000000 finops-0.0.1/pyproject.toml
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       38 2023-06-15 16:19:10.409982 finops-0.0.1/setup.cfg
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 16:19:10.405982 finops-0.0.1/src/
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 16:19:10.409982 finops-0.0.1/src/finops/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-05 14:53:44.000000 finops-0.0.1/src/finops/__init__.py
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       31 2023-06-15 15:35:51.000000 finops-0.0.1/src/finops/shareholders.py
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 16:19:10.409982 finops-0.0.1/src/finops.egg-info/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      499 2023-06-15 16:19:10.000000 finops-0.0.1/src/finops.egg-info/PKG-INFO
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      218 2023-06-15 16:19:10.000000 finops-0.0.1/src/finops.egg-info/SOURCES.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        1 2023-06-15 16:19:10.000000 finops-0.0.1/src/finops.egg-info/dependency_links.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        7 2023-06-15 16:19:10.000000 finops-0.0.1/src/finops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.005511 finops-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 16:25:46.000000 finops-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 16:25:59.005511 finops-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 16:25:46.000000 finops-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-15 16:25:46.000000 finops-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:25:59.005511 finops-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.001511 finops-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.001511 finops-0.0.2/src/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:46.000000 finops-0.0.2/src/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 16:25:46.000000 finops-0.0.2/src/finops/shareholders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.005511 finops-0.0.2/src/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/top_level.txt
```

### Comparing `finops-0.0.1/LICENSE` & `finops-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.0.1/pyproject.toml` & `finops-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "finops"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Alireza Nilgaran", email="alireza.nilgaran@gmail.com"},
 ]
 description = "A library for analyzing financial data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

