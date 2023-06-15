# Comparing `tmp/surfa-0.4.2.tar.gz` & `tmp/surfa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfa-0.4.2.tar", last modified: Tue Feb 14 04:36:28 2023, max compression
+gzip compressed data, was "surfa-0.5.0.tar", last modified: Thu Jun 15 16:05:51 2023, max compression
```

## Comparing `surfa-0.4.2.tar` & `surfa-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.485651 surfa-0.4.2/
--rw-r--r--   0 andrew     (501) staff       (20)      870 2023-02-14 04:36:28.485522 surfa-0.4.2/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)       69 2023-02-14 04:36:07.000000 surfa-0.4.2/pyproject.toml
--rw-r--r--   0 andrew     (501) staff       (20)       38 2023-02-14 04:36:28.485691 surfa-0.4.2/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     2924 2023-02-14 04:36:07.000000 surfa-0.4.2/setup.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.479237 surfa-0.4.2/surfa/
--rw-r--r--   0 andrew     (501) staff       (20)      664 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/__init__.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.480572 surfa-0.4.2/surfa/core/
--rw-r--r--   0 andrew     (501) staff       (20)      123 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3799 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/array.py
--rw-r--r--   0 andrew     (501) staff       (20)    18363 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)      755 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/istype.py
--rw-r--r--   0 andrew     (501) staff       (20)     8479 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/labels.py
--rw-r--r--   0 andrew     (501) staff       (20)     4291 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/core/slicing.py
--rw-r--r--   0 andrew     (501) staff       (20)    15410 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/freesurfer.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.480922 surfa-0.4.2/surfa/image/
--rw-r--r--   0 andrew     (501) staff       (20)      116 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/image/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    37550 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/image/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)  3167162 2023-02-14 04:36:27.000000 surfa-0.4.2/surfa/image/interp.c
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.483360 surfa-0.4.2/surfa/io/
--rw-r--r--   0 andrew     (501) staff       (20)      236 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     4966 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/affine.py
--rw-r--r--   0 andrew     (501) staff       (20)    25706 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/framed.py
--rw-r--r--   0 andrew     (501) staff       (20)     6620 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/fsio.py
--rw-r--r--   0 andrew     (501) staff       (20)     3848 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/labels.py
--rw-r--r--   0 andrew     (501) staff       (20)    12464 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/mesh.py
--rw-r--r--   0 andrew     (501) staff       (20)     2773 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/protocol.py
--rw-r--r--   0 andrew     (501) staff       (20)     2233 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/io/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.484417 surfa-0.4.2/surfa/mesh/
--rw-r--r--   0 andrew     (501) staff       (20)       86 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3003 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/cache.py
--rw-r--r--   0 andrew     (501) staff       (20)   276816 2023-02-14 04:36:27.000000 surfa-0.4.2/surfa/mesh/intersection.c
--rw-r--r--   0 andrew     (501) staff       (20)     9567 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/intersection.h
--rw-r--r--   0 andrew     (501) staff       (20)    27761 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/mesh.py
--rw-r--r--   0 andrew     (501) staff       (20)     1339 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/overlay.py
--rw-r--r--   0 andrew     (501) staff       (20)     1827 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/ray.py
--rw-r--r--   0 andrew     (501) staff       (20)    10565 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/mesh/sphere.py
--rw-r--r--   0 andrew     (501) staff       (20)     5711 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/pipeline.py
--rw-r--r--   0 andrew     (501) staff       (20)     3719 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/system.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.485005 surfa-0.4.2/surfa/transform/
--rw-r--r--   0 andrew     (501) staff       (20)      369 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/transform/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    22054 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/transform/affine.py
--rw-r--r--   0 andrew     (501) staff       (20)    17535 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/transform/geometry.py
--rw-r--r--   0 andrew     (501) staff       (20)     3589 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/transform/orientation.py
--rw-r--r--   0 andrew     (501) staff       (20)     2193 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/transform/space.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.485234 surfa-0.4.2/surfa/vis/
--rw-r--r--   0 andrew     (501) staff       (20)       56 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/vis/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    10570 2023-02-14 04:36:07.000000 surfa-0.4.2/surfa/vis/freeview.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.479834 surfa-0.4.2/surfa.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)      870 2023-02-14 04:36:28.000000 surfa-0.4.2/surfa.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      962 2023-02-14 04:36:28.000000 surfa-0.4.2/surfa.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-02-14 04:36:28.000000 surfa-0.4.2/surfa.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       39 2023-02-14 04:36:28.000000 surfa-0.4.2/surfa.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)        6 2023-02-14 04:36:28.000000 surfa-0.4.2/surfa.egg-info/top_level.txt
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-02-14 04:36:28.485349 surfa-0.4.2/test/
--rw-r--r--   0 andrew     (501) staff       (20)     8354 2023-02-14 04:36:07.000000 surfa-0.4.2/test/test_framed.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.205039 surfa-0.5.0/
+-rw-r--r--   0 andrew     (501) staff       (20)      870 2023-06-15 16:05:51.204927 surfa-0.5.0/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)       69 2023-06-15 16:05:37.000000 surfa-0.5.0/pyproject.toml
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-15 16:05:51.205074 surfa-0.5.0/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     2924 2023-06-15 16:05:37.000000 surfa-0.5.0/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.198626 surfa-0.5.0/surfa/
+-rw-r--r--   0 andrew     (501) staff       (20)      664 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/__init__.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.199905 surfa-0.5.0/surfa/core/
+-rw-r--r--   0 andrew     (501) staff       (20)      123 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3974 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/array.py
+-rw-r--r--   0 andrew     (501) staff       (20)    18376 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)      755 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/istype.py
+-rw-r--r--   0 andrew     (501) staff       (20)     8479 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/labels.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6084 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/core/slicing.py
+-rw-r--r--   0 andrew     (501) staff       (20)    15408 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/freesurfer.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.200245 surfa-0.5.0/surfa/image/
+-rw-r--r--   0 andrew     (501) staff       (20)      116 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/image/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    38553 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/image/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)  3167456 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa/image/interp.c
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.202847 surfa-0.5.0/surfa/io/
+-rw-r--r--   0 andrew     (501) staff       (20)      236 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     4966 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/affine.py
+-rw-r--r--   0 andrew     (501) staff       (20)    25706 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/framed.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6620 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/fsio.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3848 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/labels.py
+-rw-r--r--   0 andrew     (501) staff       (20)    12464 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/mesh.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2773 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/protocol.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2233 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/io/utils.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.203791 surfa-0.5.0/surfa/mesh/
+-rw-r--r--   0 andrew     (501) staff       (20)       86 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3003 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/cache.py
+-rw-r--r--   0 andrew     (501) staff       (20)   277113 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa/mesh/intersection.c
+-rw-r--r--   0 andrew     (501) staff       (20)     9567 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/intersection.h
+-rw-r--r--   0 andrew     (501) staff       (20)    26913 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/mesh.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1339 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/overlay.py
+-rw-r--r--   0 andrew     (501) staff       (20)    14900 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/mesh/sphere.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5711 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/pipeline.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3719 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/system.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204394 surfa-0.5.0/surfa/transform/
+-rw-r--r--   0 andrew     (501) staff       (20)      369 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    22054 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/affine.py
+-rw-r--r--   0 andrew     (501) staff       (20)    18060 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/geometry.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3938 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/orientation.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2193 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/transform/space.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204659 surfa-0.5.0/surfa/vis/
+-rw-r--r--   0 andrew     (501) staff       (20)       56 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/vis/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10570 2023-06-15 16:05:37.000000 surfa-0.5.0/surfa/vis/freeview.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.199180 surfa-0.5.0/surfa.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)      870 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      944 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-15 16:05:50.000000 surfa-0.5.0/surfa.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       39 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        6 2023-06-15 16:05:51.000000 surfa-0.5.0/surfa.egg-info/top_level.txt
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-15 16:05:51.204762 surfa-0.5.0/test/
+-rw-r--r--   0 andrew     (501) staff       (20)     8354 2023-06-15 16:05:37.000000 surfa-0.5.0/test/test_framed.py
```

### Comparing `surfa-0.4.2/PKG-INFO` & `surfa-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfa
-Version: 0.4.2
+Version: 0.5.0
 Summary: Utilities for medical image and surface processing.
 Home-page: https://github.com/freesurfer/surfa
 Author: Andrew Hoopes
 Author-email: freesurfer@nmr.mgh.harvard.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `surfa-0.4.2/setup.py` & `surfa-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/__init__.py` & `surfa-0.5.0/surfa/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # _____
 # SURFA
 #
 
-__version__ = '0.4.2'
+__version__ = '0.5.0'
 
 from . import system
 
 from .core import stack
 from .core import labels
 from .core import slicing
 from .core import LabelLookup
```

