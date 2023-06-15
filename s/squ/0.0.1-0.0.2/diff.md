# Comparing `tmp/squ-0.0.1.tar.gz` & `tmp/squ-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squ-0.0.1.tar", last modified: Tue Jun  6 03:20:38 2023, max compression
+gzip compressed data, was "squ-0.0.2.tar", last modified: Thu Jun 15 00:03:26 2023, max compression
```

## Comparing `squ-0.0.1.tar` & `squ-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxr-x   0 squ       (1000) squ       (1000)        0 2023-06-06 03:20:38.458120 squ-0.0.1/
--rw-rw-r--   0 squ       (1000) squ       (1000)      227 2023-06-06 03:20:38.458120 squ-0.0.1/PKG-INFO
--rw-rw-r--   0 squ       (1000) squ       (1000)        0 2023-06-06 03:11:40.000000 squ-0.0.1/README.md
--rw-rw-r--   0 squ       (1000) squ       (1000)       38 2023-06-06 03:20:38.458120 squ-0.0.1/setup.cfg
--rw-rw-r--   0 squ       (1000) squ       (1000)      328 2023-06-06 03:17:56.000000 squ-0.0.1/setup.py
-drwxrwxr-x   0 squ       (1000) squ       (1000)        0 2023-06-06 03:20:38.458120 squ-0.0.1/squ.egg-info/
--rw-rw-r--   0 squ       (1000) squ       (1000)      227 2023-06-06 03:20:38.000000 squ-0.0.1/squ.egg-info/PKG-INFO
--rw-rw-r--   0 squ       (1000) squ       (1000)      126 2023-06-06 03:20:38.000000 squ-0.0.1/squ.egg-info/SOURCES.txt
--rw-rw-r--   0 squ       (1000) squ       (1000)        1 2023-06-06 03:20:38.000000 squ-0.0.1/squ.egg-info/dependency_links.txt
--rw-rw-r--   0 squ       (1000) squ       (1000)        4 2023-06-06 03:20:38.000000 squ-0.0.1/squ.egg-info/top_level.txt
+drwxrwxr-x   0 squ       (1000) squ       (1000)        0 2023-06-15 00:03:26.062842 squ-0.0.2/
+-rw-rw-r--   0 squ       (1000) squ       (1000)      227 2023-06-15 00:03:26.062842 squ-0.0.2/PKG-INFO
+-rw-rw-r--   0 squ       (1000) squ       (1000)       40 2023-06-06 06:47:41.000000 squ-0.0.2/README.md
+-rw-rw-r--   0 squ       (1000) squ       (1000)       38 2023-06-15 00:03:26.062842 squ-0.0.2/setup.cfg
+-rw-rw-r--   0 squ       (1000) squ       (1000)      405 2023-06-15 00:02:12.000000 squ-0.0.2/setup.py
+drwxrwxr-x   0 squ       (1000) squ       (1000)        0 2023-06-15 00:03:26.058842 squ-0.0.2/squ/
+-rw-rw-r--   0 squ       (1000) squ       (1000)      106 2023-06-06 05:41:51.000000 squ-0.0.2/squ/backtrace.py
+drwxrwxr-x   0 squ       (1000) squ       (1000)        0 2023-06-15 00:03:26.062842 squ-0.0.2/squ.egg-info/
+-rw-rw-r--   0 squ       (1000) squ       (1000)      227 2023-06-15 00:03:25.000000 squ-0.0.2/squ.egg-info/PKG-INFO
+-rw-rw-r--   0 squ       (1000) squ       (1000)      169 2023-06-15 00:03:26.000000 squ-0.0.2/squ.egg-info/SOURCES.txt
+-rw-rw-r--   0 squ       (1000) squ       (1000)        1 2023-06-15 00:03:25.000000 squ-0.0.2/squ.egg-info/dependency_links.txt
+-rw-rw-r--   0 squ       (1000) squ       (1000)       29 2023-06-15 00:03:25.000000 squ-0.0.2/squ.egg-info/requires.txt
+-rw-rw-r--   0 squ       (1000) squ       (1000)        4 2023-06-15 00:03:25.000000 squ-0.0.2/squ.egg-info/top_level.txt
```

