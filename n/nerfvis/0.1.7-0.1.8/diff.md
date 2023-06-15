# Comparing `tmp/nerfvis-0.1.7.tar.gz` & `tmp/nerfvis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfvis-0.1.7.tar", last modified: Tue Jun  6 21:46:01 2023, max compression
+gzip compressed data, was "nerfvis-0.1.8.tar", last modified: Thu Jun 15 18:38:39 2023, max compression
```

## Comparing `nerfvis-0.1.7.tar` & `nerfvis-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.7/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.7/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-06 21:46:01.666007 nerfvis-0.1.7/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.7/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.662007 nerfvis-0.1.7/nerfvis/
--rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.7/nerfvis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.7/nerfvis/index.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    61183 2023-06-06 21:43:45.000000 nerfvis-0.1.7/nerfvis/scene.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/nerfvis/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.7/nerfvis/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.7/nerfvis/utils/_rotation.c
--rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.7/nerfvis/utils/_rotation.pyx
--rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.7/nerfvis/utils/sh.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-06 21:45:17.000000 nerfvis-0.1.7/nerfvis/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 21:46:01.666007 nerfvis-0.1.7/nerfvis.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-06-06 21:46:01.000000 nerfvis-0.1.7/nerfvis.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.7/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-06-06 21:46:01.666007 nerfvis-0.1.7/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.7/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-15 18:38:39.141557 nerfvis-0.1.8/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.8/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.8/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-15 18:38:39.141557 nerfvis-0.1.8/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7893 2023-06-15 18:16:03.000000 nerfvis-0.1.8/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-15 18:38:39.137557 nerfvis-0.1.8/nerfvis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       95 2023-06-15 18:28:36.000000 nerfvis-0.1.8/nerfvis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.8/nerfvis/index.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    62031 2023-06-15 18:37:24.000000 nerfvis-0.1.8/nerfvis/scene.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-15 18:38:39.137557 nerfvis-0.1.8/nerfvis/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7388 2023-06-15 18:28:58.000000 nerfvis-0.1.8/nerfvis/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.8/nerfvis/utils/_rotation.c
+-rw-rw-r--   0 alex      (1000) alex      (1000)    87637 2023-06-15 18:28:36.000000 nerfvis-0.1.8/nerfvis/utils/_rotation.pyx
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12621 2023-06-15 18:28:58.000000 nerfvis-0.1.8/nerfvis/utils/sh.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-15 18:37:29.000000 nerfvis-0.1.8/nerfvis/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-15 18:38:39.137557 nerfvis-0.1.8/nerfvis.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2023-06-15 18:38:39.000000 nerfvis-0.1.8/nerfvis.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-06-15 18:38:39.000000 nerfvis-0.1.8/nerfvis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-15 18:38:39.000000 nerfvis-0.1.8/nerfvis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-06-15 18:38:39.000000 nerfvis-0.1.8/nerfvis.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.8/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-06-15 18:38:39.141557 nerfvis-0.1.8/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1694 2023-06-15 18:28:36.000000 nerfvis-0.1.8/setup.py
```

### Comparing `nerfvis-0.1.7/LICENSE.txt` & `nerfvis-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.7/README.md` & `nerfvis-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 ![Screenshot NeRF-- Drone](https://raw.githubusercontent.com/sxyu/nerfvis/master/img/youtube_drone.gif)
 
 
 Tips:
 
 - A list of all objects with the names you gave them will be displayed in a tree view on the left side of the screen, where you can toggle them. F-strings are recommended for automatically generating object names
 - Use "/" inside names for example `image/0` to create nested trees.
-- For convenience, we accept numpy arrays, torch Tensors, and lists in general for any arguments marked at `np.ndarray`  (by default torch is not imported to avoid having it as a dependency). 
+- For convenience, we accept numpy arrays, torch Tensors, and lists in general for any arguments marked at `np.ndarray`  (by default torch is not imported to avoid having it as a dependency).
 - The initial camera pose will be automatically determined. Pass `center=[x, y, z]` (camera position) ,
-    `origin=[x,y,z]` (camera target), `forward=[x,y,z]` (forward vector), `world_up=[x,y,z]` (world space up vector) to display() or export() or embed() to manually set an initial pose. 
+    `origin=[x,y,z]` (camera target), `forward=[x,y,z]` (forward vector), `world_up=[x,y,z]` (world space up vector) to display() or export() or embed() to manually set an initial pose.
     A convenience function `scene.set_opencv()` is given to set the world up axis to `-y` (this also changes the default behavior of `add_image`).
 - Use `scene.export("path")` to manually generate a directory you can open in the browser or upload somewhere
 
 
 ## Examples
 
 ### Viewing a volume
@@ -94,35 +94,46 @@
 - Images `(n_images, h, w)`
 
 Note that OpenCV poses are now preferrred,
 although the original NeRF/PlenOctrees used OpenGL.
 
 ```python
 from nerfvis import scene
+import numpy as np
+
 # Set -y up world, and also flips the image
-scene.set_opencv() 
+scene.set_opencv()
+
+# Example data
+f = 1111.0
+images = np.random.rand(1, 800, 800, 3)
+c2ws = np.eye(4)[None]
+point_cloud = np.random.randn(10000, 3) * 0.1
+point_cloud_errs = np.random.rand(10000)
 
-# To show have errors
+# To show errors as colors
 colors = np.zeros_like(point_cloud)
 colors[:, 0] = point_cloud_errs / point_cloud_errs.max()
 scene.add_points("points", point_cloud, vert_color=colors)
 # Else
 # scene.add_points("points", point_cloud, color=[0.0, 0.0, 0.0])
 scene.add_camera_frustum("cameras", r=c2ws[:, :3, :3], t=c2ws[:, :3, 3], focal_length=f,
                          image_width=images.shape[2], image_height=images.shape[1],
-                         z=0.1, connect=False, color=[1.0, 0.0, 0.0])
+                         z=0.5, connect=False, color=[1.0, 0.0, 0.0])
 
-for i in range(len(c2w)):
+for i in range(len(c2ws)):
     scene.add_image(
                   f"images/i",
-                  images[i],
+                  images[i], # Can be path too
                   r=c2ws[i, :3, :3], t=c2ws[i, :3, 3],
-                  focal_lenght=f,
-                  z=0.1,
-                  image_size)
+                  focal_length=f,
+                  z=0.5,
+                  # NOTE: this image size is the display image size not original imge size
+                  # (that will be taken from the image). Keep it low if you are adding many images
+                  image_size=64)
 scene.add_axes()
 scene.display()
 ```
 
 Example outputs (not quite the same code):
 http://alexyu.net/nerfvis_examples/basic_scene_with_volume/
 http://alexyu.net/nerfvis_examples/bicycle_vis/
@@ -154,15 +165,15 @@
 right now. You may programmatically generate this. They will show up in the *layers* pane
 (top right of the html viewer)
 
 
 Please also `pip install torch svox tqdm scipy` for adding NeRF (`set_nerf`)
 or `pip install trimesh` for using `add_mesh_from_file(path)`.
 
-To add cameras (also used for scaling scene, initializing camera etc), use 
+To add cameras (also used for scaling scene, initializing camera etc), use
 `add_camera_frustum(focal_length=.., image_width=.., image_height=.., z=..,  r=.., t=..)`
 
 ## Viewer Controls
 
 - Left click and drag to orbit
 - Right click and drag, or CTRL+left click and drag to pan
 - Mouse wheel, middle click and drag, or ALT+left click and drag to zoom; alternatively use =/SHIFT+=
```

### Comparing `nerfvis-0.1.7/nerfvis/index.html` & `nerfvis-0.1.8/nerfvis/index.html`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.7/nerfvis/scene.py` & `nerfvis-0.1.8/nerfvis/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 """
 NeRF + Drawing
 """
-import numpy as np
-import re
+import base64
 import os
 import os.path as osp
-import base64
-from typing import Optional, List, Union, Callable, Tuple, Any, Dict
-import warnings
+import platform
+import re
 import threading
+import warnings
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+import numpy as np
+
 from . import utils
 
 _servers = []
 _server_thds = []
 
-def _f(name : str, field : str):
-    return name + '__' + field
 
-def _format_vec3(vec : np.ndarray):
-    return f'[{vec[0]}, {vec[1]}, {vec[2]}]'
+def _f(name: str, field: str):
+    return name + "__" + field
+
+
+def _format_vec3(vec: np.ndarray):
+    return f"[{vec[0]}, {vec[1]}, {vec[2]}]"
 
-def _scipy_rotation_from_auto(rot : np.ndarray):
+
+def _scipy_rotation_from_auto(rot: np.ndarray):
     if rot.shape[-1] == 3:
         q = utils.Rotation.from_rotvec(rot)
     elif rot.shape[-1] == 4:
         q = utils.Rotation.from_quat(rot)
     elif rot.shape[-1] == 9:
         q = utils.Rotation.from_matrix(rot.reshape(list(rot.shape[:-1]) + [3, 3]))
     else:
         raise NotImplementedError
     return q
 
-def _angle_axis_rotate_vector_np(r : np.ndarray, v : np.ndarray):
+
+def _angle_axis_rotate_vector_np(r: np.ndarray, v: np.ndarray):
     """
     Rotate each vector by corresponding axis-angle.
     The formula is from Ceres-solver.
     :param r: (B, 3) or (1, 3) axis-angle
     :param v: (B, 3) or (1, 3) vectors to rotate
     """
     if len(v.shape) == 1 or v.shape[0] == 1:
@@ -59,59 +66,64 @@
     if v_bad.size:
         # From Ceres
         result[bad_mask_v] = v_bad + np.cross(
             np.broadcast_to(r[bad_mask], v_bad.shape), v_bad
         )
     return result
 
-def _quaternion_rotate_vector_np(q : np.ndarray, pt : np.ndarray):
+
+def _quaternion_rotate_vector_np(q: np.ndarray, pt: np.ndarray):
     """
     Rotate a point pt by a quaternion (xyzw, Hamilton) will be normalized
     Derived from cere::UnitQuaternionRotatePoint (rotation.h)
     :param q: (B, 4) xyzw, Hamilton convention quaternion
     :param pt: (B, 3) 3D points
     :return: (B, 3) R(q) pt
     """
     q = q / np.linalg.norm(q, axis=-1, keepdims=True)
     uv = np.cross(q[..., :-1], pt) * 2
     return pt + q[..., -1:] * uv + np.cross(q[..., :-1], uv)
 
-def _rotate_vector_np(rot : np.ndarray, pt : np.ndarray):
+
+def _rotate_vector_np(rot: np.ndarray, pt: np.ndarray):
     """
     Rotate a vector, using either an axis-angle, quaternion (xyzw), or flattened rotation matrix
     :param rot: (B, 3), (B, 4), or (B, 9), the rotations
     :param pt: (B, 3), the 3D points
     :return: (B, 3), rotated points
     """
     if rot.shape[-1] == 3:
         return _angle_axis_rotate_vector_np(rot, pt)
     elif rot.shape[-1] == 4:
         return _quaternion_rotate_vector_np(rot, pt)
     elif rot.shape[-1] == 9:
-        return np.matmul(rot.reshape(list(rot.shape[:-1]) + [3, 3]), pt[..., None])[..., 0]
+        return np.matmul(rot.reshape(list(rot.shape[:-1]) + [3, 3]), pt[..., None])[
+            ..., 0
+        ]
     else:
         raise NotImplementedError
 
+
 def _to_np_array(obj) -> np.ndarray:
     if not isinstance(obj, np.ndarray):
-        if hasattr(obj, 'cpu'):
+        if hasattr(obj, "cpu"):
             obj = obj.cpu()
-        if hasattr(obj, 'detach'):
+        if hasattr(obj, "detach"):
             obj = obj.detach()
         arr = np.array(obj)
     else:
         arr = obj
     if len(arr.strides) > 0 and min(arr.strides) < 0:
         # Negative stride or non-contiguous
         arr = arr.copy()
     return np.ascontiguousarray(arr)
 
 
 class Scene:
-    def __init__(self, title : str = "Scene"):
+    def __init__(self, title: str = "Scene"):
         """
         Holds radiance field/volume/mesh/point cloud/lines objects for 3D visualization.
         Add objects using :code:`add_*` as seen below, then use
         :code:`export()`/:code:`display()`/:code:`embed()` to create a
         standalone web viewer you can open in a browser or embed in
         a notebook.
 
@@ -119,36 +131,43 @@
 
         - Multiple scenes:  `from nerfvis import Scene` then `scene = Scene('title')`
 
         :param title: title to show when saving, default 'Scene'.
                       You can change it later by setting scene.title = '...'.
         """
         self.title = title
-        self.fields : Dict["str", Any] = {}
+        self.fields: Dict["str", Any] = {}
 
         self.world_up = None
         self.cam_forward = None
-        inf = float('inf')
+        inf = float("inf")
         self.bb_min = np.array([inf, inf, inf])
         self.bb_max = np.array([-inf, -inf, -inf])
         self.default_opencv = False
 
     def _add_common(self, name, **kwargs):
         assert isinstance(name, str), "Name must be a string"
         if "time" in kwargs:
-            self.fields[_f(name, "time")] = _to_np_array(kwargs["time"]).astype(np.uint32)
+            self.fields[_f(name, "time")] = _to_np_array(kwargs["time"]).astype(
+                np.uint32
+            )
         if "color" in kwargs:
-            self.fields[_f(name, "color")] = _to_np_array(kwargs["color"]).astype(np.float32)
+            self.fields[_f(name, "color")] = _to_np_array(kwargs["color"]).astype(
+                np.float32
+            )
         if "scale" in kwargs:
             self.fields[_f(name, "scale")] = np.float32(kwargs["scale"])
         if "translation" in kwargs:
             self.fields[_f(name, "translation")] = np.array(
-                    kwargs["translation"]).astype(np.float32)
+                kwargs["translation"]
+            ).astype(np.float32)
         if "rotation" in kwargs:
-            self.fields[_f(name, "rotation")] = _to_np_array(kwargs["rotation"]).astype(np.float32)
+            self.fields[_f(name, "rotation")] = _to_np_array(kwargs["rotation"]).astype(
+                np.float32
+            )
         if "visible" in kwargs:
             self.fields[_f(name, "visible")] = int(kwargs["visible"])
         if "unlit" in kwargs:
             self.fields[_f(name, "unlit")] = int(kwargs["unlit"])
         if "vert_color" in kwargs:
             vc = _to_np_array(kwargs["vert_color"])
             if vc.dtype != np.uint8:
@@ -173,15 +192,15 @@
             transl = _to_np_array(kwargs["translation"]).astype(np.float32)
             min_xyz = min_xyz + transl
             max_xyz = max_xyz + transl
 
         self.bb_min = np.minimum(min_xyz, self.bb_min)
         self.bb_max = np.maximum(max_xyz, self.bb_max)
 
-    def add_cube(self, name : str = "cube", **kwargs):
+    def add_cube(self, name: str = "cube", **kwargs):
         """
         Add a cube with side length 1 (verts {-0.5, 0.5}^3).
 
         :param name: an identifier for this object
         :param color: (3,) color, default is orange (common param)
         :param vert_color: (36, 3) vertex color, optional advanced (common param)
         :param translation: (3,), model translation (common param)
@@ -214,15 +233,15 @@
 
     def set_title(self, title: str):
         """
         Set title of output page
         """
         self.title = title
 
-    def add_wireframe_cube(self, name : str, **kwargs):
+    def add_wireframe_cube(self, name: str, **kwargs):
         """
         Add a wireframe cube with side length 1 (verts {-0.5, 0.5}^3).
         Uses add_lines.
 
         :param name: an identifier for this object
         :param color: (3,) color, default is orange (common param)
         :param vert_color: (36, 3) vertex color, optional advanced (common param)
@@ -254,16 +273,21 @@
         self.add_lines(
             name,
             _to_np_array(verts).astype(dtype=np.float32),
             segs=_to_np_array(segs),
             **kwargs,
         )
 
-    def add_sphere(self, name : str = "sphere",
-                   rings : Optional[int]=None, sectors : Optional[int]=None, **kwargs):
+    def add_sphere(
+        self,
+        name: str = "sphere",
+        rings: Optional[int] = None,
+        sectors: Optional[int] = None,
+        **kwargs,
+    ):
         """
         Add a UV sphere with radius 1
 
         :param name: an identifier for this object
         :param rings: int, number of lateral rings in UV sphere generation, default 15
         :param sectors: int, number of sectors in UV sphere generation, default 30
         :param color: (3,) color, default is orange (common param)
@@ -284,17 +308,15 @@
         if sectors is not None:
             self.fields[_f(name, "sectors")] = int(sectors)
         p1 = np.array([-1.0, -1.0, -1.0])
         p2 = np.array([1.0, 1.0, 1.0])
         self._update_bb(p1, **kwargs)
         self._update_bb(p2, **kwargs)
 
-    def add_line(self, name : str,
-                 a : np.ndarray,
-                 b : np.ndarray, **kwargs):
+    def add_line(self, name: str, a: np.ndarray, b: np.ndarray, **kwargs):
         """
         Add a single line segment from a to b
 
         :param name: an identifier for this object
         :param a: (3,), first point
         :param b: (3,), second point
         :param color: (3,) color, default is orange (common param)
@@ -313,18 +335,21 @@
         a = _to_np_array(a)
         b = _to_np_array(b)
         self.fields[_f(name, "a")] = a.astype(np.float32)
         self.fields[_f(name, "b")] = b.astype(np.float32)
         self._update_bb(a, **kwargs)
         self._update_bb(b, **kwargs)
 
-    def add_lines(self, name : str,
-                 points : np.ndarray,
-                 segs : Optional[np.ndarray] = None,
-                 **kwargs):
+    def add_lines(
+        self,
+        name: str,
+        points: np.ndarray,
+        segs: Optional[np.ndarray] = None,
+        **kwargs,
+    ):
         """
         Add a series of line segments (in browser, lines are always size 1 right now)
 
         :param name: an identifier for this object
         :param points: (N, 3) float, list of points
         :param segs: (N, 2) int, optionally, indices between points
             for which to draw the segments. If not given, draws 1-2-3-4...
@@ -343,19 +368,17 @@
         points = _to_np_array(points)
         self.fields[name] = "lines"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if segs is not None:
             self.fields[_f(name, "segs")] = _to_np_array(segs).astype(np.int32)
         self._update_bb(points, **kwargs)
 
-    def add_points(self,
-                   name : str,
-                   points : np.ndarray,
-                   point_size : float = 1.0,
-                   **kwargs):
+    def add_points(
+        self, name: str, points: np.ndarray, point_size: float = 1.0, **kwargs
+    ):
         """
         Add a point cloud (in browser, points are always size 1 right now)
 
         :param name: an identifier for this object
         :param points: (N, 3) float, list of points
         :param point_size: float, point size
         :param color: (3,) color, default is orange (common param, can be 3 item list)
@@ -374,19 +397,22 @@
         points = _to_np_array(points)
         self.fields[name] = "points"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if point_size != 1.0:
             self.fields[_f(name, "point_size")] = np.float32(point_size)
         self._update_bb(points, **kwargs)
 
-    def add_mesh(self, name : str,
-                 points : np.ndarray,
-                 faces : Optional[np.ndarray]=None,
-                 face_size : Optional[int]=None,
-                 **kwargs):
+    def add_mesh(
+        self,
+        name: str,
+        points: np.ndarray,
+        faces: Optional[np.ndarray] = None,
+        face_size: Optional[int] = None,
+        **kwargs,
+    ):
         """
         Add a general mesh
 
         :param name: an identifier for this object
         :param points: (N, 3) float, list of points
         :param faces: (N, face_size) int, list of faces; if not given,
                 faces will be :code:`0-1-2, 3-4-5, 6-7-8`, etc (glDrawArrays)
@@ -411,30 +437,32 @@
         points = _to_np_array(points)
         self.fields[name] = "mesh"
         self.fields[_f(name, "points")] = points.astype(np.float32)
         if face_size is not None:
             self.fields[_f(name, "face_size")] = int(face_size)
             assert face_size >= 1 and face_size <= 3
         if faces is not None:
-            assert faces.ndim == 2 and (face_size is None or faces.shape[1] == face_size), \
-                    f"faces must be (N, face_size={face_size if face_size is not None else -1})"
-        if faces is not None:
+            assert faces.ndim == 2 and (
+                face_size is None or faces.shape[1] == face_size
+            ), f"faces must be (N, face_size={face_size if face_size is not None else -1})"
             self.fields[_f(name, "faces")] = _to_np_array(faces).astype(np.int32)
         self._update_bb(points, **kwargs)
 
-    def add_image(self,
-                  name : str,
-                  image : Union[str, np.ndarray],
-                  r: np.ndarray,
-                  t: np.ndarray,
-                  focal_length : float = 1111.11,
-                  z: float = -0.1,
-                  image_size : int = 64,
-                  opengl: Optional[bool] = None,
-                  **kwargs):
+    def add_image(
+        self,
+        name: str,
+        image: Union[str, np.ndarray],
+        r: np.ndarray,
+        t: np.ndarray,
+        focal_length: float = 1111.11,
+        z: float = -0.1,
+        image_size: int = 64,
+        opengl: Optional[bool] = None,
+        **kwargs,
+    ):
         """
         Add an image (as plane mesh with vertex colors)
 
         :param name: an identifier for this object
         :param path: path to the image
         :param r: (3,) or (4,) or (3, 3) or None, optional
                   C2W rotations for each camera, either as axis-angle,
@@ -454,14 +482,15 @@
                        else use OpenCV. Default: depends on if set_opencv()
                        was used.
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
         """
         if opengl is None:
             opengl = not self.default_opencv
         from PIL import Image  # pip install pillow
+
         if isinstance(image, str):
             im = Image.open(str(image))
         else:
             image = _to_np_array(image)
             if image.dtype != np.uint8:
                 image = (image * 255).astype(dtype=np.uint8)
             im = Image.fromarray(image)
@@ -509,29 +538,30 @@
         self.add_mesh(
             name,
             grid_i,
             faces=faces.reshape(-1, 3),
             face_size=3,
             vert_color=im.reshape(-1, 3).astype(np.float32) / 255.0,
             unlit=True,
-            **kwargs
+            **kwargs,
         )
 
-
     def add_camera_frustum(
-                 self, name : str,
-                 focal_length : Optional[float] = None,
-                 image_width : Optional[float] = None,
-                 image_height : Optional[float] = None,
-                 z : Optional[float] = None,
-                 r : Optional[np.ndarray] = None,
-                 t : Optional[np.ndarray] = None,
-                 connect : bool = False,
-                 update_view : bool = True,
-                 **kwargs):
+        self,
+        name: str,
+        focal_length: Optional[float] = None,
+        image_width: Optional[float] = None,
+        image_height: Optional[float] = None,
+        z: Optional[float] = None,
+        r: Optional[np.ndarray] = None,
+        t: Optional[np.ndarray] = None,
+        connect: bool = False,
+        update_view: bool = True,
+        **kwargs,
+    ):
         """
         Add one or more ideal perspective camera frustums
 
         :param name: an identifier for this object
         :param focal_length: the focal length of the camera (unnormalized), default 1111
         :param image_width: the width of the image/sensor, default 800
         :param image_height: the height of the image/sensor, default 800
@@ -618,115 +648,136 @@
             alld = np.linalg.norm(t - t[0], axis=-1)
             mind = alld[alld > 0.0].min()
             self.fields[_f(name, "z")] = np.float32(mind * 0.6)
 
         if t is not None:
             self._update_bb(t, **kwargs)
 
-
-    def add_mesh_from_file(self, path : str, name_suffix : str="", center : bool=False, **kwargs):
+    def add_mesh_from_file(
+        self, path: str, name_suffix: str = "", center: bool = False, **kwargs
+    ):
         """
         Add a mesh from path using trimesh
 
         :param path: the path to the mesh file
         :param name_suffix: object name will be basename(path) + name_suffix
         :param center: if true, centers object to mean
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
 
         Rest of keyword arguments passed to add_mesh
         """
         import trimesh  # pip install trimesh
-        mesh : trimesh.Trimesh = trimesh.load(path, force='mesh')
-        if hasattr(mesh.visual, 'vertex_colors') and len(mesh.visual.vertex_colors):
-            kwargs['vert_color'] = mesh.visual.vertex_colors[..., :3].astype(np.float32) / 255.0
+
+        mesh: trimesh.Trimesh = trimesh.load(path, force="mesh")
+        if hasattr(mesh.visual, "vertex_colors") and len(mesh.visual.vertex_colors):
+            kwargs["vert_color"] = (
+                mesh.visual.vertex_colors[..., :3].astype(np.float32) / 255.0
+            )
         verts = _to_np_array(mesh.vertices)
         if center:
             verts = verts - np.mean(verts, axis=0)
-        self.add_mesh(osp.basename(path).replace('.', '_') + name_suffix, points=verts,
-                 faces=mesh.faces, **kwargs)
+        self.add_mesh(
+            osp.basename(path).replace(".", "_") + name_suffix,
+            points=verts,
+            faces=mesh.faces,
+            **kwargs,
+        )
         self._update_bb(verts, **kwargs)
 
-    def add_axes(self, name : str = "axes", length : float = 1.0, **kwargs):
+    def add_axes(self, name: str = "axes", length: float = 1.0, **kwargs):
         """
         Add RGB-XYZ axes at [0, 0, 0] (as hardcoded lines)
 
         :param name: identifier, default "axes"
         :param length: float, length of axes
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
 
         Rest of keyword arguments passed to add_lines
         """
-        points = np.array([
-                        [0.0, 0.0, 0.0],
-                        [length, 0.0, 0.0],
-                        [0.0, 0.0, 0.0],
-                        [0.0, length, 0.0],
-                        [0.0, 0.0, 0.0],
-                        [0.0, 0.0, length],
-                    ], dtype=np.float32)
-        self.add_lines(name, points=points,
-                    segs=np.array([
-                            [0, 1],
-                            [2, 3],
-                            [4, 5],
-                        ], dtype=np.int32),
-                    vert_color=np.array([
-                            [1.0, 0.0, 0.0],
-                            [1.0, 0.0, 0.0],
-                            [0.0, 1.0, 0.0],
-                            [0.0, 1.0, 0.0],
-                            [0.0, 0.0, 1.0],
-                            [0.0, 0.0, 1.0],
-                        ], dtype=np.int32),
-                **kwargs)
+        points = np.array(
+            [
+                [0.0, 0.0, 0.0],
+                [length, 0.0, 0.0],
+                [0.0, 0.0, 0.0],
+                [0.0, length, 0.0],
+                [0.0, 0.0, 0.0],
+                [0.0, 0.0, length],
+            ],
+            dtype=np.float32,
+        )
+        self.add_lines(
+            name,
+            points=points,
+            segs=np.array(
+                [
+                    [0, 1],
+                    [2, 3],
+                    [4, 5],
+                ],
+                dtype=np.int32,
+            ),
+            vert_color=np.array(
+                [
+                    [1.0, 0.0, 0.0],
+                    [1.0, 0.0, 0.0],
+                    [0.0, 1.0, 0.0],
+                    [0.0, 1.0, 0.0],
+                    [0.0, 0.0, 1.0],
+                    [0.0, 0.0, 1.0],
+                ],
+                dtype=np.int32,
+            ),
+            **kwargs,
+        )
         self._update_bb(points, **kwargs)
 
-    def remove(self, name : str):
+    def remove(self, name: str):
         """
         Remove an object with given name.
         Note: if you overwrite an object with the same name
         type and arguments, it will overwrite the
         object in the scene.
 
         :param name: the name given to add_*
         """
         self.remove_all([name])
 
-    def remove_all(self, names : List[str]):
+    def remove_all(self, names: List[str]):
         """
         Remove object with given names
 
         :param names: list of names as given to add_*
         """
         to_delete = []
         for name in names:
-            prefix = name + '__'
+            prefix = name + "__"
             for key in self.fields:
                 if key.startswith(prefix) or key == name:
                     to_delete.append(key)
         for key in set(to_delete):
             del self.fields[key]
 
     def clear(self):
         """
         Clear all objects from the scene.
         """
         self.fields.clear()
 
-    def add_volume(self,
-                   name: str,
-                   density : np.ndarray,
-                   colors : np.ndarray,
-                   radius: float = 1.0,
-                   density_threshold: float = 1.0,
-                   data_format: str = "RGBA",
-                   **kwargs
-               ):
+    def add_volume(
+        self,
+        name: str,
+        density: np.ndarray,
+        colors: np.ndarray,
+        radius: float = 1.0,
+        density_threshold: float = 1.0,
+        data_format: str = "RGBA",
+        **kwargs,
+    ):
         """
         Add a 3D volume using the PlenOctree renderer
 
         :param name: an identifier for this object
         :param density: (Dx, Dy, Dz); dimensions need not be powers
                                       of 2 nor equal
         :param colors: (Dx, Dy, Dz, (3, channel_size));
@@ -745,17 +796,20 @@
         :param visible: bool, whether mesh should be visible on init, default true (depends on GET parameter in web version) (common param)
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
         """
         density = _to_np_array(density)
         colors = _to_np_array(colors)
         tree_data = utils.vol2plenoctree(
-                density, colors, radius,
-                density_threshold=density_threshold,
-                data_format=data_format)
+            density,
+            colors,
+            radius,
+            density_threshold=density_threshold,
+            data_format=data_format,
+        )
         self._add_common(name, **kwargs)
         self.fields[name] = "volume"
         for k in tree_data:
             self.fields[_f(name, k)] = tree_data[k]
         self._update_bb(np.array([-radius, -radius, -radius]), **kwargs)
         self._update_bb(np.array([radius, radius, radius]), **kwargs)
 
@@ -774,60 +828,64 @@
                     (common param)
         """
         tree_data = dict(np.load(file))
         self._add_common(name, **kwargs)
         self.fields[name] = "volume"
         for k in tree_data:
             self.fields[_f(name, k)] = tree_data[k]
-        radius = 0.5 / tree_data.get('invradius3', tree_data.get('invradius', None))
+        radius = 0.5 / tree_data.get("invradius3", tree_data.get("invradius", None))
         if isinstance(radius, float):
             radius = np.array([radius] * 3, dtype=np.float32)
         self._update_bb(-radius, **kwargs)
         self._update_bb(radius, **kwargs)
 
     def set_nerf(self, *args, **kwargs):
         """
         Deprecated, please use add_nerf
         """
         warnings.warn("set_nerf is deprecated, please use add_nerf")
         self.add_nerf("nerf", *args, **kwargs)
 
-    def add_nerf(self,
-                 name: str,
-                 eval_fn : Callable[..., Tuple[Any, Any]],
-                 center: Union[Tuple[float, float, float], List[float], float, np.ndarray, None]
-                        = None,
-                 radius: Union[Tuple[float, float, float], List[float], float, np.ndarray, None]
-                        = None,
-                 scale : float = 1.0,
-                 reso : int = 256,
-                 use_dirs : bool = False,
-                 sh_deg : int = 1,
-                 sh_proj_sample_count : int = 15,
-                 sh_proj_use_sparse : bool = True,
-                 sigma_thresh : float = 3.0,
-                 weight_thresh : float = 0.001,
-                 r : Optional[Any] = None,
-                 t : Optional[Any] = None,
-                 focal_length : Optional[Union[float, Tuple[float, float]]] = None,
-                 image_width : Optional[float] = None,
-                 image_height : Optional[float] = None,
-                 sigma_multiplier : float = 1.0,
-                 chunk : int=720720,
-                 device : str = "cuda:0",
-                 **kwargs):
+    def add_nerf(
+        self,
+        name: str,
+        eval_fn: Callable[..., Tuple[Any, Any]],
+        center: Union[
+            Tuple[float, float, float], List[float], float, np.ndarray, None
+        ] = None,
+        radius: Union[
+            Tuple[float, float, float], List[float], float, np.ndarray, None
+        ] = None,
+        scale: float = 1.0,
+        reso: int = 256,
+        use_dirs: bool = False,
+        sh_deg: int = 1,
+        sh_proj_sample_count: int = 15,
+        sh_proj_use_sparse: bool = True,
+        sigma_thresh: float = 3.0,
+        weight_thresh: float = 0.001,
+        r: Optional[Any] = None,
+        t: Optional[Any] = None,
+        focal_length: Optional[Union[float, Tuple[float, float]]] = None,
+        image_width: Optional[float] = None,
+        image_height: Optional[float] = None,
+        sigma_multiplier: float = 1.0,
+        chunk: int = 720720,
+        device: str = "cuda:0",
+        **kwargs,
+    ):
         """
         Discretize and display a NeRF (low quality, for visualization purposes only).
         Currently only supports PyTorch NeRFs.
         Requires tqdm, torch, svox, scipy
 
         :param eval_fn:
                         - If :code:`use_dirs=False`: NeRF function taking a batch of points :code:`(B, 3)` and returning :code:`(rgb (B, 3), sigma (B, 1))` after activation applied.
 
-                        - If :code:`use_dirs=True` then this function should take points :code:`(B, 1, 3)` and kwarg 'dirs' :code:`(1, sh_proj_sample_count, 3)`; it should return :code:`(rgb (B, sh_proj_sample_count, 3), sigma (B, 1))` sigma activation
+                        - If :code:`use_dirs=True` then this function should take points :code:`(B, 1, 3)` and kwarg 'dirs' :code:`(1, sh_proj_sample_count, 3)`; it should return :code:`(rgb (B, sh_proj_sample_count, 3), sigma (B, sh_proj_sample_count, 1))` sigma activation
                             should be applied but rgb must NOT have activation applied for SH projection to work correctly.
 
         :param center: float or (3,), xyz center of volume to discretize
                        (will try to infer from cameras from add_camera_frustum if not given)
         :param radius: float or (3,), xyz half edge length of volume to discretize
                        (will try to infer from cameras from add_camera_frustum if not given)
         :param scale: float, multiples radius by this before using it (this is provided
@@ -863,14 +921,15 @@
                             note this has a different name due to legacy
                             conflict (common param)
         :param visible: bool, whether mesh should be visible on init, default true (depends on GET parameter in web version) (common param)
         :param time: int, time at which the mesh should be displayed; -1=always display (default)
                     (common param)
         """
         import torch
+
         if center is None and not np.isinf(self.bb_min).any():
             center = (self.bb_min + self.bb_max) * 0.5
         if radius is None and not np.isinf(self.bb_min).any():
             radius = (self.bb_max - self.bb_min) * 0.5
 
         if isinstance(center, list) or isinstance(center, tuple):
             center = np.array(center)
@@ -891,18 +950,23 @@
                 c2w[:, :3, :3] = _scipy_rotation_from_auto(_to_np_array(r)).as_matrix()
             c2w = torch.from_numpy(c2w).to(device=device)
         else:
             c2w = None
 
         import torch
         from tqdm import tqdm
+
         from svox import N3Tree
         from svox.helpers import _get_c_extension
-        from .utils.sh import project_function_sparse, project_function
-        project_fun = project_function_sparse if sh_proj_use_sparse else project_function
+
+        from .utils.sh import project_function, project_function_sparse
+
+        project_fun = (
+            project_function_sparse if sh_proj_use_sparse else project_function
+        )
 
         _C = _get_c_extension()
         with torch.no_grad():
             # Hardcoded for now
             sh_dim = (sh_deg + 1) ** 2
             data_format = f"SH{sh_dim}" if use_dirs else "RGBA"
             init_grid_depth = reso.bit_length() - 2
@@ -922,50 +986,56 @@
             offset = tree.offset.cpu()
             scale = tree.invradius.cpu()
 
             arr = (torch.arange(0, reso, dtype=torch.float32) + 0.5) / reso
             xx = (arr - offset[0]) / scale[0]
             yy = (arr - offset[1]) / scale[1]
             zz = (arr - offset[2]) / scale[2]
-            grid = torch.stack(torch.meshgrid(xx, yy, zz)).reshape(3, -1).T
+            grid = (
+                torch.stack(torch.meshgrid(xx, yy, zz, indexing="ij")).reshape(3, -1).T
+            )
 
             print("  Evaluating NeRF on a grid")
             out_chunks = []
             if use_dirs:
                 print("   Note: using SH projection")
                 # Adjust chunk size according to sample count to avoid OOM
                 chunk = max(chunk // sh_proj_sample_count, 1)
             for i in tqdm(range(0, grid.shape[0], chunk)):
                 grid_chunk = grid[i : i + chunk].cuda()
                 # TODO: support mip-NeRF
                 if use_dirs:
+
                     def _spherical_func(viewdirs):
                         raw_rgb, sigma = eval_fn(grid_chunk[:, None], dirs=viewdirs)
                         return raw_rgb, sigma
 
                     rgb, sigma = project_fun(
-                            order=sh_deg,
-                            spherical_func=_spherical_func,
-                            sample_count=sh_proj_sample_count,
-                            device=grid_chunk.device)
+                        order=sh_deg,
+                        spherical_func=_spherical_func,
+                        sample_count=sh_proj_sample_count,
+                        device=grid_chunk.device,
+                    )
                 else:
                     rgb, sigma = eval_fn(grid_chunk)
                     if rgb.shape[-1] == 1:
-                        rgb = rgb.expand(-1, 3) # Grayscale
-                    elif rgb.shape[-1] != 3 and str(tree.data_format) == 'RGBA':
-                        tree.expand(f'SH{rgb.shape[-1] // 3}')
+                        rgb = rgb.expand(-1, 3)  # Grayscale
+                    elif rgb.shape[-1] != 3 and str(tree.data_format) == "RGBA":
+                        tree.expand(f"SH{rgb.shape[-1] // 3}")
 
                 rgb_sigma = torch.cat([rgb, sigma], dim=-1)
                 del grid_chunk, rgb, sigma
                 out_chunks.append(rgb_sigma.squeeze(-1))
             rgb_sigma = torch.cat(out_chunks, 0)
             del out_chunks
 
-            def _calculate_grid_weights(sigmas, c2w, focal_length, image_width, image_height):
-                print('  Performing weight thresholding ')
+            def _calculate_grid_weights(
+                sigmas, c2w, focal_length, image_width, image_height
+            ):
+                print("  Performing weight thresholding ")
                 # Weight thresholding impl
                 opts = _C.RenderOptions()
                 opts.step_size = 1e-5
                 opts.sigma_thresh = 0.0
                 opts.ndc_width = -1
 
                 cam = _C.CameraSpec()
@@ -975,15 +1045,19 @@
                 cam.fy = focal_length[1]
                 cam.width = image_width
                 cam.height = image_height
 
                 grid_data = sigmas.reshape((reso, reso, reso)).contiguous()
                 maximum_weight = torch.zeros_like(grid_data)
                 camspace_trans = torch.diag(
-                    torch.tensor([1, -1, -1, 1], dtype=sigmas.dtype, device=sigmas.device)
+                    torch.tensor(
+                        [1, -1, -1, 1],
+                        dtype=sigmas.dtype,
+                        device=sigmas.device,
+                    )
                 )
                 for idx in tqdm(range(c2w.shape[0])):
                     cam.c2w = c2w[idx]
                     cam.c2w = cam.c2w @ camspace_trans
                     grid_weight, _ = _C.grid_weight_render(
                         grid_data,
                         cam,
@@ -995,25 +1069,44 @@
                 return maximum_weight
 
             if c2w is None:
                 # Sigma thresh
                 mask = rgb_sigma[..., -1] >= sigma_thresh
             else:
                 # Weight thresh
-                assert (focal_length is not None and image_height is not None and
-                        image_width is not None), "All of r, t, focal_length, image_width, " \
-                       "image_height should be provided to set_nerf to use weight thresholding"
-                grid_weights = _calculate_grid_weights(rgb_sigma[..., -1:], c2w.float(), focal_length, image_width, image_height)
+                assert (
+                    focal_length is not None
+                    and image_height is not None
+                    and image_width is not None
+                ), (
+                    "All of r, t, focal_length, image_width, "
+                    "image_height should be provided to set_nerf to use weight thresholding"
+                )
+                grid_weights = _calculate_grid_weights(
+                    rgb_sigma[..., -1:],
+                    c2w.float(),
+                    focal_length,
+                    image_width,
+                    image_height,
+                )
                 mask = grid_weights.reshape(-1) >= weight_thresh
-            grid = grid[mask]
+            grid = grid[mask.cpu()]
             rgb_sigma = rgb_sigma[mask]
             del mask
-            assert grid.shape[0] > 0, "This NeRF is completely empty! Make sure you set the bounds reasonably"
-            print("  Grid shape =", grid.shape, "min =", grid.min(dim=0).values,
-                    " max =", grid.max(dim=0).values)
+            assert (
+                grid.shape[0] > 0
+            ), "This NeRF is completely empty! Make sure you set the bounds reasonably"
+            print(
+                "  Grid shape =",
+                grid.shape,
+                "min =",
+                grid.min(dim=0).values,
+                " max =",
+                grid.max(dim=0).values,
+            )
             grid = grid.cuda()
 
             torch.cuda.empty_cache()
 
             print("  Building octree structure")
             for i in range(init_grid_depth):
                 tree[grid].refine()
@@ -1025,71 +1118,73 @@
 
             # Just a sanity check, if it failed maybe all points got filtered out
             assert tree.max_depth == init_grid_depth
             print(" Finishing up")
 
             tree.shrink_to_fit()
             tree_data = {
-                "data_dim" : tree.data_dim,
-                "data_format" : repr(tree.data_format),
-                "child" : tree.child.cpu(),
-                "invradius3" : tree.invradius.cpu(),
-                "offset" : tree.offset.cpu(),
-                "data": tree.data.data.half().cpu().numpy()
+                "data_dim": tree.data_dim,
+                "data_format": repr(tree.data_format),
+                "child": tree.child.cpu(),
+                "invradius3": tree.invradius.cpu(),
+                "offset": tree.offset.cpu(),
+                "data": tree.data.data.half().cpu().numpy(),
             }
-            if 'nerf_scale' in kwargs:
-                kwargs['scale'] = kwargs['nerf_scale']
+            if "nerf_scale" in kwargs:
+                kwargs["scale"] = kwargs["nerf_scale"]
             self._add_common(name, **kwargs)
             self.fields[name] = "volume"
             for k in tree_data:
                 self.fields[_f(name, k)] = tree_data[k]
 
-
-    def write(self, path : str, compress : bool = True):
+    def write(self, path: str, compress: bool = True):
         """
         Write to drawlist npz which you can open with volrend
         (:code:`volrend --draw <output.npz>`;
         nerfvis_base branch recommended for more up-to-date experience)
         as well as in the web viewer. Usually, it's easier to use one of
         :code:`Scene.export()`,
         :code:`Scene.display()`, or
         :code:`Scene.emebd()`
 
         :param path: output npz path
         """
-        if not path.endswith('.draw.npz'):
-            warnings.warn('The filename does not end in .draw.npz, '
-                          'this will not work in web viewer')
+        if not path.endswith(".draw.npz"):
+            warnings.warn(
+                "The filename does not end in .draw.npz, "
+                "this will not work in web viewer"
+            )
         if self.fields:
             fields = self.fields
         else:
             # Make sure it is nonempty
-            fields = {"0" : 0}
+            fields = {"0": 0}
         if compress:
             np.savez_compressed(path, **fields)
         else:
             np.savez(path, **fields)
 
     def export(
-            self,
-            dirname : Optional[str] = None,
-            display : bool = False,
-            world_up : Optional[np.ndarray] = None,
-            cam_center : Optional[np.ndarray] = None,
-            cam_forward : Optional[np.ndarray] = None,
-            cam_origin : Optional[np.ndarray] = None,
-            compress: bool = True,
-            instructions : List[str] = [],
-            css : str = "",
-            url : str = 'localhost',
-            port : int = 8888,
-            open_browser : bool = False,
-            output_html_name : str = 'index.html',
-            embed_output : bool = False,
-            serve_nonblocking : bool = False) -> Tuple[str, str]:
+        self,
+        dirname: Optional[str] = None,
+        display: bool = False,
+        world_up: Optional[np.ndarray] = None,
+        cam_center: Optional[np.ndarray] = None,
+        cam_forward: Optional[np.ndarray] = None,
+        cam_origin: Optional[np.ndarray] = None,
+        compress: bool = True,
+        instructions: List[str] = [],
+        css: str = "",
+        url: str = "localhost",
+        port: int = 8888,
+        open_browser: bool = False,
+        output_html_name: str = "index.html",
+        embed_output: bool = False,
+        serve_nonblocking: bool = False,
+    ) -> Tuple[str, str]:
         """
         Write to a standalone web viewer
 
         :param dirname: output folder path, if not given then uses :code:`./nerfvis_scenes/(0-9a-zA-Z_ from self.title)`
         :param display: if true, serves the output using http.server (default false)
         :param world_up: (3,), optionally, world up unit vector for mouse orbiting
                                (will try to infer from cameras from add_camera_frustum if not given)
@@ -1113,15 +1208,17 @@
         :param serve_nonblocking: bool, if true, and display=True, open a server in another
                                   threading and continues execution
 
         :return: dirname, if it was not provided, returns the generated folder name;
                  url
         """
         if dirname is None:
-            dirname = osp.join("nerfvis_scenes", re.sub("[^0-9a-zA-Z_]", "", self.title))
+            dirname = osp.join(
+                "nerfvis_scenes", re.sub("[^0-9a-zA-Z_]", "", self.title)
+            )
         os.makedirs(dirname, exist_ok=True)
 
         if world_up is not None:
             world_up = _to_np_array(world_up)
         elif self.world_up is not None:
             world_up = _to_np_array(self.world_up)
         bb_available = not np.isinf(self.bb_min).any()
@@ -1145,122 +1242,153 @@
             elif cam_forward is not None and cam_origin is not None:
                 cam_center = cam_origin - cam_forward
 
         all_instructions = []
         all_instructions.extend(instructions)
         # Use lower PlenOctree render quality
         # (ugly hack, executes javascript in the browser like this)
-        all_instructions.extend(["let opt = Volrend.get_options()",
+        all_instructions.extend(
+            [
+                "let opt = Volrend.get_options()",
                 "opt.step_size = 2e-3",
                 "opt.stop_thresh = 1e-1",
                 "opt.sigma_thresh = 1e-1",
-                "Volrend.set_options(opt)"])
+                "Volrend.set_options(opt)",
+            ]
+        )
         out_npz_fname = f"volrend.draw.npz"
         all_instructions.append(f'Volrend.set_title("{self.title}")')
         if world_up is not None:
-            all_instructions.append('Volrend.set_world_up(' + _format_vec3(world_up) + ')')
+            all_instructions.append(
+                "Volrend.set_world_up(" + _format_vec3(world_up) + ")"
+            )
         if cam_center is not None:
-            all_instructions.append('Volrend.set_cam_center(' + _format_vec3(cam_center) + ')')
+            all_instructions.append(
+                "Volrend.set_cam_center(" + _format_vec3(cam_center) + ")"
+            )
         if cam_forward is not None:
             cam_forward = _to_np_array(cam_forward)
-            all_instructions.append('Volrend.set_cam_back(' + _format_vec3(-cam_forward) + ')')
+            all_instructions.append(
+                "Volrend.set_cam_back(" + _format_vec3(-cam_forward) + ")"
+            )
         if cam_origin is not None:
-            all_instructions.append('Volrend.set_cam_origin(' + _format_vec3(cam_origin) + ')')
-        index_html_src_path = osp.join(osp.dirname(osp.realpath(__file__)), "index.html")
+            all_instructions.append(
+                "Volrend.set_cam_origin(" + _format_vec3(cam_origin) + ")"
+            )
+        index_html_src_path = osp.join(
+            osp.dirname(osp.realpath(__file__)), "index.html"
+        )
         index_html_path = osp.join(dirname, output_html_name)
         if osp.isfile(index_html_path):
             os.unlink(index_html_path)
 
         out_npz_path = osp.join(dirname, out_npz_fname)
         self.write(out_npz_path, compress=compress)
 
         if embed_output:
             # Embed the output as a blob URL
-            with open(out_npz_path, 'rb') as f:
+            with open(out_npz_path, "rb") as f:
                 npz_bytes = f.read()
-                base64_npz = base64.b64encode(npz_bytes).decode('utf-8')
-                all_instructions.append('let blob_url = await fetch("data: \'application/octet-stream\';base64,' + base64_npz + '").then(res => res.blob()).then(URL.createObjectURL);')
-                all_instructions.append('Volrend.load_remote(blob_url)')
+                base64_npz = base64.b64encode(npz_bytes).decode("utf-8")
+                all_instructions.append(
+                    "let blob_url = await fetch(\"data: 'application/octet-stream';base64,"
+                    + base64_npz
+                    + '").then(res => res.blob()).then(URL.createObjectURL);'
+                )
+                all_instructions.append("Volrend.load_remote(blob_url)")
             os.unlink(out_npz_path)
         else:
             all_instructions.append(f'Volrend.load_remote("{out_npz_fname}")')
 
         # Inject JS into HTML at </body>
         with open(index_html_src_path, "r") as f:
             html = f.read()
         bodyspl = html.split("</body>")
         assert len(bodyspl) == 2, "Malformed html"
 
-        JS_INJECT = \
-"""
+        JS_INJECT = """
 <script>
 window.addEventListener("volrend_ready", async function() {
     {{instructions}};
 });
 </script>
-""".replace("{{instructions}}", ";\n".join(all_instructions))
+""".replace(
+            "{{instructions}}", ";\n".join(all_instructions)
+        )
 
         html = bodyspl[0] + JS_INJECT + "</body>" + bodyspl[1]
 
         if css:
             stylespl = html.split("</style>")
             assert len(bodyspl) >= 2, "Malformed html"
-            html = stylespl[0] + "\n" + css + "\n</style>" + "</style>".join(stylespl[1:])
+            html = (
+                stylespl[0] + "\n" + css + "\n</style>" + "</style>".join(stylespl[1:])
+            )
         with open(index_html_path, "w") as f:
             f.write(html)
 
-        final_url = ''
+        final_url = ""
         if display:
             from http.server import HTTPServer, SimpleHTTPRequestHandler
+
             class LocalHandler(SimpleHTTPRequestHandler):
                 def __init__(self, *args, **kwargs):
-                    super().__init__(*args, directory=dirname, **kwargs)
+                    if tuple(map(int, platform.python_version_tuple())) < (3, 7, 0):
+                        # Python < 3.7 legacy
+                        assert dirname is not None
+                        os.chdir(dirname)
+                    else:
+                        super().__init__(*args, directory=dirname, **kwargs)
 
             global _server_thds
             global _servers
             for s in _servers:
                 s.shutdown()
                 s.server_close()
             for thd in _server_thds:
                 thd.join()
             _servers = []
             _server_thds = []
 
             server = None
             for port_i in range(port, port + 32):
                 try:
-                    server = HTTPServer(('', port_i), LocalHandler)
-                    print(f'Serving {url}:{port_i}')
+                    server = HTTPServer(("", port_i), LocalHandler)
+                    print(f"Serving {url}:{port_i}")
                     port = port_i
                     break
                 except OSError:
                     server = None
                     pass
             assert server is not None, f"Could not find open port near {port}"
 
-            final_url = f'http://{url}:{port}'
+            final_url = f"http://{url}:{port}"
             if open_browser:
                 import webbrowser
+
                 def open_webbrowser():
                     if not webbrowser.open_new(final_url):
-                        print('Could not open web browser',
-                              '(note: server still launched, '
-                              'please just open given port manually, using port forarding)')
-                t=threading.Thread(target=open_webbrowser)
+                        print(
+                            "Could not open web browser",
+                            "(note: server still launched, "
+                            "please just open given port manually, using port forarding)",
+                        )
+
+                t = threading.Thread(target=open_webbrowser)
                 t.start()
             if serve_nonblocking:
-                t_serve=threading.Thread(target=server.serve_forever)
+                t_serve = threading.Thread(target=server.serve_forever)
                 t_serve.start()
                 _servers.append(server)
                 _server_thds.append(t_serve)
             else:
                 try:
                     server.serve_forever()
                 except KeyboardInterrupt:
-                    print('nervfvis-server interrupted')
+                    print("nervfvis-server interrupted")
         return dirname, final_url
 
     def display(self, *args, **kwargs) -> Tuple[str, str]:
         """
         Alias of :code:`Scene.export` with :code:`display=True` (serve using http.server)
 
         :param dirname: output folder path, if not given then uses :code:`./nerfvis_scenes/(0-9a-zA-Z_ from self.title)`
@@ -1280,18 +1408,15 @@
         :param open_browser: bool, if true then opens the web browser, if possible (default False)
 
         :return: dirname, if it was not provided, returns the generated folder name;
                  url
         """
         return self.export(*args, display=True, **kwargs)
 
-    def embed(self,
-              width: int = 1100,
-              height: int = 600,
-              *args, **kwargs):
+    def embed(self, width: int = 1100, height: int = 600, *args, **kwargs):
         """
         Calls :code:`Scene.export` but in addition embeds inside a notebook.
 
         NOTE 1: if the notebook is opened from a different notebook root folder
         in the future it will not work.
 
         NOTE 2: still writes files to ./nerfvis_scenes folder, and it may get large
@@ -1312,26 +1437,35 @@
         :param port: int, port for server (if display=True) default 8888
                         (if not available, tries next up to 32)
         :param open_browser: bool, if true then opens the web browser, if possible (default False)
 
         :return: dirname, if it was not provided, returns the generated folder name;
                  url
         """
-        from IPython.display import display, IFrame, HTML  # Requires IPython
-        import random, string
-        JUPYTER_ROOT = os.readlink('/proc/%s/cwd' % os.environ['JPY_PARENT_PID'])
-        dirname_rel = osp.join("nerfvis_ipy_scenes", re.sub("[^0-9a-zA-Z_]", "", self.title))
+        import random
+        import string
+
+        from IPython.display import HTML, IFrame, display  # Requires IPython
+
+        JUPYTER_ROOT = os.readlink("/proc/%s/cwd" % os.environ["JPY_PARENT_PID"])
+        dirname_rel = osp.join(
+            "nerfvis_ipy_scenes", re.sub("[^0-9a-zA-Z_]", "", self.title)
+        )
         dirname = osp.join(JUPYTER_ROOT, dirname_rel)
-        randstr = ''.join(
-                random.choice(string.ascii_uppercase + string.digits) for _ in range(10))
+        randstr = "".join(
+            random.choice(string.ascii_uppercase + string.digits) for _ in range(10)
+        )
         embed_name = "ipython_embed_" + randstr + ".html"
         #  css_inject = "#main-wrapper {max-height:101vh}"
         self.export(
-                dirname,
-                *args, display=False, open_browser=False,
-                #  css=css_inject,
-                serve_nonblocking=False, embed_output=True,
-                                 output_html_name=embed_name,
-                                 **kwargs)
+            dirname,
+            *args,
+            display=False,
+            open_browser=False,
+            #  css=css_inject,
+            serve_nonblocking=False,
+            embed_output=True,
+            output_html_name=embed_name,
+            **kwargs,
+        )
         html_file = os.path.join(dirname_rel, embed_name)
         display(IFrame(html_file, width, height))
-
```

### Comparing `nerfvis-0.1.7/nerfvis/utils/__init__.py` & `nerfvis-0.1.8/nerfvis/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 from typing import Dict
 
 import numpy as np
 
 try:
     from ._rotation import Rotation
 except:
-    from scipy.spatial.transform import Rotation # If cython not available, requires scipy
+    from scipy.spatial.transform import (
+        Rotation,
+    )  # If cython not available, requires scipy
+
 
 def _expand_bits(v):
-    v = (v | (v << 16)) & 0x030000FF;
-    v = (v | (v << 8)) & 0x0300F00F;
-    v = (v | (v << 4)) & 0x030C30C3;
-    v = (v | (v << 2)) & 0x09249249;
-    return v;
+    v = (v | (v << 16)) & 0x030000FF
+    v = (v | (v << 8)) & 0x0300F00F
+    v = (v | (v << 4)) & 0x030C30C3
+    v = (v | (v << 2)) & 0x09249249
+    return v
+
 
 def _unexpand_bits(v):
-    v &= 0x49249249;
-    v = (v | (v >> 2)) & 0xc30c30c3;
-    v = (v | (v >> 4)) & 0xf00f00f;
-    v = (v | (v >> 8)) & 0xff0000ff;
-    v = (v | (v >> 16)) & 0x0000ffff;
-    return v;
+    v &= 0x49249249
+    v = (v | (v >> 2)) & 0xC30C30C3
+    v = (v | (v >> 4)) & 0xF00F00F
+    v = (v | (v >> 8)) & 0xFF0000FF
+    v = (v | (v >> 16)) & 0x0000FFFF
+    return v
+
 
 def morton(x, y, z):
-    xx = _expand_bits(x);
-    yy = _expand_bits(y);
-    zz = _expand_bits(z);
-    return (xx << 2) + (yy << 1) + zz;
+    xx = _expand_bits(x)
+    yy = _expand_bits(y)
+    zz = _expand_bits(z)
+    return (xx << 2) + (yy << 1) + zz
+
 
 def inv_morton(code):
-    x = _unexpand_bits(code >> 2);
-    y = _unexpand_bits(code >> 1);
-    z = _unexpand_bits(code);
+    x = _unexpand_bits(code >> 2)
+    y = _unexpand_bits(code >> 1)
+    z = _unexpand_bits(code)
     return x, y, z
 
+
 def morton_grid(pow2) -> np.ndarray:
     mg = np.mgrid[:pow2, :pow2, :pow2].reshape(3, -1)
     return morton(*mg)
 
-def inv_morton_grid(pow2 : int) -> np.ndarray:
-    mg = np.arange(pow2 ** 3)
+
+def inv_morton_grid(pow2: int) -> np.ndarray:
+    mg = np.arange(pow2**3)
     x, y, z = inv_morton(mg)
     return (x * pow2 + y) * pow2 + z
 
+
 def vol2plenoctree(
-            density : np.ndarray,
-            colors : np.ndarray,
-            radius: float = 1.0,
-            density_threshold: float = 1.0,
-            data_format : str = "RGBA") -> Dict[str, np.ndarray]:
+    density: np.ndarray,
+    colors: np.ndarray,
+    radius: float = 1.0,
+    density_threshold: float = 1.0,
+    data_format: str = "RGBA",
+) -> Dict[str, np.ndarray]:
     """
     Convert arbirary volume to PlenOctree
 
     :param density: (Dx, Dy, Dz); dimensions need not be powers
                                   of 2 nor equal
     :param colors: (Dx, Dy, Dz, (3, channel_size));
                                   color data,
@@ -70,57 +80,58 @@
                    :code:`np.savez_compressed("name.npz", **returned_data)`
                    or
                    :code:`np.savez("name.npz", **returned_data)`
                    and open it with volrend.
     """
     # Check dimensions
     assert density.ndim == 3
