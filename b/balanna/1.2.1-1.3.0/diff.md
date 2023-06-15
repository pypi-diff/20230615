# Comparing `tmp/balanna-1.2.1.tar.gz` & `tmp/balanna-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanna-1.2.1.tar", last modified: Wed May 31 13:33:17 2023, max compression
+gzip compressed data, was "balanna-1.3.0.tar", last modified: Thu Jun 15 08:08:05 2023, max compression
```

## Comparing `balanna-1.2.1.tar` & `balanna-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.896885 balanna-1.2.1/
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-31 12:50:49.000000 balanna-1.2.1/LICENSE
--rw-r--r--   0 sas      (23222) tumuser  (20909)      247 2023-05-31 13:33:17.896885 balanna-1.2.1/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-31 12:50:49.000000 balanna-1.2.1/README.md
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.880885 balanna-1.2.1/balanna/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/__main__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/camera_trajectories.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     2023 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/rendering_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/trimesh.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.896885 balanna-1.2.1/balanna/utils/
--rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/geometry.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      122 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/types.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/utils/vedo_utils.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10933 2023-05-31 13:17:57.000000 balanna-1.2.1/balanna/window_base.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     5138 2023-05-31 13:27:38.000000 balanna-1.2.1/balanna/window_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4566 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/window_generator.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-31 12:50:49.000000 balanna-1.2.1/balanna/window_real_time.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-31 13:33:17.888885 balanna-1.2.1/balanna.egg-info/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      247 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/SOURCES.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/dependency_links.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/requires.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-31 13:33:17.000000 balanna-1.2.1/balanna.egg-info/top_level.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-31 13:33:17.900885 balanna-1.2.1/setup.cfg
--rw-r--r--   0 sas      (23222) tumuser  (20909)      495 2023-05-31 13:32:31.000000 balanna-1.2.1/setup.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-06-15 08:08:05.355145 balanna-1.3.0/
+-rw-r--r--   0 sele       (501) staff       (20)     1070 2023-06-14 16:44:05.000000 balanna-1.3.0/LICENSE
+-rw-r--r--   0 sele       (501) staff       (20)      247 2023-06-15 08:08:05.355345 balanna-1.3.0/PKG-INFO
+-rw-r--r--   0 sele       (501) staff       (20)      517 2023-06-14 16:44:05.000000 balanna-1.3.0/README.md
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-06-15 08:08:05.345593 balanna-1.3.0/balanna/
+-rw-r--r--   0 sele       (501) staff       (20)      809 2023-06-15 07:57:02.000000 balanna-1.3.0/balanna/__init__.py
+-rw-r--r--   0 sele       (501) staff       (20)     1069 2023-06-14 19:51:15.000000 balanna-1.3.0/balanna/__main__.py
+-rw-r--r--   0 sele       (501) staff       (20)     1581 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/camera_trajectories.py
+-rw-r--r--   0 sele       (501) staff       (20)     2023 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/rendering_dataset.py
+-rw-r--r--   0 sele       (501) staff       (20)    10078 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/trimesh.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-06-15 08:08:05.354367 balanna-1.3.0/balanna/utils/
+-rw-r--r--   0 sele       (501) staff       (20)       30 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/utils/__init__.py
+-rw-r--r--   0 sele       (501) staff       (20)      559 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/utils/geometry.py
+-rw-r--r--   0 sele       (501) staff       (20)      122 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/utils/types.py
+-rw-r--r--   0 sele       (501) staff       (20)     4463 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/utils/vedo_utils.py
+-rw-r--r--   0 sele       (501) staff       (20)    10933 2023-06-15 07:55:50.000000 balanna-1.3.0/balanna/window_base.py
+-rw-r--r--   0 sele       (501) staff       (20)     7968 2023-06-15 07:46:50.000000 balanna-1.3.0/balanna/window_dataset.py
+-rw-r--r--   0 sele       (501) staff       (20)     6107 2023-06-15 07:54:58.000000 balanna-1.3.0/balanna/window_generator.py
+-rw-r--r--   0 sele       (501) staff       (20)     7265 2023-06-14 16:44:05.000000 balanna-1.3.0/balanna/window_real_time.py
+drwxr-xr-x   0 sele       (501) staff       (20)        0 2023-06-15 08:08:05.349402 balanna-1.3.0/balanna.egg-info/
+-rw-r--r--   0 sele       (501) staff       (20)      247 2023-06-15 08:08:05.000000 balanna-1.3.0/balanna.egg-info/PKG-INFO
+-rw-r--r--   0 sele       (501) staff       (20)      517 2023-06-15 08:08:05.000000 balanna-1.3.0/balanna.egg-info/SOURCES.txt
+-rw-r--r--   0 sele       (501) staff       (20)        1 2023-06-15 08:08:05.000000 balanna-1.3.0/balanna.egg-info/dependency_links.txt
+-rw-r--r--   0 sele       (501) staff       (20)       56 2023-06-15 08:08:05.000000 balanna-1.3.0/balanna.egg-info/requires.txt
+-rw-r--r--   0 sele       (501) staff       (20)        8 2023-06-15 08:08:05.000000 balanna-1.3.0/balanna.egg-info/top_level.txt
+-rw-r--r--   0 sele       (501) staff       (20)      103 2023-06-15 08:08:05.356247 balanna-1.3.0/setup.cfg
+-rw-r--r--   0 sele       (501) staff       (20)      495 2023-06-15 08:07:20.000000 balanna-1.3.0/setup.py
```

### Comparing `balanna-1.2.1/LICENSE` & `balanna-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/README.md` & `balanna-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/__init__.py` & `balanna-1.3.0/balanna/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import balanna.camera_trajectories as camera_trajectories
 import balanna.utils as utils
 import balanna.trimesh as trimesh
 
 from balanna.rendering_dataset import render_dataset
