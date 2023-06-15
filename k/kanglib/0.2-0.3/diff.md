# Comparing `tmp/kanglib-0.2.tar.gz` & `tmp/kanglib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanglib-0.2.tar", last modified: Thu Jun 15 15:06:21 2023, max compression
+gzip compressed data, was "kanglib-0.3.tar", last modified: Thu Jun 15 15:40:50 2023, max compression
```

## Comparing `kanglib-0.2.tar` & `kanglib-0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:06:21.218537 kanglib-0.2/
--rw-r--r--   0 kang       (501) staff       (20)       49 2023-06-15 15:06:21.218427 kanglib-0.2/PKG-INFO
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:06:21.217797 kanglib-0.2/kanglib/
--rw-r--r--   0 kang       (501) staff       (20)       67 2023-06-15 15:05:28.000000 kanglib-0.2/kanglib/__init__.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:06:21.218303 kanglib-0.2/kanglib.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)       49 2023-06-15 15:06:21.000000 kanglib-0.2/kanglib.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      152 2023-06-15 15:06:21.000000 kanglib-0.2/kanglib.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 15:06:21.000000 kanglib-0.2/kanglib.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 15:06:21.000000 kanglib-0.2/kanglib.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 15:06:21.218569 kanglib-0.2/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      122 2023-06-15 15:05:56.000000 kanglib-0.2/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.938034 kanglib-0.3/
+-rw-r--r--   0 kang       (501) staff       (20)      401 2023-06-15 15:40:50.937931 kanglib-0.3/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      163 2023-06-15 15:40:46.000000 kanglib-0.3/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.937240 kanglib-0.3/kanglib/
+-rw-r--r--   0 kang       (501) staff       (20)      121 2023-06-15 15:35:23.000000 kanglib-0.3/kanglib/__init__.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 15:40:50.937808 kanglib-0.3/kanglib.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      401 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      162 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 15:40:50.000000 kanglib-0.3/kanglib.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 15:40:50.938066 kanglib-0.3/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      525 2023-06-15 15:37:59.000000 kanglib-0.3/setup.py
```

