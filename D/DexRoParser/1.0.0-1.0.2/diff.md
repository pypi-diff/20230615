# Comparing `tmp/DexRoParser-1.0.0.tar.gz` & `tmp/DexRoParser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DexRoParser-1.0.0.tar", last modified: Wed Jun 14 23:32:24 2023, max compression
+gzip compressed data, was "DexRoParser-1.0.2.tar", last modified: Wed Jun 14 23:55:37 2023, max compression
```

## Comparing `DexRoParser-1.0.0.tar` & `DexRoParser-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:32:24.716515 DexRoParser-1.0.0/
--rw-r--r--   0 ericfloyd   (501) staff       (20)     1066 2023-06-14 23:29:04.000000 DexRoParser-1.0.0/LICENSE
--rw-r--r--   0 ericfloyd   (501) staff       (20)      652 2023-06-14 23:32:24.715603 DexRoParser-1.0.0/PKG-INFO
--rw-r--r--   0 ericfloyd   (501) staff       (20)      108 2023-06-14 23:29:04.000000 DexRoParser-1.0.0/README.md
--rw-r--r--   0 ericfloyd   (501) staff       (20)      641 2023-06-14 23:30:38.000000 DexRoParser-1.0.0/pyproject.toml
--rw-r--r--   0 ericfloyd   (501) staff       (20)       38 2023-06-14 23:32:24.717003 DexRoParser-1.0.0/setup.cfg
-drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:32:24.710055 DexRoParser-1.0.0/src/
-drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:32:24.712183 DexRoParser-1.0.0/src/DexRoParser/
--rw-r--r--   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:30:07.000000 DexRoParser-1.0.0/src/DexRoParser/__init__.py
--rw-r--r--   0 ericfloyd   (501) staff       (20)    15583 2023-06-14 23:29:04.000000 DexRoParser-1.0.0/src/DexRoParser/parser.py
-drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:32:24.714610 DexRoParser-1.0.0/src/DexRoParser.egg-info/
--rw-r--r--   0 ericfloyd   (501) staff       (20)      652 2023-06-14 23:32:24.000000 DexRoParser-1.0.0/src/DexRoParser.egg-info/PKG-INFO
--rw-r--r--   0 ericfloyd   (501) staff       (20)      242 2023-06-14 23:32:24.000000 DexRoParser-1.0.0/src/DexRoParser.egg-info/SOURCES.txt
--rw-r--r--   0 ericfloyd   (501) staff       (20)        1 2023-06-14 23:32:24.000000 DexRoParser-1.0.0/src/DexRoParser.egg-info/dependency_links.txt
--rw-r--r--   0 ericfloyd   (501) staff       (20)       12 2023-06-14 23:32:24.000000 DexRoParser-1.0.0/src/DexRoParser.egg-info/top_level.txt
+drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:55:37.047656 DexRoParser-1.0.2/
+-rw-r--r--   0 ericfloyd   (501) staff       (20)     1066 2023-06-14 23:29:04.000000 DexRoParser-1.0.2/LICENSE
+-rw-r--r--   0 ericfloyd   (501) staff       (20)      652 2023-06-14 23:55:37.047315 DexRoParser-1.0.2/PKG-INFO
+-rw-r--r--   0 ericfloyd   (501) staff       (20)      108 2023-06-14 23:29:04.000000 DexRoParser-1.0.2/README.md
+-rw-r--r--   0 ericfloyd   (501) staff       (20)      641 2023-06-14 23:53:56.000000 DexRoParser-1.0.2/pyproject.toml
+-rw-r--r--   0 ericfloyd   (501) staff       (20)       38 2023-06-14 23:55:37.047769 DexRoParser-1.0.2/setup.cfg
+drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:55:37.043385 DexRoParser-1.0.2/src/
+drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:55:37.045320 DexRoParser-1.0.2/src/DexRoParser/
+-rw-r--r--   0 ericfloyd   (501) staff       (20)       68 2023-06-14 23:42:44.000000 DexRoParser-1.0.2/src/DexRoParser/__init__.py
+-rw-r--r--   0 ericfloyd   (501) staff       (20)    15583 2023-06-14 23:29:04.000000 DexRoParser-1.0.2/src/DexRoParser/parser.py
+drwxr-xr-x   0 ericfloyd   (501) staff       (20)        0 2023-06-14 23:55:37.046861 DexRoParser-1.0.2/src/DexRoParser.egg-info/
+-rw-r--r--   0 ericfloyd   (501) staff       (20)      652 2023-06-14 23:55:37.000000 DexRoParser-1.0.2/src/DexRoParser.egg-info/PKG-INFO
+-rw-r--r--   0 ericfloyd   (501) staff       (20)      242 2023-06-14 23:55:37.000000 DexRoParser-1.0.2/src/DexRoParser.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfloyd   (501) staff       (20)        1 2023-06-14 23:55:37.000000 DexRoParser-1.0.2/src/DexRoParser.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfloyd   (501) staff       (20)       12 2023-06-14 23:55:37.000000 DexRoParser-1.0.2/src/DexRoParser.egg-info/top_level.txt
```

### Comparing `DexRoParser-1.0.0/LICENSE` & `DexRoParser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DexRoParser-1.0.0/PKG-INFO` & `DexRoParser-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DexRoParser
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python package to parse Dexonline.ro (romanian dictionary site). Provides detailed descriptions of words.
 Author-email: Eric Floyd <erixefb@gmail.com>
 Project-URL: Homepage, https://github.com/Bodhi2011/DexParser/tree/main
 Project-URL: Bug Tracker, https://github.com/Bodhi2011/DexParser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `DexRoParser-1.0.0/src/DexRoParser/parser.py` & `DexRoParser-1.0.2/src/DexRoParser/parser.py`

 * *Files identical despite different names*

### Comparing `DexRoParser-1.0.0/src/DexRoParser.egg-info/PKG-INFO` & `DexRoParser-1.0.2/src/DexRoParser.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DexRoParser
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python package to parse Dexonline.ro (romanian dictionary site). Provides detailed descriptions of words.
 Author-email: Eric Floyd <erixefb@gmail.com>
 Project-URL: Homepage, https://github.com/Bodhi2011/DexParser/tree/main
 Project-URL: Bug Tracker, https://github.com/Bodhi2011/DexParser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

