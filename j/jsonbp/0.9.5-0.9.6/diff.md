# Comparing `tmp/jsonbp-0.9.5.tar.gz` & `tmp/jsonbp-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonbp-0.9.5.tar", last modified: Wed Jun 14 18:57:28 2023, max compression
+gzip compressed data, was "jsonbp-0.9.6.tar", last modified: Thu Jun 15 18:04:57 2023, max compression
```

## Comparing `jsonbp-0.9.5.tar` & `jsonbp-0.9.6.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-14 18:57:28.834683 jsonbp-0.9.5/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1074 2023-04-09 11:39:57.000000 jsonbp-0.9.5/LICENSE.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     6190 2023-06-14 18:57:28.834683 jsonbp-0.9.5/PKG-INFO
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     5597 2023-06-13 11:11:15.000000 jsonbp-0.9.5/README.rst
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-14 18:57:28.831350 jsonbp-0.9.5/jsonbp/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      572 2023-06-14 15:22:43.000000 jsonbp-0.9.5/jsonbp/__init__.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      962 2023-06-14 14:57:07.000000 jsonbp-0.9.5/jsonbp/array.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11522 2023-06-14 15:29:46.000000 jsonbp-0.9.5/jsonbp/blueprint.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      330 2023-06-14 14:59:34.000000 jsonbp-0.9.5/jsonbp/declaration.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     2917 2023-06-14 15:44:07.000000 jsonbp-0.9.5/jsonbp/error.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      479 2023-06-14 15:14:44.000000 jsonbp-0.9.5/jsonbp/error_type.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)       42 2023-06-14 14:57:24.000000 jsonbp-0.9.5/jsonbp/exception.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      354 2023-06-14 15:10:48.000000 jsonbp-0.9.5/jsonbp/field.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)       35 2023-06-14 15:10:41.000000 jsonbp-0.9.5/jsonbp/field_type.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11118 2023-06-14 18:12:56.000000 jsonbp-0.9.5/jsonbp/parser.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-14 18:57:28.834683 jsonbp-0.9.5/jsonbp/ply/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      116 2023-04-09 11:39:57.000000 jsonbp-0.9.5/jsonbp/ply/__init__.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    35241 2023-04-09 11:39:57.000000 jsonbp-0.9.5/jsonbp/ply/lex.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    98438 2023-04-09 11:39:57.000000 jsonbp-0.9.5/jsonbp/ply/yacc.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      669 2023-04-09 11:39:57.000000 jsonbp-0.9.5/jsonbp/types.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-14 18:57:28.834683 jsonbp-0.9.5/jsonbp.egg-info/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     6190 2023-06-14 18:57:28.000000 jsonbp-0.9.5/jsonbp.egg-info/PKG-INFO
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      525 2023-06-14 18:57:28.000000 jsonbp-0.9.5/jsonbp.egg-info/SOURCES.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)        1 2023-06-14 18:57:28.000000 jsonbp-0.9.5/jsonbp.egg-info/dependency_links.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)        7 2023-06-14 18:57:28.000000 jsonbp-0.9.5/jsonbp.egg-info/top_level.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      708 2023-06-14 18:57:17.000000 jsonbp-0.9.5/pyproject.toml
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)       38 2023-06-14 18:57:28.834683 jsonbp-0.9.5/setup.cfg
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-14 18:57:28.834683 jsonbp-0.9.5/tests/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      358 2023-06-14 17:27:30.000000 jsonbp-0.9.5/tests/test_caching.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     4215 2023-06-14 16:11:40.000000 jsonbp-0.9.5/tests/test_deserialization.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      512 2023-06-14 15:30:42.000000 jsonbp-0.9.5/tests/test_error_fallbacks.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1102 2023-04-09 11:39:57.000000 jsonbp-0.9.5/tests/test_parsing.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.062062 jsonbp-0.9.6/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1074 2023-04-09 11:39:57.000000 jsonbp-0.9.6/LICENSE.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       36 2023-06-15 16:37:44.000000 jsonbp-0.9.6/MANIFEST.in
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     6190 2023-06-15 18:04:57.062062 jsonbp-0.9.6/PKG-INFO
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     5597 2023-06-13 11:11:15.000000 jsonbp-0.9.6/README.md
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.058728 jsonbp-0.9.6/jsonbp/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      572 2023-06-14 15:22:43.000000 jsonbp-0.9.6/jsonbp/__init__.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      962 2023-06-14 14:57:07.000000 jsonbp-0.9.6/jsonbp/array.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11522 2023-06-14 15:29:46.000000 jsonbp-0.9.6/jsonbp/blueprint.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      330 2023-06-14 14:59:34.000000 jsonbp-0.9.6/jsonbp/declaration.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     2917 2023-06-15 15:42:36.000000 jsonbp-0.9.6/jsonbp/error.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      479 2023-06-14 15:14:44.000000 jsonbp-0.9.6/jsonbp/error_type.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       42 2023-06-14 14:57:24.000000 jsonbp-0.9.6/jsonbp/exception.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      354 2023-06-14 15:10:48.000000 jsonbp-0.9.6/jsonbp/field.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       35 2023-06-14 15:10:41.000000 jsonbp-0.9.6/jsonbp/field_type.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.058728 jsonbp-0.9.6/jsonbp/localization/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      862 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/localization/messages.en_US.ini
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      964 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/localization/messages.pt_BR.ini
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11139 2023-06-15 18:00:28.000000 jsonbp-0.9.6/jsonbp/parser.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.062062 jsonbp-0.9.6/jsonbp/ply/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      116 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/ply/__init__.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    35241 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/ply/lex.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    98438 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/ply/yacc.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      669 2023-04-09 11:39:57.000000 jsonbp-0.9.6/jsonbp/types.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.058728 jsonbp-0.9.6/jsonbp.egg-info/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     6190 2023-06-15 18:04:57.000000 jsonbp-0.9.6/jsonbp.egg-info/PKG-INFO
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      614 2023-06-15 18:04:57.000000 jsonbp-0.9.6/jsonbp.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)        1 2023-06-15 18:04:57.000000 jsonbp-0.9.6/jsonbp.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)        7 2023-06-15 18:04:57.000000 jsonbp-0.9.6/jsonbp.egg-info/top_level.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      707 2023-06-15 18:03:26.000000 jsonbp-0.9.6/pyproject.toml
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       38 2023-06-15 18:04:57.062062 jsonbp-0.9.6/setup.cfg
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2023-06-15 18:04:57.062062 jsonbp-0.9.6/tests/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      358 2023-06-15 16:47:16.000000 jsonbp-0.9.6/tests/test_caching.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     4215 2023-06-15 16:47:21.000000 jsonbp-0.9.6/tests/test_deserialization.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      512 2023-06-14 15:30:42.000000 jsonbp-0.9.6/tests/test_error_fallbacks.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1102 2023-06-15 18:01:54.000000 jsonbp-0.9.6/tests/test_parsing.py
```

### Comparing `jsonbp-0.9.5/LICENSE.txt` & `jsonbp-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/PKG-INFO` & `jsonbp-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonbp
-Version: 0.9.5
+Version: 0.9.6
 Summary: JSON Python Deserializer
 Author-email: Gustavo Venturini <gustavo.c.venturini@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vottini/jsonbp
 Keywords: JSON,deserialization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsonbp-0.9.5/README.rst` & `jsonbp-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/__init__.py` & `jsonbp-0.9.6/jsonbp/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/array.py` & `jsonbp-0.9.6/jsonbp/array.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/blueprint.py` & `jsonbp-0.9.6/jsonbp/blueprint.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/error.py` & `jsonbp-0.9.6/jsonbp/error.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/parser.py` & `jsonbp-0.9.6/jsonbp/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,19 +142,19 @@
 def p_include(p):
 	'''
 		include : INCLUDE STRING
 	'''
 
 	inclusionFile = p[2]
 	inclusionPath = os.path.join(currentPath, inclusionFile)
