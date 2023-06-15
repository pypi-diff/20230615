# Comparing `tmp/stackoverflowapithingy-0.1.5.tar.gz` & `tmp/stackoverflowapithingy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.5.tar", last modified: Thu Jun 15 11:42:29 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.6.tar", last modified: Thu Jun 15 11:43:50 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.5.tar` & `stackoverflowapithingy-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:42:29.032601 stackoverflowapithingy-0.1.5/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:42:29.032509 stackoverflowapithingy-0.1.5/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:42:29.032634 stackoverflowapithingy-0.1.5/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:42:15.000000 stackoverflowapithingy-0.1.5/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:42:29.032374 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:42:29.000000 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:42:29.000000 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:42:29.000000 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:42:29.000000 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:42:29.000000 stackoverflowapithingy-0.1.5/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:43:50.274835 stackoverflowapithingy-0.1.6/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:43:50.274726 stackoverflowapithingy-0.1.6/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:43:50.274875 stackoverflowapithingy-0.1.6/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      252 2023-06-15 11:43:43.000000 stackoverflowapithingy-0.1.6/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:43:50.274564 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:43:50.000000 stackoverflowapithingy-0.1.6/stackoverflowapithingy.egg-info/top_level.txt
```

