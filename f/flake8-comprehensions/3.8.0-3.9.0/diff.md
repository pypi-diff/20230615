# Comparing `tmp/flake8-comprehensions-3.8.0.tar.gz` & `tmp/flake8-comprehensions-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-comprehensions-3.8.0.tar", last modified: Mon Jan 10 17:10:02 2022, max compression
+gzip compressed data, was "flake8-comprehensions-3.9.0.tar", last modified: Wed May 11 10:09:30 2022, max compression
```

## Comparing `flake8-comprehensions-3.8.0.tar` & `flake8-comprehensions-3.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 17:10:02.063850 flake8-comprehensions-3.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     6723 2022-01-10 17:09:54.000000 flake8-comprehensions-3.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1074 2021-02-07 15:14:01.000000 flake8-comprehensions-3.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      245 2021-12-28 23:44:35.000000 flake8-comprehensions-3.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     8157 2022-01-10 17:10:02.064036 flake8-comprehensions-3.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     7019 2022-01-10 16:13:38.000000 flake8-comprehensions-3.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      584 2022-01-10 16:13:38.000000 flake8-comprehensions-3.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1449 2022-01-10 17:10:02.064737 flake8-comprehensions-3.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 15:14:01.000000 flake8-comprehensions-3.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 17:10:02.059023 flake8-comprehensions-3.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 17:10:02.061505 flake8-comprehensions-3.8.0/src/flake8_comprehensions/
--rw-r--r--   0 chainz     (501) staff       (20)    11216 2021-08-16 08:19:35.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-13 11:12:09.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 17:10:02.063512 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     8157 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      493 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       68 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-01-10 17:10:01.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       66 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       22 2022-01-10 17:10:02.000000 flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:09:30.114614 flake8-comprehensions-3.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     6786 2022-05-11 10:09:20.000000 flake8-comprehensions-3.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:28:19.000000 flake8-comprehensions-3.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:11.000000 flake8-comprehensions-3.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     8188 2022-05-11 10:09:30.114796 flake8-comprehensions-3.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     7019 2022-05-11 10:05:38.000000 flake8-comprehensions-3.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      635 2022-01-19 11:13:56.000000 flake8-comprehensions-3.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1466 2022-05-11 10:09:30.115869 flake8-comprehensions-3.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:56.000000 flake8-comprehensions-3.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:09:30.108265 flake8-comprehensions-3.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:09:30.112095 flake8-comprehensions-3.9.0/src/flake8_comprehensions/
+-rw-r--r--   0 chainz     (501) staff       (20)    11226 2022-01-19 11:13:56.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-13 11:12:09.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 10:09:30.114313 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     8188 2022-05-11 10:09:29.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      493 2022-05-11 10:09:30.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 10:09:29.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       67 2022-05-11 10:09:29.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/entry_points.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 10:09:28.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       66 2022-05-11 10:09:29.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       22 2022-05-11 10:09:30.000000 flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/top_level.txt
```

### Comparing `flake8-comprehensions-3.8.0/HISTORY.rst` & `flake8-comprehensions-3.9.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+3.9.0 (2022-05-11)
+------------------
+
+* Support Python 3.11.
+
 3.8.0 (2022-01-10)
 ------------------
 
 * Drop Python 3.6 support.
 
 * Remove upper bound on Flake8 version.
```

### Comparing `flake8-comprehensions-3.8.0/LICENSE` & `flake8-comprehensions-3.9.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2021 Adam Johnson
+Copyright (c) 2017 Adam Johnson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `flake8-comprehensions-3.8.0/PKG-INFO` & `flake8-comprehensions-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: flake8-comprehensions
-Version: 3.8.0
+Version: 3.9.0
 Summary: A flake8 plugin to help you write better list/set/dict comprehensions.
 Home-page: https://github.com/adamchainz/flake8-comprehensions
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-comprehensions/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8,comprehensions,list comprehension,set comprehension,dict comprehension
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====================
 flake8-comprehensions
 =====================
@@ -43,15 +43,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write better list/set/dict comprehensions.
 
 Requirements
 ============
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
@@ -182,9 +182,7 @@
 
 It's unnecessary to use a list comprehension if the elements are unchanged.
 The iterable should be wrapped in ``list()`` or ``set()`` instead.
 For example:
 
 * Rewrite ``[x for x in iterable]`` as ``list(iterable)``
 * Rewrite ``{x for x in iterable}`` as ``set(iterable)``
-
-
```

