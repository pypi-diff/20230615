# Comparing `tmp/scinumtools-1.2.2.tar.gz` & `tmp/scinumtools-1.2.3.tar.gz`

## Comparing `scinumtools-1.2.2.tar` & `scinumtools-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.2/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.2.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/units/DIP_Solver_Units.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.2.2/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/cached_data.npy
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/test_data.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/test_struct.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.2.2/tests/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.2.2/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.2.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.3/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/DIP_Solver_Units.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/cached_data.npy
+-rw-r--r--   0        0        0     6211 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_data.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_struct.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.2.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.2.3/PKG-INFO
```

### Comparing `scinumtools-1.2.2/.github/workflows/python-publish.yml` & `scinumtools-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/data/ImageClass.py` & `scinumtools-1.2.3/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.2.3/src/scinumtools/data/PlottingClass.py`

 * *Files 20% similar despite different names*

```diff
@@ -101,24 +101,43 @@
         """ Return logarithmic norm from ranges
         """
         return LogNorm(
             vmin=np.log10(np.nanmin(self._collector.zminpos)), 
             vmax=np.log10(np.nanmax(self._collector.zmax))
         )
 
-def ListToGrid(data, ncols, missing=None):
+def ListToGrid(data, ncols, missing=None, transpose=False):
     """
     Enumerate given data with an index and row/column number specified by number of columns
 
-    :param data: Any iterable data, e.g. list, array
+    :param list data: Any iterable data, e.g. list, array
     :param int ncols: Number of grid columns
     :param bool missing: List only missing grid points
+    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
     """
+    ndata = len(data)
+    nrows = int(np.ceil(ndata/ncols))
     if missing:
-        ndata = len(data)
-        nrows = int(np.ceil(ndata/ncols))
-        for i in range(ndata,ncols*nrows):
-            yield (i,int(i/ncols),int(i%ncols))        
+        for i in range(ndata, ncols*nrows):
+            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
     else:
         for i,d in enumerate(data):
-            yield (i,int(i/ncols),int(i%ncols),d)
+            yield (i,int(i%nrows),int(i/nrows),d) if transpose else (i,int(i/ncols),int(i%ncols),d)
+    
+def DictToGrid(data, ncols, missing=None, transpose=False):
+    """
+    Enumerate given data with an index and row/column number specified by number of columns
+
+    :param dict data: A Python dictionary with keys and values
+    :param int ncols: Number of grid columns
+    :param bool missing: List only missing grid points
+    :param bool transpose: Transpose grid layout from horizontal to vertical arrangement
+    """
+    ndata = len(data)
+    nrows = int(np.ceil(ndata/ncols))
+    if missing:
+        for i in range(ndata, ncols*nrows):
+            yield (i,int(i%nrows),int(i/nrows)) if transpose else (i,int(i/ncols),int(i%ncols))
+    else:
+        for i,(k,v) in enumerate(data.items()):
+            yield (i,int(i%nrows),int(i/nrows),k,v) if transpose else (i,int(i/ncols),int(i%ncols),k,v)
```

### Comparing `scinumtools-1.2.2/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.2.3/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/phys/units/DIP_Solver_Units.py` & `scinumtools-1.2.3/src/scinumtools/phys/units/DIP_Solver_Units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.2.3/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.2.3/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.2.3/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.2.3/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.2.3/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/tests/test_data.py` & `scinumtools-1.2.3/tests/test_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,34 +73,101 @@
     assert xranges.max == 9
     assert yranges.minpos == 0.10526315789473673
     assert yranges.min == -18
     assert yranges.max == 18
     
 def test_list_to_grid():
 
-    data = range(7)
+    data = range(5)
     ncols = 2
+    
+    # List all defined grid points
     grid = [
         (0, 0, 0, 0),
         (1, 0, 1, 1),
         (2, 1, 0, 2),
         (3, 1, 1, 3),
         (4, 2, 0, 4),
-        (5, 2, 1, 5),
-        (6, 3, 0, 6)
     ]
     for r,row in enumerate(ListToGrid(data,ncols)):
         assert grid[r] == row
+
+    # List all missing grid points
     grid = [
-        (7, 3, 1)
+        (5, 2, 1)
     ]
     for r,row in enumerate(ListToGrid(data,ncols,missing=True)):
         print(r,row)
         assert grid[r] == row
+
+    # List transposed grid points
+    grid = [
+        (0, 0, 0, 0),
+        (1, 1, 0, 1),
+        (2, 2, 0, 2),
+        (3, 0, 1, 3),
+        (4, 1, 1, 4),
+    ]
+    for r,row in enumerate(ListToGrid(data,ncols,transpose=True)):
+        assert grid[r] == row
+        
+    # List all missing transposed grid points
+    grid = [
+        (5, 2, 1)
+    ]
+    for r,row in enumerate(ListToGrid(data,ncols,transpose=True,missing=True)):
+        assert grid[r] == row
+        
+def test_dict_to_grid():
+
+    data = dict(
+        a = 0,
+        b = 1,
+        c = 2,
+        d = 3,
+        e = 4
+    )
+    ncols = 2
     
+    # List all defined grid points
+    grid = [
+        (0, 0, 0, 'a', 0),
+        (1, 0, 1, 'b', 1),
+        (2, 1, 0, 'c', 2),
+        (3, 1, 1, 'd', 3),
+        (4, 2, 0, 'e', 4),
+    ]
+    for r,row in enumerate(DictToGrid(data,ncols)):
+        assert grid[r] == row
+
+    # List all missing grid points
+    grid = [
+        (5, 2, 1)
+    ]
+    for r,row in enumerate(DictToGrid(data,ncols,missing=True)):
+        assert grid[r] == row
+        
+    # List all transposed grid points
+    grid = [
+        (0, 0, 0, 'a', 0),
+        (1, 1, 0, 'b', 1),
+        (2, 2, 0, 'c', 2),
+        (3, 0, 1, 'd', 3),
+        (4, 1, 1, 'e', 4),
+    ]
+    for r,row in enumerate(DictToGrid(data,ncols,transpose=True)):
+        assert grid[r] == row
+
+    # List all missing transposed grid points
+    grid = [
+        (5, 2, 1)
+    ]
+    for r,row in enumerate(DictToGrid(data,ncols,transpose=True,missing=True)):
+        assert grid[r] == row
+        
 def test_thumbnail():
 
     # Test grayscale case
     nx, ny = 300, 200
     data = np.zeros((nx,ny))
     for i in range(nx):
         for j in range(ny):
```

### Comparing `scinumtools-1.2.2/tests/test_stats.py` & `scinumtools-1.2.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/tests/test_struct.py` & `scinumtools-1.2.3/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/tests/test_units.py` & `scinumtools-1.2.3/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/.gitignore` & `scinumtools-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.2/pyproject.toml` & `scinumtools-1.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.2.2/PKG-INFO` & `scinumtools-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.2.2
+Version: 1.2.3
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

