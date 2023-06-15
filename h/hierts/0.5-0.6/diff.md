# Comparing `tmp/hierts-0.5.tar.gz` & `tmp/hierts-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierts-0.5.tar", last modified: Wed Jun 14 09:36:37 2023, max compression
+gzip compressed data, was "hierts-0.6.tar", last modified: Thu Jun 15 06:52:29 2023, max compression
```

## Comparing `hierts-0.5.tar` & `hierts-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.900236 hierts-0.5/
--rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.5/LICENSE
--rw-rw-rw-   0        0        0    14643 2023-06-14 09:36:37.899237 hierts-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.5/README.md
--rw-rw-rw-   0        0        0      793 2023-06-14 09:35:48.000000 hierts-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 09:36:37.900236 hierts-0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.853236 hierts-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.871234 hierts-0.5/src/hierts/
--rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.5/src/hierts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.898237 hierts-0.5/src/hierts/_old/
--rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.5/src/hierts/_old/reconciliation.py
--rw-rw-rw-   0        0        0    20363 2023-06-14 09:34:14.000000 hierts-0.5/src/hierts/reconciliation.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:36:37.897240 hierts-0.5/src/hierts.egg-info/
--rw-rw-rw-   0        0        0    14643 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 09:36:37.000000 hierts-0.5/src/hierts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.404559 hierts-0.6/
+-rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.6/LICENSE
+-rw-rw-rw-   0        0        0    14643 2023-06-15 06:52:29.403559 hierts-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.6/README.md
+-rw-rw-rw-   0        0        0      793 2023-06-15 06:50:31.000000 hierts-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:52:29.404559 hierts-0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.374559 hierts-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.380559 hierts-0.6/src/hierts/
+-rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.6/src/hierts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.402559 hierts-0.6/src/hierts/_old/
+-rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.6/src/hierts/_old/reconciliation.py
+-rw-rw-rw-   0        0        0    20417 2023-06-15 06:48:19.000000 hierts-0.6/src/hierts/reconciliation.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:52:29.400561 hierts-0.6/src/hierts.egg-info/
+-rw-rw-rw-   0        0        0    14643 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 06:52:29.000000 hierts-0.6/src/hierts.egg-info/top_level.txt
```

### Comparing `hierts-0.5/LICENSE` & `hierts-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hierts-0.5/PKG-INFO` & `hierts-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.5
+Version: 0.6
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hierts-0.5/README.md` & `hierts-0.6/README.md`

 * *Files identical despite different names*

### Comparing `hierts-0.5/pyproject.toml` & `hierts-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hierts"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Olivier Sprangers", email="o.r.sprangers@uva.nl" },
 ]
 description = "Hierarchical time series reconciliation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hierts-0.5/src/hierts/_old/reconciliation.py` & `hierts-0.6/src/hierts/_old/reconciliation.py`

 * *Files identical despite different names*

### Comparing `hierts-0.5/src/hierts/reconciliation.py` & `hierts-0.6/src/hierts/reconciliation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 #%% Import packages
 import numpy as np 
 import pandas as pd
 import time
 from numba import njit, prange
 from typing import List, Tuple
-from scipy.sparse import coo_matrix
+from scipy.sparse import coo_matrix, csc_matrix
 from sklearn.linear_model import LassoCV, Lasso
 #%% Functions to perform forecast reconciliation
 def reconcile_forecasts(yhat: np.ndarray, S: np.ndarray, y_train: np.ndarray=None, yhat_train: np.ndarray=None, method: str='ols', positive: bool=False) -> np.ndarray:
     """Optimal reconciliation of hierarchical forecasts using various approaches.
     
         Based on approaches from:
     
@@ -311,21 +311,26 @@
 
         :return: forecasts_methods, dataframe containing forecasts for all reconciliation methods
         :rtype: pd.DataFrame      
     
     """
     # Check to ensure correct inputs are given
     assert set(df_S.columns) == set(forecasts.index), 'Index of forecasts should match columns of df_S'
+    # Convert df_S 
+    if hasattr(df_S, "sparse"):
+        print("S is sparse")
+        S = csc_matrix(df_S.sparse.to_coo())
+    else:
+        print("S is dense")
+        S = df_S.values
     # Bottom-up forecasts
     all_aggregations = df_S.index.get_level_values('Aggregation').unique()
     all_aggregations = all_aggregations.drop(name_bottom_timeseries)
     forecasts_bu = pd.DataFrame(index=df_S.index, columns=forecasts.columns)
-    forecasts_bu.loc[name_bottom_timeseries] = forecasts.values.astype('float32')
-    for agg in all_aggregations:
-        forecasts_bu.loc[agg] = (df_S.loc[agg] @ forecasts).values.astype('float32')
+    forecasts_bu.loc[:] = (S @ forecasts.values)
 
     return forecasts_bu
 
 
 def calc_level_method_rmse(forecasts_methods: pd.DataFrame, actuals: pd.DataFrame, 
                             base: str = 'base') -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Calculate RMSE for each level, for each method for a set of forecasts.
```

### Comparing `hierts-0.5/src/hierts.egg-info/PKG-INFO` & `hierts-0.6/src/hierts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.5
+Version: 0.6
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

