# Comparing `tmp/telexception-0.1.0.tar.gz` & `tmp/Telexception-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexception-0.1.0.tar", last modified: Thu Jun 15 13:26:57 2023, max compression
+gzip compressed data, was "Telexception-0.1.1.tar", last modified: Thu Jun 15 13:37:00 2023, max compression
```

## Comparing `telexception-0.1.0.tar` & `Telexception-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
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
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:37:00.033984 Telexception-0.1.1/
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:37:00.033858 Telexception-0.1.1/PKG-INFO
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:37:00.033527 Telexception-0.1.1/Telexception.egg-info/
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:36:59.000000 Telexception-0.1.1/Telexception.egg-info/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)      366 2023-06-15 13:37:00.000000 Telexception-0.1.1/Telexception.egg-info/SOURCES.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:36:59.000000 Telexception-0.1.1/Telexception.egg-info/dependency_links.txt
+-rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:37:00.000000 Telexception-0.1.1/Telexception.egg-info/requires.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:37:00.000000 Telexception-0.1.1/Telexception.egg-info/top_level.txt
+-rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:37:00.034026 Telexception-0.1.1/setup.cfg
+-rw-r--r--   0 unn        (501) staff       (20)      650 2023-06-15 13:34:53.000000 Telexception-0.1.1/setup.py
```

