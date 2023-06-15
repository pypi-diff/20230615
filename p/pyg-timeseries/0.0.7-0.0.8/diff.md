# Comparing `tmp/pyg-timeseries-0.0.7.tar.gz` & `tmp/pyg-timeseries-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg-timeseries-0.0.7.tar", last modified: Tue Jun 14 20:31:06 2022, max compression
+gzip compressed data, was "pyg-timeseries-0.0.8.tar", last modified: Wed Jun 29 20:43:46 2022, max compression
```

## Comparing `pyg-timeseries-0.0.7.tar` & `pyg-timeseries-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-06-14 20:31:06.027465 pyg-timeseries-0.0.7/
--rw-rw-rw-   0        0        0       86 2022-06-14 20:31:06.027465 pyg-timeseries-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-14 20:31:06.018482 pyg-timeseries-0.0.7/pyg_timeseries/
--rw-rw-rw-   0        0        0     2109 2022-06-14 19:38:05.000000 pyg-timeseries-0.0.7/pyg_timeseries/__init__.py
--rw-rw-rw-   0        0        0     5754 2022-06-09 22:05:01.000000 pyg-timeseries-0.0.7/pyg_timeseries/_bar.py
--rw-rw-rw-   0        0        0    12171 2022-06-14 15:08:32.000000 pyg-timeseries-0.0.7/pyg_timeseries/_decorators.py
--rw-rw-rw-   0        0        0    57786 2022-06-13 19:13:45.000000 pyg-timeseries-0.0.7/pyg_timeseries/_ewm.py
--rw-rw-rw-   0        0        0     8484 2022-05-27 02:13:50.000000 pyg-timeseries-0.0.7/pyg_timeseries/_ewmcombine.py
--rw-rw-rw-   0        0        0     9007 2022-03-24 23:15:22.000000 pyg-timeseries-0.0.7/pyg_timeseries/_ewmxo.py
--rw-rw-rw-   0        0        0    19285 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.7/pyg_timeseries/_expanding.py
--rw-rw-rw-   0        0        0     1742 2022-05-11 23:07:36.000000 pyg-timeseries-0.0.7/pyg_timeseries/_iter.py
--rw-rw-rw-   0        0        0    18982 2022-06-14 15:59:35.000000 pyg-timeseries-0.0.7/pyg_timeseries/_linalg.py
--rw-rw-rw-   0        0        0     4353 2022-05-24 14:30:02.000000 pyg-timeseries-0.0.7/pyg_timeseries/_math.py
--rw-rw-rw-   0        0        0     6437 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.7/pyg_timeseries/_max.py
--rw-rw-rw-   0        0        0     5044 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.7/pyg_timeseries/_median.py
--rw-rw-rw-   0        0        0     6388 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.7/pyg_timeseries/_min.py
--rw-rw-rw-   0        0        0     1850 2022-05-11 23:11:00.000000 pyg-timeseries-0.0.7/pyg_timeseries/_opt.py
--rw-rw-rw-   0        0        0     2705 2022-06-06 19:34:15.000000 pyg-timeseries-0.0.7/pyg_timeseries/_pandas.py
--rw-rw-rw-   0        0        0     3561 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.7/pyg_timeseries/_rank.py
--rw-rw-rw-   0        0        0     9107 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.7/pyg_timeseries/_rms_join.py
--rw-rw-rw-   0        0        0    44938 2022-06-14 19:56:55.000000 pyg-timeseries-0.0.7/pyg_timeseries/_rolling.py
--rw-rw-rw-   0        0        0     4274 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.7/pyg_timeseries/_stride.py
--rw-rw-rw-   0        0        0     7509 2022-06-14 19:54:20.000000 pyg-timeseries-0.0.7/pyg_timeseries/_track.py
--rw-rw-rw-   0        0        0    18062 2022-05-23 17:53:18.000000 pyg-timeseries-0.0.7/pyg_timeseries/_ts.py
--rw-rw-rw-   0        0        0     4925 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.7/pyg_timeseries/_xrank.py
-drwxrwxrwx   0        0        0        0 2022-06-14 20:31:06.025474 pyg-timeseries-0.0.7/pyg_timeseries.egg-info/
--rw-rw-rw-   0        0        0       86 2022-06-14 20:31:05.000000 pyg-timeseries-0.0.7/pyg_timeseries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2022-06-14 20:31:05.000000 pyg-timeseries-0.0.7/pyg_timeseries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-14 20:31:05.000000 pyg-timeseries-0.0.7/pyg_timeseries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-06-14 20:31:05.000000 pyg-timeseries-0.0.7/pyg_timeseries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-14 20:31:06.028455 pyg-timeseries-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      230 2022-06-14 20:17:43.000000 pyg-timeseries-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-29 20:43:46.617923 pyg-timeseries-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1212 2022-06-29 20:43:46.617923 pyg-timeseries-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      718 2022-06-29 20:43:46.634878 pyg-timeseries-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-06-29 20:43:46.550104 pyg-timeseries-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2022-06-29 20:43:46.606953 pyg-timeseries-0.0.8/src/pyg_timeseries/
+-rw-rw-rw-   0        0        0     2160 2022-06-19 19:12:52.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/__init__.py
+-rw-rw-rw-   0        0        0     5754 2022-06-09 22:05:01.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_bar.py
+-rw-rw-rw-   0        0        0    12171 2022-06-14 15:08:32.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_decorators.py
+-rw-rw-rw-   0        0        0    57786 2022-06-13 19:13:45.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_ewm.py
+-rw-rw-rw-   0        0        0     8484 2022-05-27 02:13:50.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_ewmcombine.py
+-rw-rw-rw-   0        0        0     9007 2022-03-24 23:15:22.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_ewmxo.py
+-rw-rw-rw-   0        0        0    19285 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_expanding.py
+-rw-rw-rw-   0        0        0     1742 2022-05-11 23:07:36.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_iter.py
+-rw-rw-rw-   0        0        0    19417 2022-06-17 10:47:07.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_linalg.py
+-rw-rw-rw-   0        0        0     4353 2022-05-24 14:30:02.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_math.py
+-rw-rw-rw-   0        0        0     6437 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_max.py
+-rw-rw-rw-   0        0        0     5044 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_median.py
+-rw-rw-rw-   0        0        0     6388 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_min.py
+-rw-rw-rw-   0        0        0     8581 2022-06-21 12:47:29.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_multibuffer.py
+-rw-rw-rw-   0        0        0     1850 2022-05-11 23:11:00.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_opt.py
+-rw-rw-rw-   0        0        0     2705 2022-06-06 19:34:15.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_pandas.py
+-rw-rw-rw-   0        0        0     3561 2022-02-18 13:45:50.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_rank.py
+-rw-rw-rw-   0        0        0     9107 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_rms_join.py
+-rw-rw-rw-   0        0        0    45263 2022-06-21 08:52:33.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_rolling.py
+-rw-rw-rw-   0        0        0     4274 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_stride.py
+-rw-rw-rw-   0        0        0     7509 2022-06-14 19:54:20.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_track.py
+-rw-rw-rw-   0        0        0    18062 2022-05-23 17:53:18.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_ts.py
+-rw-rw-rw-   0        0        0     4925 2022-02-18 11:49:59.000000 pyg-timeseries-0.0.8/src/pyg_timeseries/_xrank.py
+drwxrwxrwx   0        0        0        0 2022-06-29 20:43:46.615942 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/
+-rw-rw-rw-   0        0        0     1212 2022-06-29 20:43:45.000000 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2022-06-29 20:43:46.000000 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-29 20:43:45.000000 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2022-06-29 20:43:46.000000 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-06-29 20:43:46.000000 pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/top_level.txt
```

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/__init__.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 from pyg_timeseries._ewmcombine import ewmcombine, ewmcombined
 from pyg_timeseries._pandas import fnna_like, reindex_3d
 from pyg_timeseries._opt import least_squares
 from pyg_timeseries._iter import ts_iterate
 from pyg_timeseries._linalg import riskparity, eigenvalues, eigenvectors, det, matmul
 from pyg_timeseries._bar import bar_r2
 from pyg_timeseries._track import minimize_tracking_error
-
+from pyg_timeseries._multibuffer import multibuffer
```

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_bar.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_bar.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_decorators.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_decorators.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_ewm.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_ewm.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_ewmcombine.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_ewmcombine.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_ewmxo.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_ewmxo.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_expanding.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_expanding.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_iter.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_iter.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_linalg.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_linalg.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,14 +155,24 @@
                                     constraints = _constraints,
                                     tol = tol,
                                     options= {'disp': False})
     # Recover the weights from the optimised object
     fit[msk] = optimize_result.x
     return fit #, matmul(masked_c, optimize_result.x, optimize_result.x)
 
