# Comparing `tmp/flake8-tidy-imports-4.8.0.tar.gz` & `tmp/flake8_tidy_imports-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-tidy-imports-4.8.0.tar", last modified: Wed May 11 11:13:38 2022, max compression
+gzip compressed data, was "flake8_tidy_imports-4.9.0.tar", last modified: Thu Jun 15 14:24:50 2023, max compression
```

## Comparing `flake8-tidy-imports-4.8.0.tar` & `flake8_tidy_imports-4.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 11:13:38.569510 flake8-tidy-imports-4.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     4313 2022-05-11 11:13:30.000000 flake8-tidy-imports-4.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:27.000000 flake8-tidy-imports-4.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:13.000000 flake8-tidy-imports-4.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     6510 2022-05-11 11:13:38.569655 flake8-tidy-imports-4.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     5423 2022-05-11 11:11:25.000000 flake8-tidy-imports-4.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:13:57.000000 flake8-tidy-imports-4.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1366 2022-05-11 11:13:38.570595 flake8-tidy-imports-4.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:57.000000 flake8-tidy-imports-4.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 11:13:38.563082 flake8-tidy-imports-4.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 11:13:38.566749 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports/
--rw-r--r--   0 chainz     (501) staff       (20)    27834 2022-05-05 21:16:32.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-11 13:28:51.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 11:13:38.569292 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     6510 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      475 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       59 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 11:13:36.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       60 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       20 2022-05-11 11:13:38.000000 flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:50.251667 flake8_tidy_imports-4.9.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4382 2023-06-15 14:24:48.000000 flake8_tidy_imports-4.9.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:26.000000 flake8_tidy_imports-4.9.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 flake8_tidy_imports-4.9.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6669 2023-06-15 14:24:50.251727 flake8_tidy_imports-4.9.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5444 2023-06-15 14:24:45.000000 flake8_tidy_imports-4.9.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 flake8_tidy_imports-4.9.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1493 2023-06-15 14:24:50.252000 flake8_tidy_imports-4.9.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:50.248913 flake8_tidy_imports-4.9.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:50.250357 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    27884 2023-02-07 15:19:25.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:27.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:50.251210 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6669 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      502 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       59 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       60 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       20 2023-06-15 14:24:50.000000 flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:24:50.251332 flake8_tidy_imports-4.9.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    20231 2023-01-17 09:13:13.000000 flake8_tidy_imports-4.9.0/tests/test_flake8_tidy_imports.py
```

### Comparing `flake8-tidy-imports-4.8.0/HISTORY.rst` & `flake8_tidy_imports-4.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+4.9.0 (2023-06-15)
+------------------
+
+* Support Python 3.12.
 
 4.8.0 (2022-05-11)
 ------------------
 
 * Support Python 3.11.
 
 4.7.0 (2022-05-05)
```

### Comparing `flake8-tidy-imports-4.8.0/LICENSE` & `flake8_tidy_imports-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-tidy-imports-4.8.0/PKG-INFO` & `flake8_tidy_imports-4.9.0/src/flake8_tidy_imports.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: flake8-tidy-imports
-Version: 4.8.0
+Version: 4.9.0
 Summary: A flake8 plugin that helps you write tidier imports.
 Home-page: https://github.com/adamchainz/flake8-tidy-imports
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/flake8-tidy-imports/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/flake8-tidy-imports/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8_tidy_imports
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 flake8-tidy-imports
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-tidy-imports/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-tidy-imports/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-tidy-imports/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-tidy-imports.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-tidy-imports/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -43,15 +46,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write tidier imports.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

### Comparing `flake8-tidy-imports-4.8.0/README.rst` & `flake8_tidy_imports-4.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===================
 flake8-tidy-imports
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-tidy-imports/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-tidy-imports/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-tidy-imports/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-tidy-imports.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-tidy-imports/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -16,15 +16,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write tidier imports.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

