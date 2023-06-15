# Comparing `tmp/pyg-cell-0.0.8.tar.gz` & `tmp/pyg-cell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg-cell-0.0.8.tar", last modified: Fri Jul 29 18:46:11 2022, max compression
+gzip compressed data, was "pyg-cell-0.0.9.tar", last modified: Fri Jul 29 19:15:35 2022, max compression
```

## Comparing `pyg-cell-0.0.8.tar` & `pyg-cell-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-29 18:46:11.164286 pyg-cell-0.0.8/
--rw-rw-rw-   0        0        0    35803 2022-07-21 07:45:47.000000 pyg-cell-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      747 2022-07-29 18:46:11.165286 pyg-cell-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      201 2022-07-21 07:45:47.000000 pyg-cell-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2022-07-21 07:45:47.000000 pyg-cell-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      726 2022-07-29 18:46:11.167284 pyg-cell-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-29 18:46:11.126147 pyg-cell-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-07-29 18:46:11.145286 pyg-cell-0.0.8/src/pyg_cell/
--rw-rw-rw-   0        0        0      652 2022-07-24 14:11:30.000000 pyg-cell-0.0.8/src/pyg_cell/__init__.py
--rw-rw-rw-   0        0        0     9063 2022-07-22 16:22:47.000000 pyg-cell-0.0.8/src/pyg_cell/_acell.py
--rw-rw-rw-   0        0        0     5186 2022-07-29 18:45:14.000000 pyg-cell-0.0.8/src/pyg_cell/_cache.py
--rw-rw-rw-   0        0        0    35211 2022-07-24 14:44:07.000000 pyg-cell-0.0.8/src/pyg_cell/_cell.py
--rw-rw-rw-   0        0        0     7148 2022-07-22 15:46:15.000000 pyg-cell-0.0.8/src/pyg_cell/_dag.py
--rw-rw-rw-   0        0        0    28184 2022-07-24 14:50:47.000000 pyg-cell-0.0.8/src/pyg_cell/_db_cell.py
--rw-rw-rw-   0        0        0     1402 2022-07-24 12:25:19.000000 pyg-cell-0.0.8/src/pyg_cell/_latest_cell.py
--rw-rw-rw-   0        0        0     2203 2022-07-21 07:45:47.000000 pyg-cell-0.0.8/src/pyg_cell/_periodic_cell.py
--rw-rw-rw-   0        0        0     3750 2022-07-28 06:26:48.000000 pyg-cell-0.0.8/src/pyg_cell/_tree.py
--rw-rw-rw-   0        0        0     1239 2022-07-29 14:52:57.000000 pyg-cell-0.0.8/src/pyg_cell/_types.py
--rw-rw-rw-   0        0        0     5182 2022-07-21 07:45:47.000000 pyg-cell-0.0.8/src/pyg_cell/app.py
-drwxrwxrwx   0        0        0        0 2022-07-29 18:46:11.163283 pyg-cell-0.0.8/src/pyg_cell.egg-info/
--rw-rw-rw-   0        0        0      747 2022-07-29 18:46:11.000000 pyg-cell-0.0.8/src/pyg_cell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2022-07-29 18:46:11.000000 pyg-cell-0.0.8/src/pyg_cell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-29 18:46:11.000000 pyg-cell-0.0.8/src/pyg_cell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-07-29 18:46:11.000000 pyg-cell-0.0.8/src/pyg_cell.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-29 18:46:11.000000 pyg-cell-0.0.8/src/pyg_cell.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-29 19:15:35.437167 pyg-cell-0.0.9/
+-rw-rw-rw-   0        0        0    35803 2022-07-21 07:45:47.000000 pyg-cell-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      747 2022-07-29 19:15:35.437167 pyg-cell-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2022-07-21 07:45:47.000000 pyg-cell-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2022-07-21 07:45:47.000000 pyg-cell-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      726 2022-07-29 19:15:35.446169 pyg-cell-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-07-29 19:15:35.393612 pyg-cell-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-07-29 19:15:35.412981 pyg-cell-0.0.9/src/pyg_cell/
+-rw-rw-rw-   0        0        0      652 2022-07-24 14:11:30.000000 pyg-cell-0.0.9/src/pyg_cell/__init__.py
+-rw-rw-rw-   0        0        0     9063 2022-07-22 16:22:47.000000 pyg-cell-0.0.9/src/pyg_cell/_acell.py
+-rw-rw-rw-   0        0        0     5517 2022-07-29 19:04:56.000000 pyg-cell-0.0.9/src/pyg_cell/_cache.py
+-rw-rw-rw-   0        0        0    35211 2022-07-24 14:44:07.000000 pyg-cell-0.0.9/src/pyg_cell/_cell.py
+-rw-rw-rw-   0        0        0     7148 2022-07-22 15:46:15.000000 pyg-cell-0.0.9/src/pyg_cell/_dag.py
+-rw-rw-rw-   0        0        0    28184 2022-07-24 14:50:47.000000 pyg-cell-0.0.9/src/pyg_cell/_db_cell.py
+-rw-rw-rw-   0        0        0     1402 2022-07-24 12:25:19.000000 pyg-cell-0.0.9/src/pyg_cell/_latest_cell.py
+-rw-rw-rw-   0        0        0     2203 2022-07-21 07:45:47.000000 pyg-cell-0.0.9/src/pyg_cell/_periodic_cell.py
+-rw-rw-rw-   0        0        0     3750 2022-07-28 06:26:48.000000 pyg-cell-0.0.9/src/pyg_cell/_tree.py
+-rw-rw-rw-   0        0        0     1239 2022-07-29 14:52:57.000000 pyg-cell-0.0.9/src/pyg_cell/_types.py
+-rw-rw-rw-   0        0        0     5182 2022-07-21 07:45:47.000000 pyg-cell-0.0.9/src/pyg_cell/app.py
+drwxrwxrwx   0        0        0        0 2022-07-29 19:15:35.436231 pyg-cell-0.0.9/src/pyg_cell.egg-info/
+-rw-rw-rw-   0        0        0      747 2022-07-29 19:15:35.000000 pyg-cell-0.0.9/src/pyg_cell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2022-07-29 19:15:35.000000 pyg-cell-0.0.9/src/pyg_cell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-29 19:15:35.000000 pyg-cell-0.0.9/src/pyg_cell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2022-07-29 19:15:35.000000 pyg-cell-0.0.9/src/pyg_cell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-07-29 19:15:35.000000 pyg-cell-0.0.9/src/pyg_cell.egg-info/top_level.txt
```

### Comparing `pyg-cell-0.0.8/LICENSE` & `pyg-cell-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/PKG-INFO` & `pyg-cell-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-cell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for data manipulation including creation of DAGs and tables
 Home-page: https://github.com/gityoav/pyg-cell
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-cell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyg-cell-0.0.8/setup.cfg` & `pyg-cell-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7967 2d63 656c 6c0d 0a76 6572   = pyg-cell..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 2059 6f61 7620 4769 740d  thor = Yoav Git.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 796f 6176 2e67 6974 4067 6d61 696c 2e63  yoav.git@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 5574 696c 6974 6965 7320 666f 7220  = Utilities for 
 00000080: 6461 7461 206d 616e 6970 756c 6174 696f  data manipulatio
 00000090: 6e20 696e 636c 7564 696e 6720 6372 6561  n including crea