+def _data_ok(data, covariances, columns):
+    if data is None or len(data.shape)!=2: ## shape OK
+        return False
+    if data.shape[1] != covariances.shape[1]: ## matching covariances
+        return False
+    if is_df(data) and columns is not None and list(columns)!=list(data.columns): # match columns if available
+        return False
+    return True
+        
+
 def riskparity(covariances, assets_risk_budget = None, columns = None, index = None, data = None, tol = None, method = 'pyrb'):
     """
     Designed to take the output from the ewmcovar calculation or a simple covariances matrix.
     Calculates risk parity weights given covariances and target budgets.
     If data is provided, will skip calculations for previously done optimizations.
     
     The faster implementation is using pyrb available from https://github.com/jcrichard/pyrb
@@ -235,15 +245,15 @@
     ---------
     >>> res2 = riskparity(cov['data'], columns = cov['columns'], index = cov['index'], data = res1.iloc[:1800])
     >>> ratio = res2/res1
     >>> assert ratio.max().max() < 1.0001 and ratio.min().min() > 0.9999
     """
     arb = assets_risk_budget; cov = covariances; idx = index; weights = None
     cov = ffill(cov)
-    if data is not None:
+    if _data_ok(data, covariances, columns):      
         if is_df(data) and index is not None: ## previous result is a timeseries
             data = data.iloc[:-1] ## remove last calculation
             mask = ~np.array([date in data.index for date in index])
             cov = cov[mask]
             idx = index[mask]
             weights = data.iloc[-1].values
             if is_df(arb):
