# Comparing `tmp/itca-0.1.3.tar.gz` & `tmp/itca-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itca-0.1.3.tar", last modified: Thu Jun 15 08:51:57 2023, max compression
+gzip compressed data, was "itca-0.1.4.tar", last modified: Thu Jun 15 16:22:00 2023, max compression
```

## Comparing `itca-0.1.3.tar` & `itca-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 08:51:57.506623 itca-0.1.3/
--rw-r--r--   0 chzhang    (501) staff       (20)     1091 2023-05-19 13:33:06.000000 itca-0.1.3/LICENSE
--rw-r--r--   0 chzhang    (501) staff       (20)     4608 2023-06-15 08:51:57.506499 itca-0.1.3/PKG-INFO
--rw-r--r--   0 chzhang    (501) staff       (20)     3892 2023-06-15 08:45:09.000000 itca-0.1.3/README.md
-drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 08:51:57.502008 itca-0.1.3/itca/
--rw-r--r--   0 chzhang    (501) staff       (20)      298 2023-06-15 08:50:04.000000 itca-0.1.3/itca/__init__.py
-drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 08:51:57.502870 itca-0.1.3/itca/datasets/
--rw-r--r--   0 chzhang    (501) staff       (20)      278 2023-05-22 03:54:15.000000 itca-0.1.3/itca/datasets/__init__.py
--rw-r--r--   0 chzhang    (501) staff       (20)  8118532 2023-05-22 02:02:59.000000 itca-0.1.3/itca/datasets/hydra.npz
--rw-r--r--   0 chzhang    (501) staff       (20)     4968 2023-05-19 13:33:06.000000 itca-0.1.3/itca/metrics.py
--rw-r--r--   0 chzhang    (501) staff       (20)    18455 2023-05-19 13:33:06.000000 itca-0.1.3/itca/search.py
--rw-r--r--   0 chzhang    (501) staff       (20)     4254 2023-05-19 13:33:06.000000 itca-0.1.3/itca/simulation_suites.py
--rw-r--r--   0 chzhang    (501) staff       (20)     9112 2023-05-22 04:35:43.000000 itca-0.1.3/itca/simulator.py
--rw-r--r--   0 chzhang    (501) staff       (20)     8157 2023-05-19 13:33:06.000000 itca-0.1.3/itca/utils.py
--rw-r--r--   0 chzhang    (501) staff       (20)     3322 2023-06-15 08:41:34.000000 itca-0.1.3/itca/visualize.py
-drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 08:51:57.502632 itca-0.1.3/itca.egg-info/
--rw-r--r--   0 chzhang    (501) staff       (20)     4608 2023-06-15 08:51:57.000000 itca-0.1.3/itca.egg-info/PKG-INFO
--rw-r--r--   0 chzhang    (501) staff       (20)      339 2023-06-15 08:51:57.000000 itca-0.1.3/itca.egg-info/SOURCES.txt
--rw-r--r--   0 chzhang    (501) staff       (20)        1 2023-06-15 08:51:57.000000 itca-0.1.3/itca.egg-info/dependency_links.txt
--rw-r--r--   0 chzhang    (501) staff       (20)       70 2023-06-15 08:51:57.000000 itca-0.1.3/itca.egg-info/requires.txt
--rw-r--r--   0 chzhang    (501) staff       (20)        5 2023-06-15 08:51:57.000000 itca-0.1.3/itca.egg-info/top_level.txt
--rw-r--r--   0 chzhang    (501) staff       (20)       38 2023-06-15 08:51:57.506661 itca-0.1.3/setup.cfg
--rw-r--r--   0 chzhang    (501) staff       (20)     3342 2023-06-15 08:51:49.000000 itca-0.1.3/setup.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 16:22:00.073435 itca-0.1.4/
+-rw-r--r--   0 chzhang    (501) staff       (20)     1091 2023-05-19 13:33:06.000000 itca-0.1.4/LICENSE
+-rw-r--r--   0 chzhang    (501) staff       (20)     4608 2023-06-15 16:22:00.073270 itca-0.1.4/PKG-INFO
+-rw-r--r--   0 chzhang    (501) staff       (20)     3892 2023-06-15 08:45:09.000000 itca-0.1.4/README.md
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 16:22:00.046865 itca-0.1.4/itca/
+-rw-r--r--   0 chzhang    (501) staff       (20)      298 2023-06-15 16:21:33.000000 itca-0.1.4/itca/__init__.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 16:22:00.048020 itca-0.1.4/itca/datasets/
+-rw-r--r--   0 chzhang    (501) staff       (20)      278 2023-05-22 03:54:15.000000 itca-0.1.4/itca/datasets/__init__.py
+-rw-r--r--   0 chzhang    (501) staff       (20)  8118532 2023-05-22 02:02:59.000000 itca-0.1.4/itca/datasets/hydra.npz
+-rw-r--r--   0 chzhang    (501) staff       (20)     4968 2023-05-19 13:33:06.000000 itca-0.1.4/itca/metrics.py
+-rw-r--r--   0 chzhang    (501) staff       (20)    18455 2023-05-19 13:33:06.000000 itca-0.1.4/itca/search.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     4254 2023-05-19 13:33:06.000000 itca-0.1.4/itca/simulation_suites.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     9112 2023-05-22 04:35:43.000000 itca-0.1.4/itca/simulator.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     8157 2023-05-19 13:33:06.000000 itca-0.1.4/itca/utils.py
+-rw-r--r--   0 chzhang    (501) staff       (20)     4174 2023-06-15 16:19:33.000000 itca-0.1.4/itca/visualize.py
+drwxr-xr-x   0 chzhang    (501) staff       (20)        0 2023-06-15 16:22:00.047678 itca-0.1.4/itca.egg-info/
+-rw-r--r--   0 chzhang    (501) staff       (20)     4608 2023-06-15 16:21:59.000000 itca-0.1.4/itca.egg-info/PKG-INFO
+-rw-r--r--   0 chzhang    (501) staff       (20)      339 2023-06-15 16:22:00.000000 itca-0.1.4/itca.egg-info/SOURCES.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)        1 2023-06-15 16:21:59.000000 itca-0.1.4/itca.egg-info/dependency_links.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)       70 2023-06-15 16:21:59.000000 itca-0.1.4/itca.egg-info/requires.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)        5 2023-06-15 16:21:59.000000 itca-0.1.4/itca.egg-info/top_level.txt
+-rw-r--r--   0 chzhang    (501) staff       (20)       38 2023-06-15 16:22:00.073482 itca-0.1.4/setup.cfg
+-rw-r--r--   0 chzhang    (501) staff       (20)     3342 2023-06-15 16:21:25.000000 itca-0.1.4/setup.py
```

### Comparing `itca-0.1.3/LICENSE` & `itca-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/PKG-INFO` & `itca-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itca
-Version: 0.1.3
+Version: 0.1.4
 Summary: A  Data-driven Criterion to Combining Ambiguous Outcome Labels in Multi-class Classification
 Home-page: https://github.com/JSB-UCLA/ITCA
 Author: Chihao Zhang
 Author-email: zhang.dabiao11@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `itca-0.1.3/README.md` & `itca-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/datasets/hydra.npz` & `itca-0.1.4/itca/datasets/hydra.npz`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/metrics.py` & `itca-0.1.4/itca/metrics.py`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/search.py` & `itca-0.1.4/itca/search.py`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/simulation_suites.py` & `itca-0.1.4/itca/simulation_suites.py`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/simulator.py` & `itca-0.1.4/itca/simulator.py`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/utils.py` & `itca-0.1.4/itca/utils.py`

 * *Files identical despite different names*

### Comparing `itca-0.1.3/itca/visualize.py` & `itca-0.1.4/itca/visualize.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,67 +10,99 @@
     if level == 0:
         name = node[1][0] + 1
     else:
         name = "c" + str(rename_node.comb_class)
         rename_node.comb_class += 1
     return name
 