-	pushEnv(); loadedBlueprint = load(inclusionPath); popEnv()
+	pushEnv()
 
-	if None == loadedBlueprint:
-		msg = f'Unable to open file "{inclusionFile}"'
-		raise SchemaViolation(msg)
+	try: loadedBlueprint = load(inclusionPath)
+	except SchemaViolation as e: raise SchemaViolation(e)
+	finally: popEnv()
 
 	for typeName in loadedBlueprint.collectTypes():
 		if typeExists(typeName, excluded=loadedBlueprint.collectSources()):
 			msg = f"Error including '{inclusionFile}': type '{typeName}' already defined"
 			raise SchemaViolation(msg)
 
 	blueprint.includes.append(loadedBlueprint)
@@ -500,15 +500,16 @@
 		return _loadedFiles[abspath]
 
 	try:
 		with open(filepath, "r") as fd:
 			contents = fd.read()
 
 	except FileNotFoundError:
-		return None
+		msg = f'Unable to open file "{filepath}"'
+		raise SchemaViolation(msg)
 
 	return loads(contents,
 		os.path.dirname(filepath),
 		os.path.basename(filepath))
 
 	
 def loads(contents, contentPath='.', contentName=None):
```

### Comparing `jsonbp-0.9.5/jsonbp/ply/lex.py` & `jsonbp-0.9.6/jsonbp/ply/lex.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/ply/yacc.py` & `jsonbp-0.9.6/jsonbp/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp/types.py` & `jsonbp-0.9.6/jsonbp/types.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/jsonbp.egg-info/PKG-INFO` & `jsonbp-0.9.6/jsonbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonbp
-Version: 0.9.5
+Version: 0.9.6
 Summary: JSON Python Deserializer
 Author-email: Gustavo Venturini <gustavo.c.venturini@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/vottini/jsonbp
 Keywords: JSON,deserialization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsonbp-0.9.5/tests/test_deserialization.py` & `jsonbp-0.9.6/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/tests/test_error_fallbacks.py` & `jsonbp-0.9.6/tests/test_error_fallbacks.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.5/tests/test_parsing.py` & `jsonbp-0.9.6/tests/test_parsing.py`

 * *Files identical despite different names*

