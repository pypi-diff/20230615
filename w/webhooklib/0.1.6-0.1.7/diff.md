# Comparing `tmp/webhooklib-0.1.6.tar.gz` & `tmp/webhooklib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.1.6.tar", last modified: Thu Jun 15 14:14:24 2023, max compression
+gzip compressed data, was "webhooklib-0.1.7.tar", last modified: Thu Jun 15 14:31:03 2023, max compression
```

## Comparing `webhooklib-0.1.6.tar` & `webhooklib-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:14:24.014600 webhooklib-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:14:24.014600 webhooklib-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 14:14:05.000000 webhooklib-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 14:14:05.000000 webhooklib-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:14:24.014600 webhooklib-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:14:24.014600 webhooklib-0.1.6/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 14:14:05.000000 webhooklib-0.1.6/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:14:24.014600 webhooklib-0.1.6/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:14:24.000000 webhooklib-0.1.6/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 14:14:24.000000 webhooklib-0.1.6/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:14:24.000000 webhooklib-0.1.6/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:14:24.000000 webhooklib-0.1.6/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 14:14:24.000000 webhooklib-0.1.6/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:31:03.961381 webhooklib-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 14:30:45.000000 webhooklib-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 14:30:45.000000 webhooklib-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:31:03.961381 webhooklib-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.1.6/pyproject.toml` & `webhooklib-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -32,15 +32,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.1.6"
+current_version = "v0.1.7"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.1.6/webhooklib/client.py` & `webhooklib-0.1.7/webhooklib/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     env = {
         k.removeprefix(ENV_PREFIX): v
         for k, v in os.environ.items()
         if k.startswith(ENV_PREFIX)
     }
     print(env)
+    print(payload)
     command = ShellCommand(**payload)
     headers = {'token': os.environ['WEBHOOK_TOKEN']}
     response = requests.post(url, headers=headers, json=command.dict())
 
     if not response.ok:
         print(response.status_code)
         print(response.text)
```

### Comparing `webhooklib-0.1.6/webhooklib/process_wrapper.py` & `webhooklib-0.1.7/webhooklib/process_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 def run_subprocess(
     command: ShellCommand,
     redis: Redis,
 ) -> None:
     logger.info('start')
+    print('run_subprocess:', command)
     p = subprocess.Popen(
         command.cmd,
         env=command.env,
         cwd=command.cwd,
         text=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
```

### Comparing `webhooklib-0.1.6/webhooklib/server.py` & `webhooklib-0.1.7/webhooklib/server.py`

 * *Files identical despite different names*

