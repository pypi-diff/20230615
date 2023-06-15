# Comparing `tmp/swaggerspect-0.0.2.tar.gz` & `tmp/swaggerspect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swaggerspect-0.0.2.tar", last modified: Thu Jun 15 09:14:27 2023, max compression
+gzip compressed data, was "dist/swaggerspect-0.0.3.tar", last modified: Thu Jun 15 13:56:13 2023, max compression
```

## Comparing `swaggerspect-0.0.2.tar` & `swaggerspect-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 09:14:27.537283 swaggerspect-0.0.2/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.2/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      322 2023-06-15 09:14:27.537283 swaggerspect-0.0.2/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1498 2023-06-15 07:56:31.000000 swaggerspect-0.0.2/README.md
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-15 09:14:27.537283 swaggerspect-0.0.2/setup.cfg
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      513 2023-06-15 09:14:08.000000 swaggerspect-0.0.2/setup.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 09:14:27.537283 swaggerspect-0.0.2/swaggerspect/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     9465 2023-06-15 09:04:00.000000 swaggerspect-0.0.2/swaggerspect/__init__.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 09:14:27.537283 swaggerspect-0.0.2/swaggerspect.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      322 2023-06-15 09:14:27.000000 swaggerspect-0.0.2/swaggerspect.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      230 2023-06-15 09:14:27.000000 swaggerspect-0.0.2/swaggerspect.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-15 09:14:27.000000 swaggerspect-0.0.2/swaggerspect.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        9 2023-06-15 09:14:27.000000 swaggerspect-0.0.2/swaggerspect.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-06-15 09:14:27.000000 swaggerspect-0.0.2/swaggerspect.egg-info/top_level.txt
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      513 2023-06-15 13:55:40.000000 swaggerspect-0.0.3/setup.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.3/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/setup.cfg
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    10488 2023-06-15 13:02:50.000000 swaggerspect-0.0.3/swaggerspect/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 12:42:58.000000 swaggerspect-0.0.3/swaggerspect/test.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        9 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      251 2023-06-15 13:56:13.000000 swaggerspect-0.0.3/swaggerspect.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1498 2023-06-15 07:56:31.000000 swaggerspect-0.0.3/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `swaggerspect-0.0.2/LICENSE` & `swaggerspect-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swaggerspect-0.0.2/README.md` & `swaggerspect-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `swaggerspect-0.0.2/setup.py` & `swaggerspect-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name='swaggerspect',
-    version='0.0.2',
+    version='0.0.3',
     description='',
     long_description="""Introspects python classes and functions and generates swagger style documentation objects.""",
     long_description_content_type="text/markdown",
     author='Egil Moeller',
     author_email='em@emrld.no',
     url='https://github.com/emerald-geomodelling/swaggerspect',
     packages=setuptools.find_packages(),
```

### Comparing `swaggerspect-0.0.2/swaggerspect/__init__.py` & `swaggerspect-0.0.3/swaggerspect/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,57 +2,77 @@
 import numpydoc.docscrape
 import ast
 import typing
 import importlib.metadata
 
 def _get_name(obj):
     if obj is None: return None
+    if obj is typing.Any: return 'typing.Any'
     return obj.__module__ + "." + obj.__name__
 
 typemap = {
     'builtins.str': 'string',
     'builtins.int': 'integer',
     'builtins.float': 'number',
     'builtins.bool': 'boolean',
     'builtins.list': 'array',
+    'builtins.dict': 'object',
+    'typing.Any': None,
     'tuple': 'array',
     'str': 'string',
     'int': 'integer',
     'float': 'number',
     'bool': 'boolean',
     'list': 'array',
-    'tuple': 'array'
+    'tuple': 'array',
+    'dict': 'object'
 }
 
 def typeof(v):
     if v is None: return None
     if v is inspect._empty: return None
     return type(v)
 
 def make_type_schema(*typenames):
     for typename in typenames:
-        orig = typename
+        orig = repr(typename)
         if typename is inspect._empty:
             continue
         if typename is None:
             continue
-        schema = {}
+        args = None
+        metadatas = None
         if not isinstance(typename, str):
             if isinstance(typename, typing._AnnotatedAlias):
-                for metadata in typename.__metadata__:
-                    schema.update({key[len("swaggerspect_"):]: getattr(metadata, key)
-                                   for key in dir(metadata) if key.startswith("swaggerspect_")})
+                metadatas = typename.__metadata__
                 typename = typename.__args__[0]
             args = typing.get_args(typename)
             typename = _get_name(typename)
-        schema["type"] = typemap.get(typename, "object")
-        schema["x-python-type"] = typename
-        #schema["x-python-orig"] = repr(orig)
-        if schema["type"] == "array" and args:
-            schema["items"] = make_type_schema(args[0])
+
+        pytypename = typename
+        typename = typemap.get(typename, "object")
+
+        schema = {}
+        if typename is not None:
+            schema["type"] = typename
+            schema["x-python-type"] = pytypename
+            #schema["x-python-orig"] = orig
+            if schema["type"] == "array" and args:
+                schema["items"] = make_type_schema(args[0])
+            elif schema["type"] == "object" and args:
+                schema["propertyNames"] = make_type_schema(args[0])
+                schema["patternProperties"] = make_type_schema(args[1])
+
+        if metadatas:
+           for metadata in metadatas:
+               schema.update({key[len("swaggerspect_"):]: getattr(metadata, key)
+                              for key in dir(metadata) if key.startswith("swaggerspect_")})
+               if hasattr(metadata, "json_schema"):
+                   schema.update(metadata.json_schema)
+            
         return schema
     return {}
 
 def make_value_schema(*values):
     for value in values:
         if value is inspect._empty:
             continue
@@ -243,19 +263,19 @@
     {"function.name": {"argname1": "value1", ... "argnameN": "valueN"}}
 
     or if multi is True (the default), a list of function calls each
     serialized as above.
     """
     if not api: return {}
     schema = {
-        "description": api["info"]["description"],
         "anyOf": [
             {
                 "type": "object",
-                "title": step["operationId"],
+                "title": step["operationId"].split(".")[-1],
+                "required": [step["operationId"]],
                 "additionalProperties": False,
                 "properties": {
                     step["operationId"]: {
                         "type": "object",
                         "additionalProperties": False,
                         "properties": {
                             parameter["name"]: merge(
@@ -269,8 +289,18 @@
                 }
             }
             for step in [path["get"] for path in api["paths"].values()]
         ]
     }
     if multi:
         schema = {"type": "array", "items": schema}
+    schema["description"] = api["info"]["description"]
     return schema
+
+class JsonSchema(object):
+    """Type annotation that accepts any type (like typing.Any), but
+    outputs the supplied JSON Schema in swaggerspect.
+    """    
+    def __new__(cls, schema):
+        self = object.__new__(cls)
+        self.json_schema = schema
+        return typing.Annotated[typing.Any, self]
```