-from balanna.window_dataset import display_dataset
-from balanna.window_generator import display_generated, display_scenes
+from balanna.window_dataset import display_dataset, display_dataset_custom, MainWindowDataset
+from balanna.window_generator import display_generated, display_scenes, display_generated_custom, MainWindowGenerator
 from balanna.window_real_time import display_real_time, RealTimeNode
 from balanna.window_base import SceneDictType
 
 
 __all__ = [
   "camera_trajectories", 
   "trimesh",
   "display_dataset",
+  "display_dataset_custom",
   "display_scenes",
   "display_generated",
+  "display_generated_custom",
   "display_real_time", 
   "RealTimeNode",
+  "MainWindowDataset",
+  "MainWindowGenerator",
   "render_dataset",
   "SceneDictType",
 ]
```

### Comparing `balanna-1.2.1/balanna/camera_trajectories.py` & `balanna-1.3.0/balanna/camera_trajectories.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/rendering_dataset.py` & `balanna-1.3.0/balanna/rendering_dataset.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/trimesh.py` & `balanna-1.3.0/balanna/trimesh.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/utils/geometry.py` & `balanna-1.3.0/balanna/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/utils/vedo_utils.py` & `balanna-1.3.0/balanna/utils/vedo_utils.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/window_base.py` & `balanna-1.3.0/balanna/window_base.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna/window_dataset.py` & `balanna-1.3.0/balanna/window_dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import copy
 import numpy as np
 import pathlib
+import pickle as pkl
 
 from matplotlib.axes import Axes
 from PyQt5 import Qt
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Type
 
 from .window_base import MainWindow, SceneDictType
 from .utils.types import contains_scene
 
 
-__all__ = ['display_dataset']
+__all__ = ['display_dataset', 'display_dataset_custom', 'MainWindowDataset']
 
 
 class MainWindowDataset(MainWindow):
 
     def __init__(
         self,
         scenes: List[SceneDictType],
         fps: float,
         video_directory: Optional[Union[pathlib.Path, str]] = None,
         horizontal: bool = True,
         loop: bool = True,
         show_labels: bool = False,
         use_scene_cam: bool = False,
+        store_directory: Optional[Union[pathlib.Path, str]] = None,
         debug: bool = False,
         parent: Qt.QWidget = None
     ):
         self.scenes = scenes
         self.fps = fps
         if len(scenes) == 0:
             return
@@ -46,14 +48,27 @@
             show_labels=show_labels,
             use_scene_cam=use_scene_cam,
             debug=debug,
             parent=parent
         )
         self.render_(scene_dict, resetcam=True)
 
+        # If store_directory is given, save the scene list to the directory.
+        if store_directory is not None:
+            print("\033[36m" + f"Storing scene in directory {store_directory}" + "\033[0m")
+            store_directory = pathlib.Path(store_directory)
+            if store_directory.exists():
+                print("\033[33m" + f"Directory {store_directory} already exists, overwriting..." + "\033[0m")
+            store_directory.mkdir(parents=True, exist_ok=True)
+            for k, scene in enumerate(scenes):
+                pkl_file = store_directory / f"{k:05d}.pkl"
+                with open(pkl_file, 'wb') as f:
+                    pkl.dump(scene, f, protocol=pkl.HIGHEST_PROTOCOL)
+            print("\033[36m" + f"... done" + "\033[0m")
+
         # Setup looping timer and connect it to render a new scene at every timer callback.
         # If loop is true, start looping right away.
         self.timer = Qt.QTimer(self)
         self.timer.timeout.connect(self.render_loop)  # noqa
         if loop:
             self.toggle_looping()
 
