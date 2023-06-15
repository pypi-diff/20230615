# Comparing `tmp/pytest_xdist_worker_stats-0.1.0.tar.gz` & `tmp/pytest_xdist_worker_stats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.0.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.1.1.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.0.tar` & `pytest_xdist_worker_stats-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-15 08:53:33.817321 pytest_xdist_worker_stats-0.1.0/LICENSE
--rw-r--r--   0        0        0     2092 2023-06-15 08:53:33.823321 pytest_xdist_worker_stats-0.1.0/README.md
--rw-r--r--   0        0        0     2831 2023-06-15 08:55:44.208548 pytest_xdist_worker_stats-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.0/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.0/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     2372 2023-06-15 08:53:33.822321 pytest_xdist_worker_stats-0.1.0/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 08:53:33.817321 pytest_xdist_worker_stats-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2004 2023-06-15 08:57:34.823044 pytest_xdist_worker_stats-0.1.1/README.md
+-rw-r--r--   0        0        0     2831 2023-06-15 08:57:22.904206 pytest_xdist_worker_stats-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-06-15 08:57:22.908206 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     2372 2023-06-15 08:53:33.822321 pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.1/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.0/LICENSE` & `pytest_xdist_worker_stats-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.0/README.md` & `pytest_xdist_worker_stats-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,24 +35,23 @@
 worker gw10 :   41 tests       5.60s runtime
 worker gw11 :   47 tests       5.59s runtime
 ================================================ 318 passed in 26.66s ================================================
 ```
 
 ## Development
 
-[Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development. Ther are some tests, obviously written in [pytest](https://pytest.org/).
+[Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development.
 
 ```shell
 $ poetry install
 $ pre-commit install
-$ pytest tests
 ```
 
 ## Thanks
 
 Many thanks to [Denys Korytkin](https://github.com/DKorytkin) for the article [How to get data from pytest-xdist nodes](https://korytkin.medium.com/how-to-get-data-from-pytest-xdist-nodes-2fbf2f0fe957).
 
 ## Changelog
 
-### 0.1.0 (Jun 15, 2023)
+### 0.1.1 (Jun 15, 2023)
 
 * First Release
```

### Comparing `pytest_xdist_worker_stats-0.1.0/pyproject.toml` & `pytest_xdist_worker_stats-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.0"
+version = "0.1.1"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pytest_xdist_worker_stats-0.1.0/pytest_xdist_worker_stats/options.py` & `pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/options.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.0/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.1.1/pytest_xdist_worker_stats/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.0/PKG-INFO` & `pytest_xdist_worker_stats-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist-worker-stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to list worker statistics after a xdist run.
 Home-page: https://github.com/mikicz/pytest-xdist-worker-stats
 License: MIT
 Keywords: pytest,xdist,pytest-xdist
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -60,25 +60,24 @@
 worker gw10 :   41 tests       5.60s runtime
 worker gw11 :   47 tests       5.59s runtime
 ================================================ 318 passed in 26.66s ================================================
 ```
 
 ## Development
 
-[Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development. Ther are some tests, obviously written in [pytest](https://pytest.org/).
+[Poetry](https://python-poetry.org/) (dependencies) and [pre-commit](https://pre-commit.com/) (coding standards) are required for development.
 
 ```shell
 $ poetry install
 $ pre-commit install
-$ pytest tests
 ```
 
 ## Thanks
 
 Many thanks to [Denys Korytkin](https://github.com/DKorytkin) for the article [How to get data from pytest-xdist nodes](https://korytkin.medium.com/how-to-get-data-from-pytest-xdist-nodes-2fbf2f0fe957).
 
 ## Changelog
 
-### 0.1.0 (Jun 15, 2023)
+### 0.1.1 (Jun 15, 2023)
 
 * First Release
```

