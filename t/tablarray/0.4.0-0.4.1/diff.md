# Comparing `tmp/tablarray-0.4.0.tar.gz` & `tmp/tablarray-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablarray-0.4.0.tar", last modified: Tue Jan 31 16:38:23 2023, max compression
+gzip compressed data, was "tablarray-0.4.1.tar", last modified: Thu Jun 15 03:45:59 2023, max compression
```

## Comparing `tablarray-0.4.0.tar` & `tablarray-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.775892 tablarray-0.4.0/
--rw-r-----   0 chris     (1000) chris     (1000)     1519 2021-01-04 01:15:28.000000 tablarray-0.4.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)    13073 2023-01-31 16:38:23.775892 tablarray-0.4.0/PKG-INFO
--rw-r-----   0 chris     (1000) chris     (1000)    12708 2022-05-21 19:08:11.000000 tablarray-0.4.0/README.rst
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-01-31 16:38:23.775892 tablarray-0.4.0/setup.cfg
--rw-r-----   0 chris     (1000) chris     (1000)     1168 2023-01-14 02:52:11.000000 tablarray-0.4.0/setup.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.771892 tablarray-0.4.0/tablarray/
--rw-r-----   0 chris     (1000) chris     (1000)      908 2023-01-07 18:42:26.000000 tablarray-0.4.0/tablarray/__init__.py
--rw-r-----   0 chris     (1000) chris     (1000)     1137 2021-10-13 02:09:36.000000 tablarray-0.4.0/tablarray/cmatmul.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.771892 tablarray-0.4.0/tablarray/kwtools/
--rw-r-----   0 chris     (1000) chris     (1000)      556 2021-01-31 00:49:29.000000 tablarray-0.4.0/tablarray/kwtools/__init__.py
--rw-r-----   0 chris     (1000) chris     (1000)     4497 2020-04-18 19:51:09.000000 tablarray-0.4.0/tablarray/kwtools/kwargs_db.py
--rw-r-----   0 chris     (1000) chris     (1000)     9668 2020-04-18 18:41:27.000000 tablarray-0.4.0/tablarray/kwtools/kwargs_scan.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.771892 tablarray-0.4.0/tablarray/linalg/
--rw-r-----   0 chris     (1000) chris     (1000)      172 2021-01-09 20:50:57.000000 tablarray-0.4.0/tablarray/linalg/__init__.py
--rw-r-----   0 chris     (1000) chris     (1000)      368 2023-01-20 17:53:23.000000 tablarray-0.4.0/tablarray/linalg/ax.py
--rw-r-----   0 chris     (1000) chris     (1000)     1599 2021-02-01 17:36:41.000000 tablarray-0.4.0/tablarray/linalg/mat1_r1.py
--rw-r-----   0 chris     (1000) chris     (1000)     1391 2021-02-01 17:36:49.000000 tablarray-0.4.0/tablarray/linalg/mat1_rn.py
--rw-r-----   0 chris     (1000) chris     (1000)     2482 2023-01-07 18:39:45.000000 tablarray-0.4.0/tablarray/misc.py
--rw-r-----   0 chris     (1000) chris     (1000)     3297 2022-01-17 00:33:40.000000 tablarray-0.4.0/tablarray/mmul.py
--rw-r-----   0 chris     (1000) chris     (1000)      868 2021-10-10 00:20:41.000000 tablarray-0.4.0/tablarray/mmul_sig.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.775892 tablarray-0.4.0/tablarray/np2ta/
--rw-r-----   0 chris     (1000) chris     (1000)      375 2020-06-17 01:46:06.000000 tablarray-0.4.0/tablarray/np2ta/__init__.py
--rw-r-----   0 chris     (1000) chris     (1000)      945 2021-02-01 17:35:27.000000 tablarray-0.4.0/tablarray/np2ta/ax2_op.py
--rw-r-----   0 chris     (1000) chris     (1000)     2647 2023-01-20 17:51:07.000000 tablarray-0.4.0/tablarray/np2ta/ax_op.py
--rw-r-----   0 chris     (1000) chris     (1000)     7408 2023-01-22 06:06:41.000000 tablarray-0.4.0/tablarray/np2ta/bin_op.py
--rw-r-----   0 chris     (1000) chris     (1000)     6685 2021-02-26 06:34:24.000000 tablarray-0.4.0/tablarray/np2ta/cbroadcast.py
--rw-r-----   0 chris     (1000) chris     (1000)     3044 2023-01-22 06:29:10.000000 tablarray-0.4.0/tablarray/np2ta/el_op.py
--rw-r-----   0 chris     (1000) chris     (1000)      437 2021-02-22 06:28:28.000000 tablarray-0.4.0/tablarray/np2ta/misc.py
--rw-r-----   0 chris     (1000) chris     (1000)      727 2020-06-16 17:25:20.000000 tablarray-0.4.0/tablarray/np2ta/new.py
--rw-r-----   0 chris     (1000) chris     (1000)      364 2020-05-18 20:04:02.000000 tablarray-0.4.0/tablarray/np2ta/op12swap.py
--rw-r-----   0 chris     (1000) chris     (1000)      811 2022-01-09 00:45:28.000000 tablarray-0.4.0/tablarray/np2ta/passwrap.py
--rw-r-----   0 chris     (1000) chris     (1000)     3268 2021-02-26 06:26:02.000000 tablarray-0.4.0/tablarray/re.py
--rw-r-----   0 chris     (1000) chris     (1000)    13708 2023-01-31 05:01:18.000000 tablarray-0.4.0/tablarray/set.py
--rw-r-----   0 chris     (1000) chris     (1000)    12835 2021-02-22 06:50:03.000000 tablarray-0.4.0/tablarray/solve.py
--rw-r-----   0 chris     (1000) chris     (1000)     8170 2021-03-01 01:11:23.000000 tablarray-0.4.0/tablarray/stack.py
--rw-r-----   0 chris     (1000) chris     (1000)    11414 2023-01-27 05:13:41.000000 tablarray-0.4.0/tablarray/ta.py
--rw-r-----   0 chris     (1000) chris     (1000)     8931 2023-01-29 21:38:19.000000 tablarray-0.4.0/tablarray/taplot.py
--rw-r-----   0 chris     (1000) chris     (1000)    14567 2021-02-01 17:34:12.000000 tablarray-0.4.0/tablarray/taprint.py
--rw-r-----   0 chris     (1000) chris     (1000)     2932 2023-01-22 03:05:17.000000 tablarray-0.4.0/tablarray/tashape.py
--rw-r-----   0 chris     (1000) chris     (1000)      151 2023-01-20 17:54:29.000000 tablarray-0.4.0/tablarray/version.py
--rw-r-----   0 chris     (1000) chris     (1000)      793 2021-02-01 17:34:28.000000 tablarray-0.4.0/tablarray/views.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-01-31 16:38:23.771892 tablarray-0.4.0/tablarray.egg-info/
--rw-r-----   0 chris     (1000) chris     (1000)    13073 2023-01-31 16:38:23.000000 tablarray-0.4.0/tablarray.egg-info/PKG-INFO
--rw-r-----   0 chris     (1000) chris     (1000)      946 2023-01-31 16:38:23.000000 tablarray-0.4.0/tablarray.egg-info/SOURCES.txt
--rw-r-----   0 chris     (1000) chris     (1000)        1 2023-01-31 16:38:23.000000 tablarray-0.4.0/tablarray.egg-info/dependency_links.txt
--rw-r-----   0 chris     (1000) chris     (1000)       23 2023-01-31 16:38:23.000000 tablarray-0.4.0/tablarray.egg-info/requires.txt
--rw-r-----   0 chris     (1000) chris     (1000)       10 2023-01-31 16:38:23.000000 tablarray-0.4.0/tablarray.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.745425 tablarray-0.4.1/
+-rw-r-----   0 chris     (1000) chris     (1000)     1519 2021-01-04 01:15:28.000000 tablarray-0.4.1/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)    13073 2023-06-15 03:45:59.745425 tablarray-0.4.1/PKG-INFO
+-rw-r-----   0 chris     (1000) chris     (1000)    12708 2022-05-21 19:08:11.000000 tablarray-0.4.1/README.rst
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-06-15 03:45:59.745425 tablarray-0.4.1/setup.cfg
+-rw-r-----   0 chris     (1000) chris     (1000)     1168 2023-01-14 02:52:11.000000 tablarray-0.4.1/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.741425 tablarray-0.4.1/tablarray/
+-rw-r-----   0 chris     (1000) chris     (1000)      908 2023-01-07 18:42:26.000000 tablarray-0.4.1/tablarray/__init__.py
+-rw-r-----   0 chris     (1000) chris     (1000)     1137 2021-10-13 02:09:36.000000 tablarray-0.4.1/tablarray/cmatmul.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.741425 tablarray-0.4.1/tablarray/kwtools/
+-rw-r-----   0 chris     (1000) chris     (1000)      556 2021-01-31 00:49:29.000000 tablarray-0.4.1/tablarray/kwtools/__init__.py
+-rw-r-----   0 chris     (1000) chris     (1000)     4497 2020-04-18 19:51:09.000000 tablarray-0.4.1/tablarray/kwtools/kwargs_db.py
+-rw-r-----   0 chris     (1000) chris     (1000)     9668 2020-04-18 18:41:27.000000 tablarray-0.4.1/tablarray/kwtools/kwargs_scan.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.741425 tablarray-0.4.1/tablarray/linalg/
+-rw-r-----   0 chris     (1000) chris     (1000)      172 2021-01-09 20:50:57.000000 tablarray-0.4.1/tablarray/linalg/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      368 2023-06-15 00:21:13.000000 tablarray-0.4.1/tablarray/linalg/ax.py
+-rw-r-----   0 chris     (1000) chris     (1000)     1599 2021-02-01 17:36:41.000000 tablarray-0.4.1/tablarray/linalg/mat1_r1.py
+-rw-r-----   0 chris     (1000) chris     (1000)     1391 2021-02-01 17:36:49.000000 tablarray-0.4.1/tablarray/linalg/mat1_rn.py
+-rw-r-----   0 chris     (1000) chris     (1000)     2482 2023-01-07 18:39:45.000000 tablarray-0.4.1/tablarray/misc.py
+-rw-r-----   0 chris     (1000) chris     (1000)     3297 2022-01-17 00:33:40.000000 tablarray-0.4.1/tablarray/mmul.py
+-rw-r-----   0 chris     (1000) chris     (1000)      868 2021-10-10 00:20:41.000000 tablarray-0.4.1/tablarray/mmul_sig.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.745425 tablarray-0.4.1/tablarray/np2ta/
+-rw-r-----   0 chris     (1000) chris     (1000)      375 2020-06-17 01:46:06.000000 tablarray-0.4.1/tablarray/np2ta/__init__.py
+-rw-r-----   0 chris     (1000) chris     (1000)      945 2021-02-01 17:35:27.000000 tablarray-0.4.1/tablarray/np2ta/ax2_op.py
+-rw-r-----   0 chris     (1000) chris     (1000)     2647 2023-01-20 17:51:07.000000 tablarray-0.4.1/tablarray/np2ta/ax_op.py
+-rw-r-----   0 chris     (1000) chris     (1000)     7408 2023-01-22 06:06:41.000000 tablarray-0.4.1/tablarray/np2ta/bin_op.py
+-rw-r-----   0 chris     (1000) chris     (1000)     6685 2021-02-26 06:34:24.000000 tablarray-0.4.1/tablarray/np2ta/cbroadcast.py
+-rw-r-----   0 chris     (1000) chris     (1000)     3044 2023-01-22 06:29:10.000000 tablarray-0.4.1/tablarray/np2ta/el_op.py
+-rw-r-----   0 chris     (1000) chris     (1000)      437 2021-02-22 06:28:28.000000 tablarray-0.4.1/tablarray/np2ta/misc.py
+-rw-r-----   0 chris     (1000) chris     (1000)      727 2020-06-16 17:25:20.000000 tablarray-0.4.1/tablarray/np2ta/new.py
+-rw-r-----   0 chris     (1000) chris     (1000)      364 2020-05-18 20:04:02.000000 tablarray-0.4.1/tablarray/np2ta/op12swap.py
+-rw-r-----   0 chris     (1000) chris     (1000)      811 2022-01-09 00:45:28.000000 tablarray-0.4.1/tablarray/np2ta/passwrap.py
+-rw-r-----   0 chris     (1000) chris     (1000)     3268 2021-02-26 06:26:02.000000 tablarray-0.4.1/tablarray/re.py
+-rw-r-----   0 chris     (1000) chris     (1000)    13712 2023-02-10 04:31:44.000000 tablarray-0.4.1/tablarray/set.py
+-rw-r-----   0 chris     (1000) chris     (1000)    12835 2021-02-22 06:50:03.000000 tablarray-0.4.1/tablarray/solve.py
+-rw-r-----   0 chris     (1000) chris     (1000)     8170 2021-03-01 01:11:23.000000 tablarray-0.4.1/tablarray/stack.py
+-rw-r-----   0 chris     (1000) chris     (1000)    11413 2023-06-15 00:09:43.000000 tablarray-0.4.1/tablarray/ta.py
+-rw-r-----   0 chris     (1000) chris     (1000)    11050 2023-06-14 17:53:17.000000 tablarray-0.4.1/tablarray/taplot.py
+-rw-r-----   0 chris     (1000) chris     (1000)    14567 2021-02-01 17:34:12.000000 tablarray-0.4.1/tablarray/taprint.py
+-rw-r-----   0 chris     (1000) chris     (1000)     3013 2023-06-13 22:04:04.000000 tablarray-0.4.1/tablarray/tashape.py
+-rw-r-----   0 chris     (1000) chris     (1000)      151 2023-06-13 20:24:04.000000 tablarray-0.4.1/tablarray/version.py
+-rw-r-----   0 chris     (1000) chris     (1000)      793 2021-02-01 17:34:28.000000 tablarray-0.4.1/tablarray/views.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-06-15 03:45:59.741425 tablarray-0.4.1/tablarray.egg-info/
+-rw-r-----   0 chris     (1000) chris     (1000)    13073 2023-06-15 03:45:59.000000 tablarray-0.4.1/tablarray.egg-info/PKG-INFO
+-rw-r-----   0 chris     (1000) chris     (1000)      946 2023-06-15 03:45:59.000000 tablarray-0.4.1/tablarray.egg-info/SOURCES.txt
+-rw-r-----   0 chris     (1000) chris     (1000)        1 2023-06-15 03:45:59.000000 tablarray-0.4.1/tablarray.egg-info/dependency_links.txt
+-rw-r-----   0 chris     (1000) chris     (1000)       23 2023-06-15 03:45:59.000000 tablarray-0.4.1/tablarray.egg-info/requires.txt
+-rw-r-----   0 chris     (1000) chris     (1000)       10 2023-06-15 03:45:59.000000 tablarray-0.4.1/tablarray.egg-info/top_level.txt
```

### Comparing `tablarray-0.4.0/LICENSE` & `tablarray-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/PKG-INFO` & `tablarray-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablarray
-Version: 0.4.0
+Version: 0.4.1
 Summary: Extend broadcasting rules of numpy to abstract tabularshape of data from cellular shape
 Home-page: https://github.com/chriscannon9001/tablarray
 Author: Chris Cannon
 Author-email: chris.cannon.9001@gmail.com
 License: BSD
 Requires-Python: >=3.2
 Description-Content-Type: text/x-rst
