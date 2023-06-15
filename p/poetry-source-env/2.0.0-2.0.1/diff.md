# Comparing `tmp/poetry_source_env-2.0.0.tar.gz` & `tmp/poetry_source_env-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_source_env-2.0.0.tar", max compression
+gzip compressed data, was "poetry_source_env-2.0.1.tar", max compression
```

## Comparing `poetry_source_env-2.0.0.tar` & `poetry_source_env-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     3950 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/poetry_source_env/__init__.py
--rw-r--r--   0        0        0     2787 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/poetry_source_env/plugin.py
--rw-r--r--   0        0        0      739 2023-05-23 20:45:14.038232 poetry_source_env-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 poetry_source_env-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-06-15 20:43:35.606705 poetry_source_env-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0     4275 2023-06-15 20:43:35.606705 poetry_source_env-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 20:43:35.606705 poetry_source_env-2.0.1/poetry_source_env/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-15 20:43:35.606705 poetry_source_env-2.0.1/poetry_source_env/plugin.py
+-rw-r--r--   0        0        0      739 2023-06-15 20:43:35.606705 poetry_source_env-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5110 1970-01-01 00:00:00.000000 poetry_source_env-2.0.1/PKG-INFO
```

### Comparing `poetry_source_env-2.0.0/LICENSE.md` & `poetry_source_env-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poetry_source_env-2.0.0/README.md` & `poetry_source_env-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 poetry-source-env is a Poetry plugin that lets you define private package sources for your project without exposing
 their URLs in `pyproject.toml`. It can load package source definitions from environment variables and expand environment
 variables in the `tool.poetry.source` section of `pyproject.toml`.
 
 This plugin is intended as a workaround for python-poetry/poetry#5958 and will be deprecated if comparable functionality
 is ever implemented in Poetry itself.
 
+Note that poetry-source-env cannot resolve repositories when installing other Poetry plugins (Poetry does not
+load plugins when running `poetry self` commands). If you need a python-poetry/poetry#5958 workaround for installing Poetry
+plugins, see https://github.com/python-poetry/poetry/issues/5958#issuecomment-1479183720.
+
 ## Installation
 
 ```bash
 poetry self add poetry-source-env
 ```
 
 ## Usage
```

### Comparing `poetry_source_env-2.0.0/poetry_source_env/plugin.py` & `poetry_source_env-2.0.1/poetry_source_env/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,23 +56,13 @@
                 }
 
                 priority = priorities.get(priority_name.casefold(), Priority.PRIMARY)
 
                 poetry.pool.add_repository(repo, priority=priority)
 
         if config.toml:
-            for repository in poetry.pool.repositories:
-                definition = next(
-                    (
-                        source
-                        for source in poetry.get_sources()
-                        if source.name == repository.name
-                    ),
-                    None,
+            for repository in poetry.get_sources():
+                poetry.pool.remove_repository(repository.name)
+                repo = LegacyRepository(
+                    expandvars(repository.name), expandvars(repository.url)
                 )
-
-                if definition:
-                    poetry.pool.remove_repository(repository.name)
-                    repo = LegacyRepository(
-                        expandvars(definition.name), expandvars(definition.url)
-                    )
-                    poetry.pool.add_repository(repo, priority=definition.priority)
+                poetry.pool.add_repository(repo, priority=repository.priority)
```

### Comparing `poetry_source_env-2.0.0/pyproject.toml` & `poetry_source_env-2.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-source-env"
-version = "2.0.0"
+version = "2.0.1"
 description = "Load Poetry package sources from environment variables"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/celsiusnarhwal/poetry-source-env"
 repository = "https://github.com/celsiusnarhwal/poetry-source-env"
```

### Comparing `poetry_source_env-2.0.0/PKG-INFO` & `poetry_source_env-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-source-env
-Version: 2.0.0
+Version: 2.0.1
 Summary: Load Poetry package sources from environment variables
 Home-page: https://github.com/celsiusnarhwal/poetry-source-env
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,18 @@
 poetry-source-env is a Poetry plugin that lets you define private package sources for your project without exposing
 their URLs in `pyproject.toml`. It can load package source definitions from environment variables and expand environment
 variables in the `tool.poetry.source` section of `pyproject.toml`.
 
 This plugin is intended as a workaround for python-poetry/poetry#5958 and will be deprecated if comparable functionality
 is ever implemented in Poetry itself.
 
+Note that poetry-source-env cannot resolve repositories when installing other Poetry plugins (Poetry does not
+load plugins when running `poetry self` commands). If you need a python-poetry/poetry#5958 workaround for installing Poetry
+plugins, see https://github.com/python-poetry/poetry/issues/5958#issuecomment-1479183720.
+
 ## Installation
 
 ```bash
 poetry self add poetry-source-env
 ```
 
 ## Usage
```

