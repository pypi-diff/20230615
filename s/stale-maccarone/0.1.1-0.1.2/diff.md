# Comparing `tmp/stale_maccarone-0.1.1.tar.gz` & `tmp/stale_maccarone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.1.1.tar", last modified: Mon Jun 12 23:23:10 2023, max compression
+gzip compressed data, was "stale_maccarone-0.1.2.tar", last modified: Wed Jun 14 22:39:55 2023, max compression
```

## Comparing `stale_maccarone-0.1.1.tar` & `stale_maccarone-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.199206 stale_maccarone-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.199206 stale_maccarone-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/add.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/file_sizes.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/file_sizes.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/file_sizes_inlined.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/file_sizes_inlined.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/fizzbuzz.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/todo.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.199206 stale_maccarone-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/src/stale_maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/caching.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/src/stale_maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/src/stale_maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-12 23:23:02.000000 stale_maccarone-0.1.1/src/stale_maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 23:23:10.000000 stale_maccarone-0.1.1/src/stale_maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:10.203206 stale_maccarone-0.1.1/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-12 23:22:42.000000 stale_maccarone-0.1.1/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/support/rename_to_stale.sh
```

### Comparing `stale_maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml` & `stale_maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/.github/workflows/publish-to-pypi.yml` & `stale_maccarone-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/.github/workflows/run-pytest.yml` & `stale_maccarone-0.1.2/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/.gitignore` & `stale_maccarone-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/LICENSE` & `stale_maccarone-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/PKG-INFO` & `stale_maccarone-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stale_maccarone
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

### Comparing `stale_maccarone-0.1.1/README.md` & `stale_maccarone-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/dev-requirements.txt` & `stale_maccarone-0.1.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/examples/file_sizes_inlined.mn.json` & `stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/examples/file_sizes_inlined.mn.py` & `stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/examples/fizzbuzz.mn.json` & `stale_maccarone-0.1.2/examples/fizzbuzz.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/examples/todo.mn.json` & `stale_maccarone-0.1.2/examples/todo.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/pyproject.toml` & `stale_maccarone-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/caching.mn.py` & `stale_maccarone-0.1.2/src/stale_maccarone/caching.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/caching.py` & `stale_maccarone-0.1.2/src/stale_maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/loader.mn.py` & `stale_maccarone-0.1.2/src/stale_maccarone/loader.mn.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
 from stale_maccarone.openai import CachedChatAPI
 from stale_maccarone.preprocessor import preprocess_maccarone
 
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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/loader.py` & `stale_maccarone-0.1.2/src/stale_maccarone/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib.machinery import ModuleSpec
 from fnmatch import fnmatchcase
 
 from stale_maccarone.openai import CachedChatAPI
 from stale_maccarone.preprocessor import preprocess_maccarone
 
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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/openai.py` & `stale_maccarone-0.1.2/src/stale_maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/preprocessor.py` & `stale_maccarone-0.1.2/src/stale_maccarone/preprocessor.py`

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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/scripts/preprocess.mn.py` & `stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.mn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import os
+import os.path
 import glob
 import logging
 
 from argparse import Namespace
 
 from stale_maccarone.openai import CachedChatAPI
+from stale_maccarone.loader import (
+    DEFAULT_CACHE_SUFFIX,
+    DEFAULT_MN_SUFFIX,
+    replace_suffix,
+)
 from stale_maccarone.preprocessor import preprocess_maccarone
 
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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/scripts/preprocess.py` & `stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import os
+import os.path
 import glob
 import logging
 
 from argparse import Namespace
 
 from stale_maccarone.openai import CachedChatAPI
+from stale_maccarone.loader import (
+    DEFAULT_CACHE_SUFFIX,
+    DEFAULT_MN_SUFFIX,
+    replace_suffix,
+)
 from stale_maccarone.preprocessor import preprocess_maccarone
 
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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/test/test_caching.py` & `stale_maccarone-0.1.2/src/stale_maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone/test/test_preprocessor.py` & `stale_maccarone-0.1.2/src/stale_maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone.egg-info/PKG-INFO` & `stale_maccarone-0.1.2/src/stale_maccarone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stale-maccarone
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

### Comparing `stale_maccarone-0.1.1/src/stale_maccarone.egg-info/SOURCES.txt` & `stale_maccarone-0.1.2/src/stale_maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.1/support/rename_to_stale.sh` & `stale_maccarone-0.1.2/support/rename_to_stale.sh`

 * *Files identical despite different names*

