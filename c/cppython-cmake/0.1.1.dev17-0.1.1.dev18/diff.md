# Comparing `tmp/cppython-cmake-0.1.1.dev17.tar.gz` & `tmp/cppython-cmake-0.1.1.dev18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-cmake-0.1.1.dev17.tar", last modified: Tue Jun 13 10:26:33 2023, max compression
+gzip compressed data, was "cppython-cmake-0.1.1.dev18.tar", last modified: Thu Jun 15 07:59:10 2023, max compression
```

## Comparing `cppython-cmake-0.1.1.dev17.tar` & `cppython-cmake-0.1.1.dev18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/LICENSE.md
--rw-r--r--   0        0        0       93 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/README.md
--rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/__init__.py
--rw-r--r--   0        0        0     3485 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/builder.py
--rw-r--r--   0        0        0     2286 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/plugin.py
--rw-r--r--   0        0        0        0 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/py.typed
--rw-r--r--   0        0        0      856 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/resolution.py
--rw-r--r--   0        0        0     3516 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/schema.py
--rw-r--r--   0        0        0     2351 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/pyproject.toml
--rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/data/default/CMakePresets.json
--rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/integration/__init__.py
--rw-r--r--   0        0        0      849 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/integration/test_generator.py
--rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/unit/__init__.py
--rw-r--r--   0        0        0     4793 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/unit/test_generator.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev17/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/LICENSE.md
+-rw-r--r--   0        0        0       93 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/README.md
+-rw-r--r--   0        0        0        3 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/__init__.py
+-rw-r--r--   0        0        0     3485 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/builder.py
+-rw-r--r--   0        0        0     2286 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/py.typed
+-rw-r--r--   0        0        0      856 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/resolution.py
+-rw-r--r--   0        0        0     3516 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/cppython_cmake/schema.py
+-rw-r--r--   0        0        0     2351 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/data/default/CMakePresets.json
+-rw-r--r--   0        0        0        3 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/integration/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/integration/test_generator.py
+-rw-r--r--   0        0        0        3 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4793 2023-06-15 07:58:42.256232 cppython-cmake-0.1.1.dev18/tests/unit/test_generator.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev18/PKG-INFO
```

### Comparing `cppython-cmake-0.1.1.dev17/LICENSE.md` & `cppython-cmake-0.1.1.dev18/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/cppython_cmake/builder.py` & `cppython-cmake-0.1.1.dev18/cppython_cmake/builder.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/cppython_cmake/plugin.py` & `cppython-cmake-0.1.1.dev18/cppython_cmake/plugin.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/cppython_cmake/resolution.py` & `cppython-cmake-0.1.1.dev18/cppython_cmake/resolution.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/cppython_cmake/schema.py` & `cppython-cmake-0.1.1.dev18/cppython_cmake/schema.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/pyproject.toml` & `cppython-cmake-0.1.1.dev18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.11"
 dependencies = [
     "cppython-core>=0.3.3.dev0",
     "cmake>=3.24.1",
 ]
-version = "0.1.1.dev17"
+version = "0.1.1.dev18"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
```

### Comparing `cppython-cmake-0.1.1.dev17/tests/integration/test_generator.py` & `cppython-cmake-0.1.1.dev18/tests/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/tests/unit/test_generator.py` & `cppython-cmake-0.1.1.dev18/tests/unit/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev17/PKG-INFO` & `cppython-cmake-0.1.1.dev18/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cppython-cmake
-Version: 0.1.1.dev17
+Version: 0.1.1.dev18
 Summary: A plugin for CPPython that enables a CMake generator for C++ projects
 License: MIT
 Author-email: Synodic Software <contact@synodic.software>
 Requires-Python: >=3.11
 Project-URL: homepage, https://github.com/Synodic-Software/CPPython-CMake
 Project-URL: repository, https://github.com/Synodic-Software/CPPython-CMake
 Description-Content-Type: text/markdown
```

