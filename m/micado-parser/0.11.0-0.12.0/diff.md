# Comparing `tmp/micado-parser-0.11.0.tar.gz` & `tmp/micado-parser-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micado-parser-0.11.0.tar", last modified: Wed Feb  8 17:36:03 2023, max compression
+gzip compressed data, was "micado-parser-0.12.0.tar", last modified: Thu Jun 15 11:57:14 2023, max compression
```

## Comparing `micado-parser-0.11.0.tar` & `micado-parser-0.12.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:36:03.406911 micado-parser-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 17:35:53.000000 micado-parser-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-08 17:36:03.406911 micado-parser-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-02-08 17:35:53.000000 micado-parser-0.11.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:36:03.406911 micado-parser-0.11.0/micado_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-08 17:36:03.000000 micado-parser-0.11.0/micado_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:36:03.406911 micado-parser-0.11.0/micadoparser/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:36:03.406911 micado-parser-0.11.0/micadoparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/utils/csar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/utils/tosca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/utils/yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4592 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/validations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-02-08 17:35:53.000000 micado-parser-0.11.0/micadoparser/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 17:36:03.406911 micado-parser-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-08 17:35:53.000000 micado-parser-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 17:36:03.406911 micado-parser-0.11.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1589 2023-02-08 17:35:53.000000 micado-parser-0.11.0/tests/test_micado_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2944 2023-02-08 17:35:53.000000 micado-parser-0.11.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:57:14.780898 micado-parser-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 11:57:01.000000 micado-parser-0.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-15 11:57:14.780898 micado-parser-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-15 11:57:01.000000 micado-parser-0.12.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:57:14.776898 micado-parser-0.12.0/micado_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 11:57:14.000000 micado-parser-0.12.0/micado_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:57:14.776898 micado-parser-0.12.0/micadoparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:57:14.780898 micado-parser-0.12.0/micadoparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/utils/csar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/utils/tosca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/utils/yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4592 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/validations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-06-15 11:57:01.000000 micado-parser-0.12.0/micadoparser/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:57:14.780898 micado-parser-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-15 11:57:01.000000 micado-parser-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:57:14.780898 micado-parser-0.12.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1589 2023-06-15 11:57:01.000000 micado-parser-0.12.0/tests/test_micado_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2944 2023-06-15 11:57:01.000000 micado-parser-0.12.0/tests/test_validator.py
```

### Comparing `micado-parser-0.11.0/LICENSE` & `micado-parser-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/PKG-INFO` & `micado-parser-0.12.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-parser
-Version: 0.11.0
+Version: 0.12.0
 Summary: Parse MiCADO ADTs for the MiCADO Submitter
 Home-page: https://github.com/micado-scale/micado-parser
 Author: Jay DesLauriers
 Author-email: j.deslauriers@westminster.ac.uk
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `micado-parser-0.11.0/README.md` & `micado-parser-0.12.0/README.md`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micado_parser.egg-info/PKG-INFO` & `micado-parser-0.12.0/micado_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micado-parser
-Version: 0.11.0
+Version: 0.12.0
 Summary: Parse MiCADO ADTs for the MiCADO Submitter
 Home-page: https://github.com/micado-scale/micado-parser
 Author: Jay DesLauriers
 Author-email: j.deslauriers@westminster.ac.uk
 Project-URL: Bug Tracker, https://github.com/micado-scale/micado-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `micado-parser-0.11.0/micado_parser.egg-info/SOURCES.txt` & `micado-parser-0.12.0/micado_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/cli.py` & `micado-parser-0.12.0/micadoparser/cli.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/exceptions.py` & `micado-parser-0.12.0/micadoparser/exceptions.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/parser.py` & `micado-parser-0.12.0/micadoparser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,23 +76,23 @@
         raise ValidationError(error, "TOSCA Parser could not parse the ADT...")
 
     return template
 
 
 def _find_other_inputs(template):
     """Find `get_input` tags in the template, then resolve and update"""
-    resolve_get_functions(
-        template.tpl,
-        "get_input",
-        lambda x: x is not None,
-        _get_input_value,
-        template,
-    )
-    # Update nodetemplate properties
     for node in template.nodetemplates:
+        resolve_get_functions(
+            node.entity_tpl,
+            "get_input",
+            lambda x: x is not None,
+            _get_input_value,
+            template,
+        )
+        # Update nodetemplate properties
         node._properties = node._create_properties()
 
 
 def _get_input_value(key, template):
     """Custom get_input resolution using parsed_params"""
     try:
         return template.parsed_params[key]
```

### Comparing `micado-parser-0.11.0/micadoparser/utils/csar.py` & `micado-parser-0.12.0/micadoparser/utils/csar.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/utils/tosca.py` & `micado-parser-0.12.0/micadoparser/utils/tosca.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/utils/utils.py` & `micado-parser-0.12.0/micadoparser/utils/utils.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/utils/yaml.py` & `micado-parser-0.12.0/micadoparser/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/validations.py` & `micado-parser-0.12.0/micadoparser/validations.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/micadoparser/validator.py` & `micado-parser-0.12.0/micadoparser/validator.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/setup.py` & `micado-parser-0.12.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="micado-parser",
-    version="0.11.0",
+    version="0.12.0",
     author="Jay DesLauriers",
     author_email="j.deslauriers@westminster.ac.uk",
     description="Parse MiCADO ADTs for the MiCADO Submitter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/micado-scale/micado-parser",
     project_urls={
```

### Comparing `micado-parser-0.11.0/tests/test_micado_parser.py` & `micado-parser-0.12.0/tests/test_micado_parser.py`

 * *Files identical despite different names*

### Comparing `micado-parser-0.11.0/tests/test_validator.py` & `micado-parser-0.12.0/tests/test_validator.py`

 * *Files identical despite different names*