### Comparing `surfa-0.4.2/surfa/core/array.py` & `surfa-0.5.0/surfa/core/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,28 +103,34 @@
         shapes = [shape] if np.isscalar(shape[0]) else shape
         shapes = [tuple(s) for s in shapes]
         if not any(s == arr.shape for s in shapes):
             reqs = list_string(shapes)
             raise ValueError(f'{name} must have shape {reqs}, but got shape {arr.shape}')
 
 
-def normalize(vec):
+def normalize(vec, inplace=False):
     """
     L2 vector normalization.
 
     Parameters
     ----------
     vec : ndarray
-        Array to check.
+        Array to normalize.
+    inplace : bool, optional
+        If True, normalize the array in-place.
 
     Returns
     -------
     normed : ndarray
     """
-    return vec / np.sqrt(np.sum(vec * vec, -1)).reshape((-1, 1))
+    lengths = np.sqrt(np.sum(vec * vec, -1)).reshape((-1, 1))
+    if inplace:
+        vec /= lengths
+        return vec
+    return vec / lengths
 
 
 def make_writeable(arr):
     """
     Enable array writeability. If this is not possible (might be the case for arrays
     constructed with non-numpy memory methods), then a copy of the input is returned.
```

### Comparing `surfa-0.4.2/surfa/core/framed.py` & `surfa-0.5.0/surfa/core/framed.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,15 +400,15 @@
 
     def unique(self):
         """
         Find all unique elements of an array, sorted.
         """
         return np.unique(self)
 
-    def onehot(self, mapping, dtype=np.uint32):
+    def onehot(self, mapping, dtype=np.int32):
         """
         Convert discrete labels to a one-hot encoded probabilistic map.
 
         Parameters
         ----------
         mapping : array_like of int
             List of label indices to one-hot encode. Label order is preserved.
