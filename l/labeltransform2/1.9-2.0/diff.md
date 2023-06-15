# Comparing `tmp/labeltransform2-1.9.tar.gz` & `tmp/labeltransform2-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-1.9.tar", last modified: Wed Jun 14 09:45:26 2023, max compression
+gzip compressed data, was "labeltransform2-2.0.tar", last modified: Thu Jun 15 11:28:47 2023, max compression
```

## Comparing `labeltransform2-1.9.tar` & `labeltransform2-2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.143720 labeltransform2-1.9/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.9/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-14 09:45:26.143720 labeltransform2-1.9/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.138717 labeltransform2-1.9/labeltransform2/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.9/labeltransform2/__init__.py
--rw-rw-rw-   0        0        0     4410 2023-06-14 09:45:11.000000 labeltransform2-1.9/labeltransform2/generate_voc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:45:26.142718 labeltransform2-1.9/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      225 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 09:45:26.000000 labeltransform2-1.9/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:45:26.143720 labeltransform2-1.9/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-14 09:42:41.000000 labeltransform2-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:28:47.124266 labeltransform2-2.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-2.0/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-15 11:28:47.108269 labeltransform2-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 11:28:47.104267 labeltransform2-2.0/labeltransform2/
+-rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-2.0/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0     4675 2023-06-15 06:30:34.000000 labeltransform2-2.0/labeltransform2/generate_voc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:28:47.108269 labeltransform2-2.0/labeltransform2/xml/
+-rw-rw-rw-   0        0        0      469 2023-06-14 03:30:14.000000 labeltransform2-2.0/labeltransform2/xml/voc.xml
+drwxrwxrwx   0        0        0        0 2023-06-15 11:28:47.107267 labeltransform2-2.0/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-06-15 11:28:47.000000 labeltransform2-2.0/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-15 11:28:47.000000 labeltransform2-2.0/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 11:28:47.000000 labeltransform2-2.0/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-15 11:28:47.000000 labeltransform2-2.0/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 11:28:47.000000 labeltransform2-2.0/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 11:28:47.124266 labeltransform2-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      420 2023-06-15 11:28:40.000000 labeltransform2-2.0/setup.py
```

### Comparing `labeltransform2-1.9/LICENSE` & `labeltransform2-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.9/README.md` & `labeltransform2-2.0/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.9/labeltransform2/generate_voc.py` & `labeltransform2-2.0/labeltransform2/generate_voc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Optional
 from pathlib import Path
 from xml.etree import ElementTree as ET
 from multiprocessing import Process
 import pandas as pd
 from copy import deepcopy
 import cv2
-from uuid import uuid4
-import shutil
+import pkg_resources
 
 
 class VocStyle:
     def __init__(self, img_dir, data: Optional[pd.DataFrame]) -> None:
         self.img_dir = Path(img_dir)
-        self.data = data
-        self.data.columns = ["name", "cls", "x1", "y1", "x2", "y2"]
-        self.names = list(set(self.data["name"].to_list()))
+        if data is not None:
+            self.data = data
+            self.data.columns = ["name", "cls", "x1", "y1", "x2", "y2"]
+            self.names = list(set(self.data["name"].to_list()))
+        else:
+            self.names = [i.stem for i in self.img_dir.glob("*.jpg") \
+                if self.img_dir.joinpath(i.stem + ".xml").exists()]
         self.cls_names = {}
     
 
     def write(self, names):
         for name in names:
             tree, root, filename, width, height, depth, obj = self.style()
             img = self.img_dir.joinpath(name + ".jpg")
@@ -29,22 +32,23 @@
             bboxes = self.data[self.data["name"]==name].to_numpy()
             for bbox in bboxes:
                 obj_ = self.new_obj(obj, bbox)
                 root.append(obj_)
             tree.write(self.img_dir.joinpath(name + ".xml"))
     
     def to_voc(self):
+        assert self.data is not None
         n = len(self.names) // 5
         name_list = [self.names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
         for names in name_list:
             task = Process(target=self.write, args=(names, ))
             task.start()
                 
     def style(self):
-        tree0 = ET.parse("./xml/voc.xml")
+        tree0 = ET.parse(pkg_resources.resource_filename("labeltransform2", "xml/voc.xml"))
         tree = deepcopy(tree0)
         root = tree.getroot()
         filename = root.find("filename")
         size = root.find("size")
         width = size.find("width")
         height = size.find("height")
         depth = size.find("depth")
@@ -114,9 +118,8 @@
 
 
 if __name__ == "__main__":
     
     names = list(range(1989))
     n = len(names) // 5
     name_list = [names[i*n:(i+1)*n if i<4 else -1] for i in range(5)]
-
-    print([len(i) for i in name_list])
+    print([len(i) for i in name_list])
```