@@ -253,14 +263,16 @@
             n = len(data)
             cov = cov[n:]
             if arb is not None and len(arb.shape) == 2:
                 arb = arb[n:]
             if idx is not None:
                 idx = idx[n:]
             weights = data[-1]
+    else:
+        data = None
 
     if isinstance(arb, list):
         if is_nums(arb):
             arb = np.array(arb)
         elif is_tss(arb):
             arb = v2na(df_reindex(df_concat(arb), index, method = 'ffill'))
     if is_pd(arb):
```

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_math.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_math.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_max.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_max.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_median.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_median.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_min.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_min.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_opt.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_opt.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_pandas.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_pandas.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_rank.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_rank.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_rms_join.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_rms_join.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_rolling.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_rolling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from pyg_timeseries._math import stdev_calculation, skew_calculation, _w
 from pyg_timeseries._decorators import compiled, first_, _data_state
-from pyg_base import pd2np, Dict, is_num, loop_all, loop, clock
+from pyg_base import pd2np, Dict, is_num, loop_all, loop, clock, is_pd, df_reindex
 
 __all__ = ['ffill', 'bfill', 'fnna', 'na2v', 'v2na', 'diff', 'shift', 'ratio', 'rolling_mean', 'rolling_sum', 'rolling_rms', 'rolling_std', 'rolling_skew', 
            'diff_', 'shift_', 'ratio_', 'rolling_mean_', 'rolling_sum_', 'rolling_rms_', 'rolling_std_', 'rolling_skew_']
 
 ###############
 ##
 ## parameters
@@ -277,45 +277,47 @@
                 prev = vec[i]
             t = time[j]
             res[j] = a[j] - prev
             vec[i] = a[j]
     return res, vec, i, t
 
 
-
 @loop_all
 @pd2np
 @compiled
 def _buffer(a, band, unit = 0.0, pos = 0):
     """
     >>> a = pd.Series(cumsum(np.random.normal(0,1,1000)), drange(-999))
     >>> ts, pos = _buffer(a, 1, 3, 0)
     >>> df_concat([a,ts])[dt(-100):].plot()
     """
     res = np.full(a.shape, np.nan)
+    b = 0.0
     if np.isnan(pos):
         pos = 0.0
     for i in range(a.shape[0]):
         if not np.isnan(a[i]):
-            b = band[i]
+            if not np.isnan(band[i]): ## we forward fill band
+                b = band[i]
             if pos < a[i] - b:
                 pos = a[i] - b
                 if unit > 0:
                     pos = np.round(pos / unit) * unit
                     if pos < a[i] - b and pos + unit < a[i] + b:
                         pos += unit
             elif pos > a[i] + b:
                 pos = a[i] + b
                 if unit > 0:
                     pos = np.round(pos / unit) * unit
                     if pos > a[i] + b and pos - unit > a[i] - b:
                         pos -= unit
             res[i] = pos
     return res, pos
-                 
+
+
 
 @loop_all
 def _tdiff(a, n, vec, i, time = None, t = None):
     time = clock(a, time, t)
     t = 0 if t is None or np.isnan(t) else t
     return _diff(a = a, n = n, vec = vec, i = i, time = time, t = t)
 
@@ -809,15 +811,17 @@
     """
     if is_num(state):
         state = Dict(pos = state)
     elif state is None:
         state = Dict(pos = 0.0)
     if is_num(band):
         band = np.full(a.shape, band)
-    return first_(_buffer(a, band = band, unit = unit, **state))
+    if is_pd(band) and is_pd(a):
+        band = df_reindex(band, a, method = 'ffill')
+    return first_(_buffer(a = a, band = band, unit = unit, **state))
     
         
 
         
 def shift(a, n=1, axis = 0, data = None, state = None):
     """
     Equivalent to a.shift() with support to arra
@@ -855,26 +859,26 @@
     --------------------------
     >>> old = a.iloc[:3]
     >>> new = a.iloc[3:]
     >>> old_ts = shift_(old)
     >>> new_ts = shift(new, **old_ts)
     >>> assert eq(new_ts, shift(a).iloc[3:])
     """
-    if n == 0:
+    if n == 0 or is_num(a):
         return a
     state = state or Dict(vec = None, i = 0,)
     state.vec = _vec(a, state.vec, n, axis=axis)
     return first_(_shift1(a, state.vec, axis = axis) if n == 1 else _shift(a, n, axis = axis, **state))
 
 def shift_(a, n=1, axis = 0, instate = None):
     """
     Equivalent to shift(a,n) but returns the full state. See shift for full details
   
     """
-    if n == 0:
+    if n == 0 or is_num(a):
         return Dict(data = a, state = instate)
     state = instate or Dict(vec = None, i = 0,)
     state.vec = _vec(a, state.vec, n, axis=axis)
     return _data_state(['data', 'vec', 'i'], _shift1(a, vec = state.vec, axis = axis) if n == 1 else _shift(a, n, axis = axis, **state))
 
 shift_.output = ['data', 'state']
         
@@ -897,22 +901,27 @@
     :Example:
     ---------
     >>> from pyg import *; import pandas as pd; import numpy as np
     >>> a = pd.Series([1.,2,3,4,5], drange(-4))
     >>> assert eq(ratio(a), pd.Series([np.nan, 2, 1.5, 4/3,1.25], drange(-4)))
     >>> assert eq(ratio(a,2), pd.Series([np.nan, np.nan, 3, 2, 5/3], drange(-4)))
     """
+    if is_num(a):
+        return 1
     state = state or Dict(vec = None, i = 0, t = np.nan)
     state.vec = _vec(a, state.vec, n, axis=axis)
     return first_(_tratio(a, n, axis = axis, time = time, **state))
 
-def ratio_(a, n=1, time = None, axis = 0, data = None, instate = None):
+def ratio_(a, n=1, time = None, axis = 0, data = None, instate = None):        
     state = instate or Dict(vec = None, i = 0, t = np.nan) 
     state.vec = _vec(a, state.vec, n, axis=axis)
-    return _data_state(['data', 'vec', 'i', 't'], _tratio(a, n, time = time, **state))
+    if is_num(a):
+        return Dict(data = 1, state = state)
+    else:
+        return _data_state(['data', 'vec', 'i', 't'], _tratio(a, n, time = time, **state))
 
 ratio_.output = ['data', 'state']
 
 
 def rolling_mean(a, n, time = None, axis = 0, data = None, state = None):
     """
     equivalent to pandas a.rolling(n).mean().
```

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_stride.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_stride.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_track.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_track.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_ts.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_ts.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries/_xrank.py` & `pyg-timeseries-0.0.8/src/pyg_timeseries/_xrank.py`

 * *Files identical despite different names*

### Comparing `pyg-timeseries-0.0.7/pyg_timeseries.egg-info/SOURCES.txt` & `pyg-timeseries-0.0.8/src/pyg_timeseries.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-setup.py
-pyg_timeseries/__init__.py
-pyg_timeseries/_bar.py
-pyg_timeseries/_decorators.py
-pyg_timeseries/_ewm.py
-pyg_timeseries/_ewmcombine.py
-pyg_timeseries/_ewmxo.py
-pyg_timeseries/_expanding.py
-pyg_timeseries/_iter.py
-pyg_timeseries/_linalg.py
-pyg_timeseries/_math.py
-pyg_timeseries/_max.py
-pyg_timeseries/_median.py
-pyg_timeseries/_min.py
-pyg_timeseries/_opt.py
-pyg_timeseries/_pandas.py
-pyg_timeseries/_rank.py
-pyg_timeseries/_rms_join.py
-pyg_timeseries/_rolling.py
-pyg_timeseries/_stride.py
-pyg_timeseries/_track.py
-pyg_timeseries/_ts.py
-pyg_timeseries/_xrank.py
-pyg_timeseries.egg-info/PKG-INFO
-pyg_timeseries.egg-info/SOURCES.txt
-pyg_timeseries.egg-info/dependency_links.txt
-pyg_timeseries.egg-info/top_level.txt
+LICENSE
+README.md
+pyproject.toml
+setup.cfg
+src/pyg_timeseries/__init__.py
+src/pyg_timeseries/_bar.py
+src/pyg_timeseries/_decorators.py
+src/pyg_timeseries/_ewm.py
+src/pyg_timeseries/_ewmcombine.py
+src/pyg_timeseries/_ewmxo.py
+src/pyg_timeseries/_expanding.py
+src/pyg_timeseries/_iter.py
+src/pyg_timeseries/_linalg.py
+src/pyg_timeseries/_math.py
+src/pyg_timeseries/_max.py
+src/pyg_timeseries/_median.py
+src/pyg_timeseries/_min.py
+src/pyg_timeseries/_multibuffer.py
+src/pyg_timeseries/_opt.py
+src/pyg_timeseries/_pandas.py
+src/pyg_timeseries/_rank.py
+src/pyg_timeseries/_rms_join.py
+src/pyg_timeseries/_rolling.py
+src/pyg_timeseries/_stride.py
+src/pyg_timeseries/_track.py
+src/pyg_timeseries/_ts.py
+src/pyg_timeseries/_xrank.py
+src/pyg_timeseries.egg-info/PKG-INFO
+src/pyg_timeseries.egg-info/SOURCES.txt
+src/pyg_timeseries.egg-info/dependency_links.txt
+src/pyg_timeseries.egg-info/requires.txt
+src/pyg_timeseries.egg-info/top_level.txt
```

