# Comparing `tmp/telexception-0.1.0.tar.gz` & `tmp/Telexception-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexception-0.1.0.tar", last modified: Thu Jun 15 13:26:57 2023, max compression
+gzip compressed data, was "Telexception-0.1.5.tar", last modified: Thu Jun 15 13:51:24 2023, max compression
```

## Comparing `telexception-0.1.0.tar` & `Telexception-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:26:57.333292 telexception-0.1.0/
--rw-r--r--   0 unn        (501) staff       (20)      209 2023-06-15 13:26:57.333167 telexception-0.1.0/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:26:57.333339 telexception-0.1.0/setup.cfg
--rw-r--r--   0 unn        (501) staff       (20)      387 2023-06-15 13:05:38.000000 telexception-0.1.0/setup.py
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:26:57.332998 telexception-0.1.0/telexception.egg-info/
--rw-r--r--   0 unn        (501) staff       (20)      209 2023-06-15 13:26:57.000000 telexception-0.1.0/telexception.egg-info/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)      187 2023-06-15 13:26:57.000000 telexception-0.1.0/telexception.egg-info/SOURCES.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:26:57.000000 telexception-0.1.0/telexception.egg-info/dependency_links.txt
--rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:26:57.000000 telexception-0.1.0/telexception.egg-info/requires.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:26:57.000000 telexception-0.1.0/telexception.egg-info/top_level.txt
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:51:24.562168 Telexception-0.1.5/
+-rw-r--r--   0 unn        (501) staff       (20)       18 2023-06-15 13:44:54.000000 Telexception-0.1.5/MANIFEST.in
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:51:24.562027 Telexception-0.1.5/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)     1486 2023-06-15 13:42:16.000000 Telexception-0.1.5/README.md
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:51:24.561690 Telexception-0.1.5/Telexception.egg-info/
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)      388 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/SOURCES.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/dependency_links.txt
+-rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/requires.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/top_level.txt
+-rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:51:24.562213 Telexception-0.1.5/setup.cfg
+-rw-r--r--   0 unn        (501) staff       (20)      650 2023-06-15 13:51:16.000000 Telexception-0.1.5/setup.py
```

