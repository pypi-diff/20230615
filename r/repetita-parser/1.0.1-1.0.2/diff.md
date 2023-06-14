# Comparing `tmp/repetita_parser-1.0.1.tar.gz` & `tmp/repetita_parser-1.0.2.tar.gz`

## Comparing `repetita_parser-1.0.1.tar` & `repetita_parser-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/src/repetita_parser/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/src/repetita_parser/demands.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/src/repetita_parser/errors.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/src/repetita_parser/instance.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/src/repetita_parser/topology.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/paths.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/test_demands.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/test_errors.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/test_instance.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/test_topology.py
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/DeutscheTelekom.0000.demands
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/DeutscheTelekom.graph
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_edge_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_edge_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_edge_memo.graph
--rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_fields.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_header.demands
--rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_memo.demands
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_node_fields.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_node_header.graph
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/tests/data/bad/bad_node_memo.graph
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/LICENSE
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/README.md
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 repetita_parser-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/demands.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/errors.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/instance.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/src/repetita_parser/topology.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/paths.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_demands.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_errors.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_instance.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/test_topology.py
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/DeutscheTelekom.0000.demands
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/DeutscheTelekom.graph
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_edge_memo.graph
+-rw-r--r--   0        0        0    18701 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_fields.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_header.demands
+-rw-r--r--   0        0        0    18707 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_memo.demands
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_fields.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_header.graph
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/tests/data/bad/bad_node_memo.graph
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/README.md
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 repetita_parser-1.0.2/PKG-INFO
```

### Comparing `repetita_parser-1.0.1/src/repetita_parser/demands.py` & `repetita_parser-1.0.2/src/repetita_parser/demands.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/src/repetita_parser/errors.py` & `repetita_parser-1.0.2/src/repetita_parser/errors.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/src/repetita_parser/instance.py` & `repetita_parser-1.0.2/src/repetita_parser/instance.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/src/repetita_parser/topology.py` & `repetita_parser-1.0.2/src/repetita_parser/topology.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/test_demands.py` & `repetita_parser-1.0.2/tests/test_demands.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/test_topology.py` & `repetita_parser-1.0.2/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/DeutscheTelekom.0000.demands` & `repetita_parser-1.0.2/tests/data/DeutscheTelekom.0000.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/DeutscheTelekom.graph` & `repetita_parser-1.0.2/tests/data/DeutscheTelekom.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_edge_fields.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_edge_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_edge_header.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_edge_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_edge_memo.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_edge_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_fields.demands` & `repetita_parser-1.0.2/tests/data/bad/bad_fields.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_header.demands` & `repetita_parser-1.0.2/tests/data/bad/bad_header.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_memo.demands` & `repetita_parser-1.0.2/tests/data/bad/bad_memo.demands`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_node_fields.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_node_fields.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_node_header.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_node_header.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/tests/data/bad/bad_node_memo.graph` & `repetita_parser-1.0.2/tests/data/bad/bad_node_memo.graph`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/.gitignore` & `repetita_parser-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/LICENSE` & `repetita_parser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repetita_parser-1.0.1/README.md` & `repetita_parser-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # python-repetita-parser
 
 A Python parser for the data format of the [REPETITA](https://github.com/svissicchio/Repetita) framework.
 This module can parse topology and demand files either **separately** or **combine** them into problem instances.
 The data can then be accessed via native Python objects.
 
 ## Usage
-A usage example is provided in [`examples/demand-visualization`](./examples/demand-visualization).
+A usage example is provided in [`examples/demand-visualization`](https://github.com/leon-richardt/python-repetita-parser/tree/main/examples/demand-visualization).
 To try it, run the following commands:
 ```bash
 $ cd examples/demand-visualization
 $ python -m venv env && source env/bin/activate
 $ pip install -r requirements.txt
 $ python demand_visualization.py data/DeutscheTelekom.{graph,0000.demands}
 ```
```

### Comparing `repetita_parser-1.0.1/pyproject.toml` & `repetita_parser-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repetita-parser"
-version = "1.0.1"
+version = "1.0.2"
 description = "A parser for the REPETITA format"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 authors = [
   { name="Leon Richardt", email="pip@leon.dev" },
 ]
```

### Comparing `repetita_parser-1.0.1/PKG-INFO` & `repetita_parser-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repetita-parser
-Version: 1.0.1
+Version: 1.0.2
 Summary: A parser for the REPETITA format
 Project-URL: Documentation, https://github.com/leon-richardt/python-repetita-parser#readme
 Project-URL: Issues, https://github.com/leon-richardt/python-repetita-parser/issues
 Project-URL: Source, https://github.com/leon-richardt/python-repetita-parser
 Author-email: Leon Richardt <pip@leon.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -26,15 +26,15 @@
 # python-repetita-parser
 
 A Python parser for the data format of the [REPETITA](https://github.com/svissicchio/Repetita) framework.
 This module can parse topology and demand files either **separately** or **combine** them into problem instances.
 The data can then be accessed via native Python objects.
 
 ## Usage
-A usage example is provided in [`examples/demand-visualization`](./examples/demand-visualization).
+A usage example is provided in [`examples/demand-visualization`](https://github.com/leon-richardt/python-repetita-parser/tree/main/examples/demand-visualization).
 To try it, run the following commands:
 ```bash
 $ cd examples/demand-visualization
 $ python -m venv env && source env/bin/activate
 $ pip install -r requirements.txt
 $ python demand_visualization.py data/DeutscheTelekom.{graph,0000.demands}
 ```
```

