# Comparing `tmp/dagster-shell-0.9.9.tar.gz` & `tmp/dagster-shell-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-shell-0.9.9.tar", last modified: Thu Sep 17 21:27:21 2020, max compression
+gzip compressed data, was "dist/dagster-shell-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:53 2020, max compression
```

## Comparing `dagster-shell-0.9.9.tar` & `dagster-shell-0.9.9rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      569 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell/
--rw-r--r--   0 bobchen    (501) staff       (20)      329 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7450 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6050 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      569 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      673 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/dagster_shell_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      404 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)      184 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/example_shell_command_solid.py
--rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/example_shell_script_solid.py
--rw-r--r--   0 bobchen    (501) staff       (20)      479 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/test_examples.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3350 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2769 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/dagster_shell_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:21.000000 dagster-shell-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:24:45.000000 dagster-shell-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      572 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell/
+-rw-r--r--   0 bobchen    (501) staff       (20)      329 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7450 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6050 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      572 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      673 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      404 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      184 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/example_shell_command_solid.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/example_shell_script_solid.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      479 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_examples.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3350 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2769 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/setup.py
```

### Comparing `dagster-shell-0.9.9/LICENSE` & `dagster-shell-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/PKG-INFO` & `dagster-shell-0.9.9rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-shell
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Dagster shell solids.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-shell
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-shell-0.9.9/dagster_shell/solids.py` & `dagster-shell-0.9.9rc1/dagster_shell/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/dagster_shell/utils.py` & `dagster-shell-0.9.9rc1/dagster_shell/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/dagster_shell.egg-info/PKG-INFO` & `dagster-shell-0.9.9rc1/dagster_shell.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-shell
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Dagster shell solids.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-shell
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-shell-0.9.9/dagster_shell.egg-info/SOURCES.txt` & `dagster-shell-0.9.9rc1/dagster_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/dagster_shell_tests/test_solids.py` & `dagster-shell-0.9.9rc1/dagster_shell_tests/test_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/dagster_shell_tests/test_utils.py` & `dagster-shell-0.9.9rc1/dagster_shell_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9/setup.py` & `dagster-shell-0.9.9rc1/setup.py`

 * *Files identical despite different names*

