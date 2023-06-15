# Comparing `tmp/catencfamily-0.0.74.tar.gz` & `tmp/catencfamily-0.0.75.tar.gz`

## Comparing `catencfamily-0.0.74.tar` & `catencfamily-0.0.75.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    34919 2020-02-02 00:00:00.000000 catencfamily-0.0.74/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.74/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.74/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.74/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.74/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    39649 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.75/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.75/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.75/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.75/PKG-INFO
```

### Comparing `catencfamily-0.0.74/src/catencfamily/encoders.py` & `catencfamily-0.0.75/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.74/src/catencfamily/utils.py` & `catencfamily-0.0.75/src/catencfamily/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 14th June, 2023
+# 15th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
@@ -914,24 +914,29 @@
             );
     plt.title(title)
     
 
     
 # Community visualization
 # Kaggle: https://www.kaggle.com/code/rahulgoel1106/commmunity-detection-using-igraph-and-networkx
-def communityVisualization(filename, pathToFolder,ax= None, title = None, withLabels = False, font_size = 8, edgewidth = 0.1, colorList =  ["orange", "yellow", "white"]):
+def communityVisualization(filename, pathToFolder, algo = nx.community.greedy_modularity_communities , ax= None, title = None, withLabels = False, font_size = 8, edgewidth = 0.1, colorList =  ["orange", "yellow", "white"]):
     """
     Desc
     ----
-    Displays communities created by modularity class.
+    Displays communities created by given community algo.
 
     Parameters
     ----------
     filename : str, Graph file
     pathToFolder : str, Path to folder having graph files
+    algo: function object to create communities
+          Default: nx.community.greedy_modularity_communities 
+          Examples: nx.community.kernighan_lin_bisection
+                    nx.community.greedy_modularity_communities
+                    nx.community.louvain_communities
     ax: Matplotlib axis object
     withLabels : boolean, Should labels be displayed? The default is False.
     font_size : int, Label font size. The default is 8.
     edgewidth: float, Edge line width
     colorList: List of colors for difft communitied. 
                Default is: ["orange", "yellow", "white"]
 
@@ -940,15 +945,15 @@
     None.
 
     """
     filepath = pathToFolder / filename
     G = nx.read_gml(filepath) 
     colors = colorList
     pos = nx.spring_layout(G)
-    lst_b = nx.community.greedy_modularity_communities(G)
+    lst_b = algo(G)
     color_map_b = {}
     keys = G.nodes()
     values = "black"
     for i in keys:
             color_map_b[i] = values
     counter = 0
     for x in lst_b:
@@ -960,14 +965,15 @@
     if withLabels:
       nx.draw_networkx_labels(G, pos, font_size = font_size, font_weight = 'bold',ax =ax)
     plt.axis("off");
     plt.title(title)
     #plt.show();    
 
 
