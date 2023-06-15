# Comparing `tmp/lamin_logger-0.4.0.tar.gz` & `tmp/lamin_logger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.4.0.tar` & `lamin_logger-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.4.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.4.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.4.0/.gitignore
--rw-r--r--   0        0        0     1753 2022-07-20 10:00:56.098007 lamin_logger-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.4.0/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.4.0/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.4.0/docs/api.md
--rw-r--r--   0        0        0     2813 2023-06-15 15:21:43.974199 lamin_logger-0.4.0/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.4.0/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.4.0/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.4.0/lamin-project.yaml
--rw-r--r--   0        0        0      271 2023-06-15 15:21:52.448649 lamin_logger-0.4.0/lamin_logger/__init__.py
--rw-r--r--   0        0        0     2029 2023-05-27 07:28:04.621343 lamin_logger-0.4.0/lamin_logger/_core.py
--rw-r--r--   0        0        0     3662 2023-06-14 17:38:57.246704 lamin_logger-0.4.0/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     4107 2023-06-15 15:21:07.826610 lamin_logger-0.4.0/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      681 2023-01-12 04:19:23.176122 lamin_logger-0.4.0/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     2758 2023-06-15 15:21:07.826983 lamin_logger-0.4.0/lamin_logger/_search.py
--rw-r--r--   0        0        0      334 2023-06-15 15:21:07.827322 lamin_logger-0.4.0/noxfile.py
--rw-r--r--   0        0        0      966 2023-06-15 15:21:07.827588 lamin_logger-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      100 2022-07-20 12:55:43.891932 lamin_logger-0.4.0/tests/test_base.py
--rw-r--r--   0        0        0     1356 2023-06-14 17:38:57.247766 lamin_logger-0.4.0/tests/test_lookup.py
--rw-r--r--   0        0        0     2140 2023-06-15 15:21:07.827793 lamin_logger-0.4.0/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.4.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     2101 2023-06-15 15:21:07.828218 lamin_logger-0.4.0/tests/test_search.py
--rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 lamin_logger-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:58:17.266637 lamin_logger-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 18:46:24.119961 lamin_logger-0.5.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 18:46:24.120069 lamin_logger-0.5.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 18:46:24.120174 lamin_logger-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 18:19:51.176749 lamin_logger-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-08-08 17:06:33.128130 lamin_logger-0.5.0/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-20 18:49:33.932419 lamin_logger-0.5.0/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 18:46:24.120507 lamin_logger-0.5.0/docs/api.md
+-rw-r--r--   0        0        0     3008 2023-06-15 18:20:51.362236 lamin_logger-0.5.0/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-23 18:45:50.337637 lamin_logger-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     1360 2023-06-15 15:57:57.600362 lamin_logger-0.5.0/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 18:46:24.121862 lamin_logger-0.5.0/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-15 18:20:32.518412 lamin_logger-0.5.0/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 18:19:51.177212 lamin_logger-0.5.0/lamin_logger/_core.py
+-rw-r--r--   0        0        0     7572 2023-06-15 18:19:51.177336 lamin_logger-0.5.0/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     3662 2023-06-15 15:58:17.267297 lamin_logger-0.5.0/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     4107 2023-06-15 15:58:17.267398 lamin_logger-0.5.0/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 18:19:51.177576 lamin_logger-0.5.0/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     2758 2023-06-15 15:58:17.267495 lamin_logger-0.5.0/lamin_logger/_search.py
+-rw-r--r--   0        0        0      334 2023-06-15 15:58:17.267619 lamin_logger-0.5.0/noxfile.py
+-rw-r--r--   0        0        0      952 2023-06-15 18:19:51.177764 lamin_logger-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 18:19:51.177888 lamin_logger-0.5.0/tests/test_base.py
+-rw-r--r--   0        0        0     1356 2023-06-15 15:58:17.267845 lamin_logger-0.5.0/tests/test_lookup.py
+-rw-r--r--   0        0        0     2140 2023-06-15 15:58:17.267943 lamin_logger-0.5.0/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:58:17.268069 lamin_logger-0.5.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2101 2023-06-15 15:58:17.268162 lamin_logger-0.5.0/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.0/PKG-INFO
```

### Comparing `lamin_logger-0.4.0/.github/workflows/build.yml` & `lamin_logger-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/.github/workflows/latest-changes.yml` & `lamin_logger-0.5.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/.gitignore` & `lamin_logger-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/.pre-commit-config.yaml` & `lamin_logger-0.5.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - id: flake8
         additional_dependencies:
           - flake8-black==0.3.3
           - flake8-typing-imports==1.10.0
         language_version: python3
         args:
           - --max-line-length=88
