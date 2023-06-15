# Comparing `tmp/dojo_truant-2023.6.13.3.tar.gz` & `tmp/dojo_truant-2023.6.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.13.3.tar", last modified: Wed Jun 14 07:20:30 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.15.1.tar", last modified: Thu Jun 15 19:10:10 2023, max compression
```

## Comparing `dojo_truant-2023.6.13.3.tar` & `dojo_truant-2023.6.15.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/jira_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/jira_product_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 07:20:30.000000 dojo_truant-2023.6.13.3/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 07:20:16.000000 dojo_truant-2023.6.13.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:20:30.938764 dojo_truant-2023.6.13.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 19:10:10.000000 dojo_truant-2023.6.15.1/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 19:09:52.000000 dojo_truant-2023.6.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:10:10.166813 dojo_truant-2023.6.15.1/setup.cfg
```

### Comparing `dojo_truant-2023.6.13.3/LICENSE.txt` & `dojo_truant-2023.6.15.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/PKG-INFO` & `dojo_truant-2023.6.15.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.13.3
+Version: 2023.6.15.1
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.3/dojo/__init__.py` & `dojo_truant-2023.6.15.1/dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/api.py` & `dojo_truant-2023.6.15.1/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/development_environment.py` & `dojo_truant-2023.6.15.1/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/dojo_group.py` & `dojo_truant-2023.6.15.1/dojo/dojo_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import requests
 
 import dojo
 
 
 class Dojo_Group(dojo.DAPI):
-    _endpoint = string.Template("/api/v2/dojo_groups/{id}/")
+    _endpoint = string.Template("/api/v2/dojo_groups/${id}/")
     _post_endpoint = "/api/v2/dojo_groups/"
     _search_endpoint = "/api/v2/dojo_groups/"
 
     _model_validation = {"configuration_permissions": {"type": list,
                                                        "required": False},
                          "name": {"type": str},
                          "description": {"type": str,
```

### Comparing `dojo_truant-2023.6.13.3/dojo/engagement.py` & `dojo_truant-2023.6.15.1/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/finding.py` & `dojo_truant-2023.6.15.1/dojo/finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/jira_instance.py` & `dojo_truant-2023.6.15.1/dojo/jira_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import requests
 
 import dojo
 
 
 class Jira_Instance(dojo.DAPI):
-    _endpoint = string.Template("/api/v2/jira_instances/{id}/")
+    _endpoint = string.Template("/api/v2/jira_instances/${id}/")
     _post_endpoint = "/api/v2/jira_instances/"
     _search_endpoint = "/api/v2/jira_instances/"
 
     _model_validation = {"configuration_name": {"type": str,
                                                 "required": True},
                          "url": {"type": str},
                          "username": {"type": str,
```

### Comparing `dojo_truant-2023.6.13.3/dojo/jira_product_configuration.py` & `dojo_truant-2023.6.15.1/dojo/jira_product_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import requests
 
 import dojo
 
 
 class Jira_Product_Configuration(dojo.DAPI):
-    _endpoint = string.Template("/api/v2/jira_product_configurations/{id}/")
+    _endpoint = string.Template("/api/v2/jira_product_configurations/${id}/")
     _post_endpoint = "/api/v2/jira_product_configurations/"
     _search_endpoint = "/api/v2/jira_product_configurations/"
 
     _model_validation = {"project_key": {"type": str,
                                          "required": True},
                          "issue_template_dir": {"type": str,
                                                 "required": False},
```

### Comparing `dojo_truant-2023.6.13.3/dojo/product.py` & `dojo_truant-2023.6.15.1/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/product_type.py` & `dojo_truant-2023.6.15.1/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/stub_finding.py` & `dojo_truant-2023.6.15.1/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/test.py` & `dojo_truant-2023.6.15.1/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/test_type.py` & `dojo_truant-2023.6.15.1/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo/write_chain.py` & `dojo_truant-2023.6.15.1/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.13.3/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.15.1/dojo_truant.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.13.3
+Version: 2023.6.15.1
 Summary: A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.13.3/pyproject.toml` & `dojo_truant-2023.6.15.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.13.3"
+version = "2023.6.15.1"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Most functionality should be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