```

### Comparing `tablarray-0.4.0/README.rst` & `tablarray-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/setup.py` & `tablarray-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/__init__.py` & `tablarray-0.4.1/tablarray/__init__.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/cmatmul.py` & `tablarray-0.4.1/tablarray/cmatmul.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/kwtools/__init__.py` & `tablarray-0.4.1/tablarray/kwtools/__init__.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/kwtools/kwargs_db.py` & `tablarray-0.4.1/tablarray/kwtools/kwargs_db.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/kwtools/kwargs_scan.py` & `tablarray-0.4.1/tablarray/kwtools/kwargs_scan.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/linalg/mat1_r1.py` & `tablarray-0.4.1/tablarray/linalg/mat1_r1.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/linalg/mat1_rn.py` & `tablarray-0.4.1/tablarray/linalg/mat1_rn.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/misc.py` & `tablarray-0.4.1/tablarray/misc.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/mmul.py` & `tablarray-0.4.1/tablarray/mmul.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/mmul_sig.py` & `tablarray-0.4.1/tablarray/mmul_sig.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/ax2_op.py` & `tablarray-0.4.1/tablarray/np2ta/ax2_op.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/ax_op.py` & `tablarray-0.4.1/tablarray/np2ta/ax_op.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/bin_op.py` & `tablarray-0.4.1/tablarray/np2ta/bin_op.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/cbroadcast.py` & `tablarray-0.4.1/tablarray/np2ta/cbroadcast.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/el_op.py` & `tablarray-0.4.1/tablarray/np2ta/el_op.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/new.py` & `tablarray-0.4.1/tablarray/np2ta/new.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/np2ta/passwrap.py` & `tablarray-0.4.1/tablarray/np2ta/passwrap.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/re.py` & `tablarray-0.4.1/tablarray/re.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/set.py` & `tablarray-0.4.1/tablarray/set.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
         xdata : dict
             N, int, length of axis
             sign, +1/-1, indicates ascending or descending order
             beg, end, first and last value of the axis
         """
         isaxis = np.logical_not(self.degeneracy(key))
         if np.sum(isaxis) != 1:
-            return None
+            return None, {}
         ax_dim = np.nonzero(isaxis)[0][0]
         # plus a little useful intel
         N = self.ts.tshape[ax_dim]
         axis = self[key]
         beg = axis.ravel()[0]
         end = axis.ravel()[-1]
         sign = np.sign(end - beg)
```

### Comparing `tablarray-0.4.0/tablarray/solve.py` & `tablarray-0.4.1/tablarray/solve.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/stack.py` & `tablarray-0.4.1/tablarray/stack.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/ta.py` & `tablarray-0.4.1/tablarray/ta.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     a : numpy.ndarray (or list or tuple)
         an Array to wrap
     cdim : int (0,1,2)
         cellular dim; normally 0 - scalar, 1 - vector, 2 - matrix
         or taShapes type
     """
 
