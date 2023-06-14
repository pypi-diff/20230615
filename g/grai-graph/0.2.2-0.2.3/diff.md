# Comparing `tmp/grai_graph-0.2.2.tar.gz` & `tmp/grai_graph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_graph-0.2.2.tar", max compression
+gzip compressed data, was "grai_graph-0.2.3.tar", max compression
```

## Comparing `grai_graph-0.2.2.tar` & `grai_graph-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      211 2023-04-29 00:58:02.888617 grai_graph-0.2.2/README.md
--rw-r--r--   0        0        0      928 2023-04-30 17:36:11.765828 grai_graph-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-02-13 20:16:22.709007 grai_graph-0.2.2/src/grai_graph/__init__.py
--rw-r--r--   0        0        0     7981 2023-03-30 16:50:54.361721 grai_graph-0.2.2/src/grai_graph/analysis.py
--rw-r--r--   0        0        0      357 2023-02-13 20:16:22.709765 grai_graph-0.2.2/src/grai_graph/client_monkeypatch.py
--rw-r--r--   0        0        0     4123 2023-02-13 20:16:22.710062 grai_graph-0.2.2/src/grai_graph/graph.py
--rw-r--r--   0        0        0     3375 2023-02-13 20:16:22.710145 grai_graph-0.2.2/src/grai_graph/utils.py
--rw-r--r--   0        0        0     2480 2023-02-13 20:16:22.710278 grai_graph-0.2.2/src/grai_graph/visualizations.py
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 grai_graph-0.2.2/setup.py
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 grai_graph-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      211 2023-05-19 11:07:12.919359 grai_graph-0.2.3/README.md
+-rw-r--r--   0        0        0      991 2023-06-14 22:53:01.212296 grai_graph-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-14 22:53:01.217484 grai_graph-0.2.3/src/grai_graph/__init__.py
+-rw-r--r--   0        0        0     9328 2023-06-14 21:02:53.363823 grai_graph-0.2.3/src/grai_graph/analysis.py
+-rw-r--r--   0        0        0      369 2023-06-14 21:02:53.293703 grai_graph-0.2.3/src/grai_graph/client_monkeypatch.py
+-rw-r--r--   0        0        0     5594 2023-06-01 16:01:43.256304 grai_graph-0.2.3/src/grai_graph/graph.py
+-rw-r--r--   0        0        0     3941 2023-06-14 22:10:38.552183 grai_graph-0.2.3/src/grai_graph/utils.py
+-rw-r--r--   0        0        0     2697 2023-06-01 16:01:43.256572 grai_graph-0.2.3/src/grai_graph/visualizations.py
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 grai_graph-0.2.3/PKG-INFO
```

### Comparing `grai_graph-0.2.2/src/grai_graph/analysis.py` & `grai_graph-0.2.3/src/grai_graph/analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,33 +3,80 @@
 import networkx as nx
 from grai_schemas.base import Node as NodeTypes
 
 from grai_graph.graph import Graph
 
 
 class GraphAnalyzer:
+    """ """
+
     def __init__(self, graph: Graph):
         self.graph = graph
 
     def downstream_nodes(self, namespace: str, name: str):
+        """
+
+        Args:
+            namespace (str):
+            name (str):
+
+        Returns:
+
+        Raises:
+
+        """
         node_id = self.graph.get_node_id(namespace, name)
         downstream = list(nx.bfs_successors(self.graph.graph, node_id))[0][1]
         return [self.graph.get_node(node_id=node) for node in downstream]
 
     def upstream_nodes(self, namespace: str, name: str):
+        """
+
+        Args:
+            namespace (str):
+            name (str):
+
+        Returns:
+
+        Raises:
+
+        """
         node_id = self.graph.get_node_id(namespace, name)
         upstream = list(nx.bfs_predecessors(self.graph.graph, node_id))[0][1]
         return [self.graph.get_node(node_id=node) for node in upstream]
 
     def test_delete_node(self, namespace: str, name: str):
+        """
+
+        Args:
+            namespace (str):
+            name (str):
+
+        Returns:
+
+        Raises:
+
+        """
         return list(self.downstream_nodes(namespace, name))
 
     def traverse_data_type_violations(
         self, node: NodeTypes, new_type: str, path: Optional[List] = None
     ) -> Generator[Tuple[List[NodeTypes], bool], None, None]:
+        """
+
+        Args:
+            node (NodeTypes):
+            new_type (str):
+            path (Optional[List], optional): (Default value = None)
+
+        Returns:
+
+        Raises:
+
+        """
         if path is None:
             path = [node]
 
         node_id = self.graph.get_node_id(node.spec.namespace, node.spec.name)
         for test_node in self.column_successors(node.spec.namespace, node.spec.name):
             test_node_id = self.graph.get_node_id(test_node.spec.namespace, test_node.spec.name)
             edge_data = self.graph.graph[node_id][test_node_id][self.graph._container_key]
@@ -51,18 +98,23 @@
                 yield (new_path, test_node_data_type == new_type)
 
             yield from self.traverse_data_type_violations(test_node, new_type, path=new_path)
 
     def test_data_type_change(self, namespace: str, name: str, new_type: bool) -> List[Tuple[List[NodeTypes], bool]]:
         """
 
-        :param namespace:
-        :param name:
-        :param expects_unique: can't evaluate anything in the case of None
-        :return:
+        Args:
+            namespace (str):
+            name (str):
+            new_type (bool):
+
+        Returns:
+
+        Raises:
+
         """
         node_id = self.graph.get_node_id(namespace, name)
 
         if node_id is None:
             return []
 
         current_node = self.graph.get_node(node_id=node_id)
@@ -73,14 +125,26 @@
         # Only looks downstream
         affected_nodes = self.traverse_data_type_violations(current_node, new_type)
         return list(affected_nodes)
 
     def traverse_unique_violations(
         self, node: NodeTypes, expects_unique: bool, path: Optional[List] = None
     ) -> Generator[Tuple[List[NodeTypes], bool], None, None]:
+        """
+
+        Args:
+            node (NodeTypes):
+            expects_unique (bool):
+            path (Optional[List], optional): (Default value = None)
+
+        Returns:
+
+        Raises:
+
+        """
         if path is None:
             path = [node]
 
         node_id = self.graph.get_node_id(node.spec.namespace, node.spec.name)
         for test_node in self.column_successors(node.spec.namespace, node.spec.name):
             test_node_id = self.graph.get_node_id(test_node.spec.namespace, test_node.spec.name)
             edge_data = self.graph.graph[node_id][test_node_id][self.graph._container_key]
@@ -104,18 +168,23 @@
             yield from self.traverse_unique_violations(test_node, expects_unique, path=new_path)
 
     def test_unique_violations(
         self, namespace: str, name: str, expects_unique: bool
     ) -> List[Tuple[List[NodeTypes], bool]]:
         """
 
-        :param namespace:
-        :param name:
-        :param expects_unique: can't evaluate anything in the case of None
-        :return:
+        Args:
+            namespace (str):
+            name (str):
+            expects_unique (bool): can't evaluate anything in the case of None
+
+        Returns:
+
+        Raises:
+
         """
         node_id = self.graph.get_node_id(namespace, name)
 
         if node_id is None:
             return []
 
         current_node = self.graph.get_node(node_id=node_id)
@@ -126,14 +195,26 @@
         # Only looks downstream
         affected_nodes = self.traverse_unique_violations(current_node, expects_unique)
         return list(affected_nodes)
 
     def traverse_null_violations(
         self, node: NodeTypes, is_nullable: bool, path: Optional[List] = None
     ) -> Generator[Tuple[List[NodeTypes], bool], None, None]:
+        """
+
+        Args:
+            node (NodeTypes):
+            is_nullable (bool):
+            path (Optional[List], optional): (Default value = None)
+
+        Returns:
+
+        Raises:
+
+        """
         if path is None:
             path = [node]
 
         node_id = self.graph.get_node_id(node.spec.namespace, node.spec.name)
         for test_node in self.column_successors(node.spec.namespace, node.spec.name):
             test_node_id = self.graph.get_node_id(test_node.spec.namespace, test_node.spec.name)
             edge_data = self.graph.graph[node_id][test_node_id][self.graph._container_key]