-          - --ignore=E203
+          - --ignore=E203,W503,BLK100,TYP001
         exclude: |
           (?x)(
               __init__.py
           )
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.6.2
     hooks:
@@ -43,22 +43,23 @@
               docs/notes/
           )
   - repo: https://github.com/Lucas-C/pre-commit-hooks
     rev: v1.1.9
     hooks:
       - id: forbid-crlf
       - id: remove-crlf
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.8.0
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
     hooks:
       - id: isort
+        name: isort (python)
         args: ["--profile", "black"]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.940
     hooks:
       - id: mypy
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.1.1
     hooks:
       - id: pydocstyle
         args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D413
+          - --ignore=D100,D101,D102,D103,D104,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
```

### Comparing `lamin_logger-0.4.0/LICENSE` & `lamin_logger-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/docs/changelog.md` & `lamin_logger-0.5.0/docs/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 |
+✨ Remove loguru and replace with standard (Scanpy-based) logger | [18](https://github.com/laminlabs/lamin-logger/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.5.0
+🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.4.0
 🚚 Temporarily added lookup | [20](https://github.com/laminlabs/lamin-logger/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.3.4
 ✨ Added download level, changed info icon to 💬 | [19](https://github.com/laminlabs/lamin-logger/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-27 | 0.3.2
 :sparkles: Add hint level | [17](https://github.com/laminlabs/lamin-logger/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-05 | 0.3.0
 🚸 Add all botocore subloggers | [16](https://github.com/laminlabs/lamin-logger/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-02-22 | 0.3rc1
 🔇 Suppress "Found credentials..." logging in aiobotocore | [15](https://github.com/laminlabs/lamin-logger/pull/15) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-06 | 0.2.4
 🚸 Set default level to INFO | [14](https://github.com/laminlabs/lamin-logger/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-01-24 | 0.2.3
 🔥 Manually provide versions for py_version_warning | [13](https://github.com/laminlabs/lamin-logger/pull/13) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-12 | 0.2.2
```

### Comparing `lamin_logger-0.4.0/docs/quickstart.ipynb` & `lamin_logger-0.5.0/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/lamin_logger/_lookup.py` & `lamin_logger-0.5.0/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/lamin_logger/_map_synonyms.py` & `lamin_logger-0.5.0/lamin_logger/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/lamin_logger/_python_version.py` & `lamin_logger-0.5.0/lamin_logger/_python_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Raise warnings for python versions that are not tested
 import platform
 
 from packaging import version
 
-from ._core import logger
+from ._logger import logger
 
 py_version = version.parse(platform.python_version())
 
 
 def py_version_warning(min_v: str, max_v: str):
     """Print warning for python versions that are not tested in CI."""
     max_v_plus_1 = (
```

### Comparing `lamin_logger-0.4.0/lamin_logger/_search.py` & `lamin_logger-0.5.0/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/pyproject.toml` & `lamin_logger-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "loguru",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lamin-logger"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `lamin_logger-0.4.0/tests/test_lookup.py` & `lamin_logger-0.5.0/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/tests/test_map_synonyms.py` & `lamin_logger-0.5.0/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/tests/test_search.py` & `lamin_logger-0.5.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.4.0/PKG-INFO` & `lamin_logger-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.4.0
+Version: 0.5.0
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru
 Requires-Dist: pandas ; extra == "dev"
 Requires-Dist: rapidfuzz ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: nbproject_test ; extra == "dev"
```

