# Comparing `tmp/datawork000-0.2.0.tar.gz` & `tmp/datawork000-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datawork000-0.2.0.tar", last modified: Thu Jun 15 08:27:13 2023, max compression
+gzip compressed data, was "dist/datawork000-0.2.1.tar", last modified: Thu Jun 15 08:37:52 2023, max compression
```

## Comparing `datawork000-0.2.0.tar` & `datawork000-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:27:13.000000 datawork000-0.2.0/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      731 2023-06-15 08:27:13.000000 datawork000-0.2.0/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      113 2023-06-15 05:51:30.000000 datawork000-0.2.0/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      731 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      173 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       12 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1050 2023-06-15 04:57:24.000000 datawork000-0.2.0/datawork000.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 08:27:13.000000 datawork000-0.2.0/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      983 2023-06-15 08:27:08.000000 datawork000-0.2.0/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:37:52.000000 datawork000-0.2.1/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      612 2023-06-15 08:37:52.000000 datawork000-0.2.1/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      113 2023-06-15 05:51:30.000000 datawork000-0.2.1/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:37:52.000000 datawork000-0.2.1/datawork000.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      612 2023-06-15 08:37:52.000000 datawork000-0.2.1/datawork000.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      173 2023-06-15 08:37:52.000000 datawork000-0.2.1/datawork000.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 08:37:52.000000 datawork000-0.2.1/datawork000.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       12 2023-06-15 08:37:52.000000 datawork000-0.2.1/datawork000.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1050 2023-06-15 04:57:24.000000 datawork000-0.2.1/datawork000.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 08:37:52.000000 datawork000-0.2.1/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      785 2023-06-15 08:37:42.000000 datawork000-0.2.1/setup.py
```

### Comparing `datawork000-0.2.0/datawork000.py` & `datawork000-0.2.1/datawork000.py`

 * *Files identical despite different names*

