# Comparing `tmp/http_error_schemas-0.0.1.tar.gz` & `tmp/http_error_schemas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_error_schemas-0.0.1.tar", last modified: Fri Jun  2 19:22:43 2023, max compression
+gzip compressed data, was "http_error_schemas-0.1.0.tar", last modified: Thu Jun 15 02:11:40 2023, max compression
```

## Comparing `http_error_schemas-0.0.1.tar` & `http_error_schemas-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:22:43.212987 http_error_schemas-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 19:22:43.212987 http_error_schemas-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 19:22:28.000000 http_error_schemas-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:22:43.212987 http_error_schemas-0.0.1/http_error_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 19:22:28.000000 http_error_schemas-0.0.1/http_error_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 19:22:28.000000 http_error_schemas-0.0.1/http_error_schemas/validation_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:22:43.212987 http_error_schemas-0.0.1/http_error_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 19:22:43.000000 http_error_schemas-0.0.1/http_error_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 19:22:43.000000 http_error_schemas-0.0.1/http_error_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:22:43.000000 http_error_schemas-0.0.1/http_error_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 19:22:43.000000 http_error_schemas-0.0.1/http_error_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 19:22:43.000000 http_error_schemas-0.0.1/http_error_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:22:43.212987 http_error_schemas-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-02 19:22:28.000000 http_error_schemas-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:11:40.364163 http_error_schemas-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 02:11:40.360163 http_error_schemas-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 02:11:21.000000 http_error_schemas-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:11:40.360163 http_error_schemas-0.1.0/http_error_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:11:21.000000 http_error_schemas-0.1.0/http_error_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-15 02:11:21.000000 http_error_schemas-0.1.0/http_error_schemas/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:11:40.360163 http_error_schemas-0.1.0/http_error_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 02:11:40.000000 http_error_schemas-0.1.0/http_error_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 02:11:40.000000 http_error_schemas-0.1.0/http_error_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:11:40.000000 http_error_schemas-0.1.0/http_error_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 02:11:40.000000 http_error_schemas-0.1.0/http_error_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 02:11:40.000000 http_error_schemas-0.1.0/http_error_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:11:40.364163 http_error_schemas-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-15 02:11:21.000000 http_error_schemas-0.1.0/setup.py
```

### Comparing `http_error_schemas-0.0.1/setup.py` & `http_error_schemas-0.1.0/setup.py`

 * *Files identical despite different names*

