# Comparing `tmp/webhooklib-0.1.2.tar.gz` & `tmp/webhooklib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.1.2.tar", last modified: Thu Jun 15 12:53:22 2023, max compression
+gzip compressed data, was "webhooklib-0.1.3.tar", last modified: Thu Jun 15 13:08:33 2023, max compression
```

## Comparing `webhooklib-0.1.2.tar` & `webhooklib-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:22.792730 webhooklib-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 12:53:22.792730 webhooklib-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 12:53:05.000000 webhooklib-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 12:53:05.000000 webhooklib-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:53:22.792730 webhooklib-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:22.792730 webhooklib-0.1.2/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-15 12:53:05.000000 webhooklib-0.1.2/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:53:22.792730 webhooklib-0.1.2/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 12:53:22.000000 webhooklib-0.1.2/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 12:53:22.000000 webhooklib-0.1.2/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:53:22.000000 webhooklib-0.1.2/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 12:53:22.000000 webhooklib-0.1.2/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 12:53:22.000000 webhooklib-0.1.2/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:08:33.643354 webhooklib-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:08:33.643354 webhooklib-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 13:08:15.000000 webhooklib-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 13:08:15.000000 webhooklib-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:08:33.643354 webhooklib-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:08:33.643354 webhooklib-0.1.3/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-15 13:08:15.000000 webhooklib-0.1.3/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:08:33.643354 webhooklib-0.1.3/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:08:33.000000 webhooklib-0.1.3/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 13:08:33.000000 webhooklib-0.1.3/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:08:33.000000 webhooklib-0.1.3/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 13:08:33.000000 webhooklib-0.1.3/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 13:08:33.000000 webhooklib-0.1.3/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.1.2/pyproject.toml` & `webhooklib-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "webhooklib"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "fastapi",
     "uvicorn",
     "redis",
+    "requests",
 ]
 
 [project.optional-dependencies]
 dev = [
     "bumpver",
     "pre-commit",
     "pytest",
@@ -31,15 +32,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.1.2"
+current_version = "v0.1.3"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.1.2/webhooklib/process_wrapper.py` & `webhooklib-0.1.3/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.1.2/webhooklib/server.py` & `webhooklib-0.1.3/webhooklib/server.py`

 * *Files identical despite different names*

