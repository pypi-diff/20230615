# Comparing `tmp/teamsgraphapi-0.0.3.tar.gz` & `tmp/teamsgraphapi-0.0.4.tar.gz`

## Comparing `teamsgraphapi-0.0.3.tar` & `teamsgraphapi-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/auth.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/graph.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/LICENCE
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/graphapi/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/graphapi/auth.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/graphapi/graph.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/LICENCE
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.4/PKG-INFO
```

### Comparing `teamsgraphapi-0.0.3/graphapi/graph.py` & `teamsgraphapi-0.0.4/graphapi/graph.py`

 * *Files identical despite different names*

### Comparing `teamsgraphapi-0.0.3/LICENCE` & `teamsgraphapi-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `teamsgraphapi-0.0.3/README.md` & `teamsgraphapi-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django) ![Bower](https://img.shields.io/bower/l/graph)  
 ## Installation
 
   
 
-TeamsGraphApi requires [python](https://nodejs.org/) 3.6+ to run.
+TeamsGraphApi requires [python](https://www.python.org/) 3.6+ to run.
 
   
 
 You can install GQL with all the optional dependencies using pip:
 
 ```sh
 pip install TeamsGraphApi
```

### Comparing `teamsgraphapi-0.0.3/pyproject.toml` & `teamsgraphapi-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "TeamsGraphApi"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ajay Vishwakarma", email="ajay.vishwakarma@codiant.com" },
 ]
 description = "wrapper for micorsoft teams graph api's"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `teamsgraphapi-0.0.3/PKG-INFO` & `teamsgraphapi-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TeamsGraphApi
-Version: 0.0.3
+Version: 0.0.4
 Summary: wrapper for micorsoft teams graph api's
 Project-URL: Homepage, https://github.com/Ajay7415/graphapi
 Project-URL: Bug Tracker, https://github.com/Ajay7415/graphapi/issues
 Author-email: Ajay Vishwakarma <ajay.vishwakarma@codiant.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
   
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django) ![Bower](https://img.shields.io/bower/l/graph)  
 ## Installation
 
   
 
-TeamsGraphApi requires [python](https://nodejs.org/) 3.6+ to run.
+TeamsGraphApi requires [python](https://www.python.org/) 3.6+ to run.
 
   
 
 You can install GQL with all the optional dependencies using pip:
 
 ```sh
 pip install TeamsGraphApi
```

