# Comparing `tmp/maccarone-0.1.1.tar.gz` & `tmp/maccarone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.1.1.tar", last modified: Mon Jun 12 23:23:24 2023, max compression
+gzip compressed data, was "maccarone-0.1.2.tar", last modified: Wed Jun 14 22:39:58 2023, max compression
```

## Comparing `maccarone-0.1.1.tar` & `maccarone-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.525112 maccarone-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.529112 maccarone-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-12 23:22:45.000000 maccarone-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 23:22:45.000000 maccarone-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 23:23:24.537113 maccarone-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:22:45.000000 maccarone-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-12 23:22:45.000000 maccarone-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.533112 maccarone-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/add.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes_inlined.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes_inlined.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/fizzbuzz.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/todo.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 23:22:45.000000 maccarone-0.1.1/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-12 23:22:45.000000 maccarone-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:23:24.537113 maccarone-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.525112 maccarone-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.533112 maccarone-0.1.1/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/caching.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/caching.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/loader.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-12 23:22:45.000000 maccarone-0.1.1/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-14 22:39:31.000000 maccarone-0.1.2/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-14 22:39:31.000000 maccarone-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 22:39:31.000000 maccarone-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-14 22:39:58.687978 maccarone-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-14 22:39:31.000000 maccarone-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 22:39:31.000000 maccarone-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes_inlined.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/file_sizes_inlined.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 22:39:31.000000 maccarone-0.1.2/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 22:39:31.000000 maccarone-0.1.2/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-14 22:39:31.000000 maccarone-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:39:58.687978 maccarone-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.683978 maccarone-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/caching.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/loader.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-14 22:39:50.000000 maccarone-0.1.2/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-14 22:39:31.000000 maccarone-0.1.2/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 22:39:58.000000 maccarone-0.1.2/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:58.687978 maccarone-0.1.2/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-14 22:39:31.000000 maccarone-0.1.2/support/rename_to_stale.sh
```

### Comparing `maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml` & `maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/.github/workflows/publish-to-pypi.yml` & `maccarone-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/.github/workflows/run-pytest.yml` & `maccarone-0.1.2/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/.gitignore` & `maccarone-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/LICENSE` & `maccarone-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/PKG-INFO` & `maccarone-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.1/README.md` & `maccarone-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/dev-requirements.txt` & `maccarone-0.1.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/examples/file_sizes_inlined.mn.json` & `maccarone-0.1.2/examples/file_sizes_inlined.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/examples/file_sizes_inlined.mn.py` & `maccarone-0.1.2/examples/file_sizes_inlined.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/examples/fizzbuzz.mn.json` & `maccarone-0.1.2/examples/fizzbuzz.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/examples/todo.mn.json` & `maccarone-0.1.2/examples/todo.mn.json`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/pyproject.toml` & `maccarone-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone/caching.mn.py` & `maccarone-0.1.2/src/maccarone/caching.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone/caching.py` & `maccarone-0.1.2/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone/loader.mn.py` & `maccarone-0.1.2/src/maccarone/loader.mn.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
 from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
 SNIPPET_START = "#" + "<<"
+DEFAULT_MN_SUFFIX = ".mn.py"
+DEFAULT_CACHE_SUFFIX = ".mn.json"
 
 class ImportFinder(MetaPathFinder):
     def __init__(
             self,
             py_string_matching: bool,
             include_pattern: str | None,
             exclude_pattern: str | None,
@@ -47,41 +49,57 @@
         if path is None or path == '':
             path = [os.getcwd()]  # top level import 
 
         for entry in path:
             basename = fullname.split(".")[-1]
             base_filename = os.path.join(entry, basename)
             py_filename = base_filename + '.py'
-            mn_filename = base_filename + '.mn.py'
+            mn_filename = base_filename + DEFAULT_MN_SUFFIX
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
             elif self.py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
                     if SNIPPET_START in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
-def py_path_to_cache_path(py_path):
-    #<<replace regex: r"\.py$" -> ".json">>
+def replace_suffix(path: str, new_suffix: str, search_suffix: str) -> str:
+    """
+    Replace suffix (i.e., file extension) per the following rules:
+
+    - Replace entire search suffix if it matches.
+    - Otherwise replace the last file extension.
+    """
+
+    if path.endswith(search_suffix):
+        return path[:-len(search_suffix)] + new_suffix
+    else:
+        (root, _) = os.path.splitext(path)
+
+        return root + new_suffix
 
 class ImportLoader(SourceLoader):
     def __init__(self, fullname, path):
         self.fullname = fullname
         self.path = path
 
     def get_filename(self, fullname):
         return self.path
 
     def get_data(self, filename):
         with open(self.path, 'r') as file:
             in_source = file.read()
 
-        cache_path = py_path_to_cache_path(self.path)
+        cache_path = replace_suffix(
+            self.path,
+            DEFAULT_CACHE_SUFFIX,
+            search_suffix=DEFAULT_MN_SUFFIX,
+        )
         chat_api = CachedChatAPI(cache_path)
 
         return preprocess_maccarone(in_source, chat_api)
 
 def enable(
         py_string_matching=True,
         include_pattern=None,
```