+
 def rename_G(G):
     rename_node.comb_class = 1
     nodes = G.nodes()
-    rename_mapping = {node:  rename_node(node) for node in nodes}
+    rename_mapping = {node: rename_node(node) for node in nodes}
     G_ = copy.copy(G)
     G_ = nx.relabel_nodes(G, rename_mapping)
     return G_
+
+
 def compare_neigbor_bidict(m1, m2):
-    assert(len(m1.inverse) - len(m2.inverse) == 1)
+    assert (len(m1.inverse) - len(m2.inverse) == 1)
     s1 = set(tuple(t) for t in m1.inverse.values())
     s2 = set(tuple(t) for t in m2.inverse.values())
     sym_diff = s2.symmetric_difference(s1)
     i, j, ij = sorted(list(sym_diff), key=len)
     node_i = (len(i) - 1, i)
     node_j = (len(j) - 1, j)
     node_ij = (len(ij) - 1, ij)
     return node_i, node_j, node_ij
 
 
 def gen_tree(path):
-    G = nx.Graph()
+    G = nx.DiGraph()
     cur = path
     while cur.children:
         cur_m = bidict(cur.mapping)
         next_m = bidict(cur.children[0].mapping)
         node_i, node_j, node_ij = compare_neigbor_bidict(cur_m, next_m)
         G.add_node(node_i)
         G.add_node(node_j)
         G.add_node(node_ij)