@@ -428,15 +428,15 @@
 
         mapping = np.asarray(mapping)
         if mapping.ndim != 1:
             raise ValueError('label mapping must be a 1D list')
 
         nlabels = len(mapping)
         inttype = np.uint16 if nlabels < np.iinfo(np.uint16).max else np.uint32
-        recoder = np.zeros(self.max() + 1, dtype=inttype)
+        recoder = np.zeros(max(nlabels, self.max() + 1), dtype=inttype)
         recoder[mapping] = np.arange(nlabels)
 
         dsize = self.data.size
         flat = np.zeros((dsize, nlabels), dtype=dtype)
         flat[np.arange(dsize), recoder[self.data.ravel()]] = 1
         flat.shape = (*self.baseshape, nlabels)
         return self.new(flat)
```

### Comparing `surfa-0.4.2/surfa/core/istype.py` & `surfa-0.5.0/surfa/core/istype.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/core/labels.py` & `surfa-0.5.0/surfa/core/labels.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/core/slicing.py` & `surfa-0.5.0/surfa/core/slicing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 import numpy as np
 
 
+def slicing_shape(slicing):
+    """
+    Compute the shape of region defined by the slicing.
+
+    Parameters
+    ----------
+    slicing : tuple of slice
+        Cropping index.
+
+    Returns
+    -------
+    shape : tuple of int
+        Shape of the slicing region.
+    """
+    return tuple([s.stop - s.start for s in slicing])
+
+
 def slicing_to_coords(slicing):
     """
     Convert a N dimensional slicing to a pair of low and high coordinates.
 
     Parameters
     ----------
     slicing : tuple of slice
@@ -33,29 +50,30 @@
     Returns
     -------
     slicing : tuple of slice
         Cropping index.
     """
     if len(coords) != 2:
         raise ValueError('expected 2 sets of coords (start and stop) for slicing')
-    return tuple([slice(a, b) for a, b in zip(*coords.astype(np.int64))])
+    coords = np.asarray(coords)
+    low = np.floor(coords.min(0)).astype(np.int64)
+    high = np.ceil(coords.max(0)).astype(np.int64)
+    return tuple([slice(a, b) for a, b in zip(low, high)])
 
 
 def expand_slicing(slicing, baseshape, delta):
     """
     Expand (or contract) the size of the cropping window.
 
     Parameters
     ----------
     slicing : tuple of slice
         Cropping index to expand.
-
     baseshape: tuple of int
         The slicing will not exceed this size.
-
     delta: scalar or array of scalars
         The amount to increase the cropping window. Negative
         values will decrease the size.
 
     Returns
     -------
     slicing : tuple of slice
@@ -64,14 +82,63 @@
     coords = slicing_to_coords(slicing).astype(np.float32)
     coords[0] = np.floor(coords[0] - delta)
     coords[1] = np.ceil(coords[1] + delta)
     coords = np.clip(coords, 0, baseshape)
     return coords_to_slicing(coords)
 
 
+def fit_slicing_to_shape(slicing, baseshape, target_shape):
+    """
+    Pad or shrink the slicing to attempt to fit a target shape.
+
+    Parameters
+    ----------
+    slicing : tuple of slice
+        Cropping index to expand.
+    baseshape: tuple of int
+        The slicing will not exceed this size.
+    target_shape: tuple of int
+        The target shape of the slicing regions.
+
+    Returns
+    -------
+    slicing : tuple of slice
+        Modified cropping index.
+    """
+    delta = (np.asarray(target_shape) - slicing_shape(slicing)) / 2
+    coords = slicing_to_coords(slicing)
+    coords[0] -= np.floor(delta).astype(np.int64)
+    coords[1] += np.ceil(delta).astype(np.int64)
+    coords = np.clip(coords, 0, baseshape)
+    return coords_to_slicing(coords)
+
+
+def convert_slicing(slicing, baseshape, affine):
+    """
+    Apply a voxel-space transform to a slicing.
+
+    Parameters
+    ----------
+    slicing : tuple of slice
+        Cropping index to expand.
+    baseshape: tuple of int
+        The slicing will not exceed this size.
+    affine: Affine
+        Voxel-space affine transform of coordinates.
+
+    Returns
+    -------
+    slicing : tuple of slice
+        Transformed cropping index.
+    """
+    coords = affine.transform(slicing_to_coords(slicing))
+    coords = np.clip(coords, 0, baseshape)
+    return coords_to_slicing(coords)
+
+
 def sane_slicing(shape, index_expression):
     """
     Clean up an index expression such that the result is a tuple with
     the proper number of dimensions and slicings to match a target shape.
 
     Parameters
     ----------
```

### Comparing `surfa-0.4.2/surfa/freesurfer.py` & `surfa-0.5.0/surfa/freesurfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     subpath : str
         File path to append to the extracted freesurfer home.
 
     Returns
     -------
     path : str
     """
-    return os.path.join(fshome(), subpath)
+    return os.path.join(home(), subpath)
 
 
 def labels():
     """
     Standard label lookup for all brain regions.
 
     Returns
```

### Comparing `surfa-0.4.2/surfa/image/framed.py` & `surfa-0.5.0/surfa/image/framed.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,15 +479,15 @@
                 raise ValueError('affine must contain source and target info if '
                                  'coordinate space is not \'voxel\'')
 
             # ensure the rotation is around the image corner before interpolating
             if rotation not in ('center', 'corner'):
                 raise ValueError("rotation must be 'center' or 'corner'")
             elif rotation == 'center':