-    assert colors.ndim == 4 and tuple(colors.shape[:3]) == tuple(density.shape), \
-            f"{density.shape} != {colors.shape[:3]}"
+    assert colors.ndim == 4 and tuple(colors.shape[:3]) == tuple(
+        density.shape
+    ), f"{density.shape} != {colors.shape[:3]}"
 
     dims = list(density.shape)
     maxdim = max(dims)
     assert maxdim <= 1024, "Voxel grid too large"
     n_levels = (maxdim - 1).bit_length()
 
     # Check data formats
     valid_data_formats = {
-        "RGBA" : 4,
-        "SH1" : 4,
-        "SH4" : 13,
-        "SH9" : 28,
-        "SH16" : 49,
+        "RGBA": 4,
+        "SH1": 4,
+        "SH4": 13,
+        "SH9": 28,
+        "SH16": 49,
     }
     assert data_format in valid_data_formats, f"Invalid ddata format {data_format}"
     data_dim = valid_data_formats[data_format]
 
     # Check if given shape matches promised format
     assert colors.shape[-1] + 1 == data_dim
 
     result = {}
-    result['data_dim'] = np.int64(data_dim)
-    result['data_format'] = data_format
-    result['invradius3'] = np.array([
-             0.5 / radius,
-             0.5 / radius,
-             0.5 / radius], dtype=np.float32)
-
-    require_pad = dims != [2 ** n_levels] * 3
-    center = np.array([radius * (1.0 - dim / 2 ** n_levels) for dim in dims],
-                      dtype=np.float32)
+    result["data_dim"] = np.int64(data_dim)
+    result["data_format"] = data_format
+    result["invradius3"] = np.array(
+        [0.5 / radius, 0.5 / radius, 0.5 / radius], dtype=np.float32
+    )
+
+    require_pad = dims != [2**n_levels] * 3
+    center = np.array(
+        [radius * (1.0 - dim / 2**n_levels) for dim in dims],
+        dtype=np.float32,
+    )
 