```

### Comparing `pyg-cell-0.0.8/src/pyg_cell/__init__.py` & `pyg-cell-0.0.9/src/pyg_cell/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_acell.py` & `pyg-cell-0.0.9/src/pyg_cell/_acell.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_cache.py` & `pyg-cell-0.0.9/src/pyg_cell/_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,22 @@
     >>> assert f(1,2).data == 3
 
     >>> @cell_cache(pk = 'key')
     >>> def f(a,b):
     >>>     return a+b
     >>> f(1,2, key = 'key', go = 1)
 
+
+    >>> from pyg import * 
+    >>> @cell_cache(db = 'test', table = 'tbl', schema = 'bbg', pk = ['ticker', 'field'], 
+                    writer = 'mss://true?schema=bbg/db_data/%ticker/%field.sql')
+    >>> def bdh(ticker, field):
+    >>>     return pd.Series(np.random.normal(100), drange(-99))
     
+    >>> ts = bdh('a', 'd')
     """
     def __init__(self, function = None, db = 'cache', schema = None, table = None, url = None, server = None, pk = None, cell = periodic_cell, writer = None, cell_kwargs = None, external = None):
         cell_kwargs  = cell_kwargs or {}
         db_kwargs = dict(pk = pk, db = db, table = table, schema = schema, url = url, server = server, writer = writer)
         if isinstance(db, partial):
             db_kwargs.update(db.keywords)
         super(cell_cache, self).__init__(function = function, cell = cell, cell_kwargs = cell_kwargs, external = external, **db_kwargs)
@@ -102,17 +109,17 @@
         else:
             return self.table
     
     @property
     def _db(self):
         mode = _get_db(self.url, self.server, self.schema)
         if mode == 'mongo':    
-            return partial(DBS[mode], table = self._table, db = self.db, pk = self._pk, url = self.url or self.server, writer = self.writer, doc = True)
+            return partial(DBS[mode], table = self._table, db = self.db, pk = self._pk, url = self.url or self.server, writer = self.writer)
         elif mode == 'sql':
-            return partial(DBS[mode], table = self._table, schema = self.schema, db = self.db, pk = self._pk, server = self.server or self.url, writer = self.writer)
+            return partial(DBS[mode], table = self._table, schema = self.schema, db = self.db, pk = self._pk, server = self.server or self.url, writer = self.writer, doc = True)
         else:
             raise ValueError('only sql or mongo are supported')            
     
     def _external_kwargs(self, args, kwargs):
         external = self._external
         external_kwargs = {key : value for key, value in kwargs.items() if key in external}
         kwargs = {key : value for key, value in kwargs.items() if key not in external}
```

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_cell.py` & `pyg-cell-0.0.9/src/pyg_cell/_cell.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_dag.py` & `pyg-cell-0.0.9/src/pyg_cell/_dag.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_db_cell.py` & `pyg-cell-0.0.9/src/pyg_cell/_db_cell.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_latest_cell.py` & `pyg-cell-0.0.9/src/pyg_cell/_latest_cell.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_periodic_cell.py` & `pyg-cell-0.0.9/src/pyg_cell/_periodic_cell.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_tree.py` & `pyg-cell-0.0.9/src/pyg_cell/_tree.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/_types.py` & `pyg-cell-0.0.9/src/pyg_cell/_types.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell/app.py` & `pyg-cell-0.0.9/src/pyg_cell/app.py`

 * *Files identical despite different names*

### Comparing `pyg-cell-0.0.8/src/pyg_cell.egg-info/PKG-INFO` & `pyg-cell-0.0.9/src/pyg_cell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-cell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for data manipulation including creation of DAGs and tables
 Home-page: https://github.com/gityoav/pyg-cell
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-cell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