### Comparing `maccarone-0.1.1/src/maccarone/loader.py` & `maccarone-0.1.2/src/maccarone/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
 from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
 SNIPPET_START = "#" + "<<"
+DEFAULT_MN_SUFFIX = ".mn.py"
+DEFAULT_CACHE_SUFFIX = ".mn.json"
 
 class ImportFinder(MetaPathFinder):
     def __init__(
             self,
             py_string_matching: bool,
             include_pattern: str | None,
             exclude_pattern: str | None,
@@ -47,42 +49,57 @@
         if path is None or path == '':
             path = [os.getcwd()]  # top level import 
 
         for entry in path:
             basename = fullname.split(".")[-1]
             base_filename = os.path.join(entry, basename)
             py_filename = base_filename + '.py'
-            mn_filename = base_filename + '.mn.py'
+            mn_filename = base_filename + DEFAULT_MN_SUFFIX
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
             elif self.py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
                     if SNIPPET_START in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
-def py_path_to_cache_path(py_path):
-    return py_path.replace(".py", ".json")
+def replace_suffix(path: str, new_suffix: str, search_suffix: str) -> str:
+    """
+    Replace suffix (i.e., file extension) per the following rules:
+
+    - Replace entire search suffix if it matches.
+    - Otherwise replace the last file extension.
+    """
+
+    if path.endswith(search_suffix):
+        return path[:-len(search_suffix)] + new_suffix
+    else:
+        (root, _) = os.path.splitext(path)
 
+        return root + new_suffix
 
 class ImportLoader(SourceLoader):
     def __init__(self, fullname, path):
         self.fullname = fullname
         self.path = path
 
     def get_filename(self, fullname):
         return self.path
 
     def get_data(self, filename):
         with open(self.path, 'r') as file:
             in_source = file.read()
 
-        cache_path = py_path_to_cache_path(self.path)
+        cache_path = replace_suffix(
+            self.path,
+            DEFAULT_CACHE_SUFFIX,
+            search_suffix=DEFAULT_MN_SUFFIX,
+        )
         chat_api = CachedChatAPI(cache_path)
 
         return preprocess_maccarone(in_source, chat_api)
 
 def enable(
         py_string_matching=True,
         include_pattern=None,
```

### Comparing `maccarone-0.1.1/src/maccarone/openai.py` & `maccarone-0.1.2/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone/preprocessor.py` & `maccarone-0.1.2/src/maccarone/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,22 @@
 
     for raw in raw_pieces:
         match raw:
             case PresentPiece(text):
                 final_source += text
 
             case MissingPiece(indent, guidance):
-                final_source += f"{indent}#<<{guidance}>>\n"
+                if "\n" in guidance:
+                    guidance_lines = "\n"
+                    guidance_lines += "\n".join(f"{indent}#{line}" for line in guidance.splitlines())
+                    guidance_lines += f"\n{indent}#"
+                else:
+                    guidance_lines = guidance
+
+                final_source += f"{indent}#<<{guidance_lines}>>\n"
                 completed = completed_pieces[id]
                 final_source += indent + indent.join(completed.splitlines(True))
                 final_source += f"{indent}#<</>>\n"
                 id += 1
 
             case _:
                 raise TypeError("unknown piece type", raw)
```

### Comparing `maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.json` & `maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'tagged_input_to_tagged_output'": "{'inputs_hash': "*

 * *                                    "'75cad4c66c74b11760e3b155fb6c652ea42d268c53f544f5f26c733cf1ed593a', "*

 * *                                    '\'value\': \'<completed id="0">\\nwith open(mn_path, "r") as '*

 * *                                    'f:\\n    mn_source = f.read()\\n</>\\n\\n<completed '*

 * *                                    'id="1">\\nif py_path is not None:\\n    with open(py_path, '*

 * *                                    '"w") as f:\\n        f.w […]*

```diff
@@ -1,6 +1,6 @@
 {
     "tagged_input_to_tagged_output": {
-        "inputs_hash": "f6eb8c528beaad4c1cdd702662650244e10726dcb97093968930adb4ff6f13e1",
-        "value": "<completed id=\"0\">\nmn_source = open(mn_path, \"r\").read()\n</>\n<completed id=\"1\">\nimport re\npy_path = re.sub(f\"{suffix}$\", \".py\", mn_path)\n</>\n<completed id=\"2\">\nif py_path is not None:\n    with open(py_path, \"w\") as f:\n        f.write(py_source)\n</>\n<completed id=\"3\">\nfor mn_file in mn_files:\n    preprocess(mn_file, print_, write, rewrite, suffix)\n</>\n<completed id=\"4\">\nimport argparse\nparser = argparse.ArgumentParser()\nparser.add_argument(\"path\", help=\"Path to the file or directory containing Maccarone snippets\")\nparser.add_argument(\"--print\", dest=\"print_\", action=\"store_true\", help=\"Print the preprocessed Python source\")\nparser.add_argument(\"--write\", action=\"store_true\", help=\"Write the preprocessed Python source to a new file\")\nparser.add_argument(\"--rewrite\", action=\"store_true\", help=\"Overwrite the input file with the preprocessed Python source\")\nparser.add_argument(\"--suffix\", default=\".mn.py\", help=\"Suffix for Maccarone snippet files (default: .mn.py)\")\nargs = parser.parse_args()\nreturn args\n</>"
+        "inputs_hash": "75cad4c66c74b11760e3b155fb6c652ea42d268c53f544f5f26c733cf1ed593a",
+        "value": "<completed id=\"0\">\nwith open(mn_path, \"r\") as f:\n    mn_source = f.read()\n</>\n\n<completed id=\"1\">\nif py_path is not None:\n    with open(py_path, \"w\") as f:\n        f.write(py_source)\n</>\n\n<completed id=\"2\">\nfor mn_file in mn_files:\n    preprocess(mn_file, print_, write, rewrite, suffix)\n</>\n\n<completed id=\"3\">\nimport argparse\nparser = argparse.ArgumentParser(description=\"Preprocess files with Maccarone snippets.\")\nparser.add_argument(\"path\", help=\"Path to the file or directory containing files to preprocess.\")\nparser.add_argument(\"--print\", dest=\"print_\", action=\"store_true\", help=\"Print the preprocessed Python source.\")\nparser.add_argument(\"--write\", action=\"store_true\", help=\"Write the preprocessed Python source to a .py file.\")\nparser.add_argument(\"--rewrite\", action=\"store_true\", help=\"Overwrite the input file with the preprocessed Python source.\")\nparser.add_argument(\"--suffix\", default=DEFAULT_MN_SUFFIX, help=\"Suffix for files to preprocess (default: %(default)s).\")\nargs = parser.parse_args()\nreturn args\n</>"
     }
 }
```

### Comparing `maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.py` & `maccarone-0.1.2/src/maccarone/scripts/preprocess.mn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import os
+import os.path
 import glob
 import logging
 
 from argparse import Namespace
 
 from maccarone.openai import CachedChatAPI
+from maccarone.loader import (
+    DEFAULT_CACHE_SUFFIX,
+    DEFAULT_MN_SUFFIX,
+    replace_suffix,
+)
 from maccarone.preprocessor import preprocess_maccarone
 
 logger = logging.getLogger(__name__)
 
 def preprocess(
         mn_path: str,
         print_: bool,
         write: bool,
         rewrite: bool,
-        suffix: str,
+        search_suffix: str,
     ) -> None:
     # produce Python source
     logger.info("preprocessing %s", mn_path)
 
-    cache_path = mn_path.replace(suffix, ".mn.json")
+    cache_path = replace_suffix(mn_path, DEFAULT_CACHE_SUFFIX, search_suffix)
     chat_api = CachedChatAPI(cache_path)
 
     #<<mn_source = read mn_path>>
 
     py_source = preprocess_maccarone(mn_source, chat_api)
 
     if write:
-        #<<py_path = regex replace mn_path: f"{suffix}$" -> ".py">>
+        py_path = replace_suffix(mn_path, ".py", search_suffix)
 
         logger.info("writing %s", py_path)
 
         if py_path == mn_path:
             raise ValueError("won't overwrite input file", mn_path)
     elif rewrite:
         py_path = mn_path
@@ -56,18 +62,17 @@
 
     #<<preprocess mn_files>>
 
 def parse_args() -> Namespace:
     #<<
     # get args for main() and return; use argparse
     # set the `print_` var for `--print`
-    # default suffix: ".mn.py"
+    # default suffix: DEFAULT_MN_SUFFIX
     #>>
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
 
 if __name__ == "__main__":
     script_main()
-
```

### Comparing `maccarone-0.1.1/src/maccarone/scripts/preprocess.py` & `maccarone-0.1.2/src/maccarone/scripts/preprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import os
+import os.path
 import glob
 import logging
 
 from argparse import Namespace
 
 from maccarone.openai import CachedChatAPI
+from maccarone.loader import (
+    DEFAULT_CACHE_SUFFIX,
+    DEFAULT_MN_SUFFIX,
+    replace_suffix,
+)
 from maccarone.preprocessor import preprocess_maccarone
 
 logger = logging.getLogger(__name__)
 
 def preprocess(
         mn_path: str,
         print_: bool,
         write: bool,
         rewrite: bool,
-        suffix: str,
+        search_suffix: str,
     ) -> None:
     # produce Python source
     logger.info("preprocessing %s", mn_path)
 
-    cache_path = mn_path.replace(suffix, ".mn.json")
+    cache_path = replace_suffix(mn_path, DEFAULT_CACHE_SUFFIX, search_suffix)
     chat_api = CachedChatAPI(cache_path)
 
-    mn_source = open(mn_path, "r").read()
+    with open(mn_path, "r") as f:
+        mn_source = f.read()
 
 
     py_source = preprocess_maccarone(mn_source, chat_api)
 
     if write:
-        import re
-        py_path = re.sub(f"{suffix}$", ".py", mn_path)
-
+        py_path = replace_suffix(mn_path, ".py", search_suffix)
 
         logger.info("writing %s", py_path)
 
         if py_path == mn_path:
             raise ValueError("won't overwrite input file", mn_path)
     elif rewrite:
         py_path = mn_path
@@ -62,25 +67,24 @@
 
     for mn_file in mn_files:
         preprocess(mn_file, print_, write, rewrite, suffix)
 
 
 def parse_args() -> Namespace:
     import argparse
-    parser = argparse.ArgumentParser()
-    parser.add_argument("path", help="Path to the file or directory containing Maccarone snippets")
-    parser.add_argument("--print", dest="print_", action="store_true", help="Print the preprocessed Python source")
-    parser.add_argument("--write", action="store_true", help="Write the preprocessed Python source to a new file")
-    parser.add_argument("--rewrite", action="store_true", help="Overwrite the input file with the preprocessed Python source")
-    parser.add_argument("--suffix", default=".mn.py", help="Suffix for Maccarone snippet files (default: .mn.py)")
+    parser = argparse.ArgumentParser(description="Preprocess files with Maccarone snippets.")
+    parser.add_argument("path", help="Path to the file or directory containing files to preprocess.")
+    parser.add_argument("--print", dest="print_", action="store_true", help="Print the preprocessed Python source.")
+    parser.add_argument("--write", action="store_true", help="Write the preprocessed Python source to a .py file.")
+    parser.add_argument("--rewrite", action="store_true", help="Overwrite the input file with the preprocessed Python source.")
+    parser.add_argument("--suffix", default=DEFAULT_MN_SUFFIX, help="Suffix for files to preprocess (default: %(default)s).")
     args = parser.parse_args()
     return args
 
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
 
 if __name__ == "__main__":
     script_main()
-
```

### Comparing `maccarone-0.1.1/src/maccarone/test/test_caching.py` & `maccarone-0.1.2/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone/test/test_preprocessor.py` & `maccarone-0.1.2/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/src/maccarone.egg-info/PKG-INFO` & `maccarone-0.1.2/src/maccarone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.1/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.1.2/src/maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.1/support/rename_to_stale.sh` & `maccarone-0.1.2/support/rename_to_stale.sh`

 * *Files identical despite different names*