-                affine = center_to_corner_rotation(affine, source.baseshape)
+                affine = center_to_corner_rotation(affine, self.baseshape)
             
             # make sure the matrix is actually inverted since we want a target to
             # source voxel mapping for resampling
             matrix_data = affine.inv().matrix
             source_data = self.framed_data
 
         else:
@@ -682,16 +682,17 @@
             Return copy of image even if requirements are already satisfied.
 
         Returns
         -------
         arr : !class
             Conformed image.
         """
+        conformed = self
         if orientation is not None:
-            conformed = self.reorient(orientation, copy=False)
+            conformed = conformed.reorient(orientation, copy=False)
         if voxsize is not None:
             conformed = conformed.resize(voxsize, method=method, copy=False)
         if shape is not None:
             conformed = conformed.reshape(shape, copy=False)
         if dtype is not None:
             conformed = conformed.astype(dtype, copy=False)
         return self.copy() if (copy and conformed is self) else conformed
@@ -721,14 +722,52 @@
         """
         grid = [np.arange(dim) for dim in self.baseshape]
         interp = RegularGridInterpolator(grid, self.data, method=method,
                                          bounds_error=bounds_error, fill_value=fill)
         sampled = interp(points)
         return sampled
 
+    def dilate(self, steps, kernel=None, mask=None):
+        """
+        Dilate binary image data.
+
+        Parameters
+        ----------
+        steps : int
+            Number of dilation steps.
+        kernel : array
+            Dilation kernel.
+        mask : array
+            Mask to apply dilation to.
+
+        Returns
+        -------
+        dilated : Image
+        """
+        return self.new(scipy.ndimage.binary_dilation(self.data, iterations=steps, structure=kernel, mask=mask))
+
+    def erode(self, steps, kernel=None, mask=None):
+        """
+        Erode binary image data.
+
+        Parameters
+        ----------
+        steps : int
+            Number of erosion steps.
+        kernel : array
+            Erosion kernel.
+        mask : array
+            Mask to apply erosion to.
+
+        Returns
+        -------
+        eroded : Image
+        """
+        return self.new(scipy.ndimage.binary_erosion(self.data, iterations=steps, structure=kernel, mask=mask))
+
     def barycenters(self, labels=None, space='image'):
         """
         Compute barycenters of the image data. If labels are not provided, the barycenter of each
         full image frame are returned.
 
         Parameters
         ----------
```

### Comparing `surfa-0.4.2/surfa/image/interp.c` & `surfa-0.5.0/surfa/image/interp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1109,195 +1109,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1328,42 +1328,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -53956,15 +53956,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_mat, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_disp, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -53973,29 +53973,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -54006,15 +54006,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -54023,29 +54023,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -54056,15 +54056,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -54073,29 +54073,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -54106,15 +54106,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -54123,29 +54123,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -54156,15 +54156,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -54173,29 +54173,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -54206,212 +54206,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -54427,15 +54427,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -54443,53 +54443,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -54497,30 +54497,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -54535,15 +54535,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54559,15 +54559,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -54575,53 +54575,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -54629,30 +54629,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54667,15 +54667,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54691,15 +54691,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -54707,53 +54707,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -54761,30 +54761,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -54799,176 +54799,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -69092,26 +69092,26 @@
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 951, __pyx_L1_error)
```

### Comparing `surfa-0.4.2/surfa/io/affine.py` & `surfa-0.5.0/surfa/io/affine.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/framed.py` & `surfa-0.5.0/surfa/io/framed.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/fsio.py` & `surfa-0.5.0/surfa/io/fsio.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/labels.py` & `surfa-0.5.0/surfa/io/labels.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/mesh.py` & `surfa-0.5.0/surfa/io/mesh.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/protocol.py` & `surfa-0.5.0/surfa/io/protocol.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/io/utils.py` & `surfa-0.5.0/surfa/io/utils.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/mesh/cache.py` & `surfa-0.5.0/surfa/mesh/cache.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/mesh/intersection.c` & `surfa-0.5.0/surfa/mesh/intersection.c`

 * *Files 1% similar despite different names*

```diff
@@ -1042,195 +1042,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1257,42 +1257,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2525,15 +2525,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_arr_selected);
   __Pyx_XDECREF((PyObject *)__pyx_v_arr_neighbors);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2542,29 +2542,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2575,15 +2575,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2592,29 +2592,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2625,15 +2625,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2642,29 +2642,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2675,15 +2675,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2692,29 +2692,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2725,15 +2725,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2742,29 +2742,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2775,212 +2775,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2996,15 +2996,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3012,53 +3012,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -3066,30 +3066,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3104,15 +3104,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3128,15 +3128,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3144,53 +3144,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -3198,30 +3198,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3236,15 +3236,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3260,15 +3260,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3276,53 +3276,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -3330,30 +3330,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3368,176 +3368,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3636,26 +3636,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -4042,15 +4042,15 @@
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../conda/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `surfa-0.4.2/surfa/mesh/intersection.h` & `surfa-0.5.0/surfa/mesh/intersection.h`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/mesh/mesh.py` & `surfa-0.5.0/surfa/mesh/mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
+import warnings
 import numpy as np
 from copy import deepcopy
 from scipy.spatial import cKDTree
 from scipy.sparse import coo_matrix
 
 from surfa.core.array import check_array
 from surfa.core.array import normalize
 from surfa.core.array import make_writeable
 from surfa.mesh.cache import cached_mesh_property
 from surfa.mesh.overlay import cast_overlay
+from surfa.mesh.overlay import Overlay
 from surfa.mesh.sphere import mesh_is_sphere
-from surfa.mesh.ray import RayIntersectionQuery
 from surfa.mesh.intersection import triangle_intersections
 from surfa.transform import ImageGeometry
 from surfa.transform import image_geometry_equal
 from surfa.transform import cast_image_geometry
 from surfa.transform import cast_space
 from surfa.transform import cast_affine
 
@@ -58,19 +59,15 @@
         self._metadata = {}
         self.metadata = metadata
 
     def copy(self):
         """
         Return a deep copy of the object.
         """
-        copied = deepcopy(self)
-        # intersection query will return None upon deep copy
-        # so let's remember to clear it from the cache
-        copied._cache.pop('_iq', None)
-        return copied
+        return deepcopy(self)
 
     def save(self, filename, fmt=None):
         """
         Write mesh to file.
 
         Parameters
         ----------