-        G.add_edge(node_i, node_ij)
-        G.add_edge(node_j, node_ij)
+        G.add_edge(node_ij, node_i)
+        G.add_edge(node_ij, node_j)
         cur = cur.children[0]
     m1 = bidict(cur.mapping)
-    m2 = bidict({i:0 for i in range(38)})
+    m2 = bidict({i: 0 for i in range(38)})
     node_i, node_j, node_ij = compare_neigbor_bidict(m1, m2)
     G.add_node(node_ij)
-    G.add_edge(node_i, node_ij)
-    G.add_edge(node_j, node_ij)
+    G.add_edge(node_ij, node_i)
+    G.add_edge(node_ij, node_j)
     return G
 
 
+def wrap_plot_ascii_tree(graph, node, level=0, last_node=False):
+    # Print the current node
+    print(" " * 4 * level, end="")
+    if last_node:
+        print("└─", end="")
+    else:
+        print("├─", end="")
+    print(node)
+
+    # Get the children of the current node
+    children = list(graph.successors(node))
+
+    # Recursively plot each child
+    for i, child in enumerate(children):
+        last = i == len(children) - 1
+        wrap_plot_ascii_tree(graph, child, level=level + 1, last_node=last)
+
+
+def plot_ascii_tree(strategy=None, graph=None):
+    if graph is None:
+        G = gen_tree(strategy.path)
+    else:
+        G = copy.copy(graph)
+    G_ = rename_G(G)
+    root_node = (len(G_) - 1) // 2
+    wrap_plot_ascii_tree(G_, "c{}".format(root_node))
+    print("Integers representing the original class labels and c* representing the combined classes.")
+
+
 def plot_tree(strategy=None, graph=None, figsize=(6, 12), node_size=350, direction="vertical",
               return_graph=False, use_pygraphviz=False):
     """
     :param gs: instance of SearchStrategy
     :param figsize: size of the figure
     :param node_size: plot node size, input to nx.draw_networkx
     :param direction: direction of the tree, "vertical" or "horizontal"
     :param return_graph: if True, return the figure
     :return:  return the graph and figure if return_graph is True, else return figure
     """
     # Either strategy or G must be provided
-    assert(strategy is not None or graph is not None)
+    assert (strategy is not None or graph is not None)
     if graph is None:
         G = gen_tree(strategy.path)
     else:
         G = copy.copy(graph)
     G_ = rename_G(G)
     if use_pygraphviz:
         try:
@@ -79,19 +111,20 @@
         except ImportError:
             raise ImportError("requires pygraphviz to visualize tree")
         pos = nx.nx_agraph.graphviz_layout(G_, prog="dot")
     else:
         try:
             pos = nx.nx_pydot.pydot_layout(G_, prog='dot')
         except FileNotFoundError:
-            raise FileNotFoundError("requires pydot to visualize tree; please find the troubleshooting guide at https://github.com/JSB-UCLA/ITCA")
+            raise FileNotFoundError(
+                "requires pydot to visualize tree; please find the troubleshooting guide at https://github.com/JSB-UCLA/ITCA")
     if direction == "horizontal":
-        flipped_pos = {node: (y, -x) for (node, (x,y)) in pos.items()}
+        flipped_pos = {node: (y, x) for (node, (x, y)) in pos.items()}
         pos = flipped_pos
     elif direction == "vertical":
-        pos = {node: (x, -y) for (node, (x,y)) in pos.items()}
+        pass
     fig, ax = plt.subplots(figsize=(6, 12))
     nx.draw_networkx(G_, pos, node_size=node_size, with_labels=True)
     if return_graph:
         return G_, fig
     else:
-        return fig
+        return fig
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `itca-0.1.3/itca.egg-info/PKG-INFO` & `itca-0.1.4/itca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itca
-Version: 0.1.3
+Version: 0.1.4
 Summary: A  Data-driven Criterion to Combining Ambiguous Outcome Labels in Multi-class Classification
 Home-page: https://github.com/JSB-UCLA/ITCA
 Author: Chihao Zhang
 Author-email: zhang.dabiao11@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `itca-0.1.3/setup.py` & `itca-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'itca'
 DESCRIPTION = 'A  Data-driven Criterion to Combining Ambiguous Outcome Labels in Multi-class Classification'
 URL = 'https://github.com/JSB-UCLA/ITCA'
 EMAIL = 'zhang.dabiao11@gmail.com'
 AUTHOR = 'Chihao Zhang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy',
     'scikit_learn',
     'networkx',
     'matplotlib',
```

