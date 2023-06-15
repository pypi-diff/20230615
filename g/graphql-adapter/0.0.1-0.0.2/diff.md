# Comparing `tmp/graphql_adapter-0.0.1.tar.gz` & `tmp/graphql_adapter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_adapter-0.0.1.tar", last modified: Thu Jun 15 16:59:04 2023, max compression
+gzip compressed data, was "graphql_adapter-0.0.2.tar", last modified: Thu Jun 15 17:07:15 2023, max compression
```

## Comparing `graphql_adapter-0.0.1.tar` & `graphql_adapter-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/src/graphql_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-15 16:58:54.000000 graphql_adapter-0.0.1/src/graphql_adapter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:59:04.226125 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-15 16:59:04.000000 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 16:59:04.000000 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:59:04.000000 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 16:59:04.000000 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:59:04.000000 graphql_adapter-0.0.1/src/graphql_adapter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:07:15.118761 graphql_adapter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-15 17:07:15.118761 graphql_adapter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:07:15.118761 graphql_adapter-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:07:15.114761 graphql_adapter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:07:15.114761 graphql_adapter-0.0.2/src/graphql_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-15 17:07:05.000000 graphql_adapter-0.0.2/src/graphql_adapter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:07:15.114761 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-15 17:07:15.000000 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 17:07:15.000000 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:07:15.000000 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 17:07:15.000000 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 17:07:15.000000 graphql_adapter-0.0.2/src/graphql_adapter.egg-info/top_level.txt
```

### Comparing `graphql_adapter-0.0.1/PKG-INFO` & `graphql_adapter-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: graphql_adapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: GraphQL Adapter for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
-# Graphql Adapter Module
+# GraphQL Adapter
 
 The `graphql_adapter` module is a Python package that simplifies interactions with GraphQL servers. It abstracts away some of the pain points of using Python with GraphQL by providing a streamlined, asynchronous interface for sending GraphQL queries and mutations.
 
+## Installation
+
+```
+pip install graphql-adapter
+```
+
 ## Usage
 
 The `graphql_adapter` module exports a single async function `graphql_request`.
 
 Here's an example of how to use it:
 
 ```python
@@ -30,15 +36,16 @@
 """
 
 variables = {"key1": "value1", "key2": "value2"}
 
 response = await graphql_request(
     query=query,
     variables=variables,
-    graphql_server="http://localhost:4000/graphql"
+    graphql_server="http://localhost:4000/graphql",
+    query_path="./gql"
 )
 
 print(response)
 ```
 
 ### Function Parameters
```

### Comparing `graphql_adapter-0.0.1/README.md` & `graphql_adapter-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-# Graphql Adapter Module
+# GraphQL Adapter
 
 The `graphql_adapter` module is a Python package that simplifies interactions with GraphQL servers. It abstracts away some of the pain points of using Python with GraphQL by providing a streamlined, asynchronous interface for sending GraphQL queries and mutations.
 
+## Installation
+
+```
+pip install graphql-adapter
+```
+
 ## Usage
 
 The `graphql_adapter` module exports a single async function `graphql_request`.
 
 Here's an example of how to use it:
 
 ```python
@@ -22,15 +28,16 @@
 """
 
 variables = {"key1": "value1", "key2": "value2"}
 
 response = await graphql_request(
     query=query,
     variables=variables,
-    graphql_server="http://localhost:4000/graphql"
+    graphql_server="http://localhost:4000/graphql",
+    query_path="./gql"
 )
 
 print(response)
 ```
 
 ### Function Parameters
```

### Comparing `graphql_adapter-0.0.1/setup.py` & `graphql_adapter-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="graphql_adapter",
-    version="0.0.1",
+    version="0.0.2",
     description="GraphQL Adapter for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `graphql_adapter-0.0.1/src/graphql_adapter/__init__.py` & `graphql_adapter-0.0.2/src/graphql_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_adapter-0.0.1/src/graphql_adapter.egg-info/PKG-INFO` & `graphql_adapter-0.0.2/src/graphql_adapter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: graphql-adapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: GraphQL Adapter for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
-# Graphql Adapter Module
+# GraphQL Adapter
 
 The `graphql_adapter` module is a Python package that simplifies interactions with GraphQL servers. It abstracts away some of the pain points of using Python with GraphQL by providing a streamlined, asynchronous interface for sending GraphQL queries and mutations.
 
+## Installation
+
+```
+pip install graphql-adapter
+```
+
 ## Usage
 
 The `graphql_adapter` module exports a single async function `graphql_request`.
 
 Here's an example of how to use it:
 
 ```python
@@ -30,15 +36,16 @@
 """
 
 variables = {"key1": "value1", "key2": "value2"}
 
 response = await graphql_request(
     query=query,
     variables=variables,
-    graphql_server="http://localhost:4000/graphql"
+    graphql_server="http://localhost:4000/graphql",
+    query_path="./gql"
 )
 
 print(response)
 ```
 
 ### Function Parameters
```

