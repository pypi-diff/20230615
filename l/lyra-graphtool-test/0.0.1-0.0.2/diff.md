# Comparing `tmp/lyra_graphtool_test-0.0.1.tar.gz` & `tmp/lyra_graphtool_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyra_graphtool_test-0.0.1.tar", max compression
+gzip compressed data, was "lyra_graphtool_test-0.0.2.tar", max compression
```

## Comparing `lyra_graphtool_test-0.0.1.tar` & `lyra_graphtool_test-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      585 2023-06-15 01:06:44.352750 lyra_graphtool_test-0.0.1/LICENSE
--rw-r--r--   0        0        0      463 2023-06-15 01:06:44.352750 lyra_graphtool_test-0.0.1/README.md
--rw-r--r--   0        0        0     1307 2023-06-15 01:07:15.536541 lyra_graphtool_test-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      387 2023-06-15 01:07:15.536541 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/__init__.py
--rw-r--r--   0        0        0    30403 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/configuration.py
--rw-r--r--   0        0        0     2141 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/edge.py
--rw-r--r--   0        0        0    26563 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/graph.py
--rw-r--r--   0        0        0    27641 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/parameters.py
--rw-r--r--   0        0        0     5833 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/utils.py
--rw-r--r--   0        0        0     2944 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/vertex.py
--rw-r--r--   0        0        0     2699 2023-06-15 01:06:44.356750 lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/worker.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      585 2023-06-15 01:21:10.420142 lyra_graphtool_test-0.0.2/LICENSE
+-rw-r--r--   0        0        0      463 2023-06-15 01:21:10.420142 lyra_graphtool_test-0.0.2/README.md
+-rw-r--r--   0        0        0     1388 2023-06-15 01:21:43.096943 lyra_graphtool_test-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      387 2023-06-15 01:21:43.096943 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/__init__.py
+-rw-r--r--   0        0        0    30403 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/configuration.py
+-rw-r--r--   0        0        0     2141 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/edge.py
+-rw-r--r--   0        0        0    26563 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/graph.py
+-rw-r--r--   0        0        0    27641 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/parameters.py
+-rw-r--r--   0        0        0     5833 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/utils.py
+-rw-r--r--   0        0        0     2944 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/vertex.py
+-rw-r--r--   0        0        0     2699 2023-06-15 01:21:10.424142 lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/worker.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 lyra_graphtool_test-0.0.2/PKG-INFO
```

### Comparing `lyra_graphtool_test-0.0.1/LICENSE` & `lyra_graphtool_test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/pyproject.toml` & `lyra_graphtool_test-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [tool.poetry]
 name = "lyra_graphtool_test"
-version = "0.0.1"
+version = "0.0.2"
 description = "Lyra Graphtool"
 authors = ["Studio X, LLC"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.24.3"
 matplotlib = "^3.7.1"
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.group.build.dependencies]
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+python-semantic-release = "^7.34.3"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
 sphinx-rtd-theme = "^1.2.2"
 nbsphinx = "^0.9.2"
 pygments = "^2.15.1"
 myst-nb = "^0.17.2"
 jupyter = "^1.0.0"
 nbconvert = "^7.5.0"
-pytest = "^7.3.2"
-pytest-cov = "^4.1.0"
-python-semantic-release = "^7.34.3"
 
 [tool.semantic_release]
 version_variable = [
     "src/lyra_graphtool_test/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"                             # branch to make releases of
```

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/configuration.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/configuration.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/edge.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/edge.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/graph.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/graph.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/parameters.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/parameters.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/utils.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/utils.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/vertex.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/vertex.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/src/lyra_graphtool_test/worker.py` & `lyra_graphtool_test-0.0.2/src/lyra_graphtool_test/worker.py`

 * *Files identical despite different names*

### Comparing `lyra_graphtool_test-0.0.1/PKG-INFO` & `lyra_graphtool_test-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyra-graphtool-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lyra Graphtool
 License: Apache-2.0
 Author: Studio X, LLC
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

