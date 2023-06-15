# Comparing `tmp/stackoverflowapithingy-0.1.2.tar.gz` & `tmp/stackoverflowapithingy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.2.tar", last modified: Thu Jun 15 11:01:17 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.3.tar", last modified: Thu Jun 15 11:21:27 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.2.tar` & `stackoverflowapithingy-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:01:17.525229 stackoverflowapithingy-0.1.2/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:01:17.525087 stackoverflowapithingy-0.1.2/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:01:17.525272 stackoverflowapithingy-0.1.2/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:00:54.000000 stackoverflowapithingy-0.1.2/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:01:17.524942 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:01:17.000000 stackoverflowapithingy-0.1.2/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:21:27.641202 stackoverflowapithingy-0.1.3/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:21:27.641085 stackoverflowapithingy-0.1.3/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:21:27.641241 stackoverflowapithingy-0.1.3/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:21:06.000000 stackoverflowapithingy-0.1.3/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:21:27.640945 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:21:27.000000 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      237 2023-06-15 11:21:27.000000 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:21:27.000000 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:21:27.000000 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:21:27.000000 stackoverflowapithingy-0.1.3/stackoverflowapithingy.egg-info/top_level.txt
```

