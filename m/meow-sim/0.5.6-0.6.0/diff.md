# Comparing `tmp/meow-sim-0.5.6.tar.gz` & `tmp/meow-sim-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.6.tar", last modified: Tue Jun 13 17:14:36 2023, max compression
+gzip compressed data, was "meow-sim-0.6.0.tar", last modified: Thu Jun 15 17:58:52 2023, max compression
```

## Comparing `meow-sim-0.5.6.tar` & `meow-sim-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-13 17:14:31.000000 meow-sim-0.5.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-13 17:14:36.093195 meow-sim-0.5.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-13 17:14:31.000000 meow-sim-0.5.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6170 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    13437 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7947 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-13 17:14:31.000000 meow-sim-0.5.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 17:14:36.093195 meow-sim-0.5.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.397406 meow-sim-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-15 17:58:48.000000 meow-sim-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-15 17:58:52.397406 meow-sim-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-15 17:58:48.000000 meow-sim-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10062 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    12777 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-06-15 17:58:48.000000 meow-sim-0.6.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.393406 meow-sim-0.6.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 17:58:52.000000 meow-sim-0.6.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-15 17:58:48.000000 meow-sim-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 17:58:52.397406 meow-sim-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:58:52.397406 meow-sim-0.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-15 17:58:48.000000 meow-sim-0.6.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.6/LICENSE` & `meow-sim-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/PKG-INFO` & `meow-sim-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.6
+Version: 0.6.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.6/README.md` & `meow-sim-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/__init__.py` & `meow-sim-0.6.0/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.6"
+__version__ = "0.6.0"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.6/meow/assets/silicon.csv` & `meow-sim-0.6.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/base_model.py` & `meow-sim-0.6.0/meow/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Provides a custom pydantic BaseModel which handles numpy arrays better """
 
+from functools import wraps
 from hashlib import md5
 from typing import Any, Tuple
 
 import numpy as np
 from pydantic.main import BaseModel as _BaseModel
-from pydantic.main import ModelMetaclass
+from pydantic.main import ModelMetaclass, PrivateAttr
 
 from .cache import cache_array, cache_model
 
 
 class _array(np.ndarray):
     """just an immutable array with a nicer repr"""
 
@@ -191,14 +192,16 @@
             return False
         return isinstance(arr, np.ndarray)
 
 
 class BaseModel(_BaseModel, metaclass=_ModelMetaclass):
     """A customized pydantic base model that handles numpy array type hints"""
 
+    _cache = PrivateAttr({})
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.__dict__.update({k: _view_arrays(k, v) for k, v in self.__dict__.items()})
         model = cache_model(self)
         if not model is self:
             object.__setattr__(self, "__dict__", model.__dict__)
 
@@ -224,15 +227,15 @@
             f"visualization for {self.__class__.__name__!r} not (yet) implemented."
         )
 
     def __hash__(self):
         try:
             arr = np.frombuffer(md5(self.json().encode()).digest(), dtype=np.uint8)[-8:]
             idx = np.arange(arr.shape[0], dtype=np.int64)[::-1]
-            return np.asarray(np.sum(arr * 255**idx), dtype=np.int_).item()
+            return int(np.sum(arr * 255**idx))
         except Exception:
             return None
 
     def __repr__(self):
         return self._repr()
 
     def __str__(self):
@@ -240,19 +243,36 @@
 
 
 def _view_arrays(key, obj):
     if isinstance(obj, dict):
         return {k: _view_arrays(k, v) for k, v in obj.items()}
     elif isinstance(obj, np.ndarray) or isinstance(obj, _array):
         obj = obj.view(_array)
-        if not key in [
-            "Ex",
-            "Ey",
-            "Ez",
-            "Hx",
-            "Hy",
-            "Hz",
-        ]:  # arbitrary: let's not spam the cache with this.
+
+        # arbitrary: let's not spam the cache with this.
+        if not key in ["Ex", "Ey", "Ez", "Hx", "Hy", "Hz"]:
             obj = cache_array(obj)
+
         return obj
     else:
         return obj
+
+
+def cache(prop):
+    prop_name = prop.__name__
+
+    @wraps(prop)
+    def getter(self):
+        stored_value = self._cache.get(prop_name)
+
+        if stored_value is not None:
+            return stored_value
+
+        computed = prop(self)
+        self._cache[prop_name] = computed
+        return computed
+
+    return getter
+
+
+def cached_property(method):
+    return property(cache(method))
```

### Comparing `meow-sim-0.5.6/meow/cache.py` & `meow-sim-0.6.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/cell.py` & `meow-sim-0.6.0/meow/cell.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 """ an EME Cell """
 
-from typing import Any, Dict, List, Tuple, Union
+from typing import List, Tuple, Union
 
 import numpy as np
 from pydantic import Field
 
-from .base_model import BaseModel
+from .base_model import BaseModel, cached_property
 from .mesh import Mesh2d
 from .structures import Structure, sort_structures
 
 
 class Cell(BaseModel):
     """A `Cell` defines a location in a `Structure` associated with a `Mesh`"""
 
     structures: List[Structure] = Field(
         description="the structures which will be sliced by the cell"
     )
     mesh: Mesh2d = Field(description="the mesh to slice the structures with")
     z_min: float = Field(description="the starting z-coordinate of the cell")
     z_max: float = Field(description="the ending z-coordinate of the cell")
-    extra: Dict[str, Any] = Field(
-        default_factory=lambda: {}, description="extra metadata"
-    )
-
-    @property
-    def mx(self):
-        """(derived) the material cross section at the Ex grid (integer y-coords, half-integer x-coords)"""
-        return self.extra["mx"]
-
-    @property
-    def my(self):
-        """(derived) the material cross section at the Ey grid (half-integer y-coords, integer x-coords)"""
-        return self.extra["my"]
-
-    @property
-    def mz(self):
-        """(derived) the material cross section at the Ez grid (integer y-coords, integer x-coords)"""
-        return self.extra["mz"]
-
-    @property
-    def materials(self):
-        """(derived) the materials in the cell"""
-        return self.extra["materials"]
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    @cached_property
+    def _computed(self):
         structures = sort_structures(self.structures)
         mx, my, mz = [np.zeros(self.mesh.Xx.shape, dtype=int) for _ in range(3)]
-        z = 0.5 * (self.z_min + self.z_max)
         # TODO: ideally we should downselect the relevant structures here...
         # structures not at z-location should ideally be ignored.
         materials = []
         for structure in structures:
-            mask_x, mask_y, mask_z = structure.geometry._mask2d(self.mesh, z)
+            mask_x, mask_y, mask_z = structure.geometry._mask2d(self.mesh, self.z)
             if (not mask_x.any()) or (not mask_y.any()) or (not mask_z.any()):
                 continue
             try:
                 material_index = materials.index(structure.material) + 1
             except ValueError:
                 materials.append(structure.material)
                 material_index = len(materials)
             mx[mask_x] = material_index
             my[mask_y] = material_index
             mz[mask_z] = material_index
-        self.extra["mx"] = mx
-        self.extra["my"] = my
-        self.extra["mz"] = mz
-        self.extra["materials"] = materials
+        return {
+            "mx": mx,
+            "my": my,
+            "mz": mz,
+            "materials": materials,
+        }
+
+    @property
+    def mx(self):
+        """(derived) the material cross section at the Ex grid (integer y-coords, half-integer x-coords)"""
+        return self._computed["mx"]
+
+    @property
+    def my(self):
+        """(derived) the material cross section at the Ey grid (half-integer y-coords, integer x-coords)"""
+        return self._computed["my"]
+
+    @property
+    def mz(self):
+        """(derived) the material cross section at the Ez grid (integer y-coords, integer x-coords)"""
+        return self._computed["mz"]
+
+    @property
+    def materials(self):
+        """(derived) the materials in the cell"""
+        return self._computed["materials"]
 
     @property
     def z(self):
         return 0.5 * (self.z_min + self.z_max)
 
     @property
     def length(self):
@@ -97,17 +95,14 @@
             plt.sca(ax)
             if len(c_list) > 1:
                 plt.title(f"m{c}")
             plt.pcolormesh(X, Y, m, cmap=cmap, vmin=0, vmax=len(self.materials))
             plt.axis("scaled")
             plt.grid(True)
 
-    class Config:
-        fields = {"extra": {"exclude": True}}
-
 
 def create_cells(
     structures: List[Structure],
     mesh: Union[Mesh2d, List[Mesh2d]],
     Ls: np.ndarray[Tuple[int], np.dtype[np.float_]],
     z_min: float = 0.0,
 ) -> List[Cell]:
```

### Comparing `meow-sim-0.5.6/meow/eme/__init__.py` & `meow-sim-0.6.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/eme/common.py` & `meow-sim-0.6.0/meow/eme/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     NL, NR = len(modes1), len(modes2)
     O_LL = np.array([inner_product(modes1[m], modes1[m]) for m in range(NL)])
     O_RR = np.array([inner_product(modes2[n], modes2[n]) for n in range(NR)])
     O_LR = np.array([[inner_product(modes1[m], modes2[n]) for n in range(NR)] for m in range(NL)])  # fmt: skip
     O_RL = np.array([[inner_product(modes2[m], modes1[n]) for n in range(NL)] for m in range(NR)])  # fmt: skip
 
-    # extra phase correction (disabled?).
+    # additional phase correction (disabled?).
 
     if conjugate_transpose:
         O_LL = np.real(O_LL)
         O_RR = np.real(O_RR)
 
     # ignoring the phase seems to corresponds best with lumerical.
```

### Comparing `meow-sim-0.5.6/meow/eme/sax.py` & `meow-sim-0.6.0/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/environment.py` & `meow-sim-0.6.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/fde/lumerical.py` & `meow-sim-0.6.0/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/fde/tidy3d.py` & `meow-sim-0.6.0/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/gds_structures.py` & `meow-sim-0.6.0/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/geometries.py` & `meow-sim-0.6.0/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/integrate.py` & `meow-sim-0.6.0/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/materials.py` & `meow-sim-0.6.0/meow/materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,78 @@
 """ Materials """
 
 import os
 import re
-from hashlib import md5
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Mapping, Tuple
 
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
-from pydantic import Field, root_validator
+from pydantic import Field, validator
 from scipy.constants import c
 from scipy.ndimage import map_coordinates
 
 from .base_model import BaseModel, _array
 from .environment import Environment
 
-MATERIAL_DATA_CACHE: Dict[str, Dict[str, Any]] = {}
-MATERIALS: Dict[str, "Material"] = {}
-
 
 class Material(BaseModel):
     """a `Material` defines the refractive index of a `Structure` within an `Environment`."""
 
     name: str = Field(description="the name of the material")
     params: Dict[str, np.ndarray[Tuple[int], np.dtype[np.float_]]] = Field(
         description="the wavelength over which the refractive index is defined."
     )
-    n: np.ndarray[Any, np.dtype[np.complex_]] = Field(
+    n: np.ndarray[Tuple[int], np.dtype[np.complex_]] = Field(
         description="the complex refractive index of the material"
     )
     meta: Dict[str, Any] = Field(
         default_factory=lambda: {}, description="metadata for the material"
     )
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        MATERIALS[self.name] = self
-
-    @root_validator(pre=True)
-    def validate(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        if isinstance(values, Material):
-            return values  # no idea why this should be neccessary, but without it we get weird errors...
+    @staticmethod
+    def _validate_array(arr):
+        if isinstance(arr, dict):
+            r = np.asarray(arr.get("real", 0.0), dtype=np.complex_)
+            i = np.asarray(arr.get("imag", 0.0), dtype=np.complex_)
+            new = r + 1j * i
+        else:
+            new = np.asarray(arr)
+        return new.view(_array)
 
-        values["params"] = params = {
-            k: np.asarray(v).view(_array) for k, v in values["params"].items()
+    @staticmethod
+    def _validate_1d(name, arr):
+        if arr.ndim != 1:
+            raise ValueError(f"{name} should be 1D. Got a {arr.ndim}D array.")
+        return arr
+
+    @validator("n", pre=True)
+    def validate_n_pre(cls, n):
+        return cls._validate_1d("n", cls._validate_array(n))
+
+    @validator("params", pre=True)
+    def validate_params_pre(cls, params):
+        if not isinstance(params, Mapping):
+            raise TypeError(f"instance of dict expected. Got: {type(params)}.")
+        return {
+            k: cls._validate_1d(f"params:{k}", cls._validate_array(v))
+            for k, v in params.items()
         }
 
-        n = values["n"]
-        if isinstance(n, dict):
-            r = np.asarray(n.get("real", 0.0), dtype=np.float_)
-            i = np.asarray(n.get("imag", 0.0), dtype=np.float_)
-            values["n"] = n = np.asarray(r + 1j * i, dtype=np.complex_)
-        else:
-            n = np.asarray(n, dtype=np.complex_)
-        n = n.view(_array)
-
-        if n.ndim != 1:
-            raise ValueError(f"Index n is not 1D. Got shape: {n.shape}")
-        for i, (p, v) in enumerate(params.items()):
-            if v.ndim != 1:
-                raise ValueError(f"Parameter {p} is not 1D. Got shape: {v.shape}")
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        MATERIALS[self.name] = self
+        for p, v in self.params.items():
             Lp = v.shape[0]
-            Ln = n.shape[0]
+            Ln = self.n.shape[0]
             if Lp != Ln:
                 raise ValueError(
                     f"length of parameter array {p} does not match length of refractive index array n. \n"
                     f"{Lp} != {Ln}"
                 )
-        values_hash = _hash_values(values)
-        if values_hash in MATERIAL_DATA_CACHE:
-            values = {
-                **MATERIAL_DATA_CACHE[values_hash],
-                "meta": values.get("meta", {}),
-            }  # shallow copy
-        else:
-            MATERIAL_DATA_CACHE[values_hash] = {
-                k: v for k, v in values.items() if k not in ["meta"]
-            }
-        return values
 
     @classmethod
     def from_path(cls, path, meta=None):
         path = _validate_path(path)
         name = re.sub(r"\.csv$", "", os.path.split(path)[-1])
         df = pd.read_csv(path)
         return cls.from_df(name, df, meta=meta)
@@ -139,14 +130,18 @@
 
     class Config:
         fields = {
             "meta": {"exclude": True},
         }
 
 
+Materials = List[Material]
+MATERIALS: Dict[str, Material] = {}
+
+
 def _to_ndgrid(df, wl_key="wl"):
     """convert stacked data to hypercube data
 
     Args:
         df: the dataframe to convert to hypercube data
         wl_key: which key to use to sort. Options: 'wl' or 'f'. Using 'f' yields better interpolation results
             as most optical phenomina are more linear in 'f' than in 'wl'.
