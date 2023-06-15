# Comparing `tmp/bayanpy-0.7.4.tar.gz` & `tmp/bayanpy-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.7.4.tar", last modified: Mon Jun  5 18:05:59 2023, max compression
+gzip compressed data, was "bayanpy-0.7.5.tar", last modified: Thu Jun 15 15:04:42 2023, max compression
```

## Comparing `bayanpy-0.7.4.tar` & `bayanpy-0.7.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.4/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-05 18:05:59.114945 bayanpy-0.7.4/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.4/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    59427 2023-05-20 16:15:23.000000 bayanpy-0.7.4/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.4/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-05 18:05:59.114945 bayanpy-0.7.4/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-06-05 18:05:59.000000 bayanpy-0.7.4/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-06-05 18:05:59.114945 bayanpy-0.7.4/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-06-05 18:05:41.000000 bayanpy-0.7.4/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-15 15:04:42.760547 bayanpy-0.7.5/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.7.5/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-15 15:04:42.760547 bayanpy-0.7.5/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5350 2023-05-07 16:54:32.000000 bayanpy-0.7.5/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-15 15:04:42.760547 bayanpy-0.7.5/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    59462 2023-06-15 15:02:17.000000 bayanpy-0.7.5/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.7.5/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-06-15 15:04:42.760547 bayanpy-0.7.5/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-06-15 15:04:42.000000 bayanpy-0.7.5/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-06-15 15:04:42.000000 bayanpy-0.7.5/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-06-15 15:04:42.000000 bayanpy-0.7.5/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-06-15 15:04:42.000000 bayanpy-0.7.5/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-06-15 15:04:42.000000 bayanpy-0.7.5/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-06-15 15:04:42.760547 bayanpy-0.7.5/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-06-15 15:04:12.000000 bayanpy-0.7.5/setup.py
```

### Comparing `bayanpy-0.7.4/LICENSE` & `bayanpy-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.4/README.md` & `bayanpy-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.7.4/bayanpy/BayanImplied.py` & `bayanpy-0.7.5/bayanpy/BayanImplied.py`

 * *Files 1% similar despite different names*

```diff
@@ -1110,15 +1110,15 @@
     root_combo_time_start = time.time()
     partition_combo = pycombo.execute(Graph, weight="actual_weight", modularity_resolution=resolution)
     communities_combo = convert_to_com_list(partition_combo[0])
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
 
-    if mod_lp - mod_combo < threshold:
+    if (mod_lp - mod_combo)/mod_lp < threshold:
         return output(develop_mode,2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time)
     best_bound = mod_lp
     incumbent = mod_combo
     root = Node([], var_vals, Graph, communities_combo_declustered)
     root.set_level(0)
     root.set_bounds(mod_combo, mod_lp)
     var_fixed_ones, var_fixed_zeros = reduced_cost_variable_fixing(model, var_vals, mod_lp, incumbent, Graph, resolution)
@@ -1127,15 +1127,16 @@
     current_node = root
     current_level = 1
     nodes_previous_level = [root]
     best_combo = root
     best_lp = root
     root_time = root_lp_time + root_combo_time
     solve_start = time.time()
-    while (best_bound - incumbent > threshold and nodes_previous_level != [] and time.time() - solve_start - root_time <= time_allowed): #add time_limit as a user parameter
+    while ( (best_bound - incumbent)/best_bound > threshold and nodes_previous_level != []
+            and time.time() - solve_start - root_time <= time_allowed): #add time_limit as a user parameter
         nodes_current_level = []
         lower_bounds = []
         upper_bounds = []
         for node in nodes_previous_level:
             if time.time() - solve_start - root_time >= time_allowed:
                 if best_combo.is_integer:
                     if best_combo.lower_bound <= best_combo.upper_bound:
```

### Comparing `bayanpy-0.7.4/setup.py` & `bayanpy-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.7.4",
+    version="0.7.5",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

