# Comparing `tmp/webhooklib-0.1.4.tar.gz` & `tmp/webhooklib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.1.4.tar", last modified: Thu Jun 15 13:29:29 2023, max compression
+gzip compressed data, was "webhooklib-0.1.5.tar", last modified: Thu Jun 15 14:09:09 2023, max compression
```

## Comparing `webhooklib-0.1.4.tar` & `webhooklib-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:29:29.536146 webhooklib-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:29:29.536146 webhooklib-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 13:29:06.000000 webhooklib-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 13:29:06.000000 webhooklib-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:29:29.536146 webhooklib-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:29:29.532146 webhooklib-0.1.4/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 13:29:06.000000 webhooklib-0.1.4/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:29:29.536146 webhooklib-0.1.4/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:29:29.000000 webhooklib-0.1.4/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 13:29:29.000000 webhooklib-0.1.4/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:29:29.000000 webhooklib-0.1.4/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 13:29:29.000000 webhooklib-0.1.4/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 13:29:29.000000 webhooklib-0.1.4/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:09:09.434533 webhooklib-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:09:09.434533 webhooklib-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 14:08:51.000000 webhooklib-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 14:08:51.000000 webhooklib-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:09:09.434533 webhooklib-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:09:09.434533 webhooklib-0.1.5/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 14:08:51.000000 webhooklib-0.1.5/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:09:09.434533 webhooklib-0.1.5/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:09:09.000000 webhooklib-0.1.5/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 14:09:09.000000 webhooklib-0.1.5/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:09:09.000000 webhooklib-0.1.5/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:09:09.000000 webhooklib-0.1.5/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 14:09:09.000000 webhooklib-0.1.5/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.1.4/pyproject.toml` & `webhooklib-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.1.4"
+version = "0.1.5"
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
-current_version = "v0.1.4"
+current_version = "v0.1.5"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.1.4/webhooklib/client.py` & `webhooklib-0.1.5/webhooklib/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import os
 import sys
 
 import requests
 from redis import Redis
+
 from webhooklib import config
 from webhooklib.models import ShellCommand
 from webhooklib.models import ShellResult
 
 ENV_PREFIX = 'WEBHOOK_ENV_'
 
 
 def main():
     redis = Redis.from_url(os.environ['REDIS_URL'])
 
     url = os.environ['WEBHOOK_URL']
-    payload = {'cmd': sys.argv[1:]}
+    payload = {
+        'cmd': sys.argv[1:],
+    }
     if 'WEBHOOK_CWD' in os.environ:
         payload['cwd'] = os.environ['WEBHOOK_CWD']
     if 'WEBHOOK_TIMEOUT' in os.environ:
         payload['timeout'] = float(os.environ['WEBHOOK_TIMEOUT'])
 
     env = {
         k.removeprefix(ENV_PREFIX): v
         for k, v in os.environ.items()
         if k.startswith(ENV_PREFIX)
     }
-
     print(env)
     command = ShellCommand(**payload)
     headers = {'token': os.environ['WEBHOOK_TOKEN']}
-    response = requests.post(url, headers=headers, json=payload)
+    response = requests.post(url, headers=headers, json=command.dict())
 
     if not response.ok:
         print(response.status_code)
         print(response.text)
         raise SystemExit(1)
 
     assert response.json() == {'process-created': 'ok'}
     print(response.json())
+    print(f'{config.PROCESS_DONE}:{command.id}')
     _, message = redis.brpop(f'{config.PROCESS_DONE}:{command.id}')
     result = ShellResult.parse_raw(message)
     print(result)
     assert result.returncode == 0
 
 
-
-
-
 if __name__ == '__main__':
     main()
```

### Comparing `webhooklib-0.1.4/webhooklib/server.py` & `webhooklib-0.1.5/webhooklib/server.py`

 * *Files identical despite different names*

