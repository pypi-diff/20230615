# Comparing `tmp/stackoverflowapithingy-0.1.1.tar.gz` & `tmp/stackoverflowapithingy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.1.tar", last modified: Thu Jun 15 10:22:11 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.2.tar", last modified: Thu Jun 15 11:01:17 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.1.tar` & `stackoverflowapithingy-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 10:22:11.653901 stackoverflowapithingy-0.1.1/
--rw-r--r--   0 benjamin   (501) staff       (20)      147 2023-06-15 10:22:11.653789 stackoverflowapithingy-0.1.1/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 10:22:11.653946 stackoverflowapithingy-0.1.1/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      147 2023-06-15 10:21:28.000000 stackoverflowapithingy-0.1.1/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 10:22:11.653643 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      147 2023-06-15 10:22:11.000000 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 10:22:11.000000 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 10:22:11.000000 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 10:22:11.000000 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 10:22:11.000000 stackoverflowapithingy-0.1.1/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:01:17.525229 stackoverflowapithingy-0.1.2/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:01:17.525087 stackoverflowapithingy-0.1.2/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:01:17.525272 stackoverflowapithingy-0.1.2/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:00:54.000000 stackoverflowapithingy-0.1.2/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:01:17.524942 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/top_level.txt
```