@@ -157,18 +238,24 @@
 
             yield from self.traverse_null_violations(test_node, is_nullable, path=new_path)
 
     def test_nullable_violations(
         self, namespace: str, name: str, is_nullable: bool
     ) -> List[Tuple[List[NodeTypes], bool]]:
         """
-        :param namespace:
-        :param name:
-        :param is_nullable: can't evaluate anything in the case of None
-        :return:
+
+        Args:
+            namespace (str):
+            name (str):
+            is_nullable (bool): can't evaluate anything in the case of None
+
+        Returns:
+
+        Raises:
+
         """
         node_id = self.graph.get_node_id(namespace, name)
 
         if node_id is None:
             return []
 
         current_node = self.graph.get_node(node_id=node_id)
@@ -178,17 +265,39 @@
 
         # Only looks downstream
         affected_nodes = self.traverse_null_violations(current_node, is_nullable)
 
         return list(affected_nodes)
 
     def column_predecessors(self, namespace: str, name: str):
+        """
+
+        Args:
+            namespace (str):
+            name (str):
+
+        Returns:
+
+        Raises:
+
+        """
         node_id = self.graph.get_node_id(namespace, name)
         predecessors = (self.graph.get_node(node_id=node_id) for node_id in self.graph.graph.predecessors(node_id))
         col_predecessors = tuple(node for node in predecessors if node.spec.metadata.grai.node_type == "Column")
         return col_predecessors
 
     def column_successors(self, namespace: str, name: str):
+        """
+
+        Args:
+            namespace (str):
+            name (str):
+
+        Returns:
+
+        Raises:
+
+        """
         node_id = self.graph.get_node_id(namespace, name)
         successors = (self.graph.get_node(node_id=node_id) for node_id in self.graph.graph.successors(node_id))
         col_successors = tuple(node for node in successors if node.spec.metadata.grai.node_type == "Column")
         return col_successors
```

### Comparing `grai_graph-0.2.2/src/grai_graph/utils.py` & `grai_graph-0.2.3/src/grai_graph/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 from grai_schemas.v1 import EdgeV1, NodeV1
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnAttributes,
     ColumnToColumnMetadata,
-    EdgeTypeLabels,
+    EdgeMetadataTypeLabels,
     GenericEdgeMetadataV1,
 )
 from grai_schemas.v1.metadata.nodes import (
     ColumnAttributes,
     ColumnMetadata,
-    NodeTypeLabels,
+    NodeMetadataTypeLabels,
 )
 from pydantic import BaseModel
 
 from grai_graph import analysis, graph
 
 DEFAULT_NAMESPACE = "test"
 
 
 class TestNodeObj(BaseModel):
+    """ """
+
     name: str
     namespace: Optional[str] = DEFAULT_NAMESPACE
     node_attributes: Optional[ColumnAttributes] = None
 
     def __hash__(self):
         return hash((self.name, self.namespace))
 
 
 def mock_v1_node(node: Union[str, TestNodeObj]):
+    """
+
+    Args:
+        node (Union[str, TestNodeObj]):
+
+    Returns:
+
+    Raises:
+
+    """
     if isinstance(node, str):
         node = TestNodeObj(name=node)
 
     metadata = node.node_attributes if node.node_attributes is not None else {}
     node_dict = {
         "type": "Node",
         "version": "v1",
@@ -40,26 +52,38 @@
             "id": None,
             "name": node.name,
             "namespace": node.namespace,
             "data_source": "test_source",
             "display_name": node.name,
             "is_active": True,
             "metadata": {
-                "grai": ColumnMetadata(node_type=NodeTypeLabels.column.value, node_attributes=metadata).dict()
+                "grai": ColumnMetadata(node_type=NodeMetadataTypeLabels.column.value, node_attributes=metadata).dict()
             },
         },
     }
     return NodeV1(**node_dict)
 
 
 def mock_v1_edge(
     source_node: Union[str, TestNodeObj],
     destination_node: Union[str, TestNodeObj],
     metadata={},
 ):