@@ -413,60 +410,29 @@
 
     def nearest_vertex(self, points, k=1):
         """
         Locate the nearest `k` vertices from a point or list of points.
 
         Parameters
         ----------
-        origins : (n, 3) float
-            Ray vector origin points.
-        origins : (n, 3) float
-            Ray vector directions (can be unnormalized).
+        points : (n, 3) float
+            Point or list of points to query.
+        k : int, optional
+            Number of nearest vertices to search for.
 
         Returns
         -------
-        faces : (n,) int
-            Indices of intersected faces. Index will be -1 if intersection was not found.
+        vertices : (n,) int
+            Indices of nearest vertices.
         dists : (n,) float
-            Distance to intersection point from ray origin.
-        bary : (n, 3) float
-            Barycentric weights representing the intersection point on the triangle face.
+            Distance to vertex.
         """
         dist, nn = self.kdtree.query(points, k=k, workers=-1)
         return (nn, dist)
 
-    @cached_mesh_property
-    def _iq(self):
-        """
-        Cached intersection query for ray-tracing.
-        """
-        return RayIntersectionQuery(self)
-
-    def ray_intersection(self, origins, dirs):
-        """
-        Compute intersections between rays and mesh triangles.
-
-        Parameters
-        ----------
-        origins : (n, 3) float
-            Ray vector origin points.
-        origins : (n, 3) float
-            Ray vector directions (can be unnormalized).
-
-        Returns
-        -------
-        faces : (n,) int
-            Indices of intersected faces. Index will be -1 if intersection was not found.
-        dists : (n,) float
-            Distance to intersection point from ray origin.
-        bary : (n, 3) float
-            Barycentric weights representing the intersection point on the triangle face.
-        """
-        return self._iq.ray_intersection(origins, dirs)
-
     def smooth_overlay(self, overlay, iters=10, step=0.5, weighted=True, pinned=None):
         """
         Smooth the scalar values of an overlay along the mesh.
 
         Parameters
         ----------
         overlay : Overlay
@@ -549,59 +515,65 @@
         Convert a face-specific overlay to a vertex-specific overlay.
 
         Parameters
         ----------
         overlay : Overlay
             Face overlay to convert, must have points equal to the number
             of mesh faces.
-        method: {'mean', 'min', 'max'}
+        method: {'mean', 'min', 'max', 'sum'}
             Reduction method to gather face scalars over vertices.
 
         Returns
         -------
         scalars : Overlay
         """
         if overlay.shape[0] != self.nfaces:
             raise ValueError(f'expected overlay to have {self.nfaces} points to match '
                              f'the number of mesh faces, but instead got {overlay.shape[0]}')
         overlay = cast_overlay(overlay)
   
-        # 
+        shape = (self.nvertices, overlay.nframes)
+
         method = str(method).lower()
         if method == 'mean':
-            buffer = np.zeros(self.nvertices)
+            buffer = np.zeros(shape)
             np.add.at(buffer, self.faces[:, 0], overlay)
             np.add.at(buffer, self.faces[:, 1], overlay)
             np.add.at(buffer, self.faces[:, 2], overlay)
-            buffer /= np.bincount(self.faces.flat)
+            buffer /= np.bincount(self.faces.flat).reshape(-1, 1)
         elif method == 'max':
-            buffer = np.full(self.nvertices, overlay.min(), dtype=overlay.dtype)
+            buffer = np.full(shape, overlay.min(), dtype=overlay.dtype)
             np.maximum.at(buffer, self.faces[:, 0], overlay)
             np.maximum.at(buffer, self.faces[:, 1], overlay)
             np.maximum.at(buffer, self.faces[:, 2], overlay)
         elif method == 'min':
-            buffer = np.full(self.nvertices, overlay.max(), dtype=overlay.dtype)
+            buffer = np.full(shape, overlay.max(), dtype=overlay.dtype)
             np.minimum.at(buffer, self.faces[:, 0], overlay)
             np.minimum.at(buffer, self.faces[:, 1], overlay)
             np.minimum.at(buffer, self.faces[:, 2], overlay)
+        elif method == 'sum':
+            buffer = np.zeros(shape, dtype=overlay.dtype)
+            np.add.at(buffer, self.faces[:, 0], overlay)
+            np.add.at(buffer, self.faces[:, 1], overlay)
+            np.add.at(buffer, self.faces[:, 2], overlay)
         else:
