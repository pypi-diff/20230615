# Comparing `tmp/crispy-parser-1.0.1.tar.gz` & `tmp/crispy-parser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispy-parser-1.0.1.tar", last modified: Wed Jun 14 18:35:57 2023, max compression
+gzip compressed data, was "crispy-parser-1.1.0.tar", last modified: Thu Jun 15 03:13:59 2023, max compression
```

## Comparing `crispy-parser-1.0.1.tar` & `crispy-parser-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/crispy.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/duplicate_name_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/missing_value_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/no_arguments_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_add_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_crispy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_parse_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_parse_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_show_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/tests/test_try_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/crispy/unexpected_argument_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/crispy_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 18:35:57.000000 crispy-parser-1.0.1/crispy_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:35:57.633542 crispy-parser-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-14 18:35:49.000000 crispy-parser-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/crispy/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/crispy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/duplicate_name_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/missing_value_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/no_arguments_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/crispy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_add_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_crispy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_parse_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_show_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/tests/test_try_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/crispy/unexpected_argument_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/crispy_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-15 03:13:59.000000 crispy-parser-1.1.0/crispy_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 03:13:59.000000 crispy-parser-1.1.0/crispy_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:13:59.000000 crispy-parser-1.1.0/crispy_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:13:59.000000 crispy-parser-1.1.0/crispy_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 03:13:59.177361 crispy-parser-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 03:13:52.000000 crispy-parser-1.1.0/setup.py
```

### Comparing `crispy-parser-1.0.1/LICENSE` & `crispy-parser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/PKG-INFO` & `crispy-parser-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: crispy-parser
-Version: 1.0.1
+Version: 1.1.0
 Summary: Crispy is a simple command line argument parser, ready to be integrated to any project of any size!
 Home-page: https://github.com/fybx/crispy
 Author: F. Y. BALABAN, <fybalaban@fybx.dev>
 Author-email: fybalaban@fybx.dev
 License: GNU LGPL-v2.1
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## crispy [![Test crispy](https://github.com/fybx/crispy/actions/workflows/flow-test_crispy.yml/badge.svg?branch=main)](https://github.com/fybx/crispy/actions/workflows/flow-test_crispy.yml) [![Upload Python Package](https://github.com/fybx/crispy/actions/workflows/flow-publish_package.yml/badge.svg?branch=main)](https://github.com/fybx/crispy/actions/workflows/flow-publish_package.yml)
 
 `crispy` is my take on parsing command-line arguments. It is a dead simple tool that allows you to define your own keys for systematically gathering variables.
```

### Comparing `crispy-parser-1.0.1/README.md` & `crispy-parser-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_add_variable.py` & `crispy-parser-1.1.0/crispy/tests/test_add_variable.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_crispy.py` & `crispy-parser-1.1.0/crispy/tests/test_crispy.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_parse_arguments.py` & `crispy-parser-1.1.0/crispy/tests/test_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_parse_string.py` & `crispy-parser-1.1.0/crispy/tests/test_parse_string.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_show_keys.py` & `crispy-parser-1.1.0/crispy/tests/test_show_keys.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy/tests/test_try_parse.py` & `crispy-parser-1.1.0/crispy/tests/test_try_parse.py`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/crispy_parser.egg-info/PKG-INFO` & `crispy-parser-1.1.0/crispy_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: crispy-parser
-Version: 1.0.1
+Version: 1.1.0
 Summary: Crispy is a simple command line argument parser, ready to be integrated to any project of any size!
 Home-page: https://github.com/fybx/crispy
 Author: F. Y. BALABAN, <fybalaban@fybx.dev>
 Author-email: fybalaban@fybx.dev
 License: GNU LGPL-v2.1
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## crispy [![Test crispy](https://github.com/fybx/crispy/actions/workflows/flow-test_crispy.yml/badge.svg?branch=main)](https://github.com/fybx/crispy/actions/workflows/flow-test_crispy.yml) [![Upload Python Package](https://github.com/fybx/crispy/actions/workflows/flow-publish_package.yml/badge.svg?branch=main)](https://github.com/fybx/crispy/actions/workflows/flow-publish_package.yml)
 
 `crispy` is my take on parsing command-line arguments. It is a dead simple tool that allows you to define your own keys for systematically gathering variables.
```

### Comparing `crispy-parser-1.0.1/crispy_parser.egg-info/SOURCES.txt` & `crispy-parser-1.1.0/crispy_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crispy-parser-1.0.1/setup.py` & `crispy-parser-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
     f.close()
 
 setup(
     name='crispy-parser',
-    version='1.0.1',
+    version='1.1.0',
     packages=['crispy', 'crispy.tests'],
     url='https://github.com/fybx/crispy',
     license='GNU LGPL-v2.1',
     author='F. Y. BALABAN, <fybalaban@fybx.dev>',
     author_email='fybalaban@fybx.dev',
     description='Crispy is a simple command line argument parser, ready to be integrated to any project of any size!',
     long_description=readme,
     long_description_content_type='text/markdown',
-    python_requires=">=3.10"
+    python_requires=">=3.7"
 )
```