-    def __init__(self, a, cdim, view='table'):
+    def __init__(self, a, cdim, view='cell'):
         # ensure type of self.base
         if isinstance(a, np.ndarray):
             self.base = a          # based on ndarray
         elif misc.istablarray(a):
             self.base = a.base    # based on ATC type
             cdim = a.ts
         else:
```

### Comparing `tablarray-0.4.0/tablarray/taprint.py` & `tablarray-0.4.1/tablarray/taprint.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray/tashape.py` & `tablarray-0.4.1/tablarray/tashape.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     def cslice(self, indices):
         """align slice indices only to the cellular structure,
         spanning :,... across all tabular dimensions"""
         cslice = indices
         # calculate cdim for cellular aligned slice
         cdim = self.cdim
         for idx in cslice:
-            if idx != slice(None):
+            #if idx != slice(None):  # FIXME: dim doesn't drop for any slice
+            if type(idx) is not slice:
                 cdim -= 1
         assert len(cslice) <= self.cdim, (
                 'got len(*cslice)==%d instead of required <=%d'
                 % (len(cslice), self.cdim))
         tspan = [slice(None)] * self.tdim
         spanning_slice = tspan + cslice
         return spanning_slice, cdim
```

### Comparing `tablarray-0.4.0/tablarray/views.py` & `tablarray-0.4.1/tablarray/views.py`

 * *Files identical despite different names*

### Comparing `tablarray-0.4.0/tablarray.egg-info/PKG-INFO` & `tablarray-0.4.1/tablarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablarray
-Version: 0.4.0
+Version: 0.4.1
 Summary: Extend broadcasting rules of numpy to abstract tabularshape of data from cellular shape
 Home-page: https://github.com/chriscannon9001/tablarray
 Author: Chris Cannon
 Author-email: chris.cannon.9001@gmail.com
 License: BSD
 Requires-Python: >=3.2
 Description-Content-Type: text/x-rst
```

### Comparing `tablarray-0.4.0/tablarray.egg-info/SOURCES.txt` & `tablarray-0.4.1/tablarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

