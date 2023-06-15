# Comparing `tmp/py3d-0.1.2.tar.gz` & `tmp/py3d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.2.tar", last modified: Wed Jun 14 01:21:24 2023, max compression
+gzip compressed data, was "py3d-0.1.3.tar", last modified: Thu Jun 15 01:10:55 2023, max compression
```

## Comparing `py3d-0.1.2.tar` & `py3d-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.702869 py3d-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-14 01:21:24.702869 py3d-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-14 01:21:03.000000 py3d-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.698869 py3d-0.1.2/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28565 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-14 01:20:17.000000 py3d-0.1.2/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 01:21:24.702869 py3d-0.1.2/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-14 01:21:24.000000 py3d-0.1.2/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 01:21:24.702869 py3d-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-14 01:20:17.000000 py3d-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.788986 py3d-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-15 01:10:55.788986 py3d-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-15 01:10:34.000000 py3d-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.784986 py3d-0.1.3/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28901 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-15 01:09:50.000000 py3d-0.1.3/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 01:10:55.788986 py3d-0.1.3/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-15 01:10:55.000000 py3d-0.1.3/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 01:10:55.788986 py3d-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-15 01:09:50.000000 py3d-0.1.3/setup.py
```

### Comparing `py3d-0.1.2/PKG-INFO` & `py3d-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.2
+Version: 0.1.3
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.2/README.md` & `py3d-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.2/py3d/core.py` & `py3d-0.1.3/py3d/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         base_dims = len(self.BASE_SHAPE)
         if base_dims:
             return self.shape[:-base_dims]
         else:
             return self.shape
 
     @classmethod
-    def rand(cls, *n) -> Vector:
+    def rand(cls, *n) -> Vector | Vector2 | Vector3 | Vector4:
         n += cls.BASE_SHAPE
         return numpy.random.rand(*n).view(cls)
 
     def to_csv(self, path):
         numpy.savetxt(path, self, delimiter=',')
 
     @property
@@ -871,16 +871,25 @@
         self[..., 3:7] = v
 
     def paint(self, color):
         self.color = color
         return self
 
     def __add__(self, v: Point) -> Point:
-        assert self.TYPE == v.TYPE, "Different TYPE"
-        return numpy.concatenate((self, v), axis=0).view(self.__class__)
+        '''
+        Concatenate two Point
+        '''
+        assert self.TYPE == v.TYPE, f"Different TYPE {self.TYPE}, {v.TYPE}"
+        assert self.shape[1:] == v.shape[1:
+                                         ], f"Different shape {self.shape[1:-1]}, {v.shape[1:-1]}"
+        return numpy.concatenate((self, v), axis=0).view(Point)
+
+    def __iadd__(self, v: Point) -> Point:
+        self = self.__add__(v)
+        return self
 
     def __matmul__(self, transform: Transform) -> Point:
         vertex = self.xyz @ transform
         ret = self.__class__(*vertex.n)
         ret.xyz = vertex
         return ret
```

### Comparing `py3d-0.1.2/py3d/viewer.html` & `py3d-0.1.3/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.1.2/py3d.egg-info/PKG-INFO` & `py3d-0.1.3/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.2
+Version: 0.1.3
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.2/setup.py` & `py3d-0.1.3/setup.py`

 * *Files identical despite different names*

