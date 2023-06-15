# Comparing `tmp/lazycon-0.6.2.tar.gz` & `tmp/lazycon-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycon-0.6.2.tar", last modified: Tue Jan 24 09:52:27 2023, max compression
+gzip compressed data, was "lazycon-0.6.3.tar", last modified: Thu Jun 15 17:44:43 2023, max compression
```

## Comparing `lazycon-0.6.2.tar` & `lazycon-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:52:27.718784 lazycon-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-24 09:52:23.000000 lazycon-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-24 09:52:23.000000 lazycon-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-24 09:52:27.718784 lazycon-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-24 09:52:23.000000 lazycon-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:52:27.714784 lazycon-0.6.2/lazycon/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:52:27.718784 lazycon-0.6.2/lazycon/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/semantics/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/semantics/locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/semantics/visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/statements.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/thunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-24 09:52:23.000000 lazycon-0.6.2/lazycon/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:52:27.714784 lazycon-0.6.2/lazycon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-24 09:52:27.000000 lazycon-0.6.2/lazycon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-24 09:52:27.000000 lazycon-0.6.2/lazycon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 09:52:27.000000 lazycon-0.6.2/lazycon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-24 09:52:27.000000 lazycon-0.6.2/lazycon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-24 09:52:27.000000 lazycon-0.6.2/lazycon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-24 09:52:23.000000 lazycon-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 09:52:27.718784 lazycon-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-01-24 09:52:23.000000 lazycon-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:44:43.367850 lazycon-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-15 17:44:40.000000 lazycon-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-15 17:44:40.000000 lazycon-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-15 17:44:43.367850 lazycon-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-15 17:44:40.000000 lazycon-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:44:43.367850 lazycon-0.6.3/lazycon/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:44:43.367850 lazycon-0.6.3/lazycon/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/semantics/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/semantics/locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/semantics/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/thunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-15 17:44:40.000000 lazycon-0.6.3/lazycon/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:44:43.367850 lazycon-0.6.3/lazycon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-15 17:44:43.000000 lazycon-0.6.3/lazycon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 17:44:43.000000 lazycon-0.6.3/lazycon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:44:43.000000 lazycon-0.6.3/lazycon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 17:44:43.000000 lazycon-0.6.3/lazycon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 17:44:43.000000 lazycon-0.6.3/lazycon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-15 17:44:40.000000 lazycon-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:44:43.367850 lazycon-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-15 17:44:40.000000 lazycon-0.6.3/setup.py
```

### Comparing `lazycon-0.6.2/LICENSE` & `lazycon-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/PKG-INFO` & `lazycon-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lazycon
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easy config files in pure Python
 Home-page: https://github.com/maxme1/lazycon
-Author: maxme1
-Author-email: maxs987@gmail.com
+Author: Max
+Author-email: max@ira-labs.com
 License: MIT
-Download-URL: https://github.com/maxme1/lazycon/archive/v0.6.2.tar.gz
+Download-URL: https://github.com/maxme1/lazycon/archive/v0.6.3.tar.gz
 Keywords: config,lazy,interpreter
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lazycon-0.6.2/README.md` & `lazycon-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/console.py` & `lazycon-0.6.3/lazycon/console.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/main.py` & `lazycon-0.6.3/lazycon/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .exceptions import EntryError, ExceptionWrapper, SemanticError
 from .scope import Scope, Builtins
 from .parser import parse_file, parse_string
 from .render import ScopeEval
 from .statements import ImportConfig, Definitions
 
 PathOrStr = Union[os.PathLike, str]
+_NO_ARG = object()
 
 
 class Config:
     """
     A config interpreter.
 
     Parameters
@@ -147,17 +148,21 @@
 
     def __getitem__(self, name: str):
         try:
             return self.get(name)
         except EntryError:
             raise KeyError(f'"{name}" is not defined.') from None
 
-    def get(self, name: str):
+    def get(self, name: str, default: Any = _NO_ARG):
         try:
             return self._scope[name]
+        except EntryError:
+            if default is not _NO_ARG:
+                return default
+            raise
         except ExceptionWrapper as e:
             raise e.exception from None
 
     def eval(self, expression: str):
         """Evaluate the given `expression`."""
         try:
             return eval(expression, ScopeEval(self._scope))
```

### Comparing `lazycon-0.6.2/lazycon/parser.py` & `lazycon-0.6.3/lazycon/parser.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/render.py` & `lazycon-0.6.3/lazycon/render.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/scope.py` & `lazycon-0.6.3/lazycon/scope.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/semantics/analyzer.py` & `lazycon-0.6.3/lazycon/semantics/analyzer.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/semantics/locals.py` & `lazycon-0.6.3/lazycon/semantics/locals.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/semantics/visitor.py` & `lazycon-0.6.3/lazycon/semantics/visitor.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/statements.py` & `lazycon-0.6.3/lazycon/statements.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/thunk.py` & `lazycon-0.6.3/lazycon/thunk.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon/visitor.py` & `lazycon-0.6.3/lazycon/visitor.py`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/lazycon.egg-info/PKG-INFO` & `lazycon-0.6.3/lazycon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lazycon
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easy config files in pure Python
 Home-page: https://github.com/maxme1/lazycon
-Author: maxme1
-Author-email: maxs987@gmail.com
+Author: Max
+Author-email: max@ira-labs.com
 License: MIT
-Download-URL: https://github.com/maxme1/lazycon/archive/v0.6.2.tar.gz
+Download-URL: https://github.com/maxme1/lazycon/archive/v0.6.3.tar.gz
 Keywords: config,lazy,interpreter
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lazycon-0.6.2/lazycon.egg-info/SOURCES.txt` & `lazycon-0.6.3/lazycon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazycon-0.6.2/setup.py` & `lazycon-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     name=name,
     packages=find_packages(include=(name,)),
     include_package_data=True,
     version=version,
     description='Easy config files in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author='maxme1',
-    author_email='maxs987@gmail.com',
+    author='Max',
+    author_email='max@ira-labs.com',
     license='MIT',
     url='https://github.com/maxme1/lazycon',
     download_url='https://github.com/maxme1/lazycon/archive/v%s.tar.gz' % version,
     keywords=['config', 'lazy', 'interpreter'],
     classifiers=classifiers,
     install_requires=[],
     python_requires='>=3.6',
```

