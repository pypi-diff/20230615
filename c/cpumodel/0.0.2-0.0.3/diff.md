# Comparing `tmp/cpumodel-0.0.2.tar.gz` & `tmp/cpumodel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpumodel-0.0.2.tar", max compression
+gzip compressed data, was "cpumodel-0.0.3.tar", max compression
```

## Comparing `cpumodel-0.0.2.tar` & `cpumodel-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4521 2023-06-15 11:41:57.719245 cpumodel-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/__main__.py
--rw-r--r--   0        0        0     2078 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/amd.py
--rw-r--r--   0        0        0     3371 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/cpumodel.py
--rw-r--r--   0        0        0     5506 2023-06-15 11:41:57.719245 cpumodel-0.0.2/cpumodel/intel.py
--rw-r--r--   0        0        0      455 2023-06-15 11:42:21.788808 cpumodel-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5023 1970-01-01 00:00:00.000000 cpumodel-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4521 2023-06-15 14:54:01.497478 cpumodel-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 14:54:01.497478 cpumodel-0.0.3/cpumodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:54:01.497478 cpumodel-0.0.3/cpumodel/__main__.py
+-rw-r--r--   0        0        0     2078 2023-06-15 14:54:01.497478 cpumodel-0.0.3/cpumodel/amd.py
+-rw-r--r--   0        0        0     3376 2023-06-15 14:54:01.497478 cpumodel-0.0.3/cpumodel/cpumodel.py
+-rw-r--r--   0        0        0     5506 2023-06-15 14:54:01.497478 cpumodel-0.0.3/cpumodel/intel.py
+-rw-r--r--   0        0        0      455 2023-06-15 14:54:18.901082 cpumodel-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5023 1970-01-01 00:00:00.000000 cpumodel-0.0.3/PKG-INFO
```

### Comparing `cpumodel-0.0.2/README.md` & `cpumodel-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cpumodel-0.0.2/cpumodel/amd.py` & `cpumodel-0.0.3/cpumodel/amd.py`

 * *Files identical despite different names*

### Comparing `cpumodel-0.0.2/cpumodel/cpumodel.py` & `cpumodel-0.0.3/cpumodel/cpumodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             dd[k] = type(v)(drop_nones(vv) if isinstance(vv, dict) else vv
                             for vv in v)
         elif v is not None:
             dd[k] = v
     return dd
 
 
-def get_cpu_model(cpustring):
+def get_cpu_model(cpustring=None):
     """
     Get info about the CPU model and return it as a dict
     """
 
     if cpustring:
         # Use supplied CPU string
         cpuinfo = {}
```

### Comparing `cpumodel-0.0.2/cpumodel/intel.py` & `cpumodel-0.0.3/cpumodel/intel.py`

 * *Files identical despite different names*

### Comparing `cpumodel-0.0.2/PKG-INFO` & `cpumodel-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpumodel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get info about your CPU
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