### Comparing `flake8-tidy-imports-4.8.0/setup.cfg` & `flake8_tidy_imports-4.9.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 [metadata]
-name = flake8-tidy-imports
-version = 4.8.0
+name = flake8_tidy_imports
+version = 4.9.0
 description = A flake8 plugin that helps you write tidier imports.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/flake8-tidy-imports
 author = Adam Johnson
 author_email = me@adamj.eu
-url = https://github.com/adamchainz/flake8-tidy-imports
-project_urls = 
-	Changelog = https://github.com/adamchainz/flake8-tidy-imports/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
 license = MIT
-keywords = flake8_tidy_imports
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Flake8
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
-	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Typing :: Typed
+keywords = flake8_tidy_imports
+project_urls = 
+	Changelog = https://github.com/adamchainz/flake8-tidy-imports/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
-include_package_data = True
 install_requires = 
 	flake8>=3.8.0
-	importlib-metadata ; python_version < "3.8"
+	importlib-metadata;python_version < "3.8"
 python_requires = >=3.7
+include_package_data = True
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 flake8.extension =
```

### Comparing `flake8-tidy-imports-4.8.0/src/flake8_tidy_imports/__init__.py` & `flake8_tidy_imports-4.9.0/src/flake8_tidy_imports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 import ast
 import re
 import sys
-from typing import TYPE_CHECKING, Any, Generator, Pattern
+from typing import Any
+from typing import Generator
+from typing import Pattern
+from typing import TYPE_CHECKING
 
 from flake8.options.manager import OptionManager
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import version
 else:
     from importlib_metadata import version
@@ -111,38 +114,35 @@
                 yield from rule_func(node)
 
     def rule_I250(
         self, node: ast.AST
     ) -> Generator[tuple[int, int, str, type[Any]], None, None]:
         if isinstance(node, ast.Import):
             for alias in node.names:
-
                 if "." not in alias.name:
                     from_name = None
                     imported_name = alias.name
                 else:
                     from_name, imported_name = alias.name.rsplit(".", 1)
 
                 if imported_name == alias.asname:
-
                     if from_name:
                         rewritten = f"from {from_name} import {imported_name}"
                     else:
                         rewritten = f"import {imported_name}"
 
                     yield (
                         node.lineno,
                         node.col_offset,
                         self.message_I250.format(rewritten),
                         type(self),
                     )
         elif isinstance(node, ast.ImportFrom):
             for alias in node.names:
                 if alias.name == alias.asname:
-
                     rewritten = f"from {node.module} import {alias.name}"
 
                     yield (
                         node.lineno,
                         node.col_offset,
                         self.message_I250.format(rewritten),
                         type(self),
@@ -193,15 +193,14 @@
 
         # Sort from most to least specific paths.
         module_names.sort(key=len, reverse=True)
 
         warned: set[str] = set()
 
         for module_name in module_names:
-
             is_banned, msg = self._is_module_banned(module_name)
             if is_banned:
                 message = self.message_I251.format(name=module_name, msg=msg)
                 if any(mod.startswith(module_name) for mod in warned):
                     # Do not show an error for this line if we already showed
                     # a more specific error.
                     continue
```

### Comparing `flake8-tidy-imports-4.8.0/src/flake8_tidy_imports.egg-info/PKG-INFO` & `flake8_tidy_imports-4.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: flake8-tidy-imports
-Version: 4.8.0
+Name: flake8_tidy_imports
+Version: 4.9.0
 Summary: A flake8 plugin that helps you write tidier imports.
 Home-page: https://github.com/adamchainz/flake8-tidy-imports
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
-Project-URL: Changelog, https://github.com/adamchainz/flake8-tidy-imports/blob/main/HISTORY.rst
+Project-URL: Changelog, https://github.com/adamchainz/flake8-tidy-imports/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8_tidy_imports
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 flake8-tidy-imports
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/flake8-tidy-imports/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/flake8-tidy-imports/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/flake8-tidy-imports/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/flake8-tidy-imports.svg?style=for-the-badge
    :target: https://pypi.org/project/flake8-tidy-imports/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :target: https://github.com/psf/black
@@ -43,15 +46,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write tidier imports.
 
 Requirements
 ============
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