@@ -64,19 +79,22 @@
     def render_current_index(self, resetcam: bool = False) -> None:
         if 0 <= self.__frame_idx < len(self.scenes):
             scene_dict = self.scenes[self.__frame_idx]
 
             # The same matplotlib.Axes cannot be used multiple times, as it is assigned to a figure during
             # plotting. Therefore, we need to create a copy of the scene dictionary to be able to reuse it
             # when plotting the scene again later.
-            scene_dict_safe = dict()
-            for key, value in scene_dict.items():
-                if key in self.figure_key_dict.keys():
-                    value = copy.deepcopy(value)
-                scene_dict_safe[key] = value
+            if any(isinstance(value, Axes) for value in scene_dict.values()):
+                scene_dict_safe = dict()
+                for key, value in scene_dict.items():
+                    if key in self.figure_key_dict.keys():
+                        value = copy.deepcopy(value)
+                    scene_dict_safe[key] = value
+            else:
+                scene_dict_safe = scene_dict
 
             self.render_(scene_dict_safe, resetcam=resetcam)
         else:
             # Reset frame index to a valid index.
             self.__frame_idx = max(min(self.__frame_idx, len(self.scenes) - 1), 0)
             # Stop the timer, if it is running.
             if self.timer.isActive():
@@ -104,45 +122,91 @@
     def toggle_looping(self):
         if self.timer.isActive():
             self.timer.stop()
         else:
             self.timer.start(int(1 / self.fps * 1000))  # in milliseconds
 
 
