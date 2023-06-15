# Comparing `tmp/harissumcheck-0.1.tar.gz` & `tmp/harissumcheck-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harissumcheck-0.1.tar", last modified: Thu Jun 15 08:59:48 2023, max compression
+gzip compressed data, was "harissumcheck-0.2.tar", last modified: Thu Jun 15 09:03:53 2023, max compression
```

## Comparing `harissumcheck-0.1.tar` & `harissumcheck-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 08:59:48.181321 harissumcheck-0.1/
--rw-rw-r--   0 haris     (1000) haris     (1000)      192 2023-06-15 08:59:48.181321 harissumcheck-0.1/PKG-INFO
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 08:59:48.181321 harissumcheck-0.1/harissumcheck/
--rw-rw-r--   0 haris     (1000) haris     (1000)       33 2023-06-15 08:56:59.000000 harissumcheck-0.1/harissumcheck/__init__.py
--rw-rw-r--   0 haris     (1000) haris     (1000)      126 2023-06-15 08:54:11.000000 harissumcheck-0.1/harissumcheck/harissumcheck.py
--rw-rw-r--   0 haris     (1000) haris     (1000)       54 2023-06-15 08:49:48.000000 harissumcheck-0.1/harissumcheck/number.py
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 08:59:48.181321 harissumcheck-0.1/harissumcheck.egg-info/
--rw-rw-r--   0 haris     (1000) haris     (1000)      192 2023-06-15 08:59:48.000000 harissumcheck-0.1/harissumcheck.egg-info/PKG-INFO
--rw-rw-r--   0 haris     (1000) haris     (1000)      237 2023-06-15 08:59:48.000000 harissumcheck-0.1/harissumcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)        1 2023-06-15 08:59:48.000000 harissumcheck-0.1/harissumcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)       14 2023-06-15 08:59:48.000000 harissumcheck-0.1/harissumcheck.egg-info/top_level.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)       38 2023-06-15 08:59:48.181321 harissumcheck-0.1/setup.cfg
--rw-rw-r--   0 haris     (1000) haris     (1000)      305 2023-06-15 08:59:36.000000 harissumcheck-0.1/setup.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 09:03:53.734610 harissumcheck-0.2/
+-rw-rw-r--   0 haris     (1000) haris     (1000)      192 2023-06-15 09:03:53.734610 harissumcheck-0.2/PKG-INFO
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 09:03:53.734610 harissumcheck-0.2/harissumcheck/
+-rw-rw-r--   0 haris     (1000) haris     (1000)       38 2023-06-15 09:03:34.000000 harissumcheck-0.2/harissumcheck/__init__.py
+-rw-rw-r--   0 haris     (1000) haris     (1000)      126 2023-06-15 08:54:11.000000 harissumcheck-0.2/harissumcheck/harissumcheck.py
+-rw-rw-r--   0 haris     (1000) haris     (1000)       54 2023-06-15 08:49:48.000000 harissumcheck-0.2/harissumcheck/number.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-06-15 09:03:53.734610 harissumcheck-0.2/harissumcheck.egg-info/
+-rw-rw-r--   0 haris     (1000) haris     (1000)      192 2023-06-15 09:03:53.000000 harissumcheck-0.2/harissumcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 haris     (1000) haris     (1000)      237 2023-06-15 09:03:53.000000 harissumcheck-0.2/harissumcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)        1 2023-06-15 09:03:53.000000 harissumcheck-0.2/harissumcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)       14 2023-06-15 09:03:53.000000 harissumcheck-0.2/harissumcheck.egg-info/top_level.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)       38 2023-06-15 09:03:53.734610 harissumcheck-0.2/setup.cfg
+-rw-rw-r--   0 haris     (1000) haris     (1000)      305 2023-06-15 09:03:46.000000 harissumcheck-0.2/setup.py
```