-            raise ValueError(f'unknown method `{method}`, expected one of: mean/min/max')
+            raise ValueError(f'unknown method `{method}`, expected one of: mean/min/max/sum')
 
         return overlay.new(buffer)
 
     def vertex_to_face_overlay(self, overlay, method='mean'):
         """
         Convert a vertex-specific overlay to a face-specific overlay.
 
         Parameters
         ----------
         overlay : Overlay
             Vertex overlay to convert, must have points equal to the number
             of mesh vertices.
-        method: {'mean', 'min', 'max'}
+        method: {'mean', 'min', 'max', 'sum'}
             Reduction method to gather vertex scalars over faces.
 
         Returns
         -------
         scalars : Overlay
         """
         if overlay.shape[0] != self.nvertices:
@@ -616,16 +588,18 @@
         method = str(method).lower()
         if method == 'mean':
             reduced = gathered.mean(1)
         elif method == 'max':
             reduced = gathered.max(1)
         elif method == 'min':
             reduced = gathered.min(1)
+        elif method == 'sum':
+            reduced = gathered.sum(1)
         else:
-            raise ValueError(f'unknown method `{method}`, expected one of: mean/min/max')
+            raise ValueError(f'unknown method `{method}`, expected one of: mean/min/max/sum')
 
         return overlay.new(reduced)
 
     def find_self_intersecting_faces(self, knn=50, overlay=False):
         """
         Locate any faces in the mesh topology that are self-intersecting with each other.
         To fix these intersections, see `mesh.remove_self_intersections`.
@@ -646,14 +620,15 @@
         """
 
         # we want to compute an triangle intersection test between nearby faces, so
         # build a kd tree for the centers of each triangle and lookup closest pairs.
         # the intesection code will be smart enough to ignore self-referencing hits
         # as well as immediate neighboring faces
         centers = self.triangles.mean(1)
+        knn = min([centers.shape[0], knn])
         _, neighbors = cKDTree(centers).query(centers, k=knn, workers=-1)
 
         # given this list of neighboring faces, compute triangle-triangle intersections
         neighbors = np.ascontiguousarray(neighbors.astype(np.int32))
         selected = np.arange(self.nfaces, dtype=np.int32)
         intersecting = triangle_intersections(self.vertices, self.faces.astype(np.int32), selected, neighbors)
```

### Comparing `surfa-0.4.2/surfa/mesh/overlay.py` & `surfa-0.5.0/surfa/mesh/overlay.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/mesh/sphere.py` & `surfa-0.5.0/surfa/mesh/sphere.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import surfa as sf
 
+from scipy.spatial import cKDTree
 from scipy.interpolate import RegularGridInterpolator
 
 from surfa.core.array import normalize
 from surfa.mesh.overlay import cast_overlay
 from surfa.image.framed import cast_slice
 
 
@@ -49,14 +50,32 @@
     """
     if not mesh.is_sphere:
         message = ('mesh is not spherical, meaning its center is not close to zero '
                    'or there is substantial variability across radii')
         raise ValueError(message)
 
 
+def conform_sphere(mesh):
+    """
+    Conform sphere mesh to a guaranteed radius of 1.
+    
+    Parameters
+    ----------
+    mesh : Mesh
+        Spherical mesh to conform.
+
+    Returns
+    -------
+    conformed : Mesh
+    """
+    mesh = mesh.copy()
+    normalize(mesh.vertices, inplace=True)
+    return mesh
+
+
 def cartesian_to_spherical(points):
     """
     Convert a set of cartesian points to spherical coordinates (phi, theta) around the origin.
 
     Parameters
     ----------
     points : (n, 3) float
