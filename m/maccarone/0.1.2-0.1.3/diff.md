# Comparing `tmp/maccarone-0.1.2.tar.gz` & `tmp/maccarone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.1.2.tar", last modified: Wed Jun 14 22:39:58 2023, max compression
+gzip compressed data, was "maccarone-0.1.3.tar", last modified: Thu Jun 15 00:28:41 2023, max compression
```

## Comparing `maccarone-0.1.2.tar` & `maccarone-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-14 22:39:31.000000 maccarone-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 22:39:31.000000 maccarone-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-14 22:39:58.687978 maccarone-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-14 22:39:31.000000 maccarone-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 22:39:31.000000 maccarone-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/add.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes_inlined.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes_inlined.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/fizzbuzz.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/todo.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 22:39:31.000000 maccarone-0.1.2/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-14 22:39:31.000000 maccarone-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:39:58.687978 maccarone-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/caching.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/caching.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/loader.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-14 22:39:31.000000 maccarone-0.1.2/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.589056 maccarone-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.585056 maccarone-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.585056 maccarone-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 00:28:14.000000 maccarone-0.1.3/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-15 00:28:14.000000 maccarone-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-15 00:28:14.000000 maccarone-0.1.3/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 00:28:14.000000 maccarone-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 00:28:14.000000 maccarone-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-15 00:28:41.589056 maccarone-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 00:28:14.000000 maccarone-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-15 00:28:14.000000 maccarone-0.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.585056 maccarone-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/file_sizes_inlined.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/file_sizes_inlined.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 00:28:14.000000 maccarone-0.1.3/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 00:28:14.000000 maccarone-0.1.3/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-15 00:28:14.000000 maccarone-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:28:41.589056 maccarone-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.585056 maccarone-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.585056 maccarone-0.1.3/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/caching.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-15 00:28:33.000000 maccarone-0.1.3/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/loader.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 00:28:33.000000 maccarone-0.1.3/src/maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.589056 maccarone-0.1.3/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/scripts/preprocess.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-15 00:28:33.000000 maccarone-0.1.3/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.589056 maccarone-0.1.3/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-15 00:28:14.000000 maccarone-0.1.3/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.589056 maccarone-0.1.3/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 00:28:41.000000 maccarone-0.1.3/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:41.589056 maccarone-0.1.3/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-15 00:28:14.000000 maccarone-0.1.3/support/rename_to_stale.sh
```

### Comparing `maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml` & `maccarone-0.1.3/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/.github/workflows/publish-to-pypi.yml` & `maccarone-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/.github/workflows/run-pytest.yml` & `maccarone-0.1.3/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/.gitignore` & `maccarone-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/LICENSE` & `maccarone-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/PKG-INFO` & `maccarone-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.2/README.md` & `maccarone-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/dev-requirements.txt` & `maccarone-0.1.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/examples/file_sizes_inlined.mn.json` & `maccarone-0.1.3/examples/file_sizes_inlined.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/examples/file_sizes_inlined.mn.py` & `maccarone-0.1.3/examples/file_sizes_inlined.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/examples/fizzbuzz.mn.json` & `maccarone-0.1.3/examples/fizzbuzz.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/examples/todo.mn.json` & `maccarone-0.1.3/examples/todo.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/pyproject.toml` & `maccarone-0.1.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 [project]
 name = "maccarone"
 readme = "README.md"
 description = "Mix natural language into your Python code"
 requires-python = ">=3.10"
 dependencies = [
     "openai",
-    "pytest",
-    "pytest-asyncio",
+    "parsimonious",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/bsilverthorn/maccarone"
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
+    "pytest",
+    "pytest-asyncio",
     "ipython",
     "pip-tools",
     "stale_maccarone==0.0.12",
-    "parsimonious",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `maccarone-0.1.2/src/maccarone/caching.mn.py` & `maccarone-0.1.3/src/maccarone/caching.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/caching.py` & `maccarone-0.1.3/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/loader.mn.py` & `maccarone-0.1.3/src/maccarone/loader.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/loader.py` & `maccarone-0.1.3/src/maccarone/loader.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/openai.py` & `maccarone-0.1.3/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/preprocessor.py` & `maccarone-0.1.3/src/maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.json` & `maccarone-0.1.3/src/maccarone/scripts/preprocess.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.py` & `maccarone-0.1.3/src/maccarone/scripts/preprocess.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/scripts/preprocess.py` & `maccarone-0.1.3/src/maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/test/test_caching.py` & `maccarone-0.1.3/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone/test/test_preprocessor.py` & `maccarone-0.1.3/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/src/maccarone.egg-info/PKG-INFO` & `maccarone-0.1.3/src/maccarone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.2/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.1.3/src/maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.2/support/rename_to_stale.sh` & `maccarone-0.1.3/support/rename_to_stale.sh`

 * *Files identical despite different names*