+
 def transformBinnedDF2Communities(columnNames,pathToGraphFolder, train_binned, algo):
     """
     Desc
     -----
     Replace every column in the binned the Dataframe as per network community
     Example binned/discrete dataframe:
             'a'     'b
@@ -999,15 +1005,18 @@
     Parameters
     -----------     
     columnNames: list of cat cols
     pathToGraphFolder: str: Folder that has graph files     
     train_binned: DataFrame with binned/discrete columns  
     algo: function object: networkx algorithm to be used to 
           discover communities.
-          Example: nx.community.greedy_modularity_communities  
+          Examples: nx.community.kernighan_lin_bisection
+                    nx.community.greedy_modularity_communities
+                    nx.community.louvain_communities
+
           
     Returns
     -------
     map_list: list of dictionaries. Each dictionary maps
               levels in a column to a community 
     df: DataFrame: Transformed train_binned DataFrame.
         If train_binned had columns other than columnNames,
@@ -1060,14 +1069,19 @@
       #   cm_mod:      {'434', '435' },    {'23' , '78'}
       #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
 
       counter = 0  # Assigns values in dict
       fset_dict = {}  # Start with blank dict
       # For every frozenset
       for i in cm_mod:
+        # If set i is not a frozenset, make it so
+        # else its members cannot be used as dict keys
+        if not isinstance(i,frozenset):
+            i = frozenset(i)
+            
         # For every item in this frozenset
         for g in i:
           # Set class to the value of counter
           fset_dict[g] = counter
 
         # Increment counter for next class
         counter  +=1
@@ -1078,12 +1092,145 @@
       # Extract column name from file:
       colToProject = file.split('_')[0]
       # Map train_binned column using the dict
       df[file] = train_binned[colToProject].map(fset_dict)
       # Continue for loop for the next filelist
     return map_list,df
 
+
+
+def transformBinnedDF2CommunitiesAll(pathToGraphFolder, train_binned, algo):
+    """
+    Desc
+    -----
+    Search out all graph files and Replace every column in the binned Dataframe 
+    as per network community
+    Example binned/discrete dataframe:
+            'a'     'b
+            --      ---
+            434     709
+            435     789
+            23      710
+            78      756
+
+    Replace col 'a' as per communities discovered in network 'a_projected_b.gml':
+    434 & 435 belong to one community and 23 & 78 to other.
+
+            'a'     'b'
+            ---     ---
+             0      709
+             0      789
+             1      710
+             1      756
+
+    Similarly, replace col 'b' as per communities in 'b_projected_a.gml':
+
+            'a'     'b'
+            ---     ---
+             0      1
+             0      0
+             1      0
+             1      1
+
+    Parameters
+    -----------
+    pathToGraphFolder: str: Folder that has graph files
+    train_binned: DataFrame with binned/discrete columns
+    algo: function object: networkx algorithm to be used to
+          discover communities.
+          Example: nx.community.greedy_modularity_communities
+
+    Returns
+    -------
+    map_list: list of dictionaries. Each dictionary maps
+              levels in a column to a community
+    df: DataFrame: Transformed train_binned DataFrame.
+        If train_binned had columns other than columnNames,
+        df would not contain those columns
+
+
+    """
+    # 15.1 Path where .gml files are placed:
+
+    # 1. From col-names names, create graph filenames:
+    filelist = sorted(list(Path(pathToGraphFolder).iterdir()))
+    filelist = [i   for i in filelist if "_projected_" in str(i) ]
+    filelist = [str(i).split("/")[-1]   for i in filelist ]
+
+    # 2. For every file in the filelist
+    map_list = []  # Start with a blank list of dictionaries
+    # df will store dataframe train_binned after each bin-col is mapped
+    #
+    df = pd.DataFrame()
+    for file in filelist:
+      # 2.1 Load network
+      # Get full filename that includes filepath
+      filepath = Path(pathToGraphFolder) / file
+      # Read the file as a network
+      G = nx.read_gml(filepath)
+
+      # 2.2 Calculate community classes using algo
+      #    cm_mod contains as many frozensets of nodes
+      #    as there are communities:
+      cm_mod = algo(G)
+
+      # 3.0 We now create dict corresponding to
+      #     all communities in cm_mod
+      #    Example:
+      #                 frozenset1         frozenset2
+      #   cm_mod:      {'434', '435' },    {'23' , '78'}
+      #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
+
+      counter = 0  # Assigns values in dict
+      fset_dict = {}  # Start with blank dict
+      # For every frozenset
+      for i in cm_mod:
+        if not isinstance(i,frozenset):
+          i = frozenset(i)
+        # For every item in this frozenset
+        for g in i:
+          # Set class to the value of counter
+          fset_dict[g] = counter
+
+        # Increment counter for next class
+        counter  +=1
+      # Now that map dict for the modularity
+      # classes are ready, append it to map_list
+      map_list.append(fset_dict)
+
+      # Extract column name from file:
+      colToProject = file.split('_projected_')[0]
+      # Map train_binned column using the dict
+      if colToProject in train_binned.columns:
+        df[file] = train_binned[colToProject].map(fset_dict)
+      # Continue for loop for the next filelist
+    return map_list,df
     
+
+
+# Function to remove const columns from DataFrame
+# https://stackoverflow.com/a/20210048
+def remConstColumns(df):
+    """
+    Desc
+    ----
+    Removes const columns from dataframe df
+
+    Parameters
+    ----------
+    df : pandas DataFrame
+
+    Returns
+    -------
+    df : pandas DataFrame
+
+    """
+    print(f"Datashape before processing: {df.shape}")
+    df = df.loc[:, (df != df.iloc[0]).any()] 
+    print(f"Datashape after processing: {df.shape}")
+    return df
+
+
 ################### That's all folks #######################
```

### Comparing `catencfamily-0.0.74/LICENSE` & `catencfamily-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.74/README.md` & `catencfamily-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.74/pyproject.toml` & `catencfamily-0.0.75/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.74"
+version = "0.0.75"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.74/PKG-INFO` & `catencfamily-0.0.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.74
+Version: 0.0.75
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