@@ -90,14 +109,121 @@
     """
     x = np.sin(points[:, 0]) * np.cos(points[:, 1])
     y = np.sin(points[:, 0]) * np.sin(points[:, 1])
     z = np.cos(points[:, 0])
     return np.stack([x, y, z], axis=1)
 
 
+def barycentric_spherical_map(source, target, neighborhood=10):
+    """
+    Map the points of a target sphere to the barycentric coordinates of the nearest
+    triangle on a source sphere.
+
+    Parameters
+    ----------
+    source : Mesh
+        Source sphere mesh.
+    target : Mesh
+        Target sphere mesh.
+    neighborhood : int, optional
+        Max number of nearest triangles to consider for each target point.
+
+    Returns
+    -------
+    faces, barycenters : (n, 3) int, (n, 3) float
+    """
+    source = conform_sphere(source)
+    target = conform_sphere(target)
+
+    # compute the k-nearest triangles to each target point. this is used to limit the
+    # number of triangles that are considered for each target point
+    centers = source.triangles.mean(1)
+    nearest = cKDTree(centers).query(target.vertices, k=neighborhood, workers=-1)[1].T
+
+    # initialize
+    intersecting_faces = np.full(target.nvertices, -1, dtype=np.int64)
+    intersecting_barycenters = np.zeros((target.nvertices, 3), dtype=np.float64)
+
+    dot = lambda a, b: np.dot(a * b, [1.0] * a.shape[1])
+    tolerance = np.finfo(np.float64).resolution * 100
+
+    # iterate over the nearest triangles, in order of increasing distance
+    for faces in nearest:
+
+        # mark target points that have not yet been assigned a face
+        remaining = intersecting_faces == -1
+
+        # stop if all target points have been assigned a face
+        if np.count_nonzero(remaining) == 0:
+            break
+
+        # gather triangle properties
+        faces = faces[remaining]
+        triangles = source.triangles[faces]
+        normals = source.face_normals[faces]
+
+        # the ray is the vector represented by the target point since the
+        # spheres should be centered at the origin. the ray is scaled to be
+        # just shy of the radius of the sphere to avoid missing the triangle
+        rays = target.vertices[remaining] * 0.95
+
+        # find the intersection location of the rays with the planes
+        projection_ori = dot(triangles[:, 0], normals)
+        projection_dir = dot(rays, normals)
+        
+        # first check if the ray intersects the triangle plane
+        hits = np.abs(projection_dir) > 1e-5
+        
+        # filter the triangles that do intersect
+        remaining[remaining] = hits
+        rays = rays[hits]
+        triangles = triangles[hits]
+
+        # find the distance to the intersection point
+        distance = np.divide(projection_ori[hits], projection_dir[hits])
+        location = rays[hits] * distance.reshape((-1, 1))
+
+        # find the barycentric coordinates of each plane intersection on the triangle
+
+        edges = triangles[:, 1:] - triangles[:, :1]
+        w = location - triangles[:, 0].reshape((-1, 3))
+
+        dot00 = dot(edges[:, 0], edges[:, 0])
+        dot01 = dot(edges[:, 0], edges[:, 1])
+        dot02 = dot(edges[:, 0], w)
+        dot11 = dot(edges[:, 1], edges[:, 1])
+        dot12 = dot(edges[:, 1], w)
+
+        inverse_denominator = 1.0 / (dot00 * dot11 - dot01 * dot01)
+        barycentric = np.zeros((len(triangles), 3), dtype=np.float64)
+        barycentric[:, 2] = (dot00 * dot12 - dot01 * dot02) * inverse_denominator
+        barycentric[:, 1] = (dot11 * dot02 - dot01 * dot12) * inverse_denominator
+        barycentric[:, 0] = 1 - barycentric[:, 1] - barycentric[:, 2]
+
+        # the plane intersection is inside the triangle if all barycentric
+        # coordinates are between 0.0 and 1.0
+        hits = np.logical_and((barycentric > -tolerance).all(axis=1),
+                              (barycentric < (1 + tolerance)).all(axis=1),
+                              dot(location, rays) > -1e-6)
+
+        # filter the triangles that pass all intersection tests
+        remaining[remaining] = hits
+        intersecting_faces[remaining] = faces[hits]
+        intersecting_barycenters[remaining] = barycentric[hits]
+
+    # if any target points were not assigned a face, just assign them the
+    # center of the nearest face
+    if np.count_nonzero(remaining) != 0:
+        missing = intersecting_faces == -1
+        intersecting_faces[missing] = nearest[0][missing]
+        intersecting_barycenters[missing] = 0.33333333
+
+    return intersecting_faces, intersecting_barycenters
+
+
 class SphericalResamplingNearest:
 
     def __init__(self, source, target):
         """
         Nearest-neighbor map to transfer vertex information between two aligned spheres.
         The computed map will interpolate scalars from the source surface mesh to the
         target surface mesh.
@@ -147,18 +273,15 @@
         Parameters
         ----------
         source, target : Mesh
         """
         require_sphere(source)
         require_sphere(target)
 
-        dirs = normalize(target.vertices)
-        min_radius = np.sqrt(np.sum(source.vertices ** 2, 1)).min() * 0.99
-        origins = dirs * min_radius
-        faces, dists, bary = source.ray_intersection(origins, dirs)
+        faces, bary = barycentric_spherical_map(source, target)
 
         self._nv = source.nvertices
         self._vertices = source.faces[faces]
         self._weights = bary[:, :, np.newaxis]
 
     def sample(self, overlay):
         """
@@ -274,18 +397,17 @@
         self._sphere_coords = cartesian_to_spherical(sphere.vertices)
         self._nv = sphere.nvertices
 
         points = np.zeros((*shape, 2))
         points[:, :, 0] = np.linspace(0, np.pi, shape[0])[:, np.newaxis]
         points[:, :, 1] = np.linspace(0, 2 * np.pi, shape[1] + 1)[np.newaxis, :-1]
         points = points.reshape((-1, 2), order='C')
-        
+
         dirs = spherical_to_cartesian(points)
-        origins = dirs * np.sqrt(np.sum(sphere.vertices ** 2, 1)).min() * 0.99
-        faces, dists, bary = sphere.ray_intersection(origins, dirs)
+        faces, bary = barycentric_spherical_map(sphere, sf.Mesh(dirs))
 
         self._forward_vertices = sphere.faces[faces]
         self._forward_weights = bary[:, :, np.newaxis]
 
         x = np.linspace(0, np.pi, shape[0])
         y = np.linspace(0, 2 * np.pi, shape[1] + 1)
         self._meshgrid = (x, y)