### Comparing `flake8-comprehensions-3.8.0/README.rst` & `flake8-comprehensions-3.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write better list/set/dict comprehensions.
 
 Requirements
 ============
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
```

### Comparing `flake8-comprehensions-3.8.0/pyproject.toml` & `flake8-comprehensions-3.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 target-version = ['py37']
 
 [tool.isort]
 profile = "black"
+add_imports = "from __future__ import annotations"
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 mypy_path = "src/"
```

### Comparing `flake8-comprehensions-3.8.0/setup.cfg` & `flake8-comprehensions-3.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-comprehensions
-version = 3.8.0
+version = 3.9.0
 description = A flake8 plugin to help you write better list/set/dict comprehensions.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/flake8-comprehensions
 project_urls = 
@@ -20,15 +20,15 @@
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-license_file = LICENSE
+	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires =
```

### Comparing `flake8-comprehensions-3.8.0/src/flake8_comprehensions/__init__.py` & `flake8-comprehensions-3.9.0/src/flake8_comprehensions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import ast
 import sys
-from typing import Any, Generator, Optional, Tuple, Type
+from typing import Any, Generator
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import version
 else:
     from importlib_metadata import version
 
 
@@ -37,15 +39,15 @@
         "C411": "C411 Unnecessary list call - remove the outer call to list().",
         "C413": "C413 Unnecessary {outer} call around {inner}(){remediation}.",
         "C414": "C414 Unnecessary {inner} call within {outer}().",
         "C415": "C415 Unnecessary subscript reversal of iterable within {func}().",
         "C416": "C416 Unnecessary {type} comprehension - rewrite using {type}().",
     }
 
-    def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
+    def run(self) -> Generator[tuple[int, int, str, type[Any]], None, None]:
         for node in ast.walk(self.tree):
             if isinstance(node, ast.Call) and isinstance(node.func, ast.Name):
                 num_positional_args = len(node.args)
                 num_keyword_args = len(node.keywords)
 
                 if (
                     num_positional_args == 1
@@ -161,15 +163,15 @@
                     and num_positional_args > 0
                     and isinstance(node.args[0], ast.Call)
                     and isinstance(node.args[0].func, ast.Name)
                     and node.args[0].func.id == "sorted"
                 ):
                     remediation = ""
                     if node.func.id == "reversed":
-                        reverse_flag_value: Optional[bool] = False
+                        reverse_flag_value: bool | None = False
                         for keyword in node.args[0].keywords:
                             if keyword.arg != "reverse":
                                 continue
                             if isinstance(keyword.value, ast.NameConstant):
                                 reverse_flag_value = keyword.value.value
                             elif isinstance(keyword.value, ast.Num):
                                 reverse_flag_value = bool(keyword.value.n)
```

### Comparing `flake8-comprehensions-3.8.0/src/flake8_comprehensions.egg-info/PKG-INFO` & `flake8-comprehensions-3.9.0/src/flake8_comprehensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: flake8-comprehensions
-Version: 3.8.0
+Version: 3.9.0
 Summary: A flake8 plugin to help you write better list/set/dict comprehensions.
 Home-page: https://github.com/adamchainz/flake8-comprehensions
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-comprehensions/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: flake8,comprehensions,list comprehension,set comprehension,dict comprehension
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====================
 flake8-comprehensions
 =====================
@@ -43,15 +43,15 @@
    :alt: pre-commit
 
 A `flake8 <https://flake8.readthedocs.io/en/latest/index.html>`_ plugin that helps you write better list/set/dict comprehensions.
 
 Requirements
 ============
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 Installation
 ============
 
 First, install with ``pip``:
 
 .. code-block:: sh
@@ -182,9 +182,7 @@
 
 It's unnecessary to use a list comprehension if the elements are unchanged.
 The iterable should be wrapped in ``list()`` or ``set()`` instead.
 For example:
 
 * Rewrite ``[x for x in iterable]`` as ``list(iterable)``
 * Rewrite ``{x for x in iterable}`` as ``set(iterable)``
-
-
```

