# Comparing `tmp/lyra_graphtool_test-0.0.3.tar.gz` & `tmp/lyra_graphtool_test-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyra_graphtool_test-0.0.3.tar", max compression
+gzip compressed data, was "lyra_graphtool_test-0.0.4.tar", max compression
```

## Comparing `lyra_graphtool_test-0.0.3.tar` & `lyra_graphtool_test-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      585 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/LICENSE
--rw-r--r--   0        0        0      463 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/README.md
--rw-r--r--   0        0        0     1388 2023-06-15 01:46:27.998173 lyra_graphtool_test-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      387 2023-06-15 01:46:27.998173 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/__init__.py
--rw-r--r--   0        0        0    30403 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/configuration.py
--rw-r--r--   0        0        0     2141 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/edge.py
--rw-r--r--   0        0        0    26563 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/graph.py
--rw-r--r--   0        0        0    27641 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/parameters.py
--rw-r--r--   0        0        0     5833 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/utils.py
--rw-r--r--   0        0        0     2944 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/vertex.py
--rw-r--r--   0        0        0     2699 2023-06-15 01:46:03.269596 lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/worker.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2023-06-15 01:51:39.632105 lyra_graphtool_test-0.0.4/LICENSE
+-rw-r--r--   0        0        0      463 2023-06-15 01:51:39.632105 lyra_graphtool_test-0.0.4/README.md
+-rw-r--r--   0        0        0     1388 2023-06-15 01:52:22.063896 lyra_graphtool_test-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      387 2023-06-15 01:52:22.063896 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/__init__.py
+-rw-r--r--   0        0        0    30403 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/configuration.py
+-rw-r--r--   0        0        0     2141 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/edge.py
+-rw-r--r--   0        0        0    26563 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/graph.py
+-rw-r--r--   0        0        0    27641 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/parameters.py
+-rw-r--r--   0        0        0     5833 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/utils.py
+-rw-r--r--   0        0        0     2944 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/vertex.py
+-rw-r--r--   0        0        0     2699 2023-06-15 01:51:39.636105 lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/worker.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.0.4/PKG-INFO
```

### Comparing `lyra_graphtool_test-0.0.3/LICENSE` & `lyra_graphtool_test-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/pyproject.toml` & `lyra_graphtool_test-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyra_graphtool_test"
-version = "0.0.3"
+version = "0.0.4"
 description = "Lyra Graphtool"
 authors = ["Studio X, LLC"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/configuration.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/configuration.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/edge.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/edge.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/graph.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/graph.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/parameters.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/parameters.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/utils.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/utils.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/vertex.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/vertex.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/src/lyra_graphtool_test/worker.py` & `lyra_graphtool_test-0.0.4/src/lyra_graphtool_test/worker.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.3/PKG-INFO` & `lyra_graphtool_test-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyra-graphtool-test
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lyra Graphtool
 License: Apache-2.0
 Author: Studio X, LLC
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