@@ -256,22 +251,14 @@
 
 def _sort_rows(df, not_by=("nr", "ni"), wl_key="wl"):
     not_by = ["wl", "f"] + list(not_by)
     by = [c for c in df.columns if c not in not_by] + [wl_key]
     return df.sort_values(by=by).reset_index(drop=True)
 
 
-def _hash_values(values):
-    values = {k: v for k, v in values.items() if k not in ["meta"]}
-    df = pd.DataFrame(
-        {**values["params"], "nr": np.real(values["n"]), "ni": np.imag(values["n"])}
-    )
-    return md5(np.asarray(df.values * 1e9, dtype=np.int64).tobytes()).hexdigest()
-
-
 def _validate_path(path):
     if not path.endswith(".csv"):
         path = f"{path}.csv"
     path_parts = path.replace("\\", "/").split("/")
     if not os.path.exists(path) and len(path_parts) == 1:
         lib_path = os.path.dirname(os.path.abspath(__file__))
         path = os.path.join(lib_path, "assets", path)
@@ -285,9 +272,7 @@
     path="silicon",
     meta={"color": (0.9, 0, 0, 0.9)},
 )
 silicon_oxide = Material.from_path(
     path="silicon_oxide",
     meta={"color": (0.9, 0.9, 0.9, 0.9)},
 )
