# Comparing `tmp/catbridge-0.3.tar.gz` & `tmp/catbridge-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catbridge-0.3.tar", last modified: Wed Jun 14 09:36:22 2023, max compression
+gzip compressed data, was "catbridge-0.4.tar", last modified: Thu Jun 15 05:24:56 2023, max compression
```

## Comparing `catbridge-0.3.tar` & `catbridge-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-14 09:36:22.076522 catbridge-0.3/
--rw-r--r--   0 bowen      (501) staff       (20)     1073 2023-06-13 01:32:07.000000 catbridge-0.3/LICENSE
--rw-r--r--   0 bowen      (501) staff       (20)      473 2023-06-14 09:36:22.076326 catbridge-0.3/PKG-INFO
--rw-r--r--   0 bowen      (501) staff       (20)      153 2023-06-13 01:42:37.000000 catbridge-0.3/README.md
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-14 09:36:22.075074 catbridge-0.3/catbridge/
--rw-r--r--   0 bowen      (501) staff       (20)       24 2023-06-13 07:10:57.000000 catbridge-0.3/catbridge/__init__.py
--rw-r--r--   0 bowen      (501) staff       (20)    38461 2023-06-14 09:29:36.000000 catbridge-0.3/catbridge/catbridge.py
-drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-14 09:36:22.076069 catbridge-0.3/catbridge.egg-info/
--rw-r--r--   0 bowen      (501) staff       (20)      473 2023-06-14 09:36:11.000000 catbridge-0.3/catbridge.egg-info/PKG-INFO
--rw-r--r--   0 bowen      (501) staff       (20)      203 2023-06-14 09:36:21.000000 catbridge-0.3/catbridge.egg-info/SOURCES.txt
--rw-r--r--   0 bowen      (501) staff       (20)        1 2023-06-14 09:36:11.000000 catbridge-0.3/catbridge.egg-info/dependency_links.txt
--rw-r--r--   0 bowen      (501) staff       (20)       10 2023-06-14 09:36:11.000000 catbridge-0.3/catbridge.egg-info/top_level.txt
--rw-r--r--   0 bowen      (501) staff       (20)       38 2023-06-14 09:36:22.076575 catbridge-0.3/setup.cfg
--rw-r--r--   0 bowen      (501) staff       (20)      602 2023-06-14 09:35:57.000000 catbridge-0.3/setup.py
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.138246 catbridge-0.4/
+-rw-r--r--   0 bowen      (501) staff       (20)     1073 2023-06-13 01:32:07.000000 catbridge-0.4/LICENSE
+-rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-15 05:24:56.138038 catbridge-0.4/PKG-INFO
+-rw-r--r--   0 bowen      (501) staff       (20)     1437 2023-06-15 05:21:37.000000 catbridge-0.4/README.md
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.136721 catbridge-0.4/catbridge/
+-rw-r--r--   0 bowen      (501) staff       (20)       24 2023-06-13 07:10:57.000000 catbridge-0.4/catbridge/__init__.py
+-rw-r--r--   0 bowen      (501) staff       (20)    38461 2023-06-14 09:29:36.000000 catbridge-0.4/catbridge/catbridge.py
+drwxr-xr-x   0 bowen      (501) staff       (20)        0 2023-06-15 05:24:56.137779 catbridge-0.4/catbridge.egg-info/
+-rw-r--r--   0 bowen      (501) staff       (20)     2004 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/PKG-INFO
+-rw-r--r--   0 bowen      (501) staff       (20)      203 2023-06-15 05:24:56.000000 catbridge-0.4/catbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 bowen      (501) staff       (20)        1 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 bowen      (501) staff       (20)       10 2023-06-15 05:24:44.000000 catbridge-0.4/catbridge.egg-info/top_level.txt
+-rw-r--r--   0 bowen      (501) staff       (20)       38 2023-06-15 05:24:56.138304 catbridge-0.4/setup.cfg
+-rw-r--r--   0 bowen      (501) staff       (20)      850 2023-06-15 05:23:33.000000 catbridge-0.4/setup.py
```

### Comparing `catbridge-0.3/LICENSE` & `catbridge-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catbridge-0.3/catbridge/catbridge.py` & `catbridge-0.4/catbridge/catbridge.py`

 * *Files identical despite different names*