-    result['offset'] = (0.5 * (1.0 - center / radius)).astype(
-            np.float32)
+    result["offset"] = (0.5 * (1.0 - center / radius)).astype(np.float32)
 
     # Construct mask hierarchy
     hierarchy = []
-    pow2 = 2 ** n_levels
+    pow2 = 2**n_levels
     mask = np.zeros((pow2, pow2, pow2), dtype=bool)
     density_mask = density > density_threshold
-    mask[:dims[0], :dims[1], :dims[2]] = density_mask
+    mask[: dims[0], : dims[1], : dims[2]] = density_mask
 
     hierarchy.append(mask)
     while pow2 > 1:
         mask = mask.reshape((pow2 // 2, 2, pow2 // 2, 2, pow2 // 2, 2))
         mask = mask.any(axis=(1, 3, 5))
         pow2 //= 2
         hierarchy.append(mask)
@@ -134,63 +145,84 @@
     curr_indices = np.zeros(1, dtype=np.uint32)
     for i, (mask, next_mask) in enumerate(zip(hierarchy[:-1], hierarchy[1:])):
         nnodes = mask.sum()
         pow2 = mask.shape[0]
 
         if i == len(hierarchy) - 2:
             # Construct the last tree level
-            child = np.zeros((nnodes, 2, 2, 2), dtype=np.uint32);
+            child = np.zeros((nnodes, 2, 2, 2), dtype=np.uint32)
             if require_pad:
                 # Data is not power of 2, pad it
                 npow2 = 2 * pow2
-                density = np.pad(density,
-                                 [(0, npow2 - dims[0]), (0, npow2 - dims[1]),
-                                  (0, npow2 - dims[2])])
-                colors = np.pad(colors,
-                                [(0, npow2 - dims[0]), (0, npow2 - dims[1]),
-                                 (0, npow2 - dims[2]), (0, 0)])
+                density = np.pad(
+                    density,
+                    [
+                        (0, npow2 - dims[0]),
+                        (0, npow2 - dims[1]),
+                        (0, npow2 - dims[2]),
+                    ],
+                )
+                colors = np.pad(
+                    colors,
+                    [
+                        (0, npow2 - dims[0]),
+                        (0, npow2 - dims[1]),
+                        (0, npow2 - dims[2]),
+                        (0, 0),
+                    ],
+                )
 
             mask_indices = curr_indices[mask.reshape(-1)]
-            density_i = np.empty((nnodes, 2, 2, 2, 1), dtype=np.float16);
-            density_i[mask_indices] = density.reshape(
-                    pow2, 2, pow2, 2, pow2, 2, 1).transpose(
-                            0, 2, 4, 1, 3, 5, 6).reshape(
-                            -1, 2, 2, 2, 1)[mask.flatten()].astype(np.float16)
-            colors_i = np.empty((nnodes, 2, 2, 2, data_dim - 1), dtype=np.float16);
-            colors_i[mask_indices] = colors.reshape(
-                    pow2, 2, pow2, 2, pow2, 2, data_dim - 1).transpose(
-                            0, 2, 4, 1, 3, 5, 6).reshape(
-                            -1, 2, 2, 2, data_dim - 1)[mask.flatten()].astype(np.float16)
-            data = np.concatenate([colors_i.astype(np.float16),
-                                   density_i.astype(np.float16)], -1)
+            density_i = np.empty((nnodes, 2, 2, 2, 1), dtype=np.float16)
+            density_i[mask_indices] = (
+                density.reshape(pow2, 2, pow2, 2, pow2, 2, 1)
+                .transpose(0, 2, 4, 1, 3, 5, 6)
+                .reshape(-1, 2, 2, 2, 1)[mask.flatten()]
+                .astype(np.float16)
+            )
+            colors_i = np.empty((nnodes, 2, 2, 2, data_dim - 1), dtype=np.float16)
+            colors_i[mask_indices] = (
+                colors.reshape(pow2, 2, pow2, 2, pow2, 2, data_dim - 1)
+                .transpose(0, 2, 4, 1, 3, 5, 6)
+                .reshape(-1, 2, 2, 2, data_dim - 1)[mask.flatten()]
+                .astype(np.float16)
+            )
+            data = np.concatenate(
+                [colors_i.astype(np.float16), density_i.astype(np.float16)], -1
+            )
         else:
             # Construct an internal level
             mg, img = morton_grid(pow2 * 2), inv_morton_grid(pow2 * 2)
-            next_indices = np.cumsum(next_mask.reshape(-1)[img], dtype=np.uint32)[mg] - 1
+            next_indices = (
+                np.cumsum(next_mask.reshape(-1)[img], dtype=np.uint32)[mg] - 1
+            )
             next_indices[~next_mask.reshape(-1)] = 0
 
-            child = (next_indices.reshape(pow2, 2, pow2, 2, pow2, 2) + nnodes -
-                     curr_indices.reshape(pow2, 1, pow2, 1, pow2, 1))
+            child = (
+                next_indices.reshape(pow2, 2, pow2, 2, pow2, 2)
+                + nnodes
+                - curr_indices.reshape(pow2, 1, pow2, 1, pow2, 1)
+            )
             child = child.reshape(pow2 * 2, pow2 * 2, pow2 * 2)
             child[~next_mask] = 0
             child = child.reshape(pow2, 2, pow2, 2, pow2, 2)
-            child = child.transpose(0, 2, 4, 1, 3, 5).reshape(pow2 ** 3, 2, 2, 2)
+            child = child.transpose(0, 2, 4, 1, 3, 5).reshape(pow2**3, 2, 2, 2)
 
-            child_tmp = np.empty((nnodes, 2, 2, 2), dtype=np.uint32);
+            child_tmp = np.empty((nnodes, 2, 2, 2), dtype=np.uint32)
             child_tmp[curr_indices[mask.reshape(-1)]] = child[mask.reshape(-1)]
             child = child_tmp
 
             # For now, all interior nodes will be empty
-            data = np.zeros((nnodes, 2, 2, 2, data_dim), dtype=np.float16);
+            data = np.zeros((nnodes, 2, 2, 2, data_dim), dtype=np.float16)
             curr_indices = next_indices
 
         all_child.append(child)
         all_data.append(data)
 
     child = np.concatenate(all_child, 0)
     data = np.concatenate(all_data, 0)
-    result['child'] = child.view(np.int32)
-    result['data'] = data
+    result["child"] = child.view(np.int32)
+    result["data"] = data
     return result
 
 
-__all__ = ('Rotation', 'vol2plenoctree')
+__all__ = ("Rotation", "vol2plenoctree")
```

### Comparing `nerfvis-0.1.7/nerfvis/utils/_rotation.c` & `nerfvis-0.1.8/nerfvis/utils/_rotation.c`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.7/nerfvis/utils/_rotation.pyx` & `nerfvis-0.1.8/nerfvis/utils/_rotation.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Taken from scipy
 import re
 import warnings
+
 import numpy as np
 
 cimport numpy as np
+from numpy.math cimport NAN
+from numpy.math cimport PI as pi  # avoid MSVC error
+from numpy.math cimport isnan
+
 cimport cython
 from cython.view cimport array
-from libc.math cimport sqrt, sin, cos, atan2, acos
-from numpy.math cimport PI as pi, NAN, isnan # avoid MSVC error
+from libc.math cimport acos, atan2, cos, sin, sqrt
 
 np.import_array()
 
 # utilities for empty array initialization
 cdef inline double[:] _empty1(int n):
     return array(shape=(n,), itemsize=sizeof(double), format=b"d")
 cdef inline double[:, :] _empty2(int n1, int n2):
```

### Comparing `nerfvis-0.1.7/nerfvis/utils/sh.py` & `nerfvis-0.1.8/nerfvis/utils/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Sperical harmonics projection related functions
 
 Some codes are borrowed from:
 https://github.com/google/spherical-harmonics/blob/master/sh/spherical_harmonics.cc
 """
-from typing import Callable
 import math
+from typing import Callable
+
 import torch
 
 kHardCodedOrderLimit = 4
 
 
 def spher2cart(theta, phi):
     """Convert spherical coordinates into Cartesian coordinates (radius 1)."""
@@ -261,19 +262,21 @@
         # to spherical coordinates).
         # return EvalSHSlow(l, m, dx, dy, dz)
         raise NotImplementedError
 
 
 def spherical_uniform_sampling(sample_count, device="cpu"):
     # See: https://www.bogotobogo.com/Algorithms/uniform_distribution_sphere.php
-    u1 = torch.arange(0, sample_count, dtype=torch.float32, device=device) + \
-         torch.rand([sample_count], dtype=torch.float32, device=device)
+    u1 = torch.arange(0, sample_count, dtype=torch.float32, device=device) + torch.rand(
+        [sample_count], dtype=torch.float32, device=device
+    )
     u1 /= sample_count
-    u2 = torch.arange(0, sample_count, dtype=torch.float32, device=device) + \
-         torch.rand([sample_count], dtype=torch.float32, device=device)
+    u2 = torch.arange(0, sample_count, dtype=torch.float32, device=device) + torch.rand(
+        [sample_count], dtype=torch.float32, device=device
+    )
     u2 /= sample_count
     u2 = u2[torch.randperm(sample_count, device=device)]
     theta = torch.acos(2.0 * u1 - 1.0)
     phi = 2.0 * math.pi * u2
     return theta.to(device), phi.to(device)
 
 
@@ -289,15 +292,17 @@
 
     # generate sample_count uniformly and stratified samples over the sphere
     # See http://www.bogotobogo.com/Algorithms/uniform_distribution_sphere.php
     theta, phi = spherical_uniform_sampling(sample_count, device=device)
     dirs = spher2cart(theta, phi)  # [sample_count, 3]
 
     # evaluate the analytic function for the current spherical coords
-    func_value, others = spherical_func(dirs[None])  # func_value [batch_size, sample_count, C]
+    func_value, others = spherical_func(
+        dirs[None]
+    )  # func_value [batch_size, sample_count, C]
 
     batch_size = func_value.shape[0]
 
     # This is the approach demonstrated in [1] and is useful for arbitrary
     # functions on the sphere that are represented analytically.
     coeffs = torch.empty(
         [batch_size, C, GetCoefficientCount(order)], dtype=torch.float32
@@ -330,44 +335,50 @@
     assert order >= 0, "Order must be at least zero."
     assert sample_count > 0, "Sample count must be at least one."
     C = 3  # rgb channels
 
     # generate sample_count uniformly and stratified samples over the sphere
     # See http://www.bogotobogo.com/Algorithms/uniform_distribution_sphere.php
     theta, phi = spherical_uniform_sampling(sample_count, device=device)
-    dirs = spher2cart(theta, phi)   # [sample_count, 3]
+    dirs = spher2cart(theta, phi)  # [sample_count, 3]
 
     # evaluate the analytic function for the current spherical coords
-    func_value, others = spherical_func(dirs[None])  # func_value [batch_size, sample_count, C]
+    func_value, others = spherical_func(
+        dirs[None]
+    )  # func_value [batch_size, sample_count, C]
     batch_size = func_value.shape[0]
 
     coeff_count = GetCoefficientCount(order)
-    basis_vals = torch.empty(
-        [sample_count, coeff_count], dtype=torch.float32
-    ).to(device)
+    basis_vals = torch.empty([sample_count, coeff_count], dtype=torch.float32).to(
+        device
+    )
 
     # evaluate the SH basis functions up to band O, scale them by the
     # function's value and accumulate them over all generated samples
     for l in range(order + 1):  # end inclusive
         for m in range(-l, l + 1):  # end inclusive
             basis_vals[:, GetIndex(l, m)] = EvalSH(l, m, dirs)
 
     basis_vals = basis_vals.view(
-           sample_count, coeff_count) # [sample_count, coeff_count]
+        sample_count, coeff_count
+    )  # [sample_count, coeff_count]
     func_value = func_value.transpose(0, 1).reshape(
-           sample_count, batch_size * C) # [sample_count, batch_size * C]
-    soln = torch.lstsq(func_value, basis_vals).solution[:basis_vals.size(1)]
+        sample_count, batch_size * C
+    )  # [sample_count, batch_size * C]
+    soln = torch.linalg.lstsq(basis_vals, func_value).solution
     soln = soln.T.reshape(batch_size, -1)
     others = others[:, :1, :]
     others = others.reshape(batch_size, -1)
     return soln, others
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     batch_size = 2
+
     def sphfunc_one(x):
-        return (EvalSH(1, -1, x) + EvalSH(1, 1, x) * 0.5)[None, :, None].expand(batch_size, -1, 3), None
+        return (EvalSH(1, -1, x) + EvalSH(1, 1, x) * 0.5)[None, :, None].expand(
+            batch_size, -1, 3
+        ), None
         #  return torch.ones([batch_size] + list(x.shape[:-1]) + [3]), None
 
     coeffs, others = project_function_sparse(1, sphfunc_one, 10)
     print(coeffs)
-
```

