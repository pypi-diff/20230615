# Comparing `tmp/stale_maccarone-0.1.2.tar.gz` & `tmp/stale_maccarone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.1.2.tar", last modified: Wed Jun 14 22:39:55 2023, max compression
+gzip compressed data, was "stale_maccarone-0.1.3.tar", last modified: Thu Jun 15 00:28:40 2023, max compression
```

## Comparing `stale_maccarone-0.1.2.tar` & `stale_maccarone-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/add.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/fizzbuzz.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/todo.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.641556 stale_maccarone-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/caching.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-14 22:39:47.000000 stale_maccarone-0.1.2/src/stale_maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 22:39:55.000000 stale_maccarone-0.1.2/src/stale_maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:39:55.645556 stale_maccarone-0.1.2/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-14 22:39:30.000000 stale_maccarone-0.1.2/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.855324 stale_maccarone-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.843324 stale_maccarone-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.847324 stale_maccarone-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 00:28:40.855324 stale_maccarone-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.851324 stale_maccarone-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/file_sizes_inlined.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/file_sizes_inlined.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:28:40.855324 stale_maccarone-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.843324 stale_maccarone-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.851324 stale_maccarone-0.1.3/src/stale_maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.851324 stale_maccarone-0.1.3/src/stale_maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.851324 stale_maccarone-0.1.3/src/stale_maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-15 00:28:33.000000 stale_maccarone-0.1.3/src/stale_maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.851324 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 00:28:40.000000 stale_maccarone-0.1.3/src/stale_maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:40.855324 stale_maccarone-0.1.3/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-15 00:28:14.000000 stale_maccarone-0.1.3/support/rename_to_stale.sh
```

### Comparing `stale_maccarone-0.1.2/.github/workflows/publish-to-pypi-stale.yml` & `stale_maccarone-0.1.3/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/.github/workflows/publish-to-pypi.yml` & `stale_maccarone-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/.github/workflows/run-pytest.yml` & `stale_maccarone-0.1.3/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/.gitignore` & `stale_maccarone-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/LICENSE` & `stale_maccarone-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/PKG-INFO` & `stale_maccarone-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stale_maccarone
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

### Comparing `stale_maccarone-0.1.2/README.md` & `stale_maccarone-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/dev-requirements.txt` & `stale_maccarone-0.1.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.json` & `stale_maccarone-0.1.3/examples/file_sizes_inlined.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/examples/file_sizes_inlined.mn.py` & `stale_maccarone-0.1.3/examples/file_sizes_inlined.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/examples/fizzbuzz.mn.json` & `stale_maccarone-0.1.3/examples/fizzbuzz.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/examples/todo.mn.json` & `stale_maccarone-0.1.3/examples/todo.mn.json`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/pyproject.toml` & `stale_maccarone-0.1.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 [project]
 name = "stale_maccarone"
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
 stale_maccarone = "stale_maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/caching.mn.py` & `stale_maccarone-0.1.3/src/stale_maccarone/caching.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/caching.py` & `stale_maccarone-0.1.3/src/stale_maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/loader.mn.py` & `stale_maccarone-0.1.3/src/stale_maccarone/loader.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/loader.py` & `stale_maccarone-0.1.3/src/stale_maccarone/loader.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/openai.py` & `stale_maccarone-0.1.3/src/stale_maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/preprocessor.py` & `stale_maccarone-0.1.3/src/stale_maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.mn.py` & `stale_maccarone-0.1.3/src/stale_maccarone/scripts/preprocess.mn.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/scripts/preprocess.py` & `stale_maccarone-0.1.3/src/stale_maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/test/test_caching.py` & `stale_maccarone-0.1.3/src/stale_maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone/test/test_preprocessor.py` & `stale_maccarone-0.1.3/src/stale_maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone.egg-info/PKG-INFO` & `stale_maccarone-0.1.3/src/stale_maccarone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stale-maccarone
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

### Comparing `stale_maccarone-0.1.2/src/stale_maccarone.egg-info/SOURCES.txt` & `stale_maccarone-0.1.3/src/stale_maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.1.2/support/rename_to_stale.sh` & `stale_maccarone-0.1.3/support/rename_to_stale.sh`

 * *Files identical despite different names*