-def display_dataset(
+def display_dataset_custom(
+    main_window_class: Type[MainWindowDataset],
     scenes: List[SceneDictType],
     horizontal: bool = True,
     loop: bool = False,
     fps: float = 30.0,
     video_directory: Optional[Union[pathlib.Path, str]] = None,
     show_labels: bool = False,
     use_scene_cam: bool = False,
+    store_directory: Optional[Union[pathlib.Path, str]] = None,
     debug: bool = False
 ):
-    """Display scenes stored in scene iterator as PyQt app.
+    """Display scenes stored in scene iterator as PyQt app with a custom main window dataset class.
 
     The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
     See SceneDictType for currently supported object types.
 
     Args:
+        main_window_class
         scenes: sorted list of scene dictionaries.
         horizontal: window orientation, horizontal or vertical stacking.
         loop: start looping from beginning.
         fps: frames (i.e. scenes) per second for looping.
         video_directory: directory for storing screenshots.
         show_labels: display the scene dict keys.
         use_scene_cam: use camera transform from trimesh scenes.
+        store_directory: path to directory storing scene pickle files.
         debug: printing debug information.
     """
     app = Qt.QApplication([])
-    window = MainWindowDataset(
+    window = main_window_class(
         scenes=scenes,
         fps=fps,
         video_directory=video_directory,
         horizontal=horizontal,
         loop=loop,
         show_labels=show_labels,
         debug=debug,
-        use_scene_cam=use_scene_cam
+        use_scene_cam=use_scene_cam,
+        store_directory=store_directory
     )
     app.aboutToQuit.connect(window.on_close)
     app.exec_()
+
+
+def display_dataset(
+    scenes: List[SceneDictType],
+    horizontal: bool = True,
+    loop: bool = False,
+    fps: float = 30.0,
+    video_directory: Optional[Union[pathlib.Path, str]] = None,
+    show_labels: bool = False,
+    use_scene_cam: bool = False,
+    store_directory: Optional[Union[pathlib.Path, str]] = None,
+    debug: bool = False
+):
+    """Display scenes stored in scene iterator as PyQt app.
+
+    The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
+    See SceneDictType for currently supported object types.
+
+    Args:
+        scenes: sorted list of scene dictionaries.
+        horizontal: window orientation, horizontal or vertical stacking.
+        loop: start looping from beginning.
+        fps: frames (i.e. scenes) per second for looping.
+        video_directory: directory for storing screenshots.
+        show_labels: display the scene dict keys.
+        use_scene_cam: use camera transform from trimesh scenes.
+        store_directory: path to directory storing scene pickle files.
+        debug: printing debug information.
+    """
+    return display_dataset_custom(
+        main_window_class=MainWindowDataset,
+        scenes=scenes,
+        horizontal=horizontal,
+        loop=loop,
+        fps=fps,
+        video_directory=video_directory,
+        show_labels=show_labels,
+        use_scene_cam=use_scene_cam,
+        store_directory=store_directory,
+        debug=debug
+    )
```

### Comparing `balanna-1.2.1/balanna/window_generator.py` & `balanna-1.3.0/balanna/window_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import pathlib
 
 from matplotlib.axes import Axes
 from PyQt5 import Qt
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional, Union, Type
 
 from .window_base import MainWindow, SceneDictType
 from .utils.types import contains_scene
 
 
-__all__ = ['display_scenes', 'display_generated']
+__all__ = ['display_scenes', 'display_generated', 'display_generated_custom', 'MainWindowGenerator']
 
 
 class MainWindowGenerator(MainWindow):
 
     def __init__(
         self,
         scene_iterator: Iterable[SceneDictType],
@@ -86,51 +86,91 @@
     def toggle_looping(self):
         if self.timer.isActive():
             self.timer.stop()
         else:
             self.timer.start(int(1 / self.fps * 1000))  # in milliseconds
 
 
-def display_generated(
+def display_generated_custom(
+    main_window_class: Type[MainWindowGenerator],
     scene_iterator: Iterable[SceneDictType],
     horizontal: bool = True,
     loop: bool = False,
     fps: float = 30.0,
     video_directory: Optional[Union[pathlib.Path, str]] = None,
     show_labels: bool = False,
     use_scene_cam: bool = False,
     debug: bool = False
 ):
-    """Display scenes stored in scene iterator as PyQt app.
+    """Display scenes stored in scene iterator as PyQt app using custom main window class.
 
     The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
     See SceneDictType for currently supported object types.
 
     Args:
+        main_window_class: custom main window class.
         scene_iterator: iterator function to get the scene dictionaries.
         horizontal: window orientation, horizontal or vertical stacking.
         loop: start looping from beginning.
         fps: frames (i.e. scenes) per second for looping.
         video_directory: directory for storing screenshots.
         show_labels: display the scene dict keys.
         use_scene_cam: use camera transform from trimesh scenes.
         debug: printing debug information.
     """
     app = Qt.QApplication([])
-    window = MainWindowGenerator(
+    window = main_window_class(
         scene_iterator=scene_iterator,
         fps=fps,
         video_directory=video_directory,
         horizontal=horizontal,
         loop=loop,
         show_labels=show_labels,
         debug=debug,
         use_scene_cam=use_scene_cam
     )
     app.aboutToQuit.connect(window.on_close)
     app.exec_()
 
 
+def display_generated(
+    scene_iterator: Iterable[SceneDictType],
+    horizontal: bool = True,
+    loop: bool = False,
+    fps: float = 30.0,
+    video_directory: Optional[Union[pathlib.Path, str]] = None,
+    show_labels: bool = False,
+    use_scene_cam: bool = False,
+    debug: bool = False
+):
+    """Display scenes stored in scene iterator as PyQt app.
+
+    The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
+    See SceneDictType for currently supported object types.
+
+    Args:
+        scene_iterator: iterator function to get the scene dictionaries.
+        horizontal: window orientation, horizontal or vertical stacking.
+        loop: start looping from beginning.
+        fps: frames (i.e. scenes) per second for looping.
+        video_directory: directory for storing screenshots.
+        show_labels: display the scene dict keys.
+        use_scene_cam: use camera transform from trimesh scenes.
+        debug: printing debug information.
+    """
+    return display_generated_custom(
+        main_window_class=MainWindowGenerator,
+        scene_iterator=scene_iterator,
+        horizontal=horizontal,
+        loop=loop,
+        fps=fps,
+        video_directory=video_directory,
+        show_labels=show_labels,
+        debug=debug,
+        use_scene_cam=use_scene_cam
+    )
+
+
 def display_scenes(*args, **kwargs):
     print("\033[93m" + f"display_scenes() is out-dated and will be removed in the next version, "
                        f"use display_generated() instead" + "\033[0m")
     return display_generated(*args, **kwargs)
```

### Comparing `balanna-1.2.1/balanna/window_real_time.py` & `balanna-1.3.0/balanna/window_real_time.py`

 * *Files identical despite different names*

### Comparing `balanna-1.2.1/balanna.egg-info/SOURCES.txt` & `balanna-1.3.0/balanna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

