# Comparing `tmp/shell_interface-0.10.0.tar.gz` & `tmp/shell_interface-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_interface-0.10.0.tar", max compression
+gzip compressed data, was "shell_interface-0.9.0.tar", max compression
```

## Comparing `shell_interface-0.10.0.tar` & `shell_interface-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35106 2023-06-15 09:18:53.630323 shell_interface-0.10.0/LICENSE
--rw-r--r--   0        0        0     1198 2023-06-15 10:35:44.834898 shell_interface-0.10.0/pyproject.toml
--rw-r--r--   0        0        0      363 2023-06-15 10:35:20.354849 shell_interface-0.10.0/src/shell_interface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 09:30:30.916346 shell_interface-0.10.0/src/shell_interface/py.typed
--rw-r--r--   0        0        0     1851 2023-06-15 09:30:30.916346 shell_interface-0.10.0/src/shell_interface/shell_interface.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 shell_interface-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0    35106 2023-06-15 09:18:53.630323 shell_interface-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1197 2023-06-15 10:28:46.770111 shell_interface-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-06-15 10:21:50.909541 shell_interface-0.9.0/src/shell_interface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:30:30.916346 shell_interface-0.9.0/src/shell_interface/py.typed
+-rw-r--r--   0        0        0     1851 2023-06-15 09:30:30.916346 shell_interface-0.9.0/src/shell_interface/shell_interface.py
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 shell_interface-0.9.0/PKG-INFO
```

### Comparing `shell_interface-0.10.0/LICENSE` & `shell_interface-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_interface-0.10.0/pyproject.toml` & `shell_interface-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-interface"
-version = "0.10.0"
+version = "0.9.0"
 description = "Helpful and convenient utilities to interact with UNIX shells"
 authors = ["Max Görner <max@familie-goerner.eu>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 loguru = "^0.7.0"
```

### Comparing `shell_interface-0.10.0/src/shell_interface/shell_interface.py` & `shell_interface-0.9.0/src/shell_interface/shell_interface.py`

 * *Files identical despite different names*

### Comparing `shell_interface-0.10.0/PKG-INFO` & `shell_interface-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-interface
-Version: 0.10.0
+Version: 0.9.0
 Summary: Helpful and convenient utilities to interact with UNIX shells
 License: GPL-3.0-or-later
 Author: Max Görner
 Author-email: max@familie-goerner.eu
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