-
-Materials = List[Material]
```

### Comparing `meow-sim-0.5.6/meow/mesh.py` & `meow-sim-0.6.0/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow/mode.py` & `meow-sim-0.6.0/meow/mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ An EigenMode """
 
 import pickle
 import warnings
 from itertools import product
-from typing import Any, List, Tuple
+from typing import List, Tuple
 
 import numpy as np
-from pydantic import Field, PrivateAttr
+from pydantic import Field
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
 
-from .base_model import BaseModel
+from .base_model import BaseModel, cached_property
 from .cross_section import CrossSection
 from .integrate import integrate_2d
 from .visualize import _figsize_visualize_mode
 
 
 class Mode(BaseModel):
     """A `Mode` contains the field information for a given `CrossSection`."""
@@ -39,70 +39,53 @@
     Hy: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = Field(
         description="the Hy-fields of the mode"
     )
     Hz: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = Field(
         description="the Hz-fields of the mode"
     )
 
-    _Px: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
-    _Py: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
-    _Pz: np.ndarray[Tuple[int, int], np.dtype[np.complex_]] = PrivateAttr()
-    _A: np.float_ = PrivateAttr()
-
-    def __init__(self, **data: Any):
-        super().__init__(**data)
-        self._Px = None  # type: ignore
-        self._Py = None  # type: ignore
-        self._Pz = None  # type: ignore
-        self._A = None  # type: ignore
-
     @property
     def te_fraction(self):
         """the TE polarization fraction of the mode."""
         return te_fraction(self)
 
-    def _calc_poynting(self):
+    @cached_property
+    def _pointing(self):
         """calculate and cache the poynting vector"""
         vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
         vecH = np.stack([self.Hx, self.Hy, self.Hz], axis=-1)
         vecP = np.cross(vecE, vecH)
-        self._Px, self._Py, self._Pz = np.rollaxis(vecP, -1)
-
-    def _calc_area(self):
-        vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
-        E_sq = norm(vecE, axis=-1, ord=2)
-        E_qu = E_sq**2
-        x = self.cs.mesh.x_
-        y = self.cs.mesh.y_
-        self._A = np.float_(integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu))
+        Px, Py, Pz = np.rollaxis(vecP, -1)
+        return {
+            "Px": Px,
+            "Py": Py,
+            "Pz": Pz,
+        }
 
     @property
     def Px(self):
-        if self._Px is None:
-            self._calc_poynting()
-        return self._Px
+        return self._pointing["Px"]
 
     @property
     def Py(self):
-        if self._Py is None:
-            self._calc_poynting()
-        return self._Py
+        return self._pointing["Py"]
 
     @property
     def Pz(self):
-        if self._Pz is None:
-            self._calc_poynting()
-        return self._Pz
+        return self._pointing["Pz"]
 
-    @property
+    @cached_property
     def A(self):
         """mode area"""
-        if self._A is None:
-            self._calc_area()
-        return self._A
+        vecE = np.stack([self.Ex, self.Ey, self.Ez], axis=-1)
+        E_sq = norm(vecE, axis=-1, ord=2)
+        E_qu = E_sq**2
+        x = self.cs.mesh.x_
+        y = self.cs.mesh.y_
+        return np.float_(integrate_2d(x, y, E_sq) ** 2 / integrate_2d(x, y, E_qu))
 
     @property
     def env(self):
         return self.cs.env
 
     @property
     def mesh(self):
```

### Comparing `meow-sim-0.5.6/meow/structures.py` & `meow-sim-0.6.0/meow/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """ a Structure is a combination of a geometry with a material (and an optional mesh order) """
 
 import numpy as np
-from pydantic import Field, validator
+from pydantic import Field
 
 from .base_model import BaseModel
 from .geometries import Geometry
 from .materials import Material
 
 
 class Structure(BaseModel):
     """a `Structure` is an association between a `Geometry` and a `Material`"""
 
     material: Material = Field(description="the material of the structure")
     geometry: Geometry = Field(description="the geometry of the structure")
     mesh_order: int = Field(default=5, description="the mesh order of the structure")
 
-    @validator("material")
-    def validate_material(cls, material):
-        return Material.parse_obj(material)
-
     def _lumadd(self, sim, env, unit=1e-6, xyz="yzx"):
         material_name = self.material._lumadd(sim, env, unit)
         self.geometry._lumadd(sim, material_name, self.mesh_order, unit, xyz)
 
     def _trimesh(self, color=None, scale=None):
         return self.geometry._trimesh(
             color=(color or self.material.meta.get("color")),
```

### Comparing `meow-sim-0.5.6/meow/visualize.py` & `meow-sim-0.6.0/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.0/meow_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.6
+Version: 0.6.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.6/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/pyproject.toml` & `meow-sim-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.6"
+version = "0.6.0"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.6/tests/test_deserialization.py` & `meow-sim-0.6.0/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/tests/test_mode_operators.py` & `meow-sim-0.6.0/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.6/tests/test_nbs.py` & `meow-sim-0.6.0/tests/test_nbs.py`

 * *Files identical despite different names*

