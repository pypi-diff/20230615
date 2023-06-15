# Comparing `tmp/stackoverflowapithingy-0.1.6.tar.gz` & `tmp/stackoverflowapithingy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.6.tar", last modified: Thu Jun 15 11:43:50 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.7.tar", last modified: Thu Jun 15 11:53:33 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.6.tar` & `stackoverflowapithingy-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:43:50.274835 stackoverflowapithingy-0.1.6/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:43:50.274726 stackoverflowapithingy-0.1.6/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:43:50.274875 stackoverflowapithingy-0.1.6/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      252 2023-06-15 11:43:43.000000 stackoverflowapithingy-0.1.6/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:43:50.274564 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.653395 stackoverflowapithingy-0.1.7/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:53:33.653291 stackoverflowapithingy-0.1.7/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:53:33.653437 stackoverflowapithingy-0.1.7/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:53:30.000000 stackoverflowapithingy-0.1.7/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.652588 stackoverflowapithingy-0.1.7/stackoverflowapithingy/
+-rw-r--r--   0 benjamin   (501) staff       (20)      140 2023-06-15 11:41:43.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1485 2023-06-15 11:19:18.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy/stackoverflow.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.653136 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      312 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/top_level.txt
```

