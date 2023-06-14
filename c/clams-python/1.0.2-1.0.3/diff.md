# Comparing `tmp/clams-python-1.0.2.tar.gz` & `tmp/clams-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.0.2.tar", last modified: Fri Jun  2 02:42:07 2023, max compression
+gzip compressed data, was "clams-python-1.0.3.tar", last modified: Wed Jun 14 22:29:53 2023, max compression
```

## Comparing `clams-python-1.0.2.tar` & `clams-python-1.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-06-02 02:41:33.000000 clams-python-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 02:41:33.000000 clams-python-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-02 02:42:07.957961 clams-python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-02 02:41:33.000000 clams-python-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 02:41:33.000000 clams-python-1.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.949961 clams-python-1.0.2/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/README.md.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-02 02:41:33.000000 clams-python-1.0.2/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.953961 clams-python-1.0.2/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 02:42:07.000000 clams-python-1.0.2/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 02:41:33.000000 clams-python-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:42:07.957961 clams-python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-02 02:41:33.000000 clams-python-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:42:07.957961 clams-python-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-06-02 02:41:33.000000 clams-python-1.0.2/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-02 02:41:33.000000 clams-python-1.0.2/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-06-14 22:29:22.000000 clams-python-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 22:29:22.000000 clams-python-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-14 22:29:53.870197 clams-python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-14 22:29:22.000000 clams-python-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 22:29:23.000000 clams-python-1.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.862196 clams-python-1.0.3/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/README.md.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-14 22:29:22.000000 clams-python-1.0.3/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.866196 clams-python-1.0.3/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 22:29:53.000000 clams-python-1.0.3/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 22:29:22.000000 clams-python-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:29:53.870197 clams-python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-14 22:29:22.000000 clams-python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:29:53.870197 clams-python-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-06-14 22:29:22.000000 clams-python-1.0.3/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-14 22:29:22.000000 clams-python-1.0.3/tests/test_clamscli.py
```

### Comparing `clams-python-1.0.2/LICENSE` & `clams-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/PKG-INFO` & `clams-python-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.2/README.md` & `clams-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/__init__.py` & `clams-python-1.0.3/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/app/__init__.py` & `clams-python-1.0.3/clams/app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         :param runtime_params: key-value pairs of runtime parameters
         :return: a copy of parameter map, with default values added
         :raises ValueError: when a value for a required parameter is not found in the input
         """
         conf = {}
         for parameter in self.metadata.parameters:
             if parameter.name in runtime_params:
-                conf[parameter.name] = str(runtime_params[parameter.name])
+                conf[parameter.name] = runtime_params[parameter.name]
             elif parameter.default is not None:
                 conf[parameter.name] = parameter.default
             else:
                 raise ValueError(f"Cannot find configuration for a required parameter \"{parameter.name}\".")
         return conf
 
     def sign_view(self, view: View, runtime_conf: Optional[dict] = None) -> None:
```

### Comparing `clams-python-1.0.2/clams/appmetadata/__init__.py` & `clams-python-1.0.3/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/__init__.py` & `clams-python-1.0.3/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/app/.gitignore.template` & `clams-python-1.0.3/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/app/Containerfile.template` & `clams-python-1.0.3/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/app/README.md.template` & `clams-python-1.0.3/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/app/app.py.template` & `clams-python-1.0.3/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/app/metadata.py.template` & `clams-python-1.0.3/clams/develop/templates/app/metadata.py.template`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The purpose of this file is to define the metadata of the app with minimal imports. 
 
 DO NOT CHANGE the name of the file
 """
 
 from mmif import DocumentTypes, AnnotationTypes
 
+from clams.app import ClamsApp
 from clams.appmetadata import AppMetadata
 
 
 # DO NOT CHANGE the function name 
 def appmetadata() -> AppMetadata:
     """
     Function to set app-metadata values and return it as an ``AppMetadata`` obj.
@@ -47,8 +48,11 @@
     # CHANGE this line and make sure return the compiled `metadata` instance
     return None
 
 
 # DO NOT CHANGE the main block
 if __name__ == '__main__':
     import sys
+    metadata = appmetadata()
+    for param in ClamsApp.universal_parameters:
+        metadata.add_parameter(**param)
     sys.stdout.write(appmetadata().jsonify(pretty=True))
```

### Comparing `clams-python-1.0.2/clams/develop/templates/gha/README.md.template` & `clams-python-1.0.3/clams/develop/templates/gha/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.0.3/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/restify/__init__.py` & `clams-python-1.0.3/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams/source/__init__.py` & `clams-python-1.0.3/clams/source/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.3/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.0.2/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.3/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/setup.py` & `clams-python-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/tests/test_clamsapp.py` & `clams-python-1.0.3/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.0.2/tests/test_clamscli.py` & `clams-python-1.0.3/tests/test_clamscli.py`

 * *Files identical despite different names*