```

### Comparing `surfa-0.4.2/surfa/pipeline.py` & `surfa-0.5.0/surfa/pipeline.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/system.py` & `surfa-0.5.0/surfa/system.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/transform/affine.py` & `surfa-0.5.0/surfa/transform/affine.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/transform/geometry.py` & `surfa-0.5.0/surfa/transform/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class ImageGeometry:
 
     def __init__(self, shape, voxsize=None, rotation=None, center=None, shear=None, vox2world=None):
         """
 
-        Defines the correspondence between voxel coordinates and world coordinates for an image.
+        Defines the correspondence between voxel coordinates and "world" coordinates, eg, RAS, for an image.
 
         This correspondence can be represented by either a singular affine (voxel-to-world
         transform matrix) or a set of linear components (voxel scale, position, rotation,
         and shear). These parameters and corresponding coordinates transforms are appropriately
         recomputed upon any modification.
 
         Parameters
@@ -295,16 +295,19 @@
     @world2vox.setter
     def world2vox(self, value):
         value = cast_affine(value)
         self.update(vox2world=value.inv())
 
     @property
     def vox2surf(self):
-        """
-        Affine transform that maps voxel (image) to surface coordinates.
+        """Affine transform that maps voxel (image) to surface
+        coordinates. Surface coordinates are centered near the center
+        of the volume and aligned with the voxel coordinates in LIA
+        rotation.
+
         """
         def func():
             rot = orientation_to_rotation_matrix('LIA')
             return compose_centered_affine(self.shape, self.voxsize, rot, np.zeros(3), np.zeros(3))
         return self._retrieve_or_compute_affine('vs', func)
 
     @property
@@ -327,14 +330,27 @@
     def surf2world(self):
         """
         Affine transform that maps surface to world coordinates.
         """
         func = lambda : self.vox2world @ self.surf2vox
         return self._retrieve_or_compute_affine('sw', func)
 
+    @property
+    def vox2vxm(self):
+        # voxel morph centers the col,row,slice
+        M = np.eye(4);
+        M[0][3] = (self._shape[0]-1)/2;
+        M[1][3] = (self._shape[1]-1)/2;
+        M[2][3] = (self._shape[2]-1)/2;
+        return(Affine(M));
+
+    @property
+    def vxm2vox(self):
+        return(self.vox2vxm.inv())
+
     def _retrieve_or_compute_affine(self, name, func):
         """
         Internal utility to compute and cache affine matrices when called.
         """
         retrieved = self._affines.get(name)
         if retrieved is not None:
             return retrieved
@@ -355,14 +371,15 @@
             Target coordinate space.
 
         Returns
         -------
         Affine
             Retrieved affine.
         """
+        # Andrew, what were you thinking?
         a = str(cast_space(source))[0]
         b = str(cast_space(target))[0]
         # lets use the first character of the space for a quick lookup
         aff = {
             'vw': self.vox2world,
             'vs': self.vox2surf,
             'wv': self.world2vox,
@@ -396,14 +413,15 @@
             voxsize = np.linalg.norm(self.vox2world[:, :3], axis=0)
             rotation = self.vox2world[:3, :3] / voxsize
             return (voxsize, rotation, center)
         else:
             return (self.voxsize, self.rotation, self.center)
 
 
+
 def decompose_centered_affine(shape, affine):
     """
     Decompose an image-to-world affine into geometry parameters.
 
     Parameters
     ----------
     shape : array_like
@@ -523,7 +541,9 @@
         np.allclose(a.vox2world.matrix, b.vox2world.matrix, atol=tol, rtol=0.0),
     )
 
     if not all(matches):
         return False
 
     return True
+
+
```

### Comparing `surfa-0.4.2/surfa/transform/orientation.py` & `surfa-0.5.0/surfa/transform/orientation.py`

 * *Files 14% similar despite different names*

```diff
@@ -127,7 +127,22 @@
     name = name.replace('L', 'left')
     name = name.replace('R', 'right')
     name = name.replace('P', 'posterior')
     name = name.replace('A', 'anterior')
     name = name.replace('I', 'inferior')
     name = name.replace('S', 'superior')
     return name
+
+
+def random_orientation():
+    """
+    Generate a random orientation string.
+
+    Returns
+    -------
+    str
+        Random orientation.
+    """
+    orientation = [d[np.random.randint(2)] for d in ('LR', 'PA', 'IS')]
+    orientation = np.asarray(orientation)
+    orientation = ''.join(orientation[np.random.permutation(3)])
+    return orientation
```

### Comparing `surfa-0.4.2/surfa/transform/space.py` & `surfa-0.5.0/surfa/transform/space.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa/vis/freeview.py` & `surfa-0.5.0/surfa/vis/freeview.py`

 * *Files identical despite different names*

### Comparing `surfa-0.4.2/surfa.egg-info/PKG-INFO` & `surfa-0.5.0/surfa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfa
-Version: 0.4.2
+Version: 0.5.0
 Summary: Utilities for medical image and surface processing.
 Home-page: https://github.com/freesurfer/surfa
 Author: Andrew Hoopes
 Author-email: freesurfer@nmr.mgh.harvard.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `surfa-0.4.2/surfa.egg-info/SOURCES.txt` & `surfa-0.5.0/surfa.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 surfa/io/utils.py
 surfa/mesh/__init__.py
 surfa/mesh/cache.py
 surfa/mesh/intersection.c
 surfa/mesh/intersection.h
 surfa/mesh/mesh.py
 surfa/mesh/overlay.py
-surfa/mesh/ray.py
 surfa/mesh/sphere.py
 surfa/transform/__init__.py
 surfa/transform/affine.py
 surfa/transform/geometry.py
 surfa/transform/orientation.py
 surfa/transform/space.py
 surfa/vis/__init__.py
```

### Comparing `surfa-0.4.2/test/test_framed.py` & `surfa-0.5.0/test/test_framed.py`

 * *Files identical despite different names*