+    """
+
+    Args:
+        source_node (Union[str, TestNodeObj]):
+        destination_node (Union[str, TestNodeObj]):
+        metadata:  (Default value = {})
+
+    Returns:
+
+    Raises:
+
+    """
     if isinstance(source_node, str):
         source_node = TestNodeObj(name=source_node)
     if isinstance(destination_node, str):
         destination_node = TestNodeObj(name=destination_node)
 
     edge_dict = {
         "type": "Edge",
@@ -73,24 +97,35 @@
             "destination": {
                 "name": destination_node.name,
                 "namespace": destination_node.namespace,
             },
             "is_active": True,
             "metadata": {
                 "grai": ColumnToColumnMetadata(
-                    edge_type=EdgeTypeLabels.column_to_column.value,
+                    edge_type=EdgeMetadataTypeLabels.column_to_column.value,
                     edge_attributes=metadata,
                 ).dict()
             },
         },
     }
     return EdgeV1(**edge_dict)
 
 
 def build_graph_from_map(map: Dict[Union[str, TestNodeObj], List[Tuple[str, ColumnToColumnAttributes]]]) -> graph.Graph:
+    """
+
+    Args:
+        map (Dict[Union[str, TestNodeObj]):
+        List]]]:
+
+    Returns:
+
+    Raises:
+
+    """
     nodes = [node if isinstance(node, TestNodeObj) else TestNodeObj(name=node) for node in map.keys()]
     node_name_map = {node.name: node for node in nodes}
     nodes = [mock_v1_node(node) for node in nodes]
 
     edges = (
         (source, node_name_map[destination], meta)
         for source, dest_meta in map.items()
@@ -99,9 +134,20 @@
     edges = [mock_v1_edge(*args) for args in edges]
     return graph.build_graph(nodes, edges, "v1")
 
 
 def get_analysis_from_map(
     map: Dict[Union[str, TestNodeObj], Dict[ColumnToColumnAttributes, List[str]]]
 ) -> analysis.GraphAnalyzer:
+    """
+
+    Args:
+        map (Dict[Union[str, TestNodeObj]):
+        Dict]]]:
+
+    Returns:
+
+    Raises:
+
+    """
     graph = build_graph_from_map(map)
     return analysis.GraphAnalyzer(graph)
```

### Comparing `grai_graph-0.2.2/src/grai_graph/visualizations.py` & `grai_graph-0.2.3/src/grai_graph/visualizations.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,28 @@
     graph: nx.DiGraph,
     file_name: Union[Path, str],
     sort: bool = True,
     file_format=None,
     dpi: Optional[int] = 800,
 ) -> None:
     """Output a graph to a file, either as image or as dot file.
+
     Args:
-        graph: the DiGraph to write or plot
-        file_name: the file name to write to.
-        sort: create a copy of the graph with sorted keys
+        graph (nx.DiGraph): the DiGraph to write or plot
+        file_name (Union[Path, str]): the file name to write to.
+        sort (bool, optional): create a copy of the graph with sorted keys (Default value = True)
         file_format: graphviz output format, if None, the file_name extension is used as format
-            https://graphviz.org/doc/info/output.html
-        dpi: Output image resolution
+    https://graphviz.org/doc/info/output.html (Default value = None)
+        dpi (Optional[int], optional): (Default value = 800)
+
     Returns:
-        Nothing
+
     Raises:
         ValueError when the file_name does not end on .svg, .png or .dot
+
     """
     G = graph.copy()
 
     G.graph["node"] = {"shape": "box", "color": "red"}
     if dpi is not None:
         graph.graph["graph"] = {"dpi": dpi}
 
@@ -56,20 +59,25 @@
 
 def plot_graph(
     graph: nx.DiGraph,
     dpi: int = 800,
     figsize: Optional[Tuple[int, int]] = None,
 ):
     """
+
     Args:
-        graph: the DiGraph to write or plot
-        dpi: dpi of the matplotlib figure.
-        figsize: figure size
+        graph (nx.DiGraph): the DiGraph to write or plot
+        dpi (int, optional): dpi of the matplotlib figure. (Default value = 800)
+        figsize (Optional[Tuple[int, int]], optional): (Default value = None)
+
     Returns:
-        Displays the image
+        : Displays the image
+
+    Raises:
+
     """
     import os
     import tempfile
 
     from matplotlib import image as mpimg
     from matplotlib import pyplot as plt
```

### Comparing `grai_graph-0.2.2/PKG-INFO` & `grai_graph-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-graph
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: vis
-Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.5,<0.2.0)
+Requires-Dist: grai-client (>=0.2.18,<0.3.0)
+Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "vis"
 Requires-Dist: networkx (>=2.8.5,<3.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "vis"
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-graph
 Description-Content-Type: text/markdown
```

