# Comparing `tmp/pymermaiddiagram-0.0.1.tar.gz` & `tmp/pymermaiddiagram-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymermaiddiagram-0.0.1.tar", last modified: Sun Jun  4 10:31:30 2023, max compression
+gzip compressed data, was "pymermaiddiagram-0.0.2.tar", last modified: Thu Jun 15 15:47:35 2023, max compression
```

## Comparing `pymermaiddiagram-0.0.1.tar` & `pymermaiddiagram-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:30.289897 pymermaiddiagram-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-04 10:31:30.285897 pymermaiddiagram-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 10:31:30.289897 pymermaiddiagram-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:30.285897 pymermaiddiagram-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:30.285897 pymermaiddiagram-0.0.1/src/pymermaiddiagram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram/pymermaid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:30.285897 pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-04 10:31:30.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-04 10:31:30.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:31:30.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 10:31:30.000000 pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:31:30.285897 pymermaiddiagram-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-04 10:31:16.000000 pymermaiddiagram-0.0.1/test/test_pymermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.011519 pymermaiddiagram-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:47:35.011519 pymermaiddiagram-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/pymermaiddiagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram/pymermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 15:47:35.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/test/test_pymermaid.py
```

### Comparing `pymermaiddiagram-0.0.1/LICENSE.txt` & `pymermaiddiagram-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymermaiddiagram-0.0.1/PKG-INFO` & `pymermaiddiagram-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymermaiddiagram
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to create mermaid.js diagrams using python
 Author-email: Gioele SL Fierro <hck@gslf.it>
 Project-URL: Homepage, https://github.com/gslf/PyMermade
 Project-URL: Bug Tracker, https://github.com/gslf/PyMermade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,24 @@
 
 # PyMermaid
 ### A library to create mermaid.js diagrams using python
 ##### Gioele SL Fierro
 
 ---
 
+![pymermaiddiagram logo](/res/pymermaiddiagram.jpg)
+
 ### How to use pymermaiddiagrams
 
 ```python
 import base64
 import requests
 import io
 from PIL import Image
-from pymermaiddiagrams import createDiagram
+from pymermaiddiagram import createDiagram
 
 def main():
     """Example usage of the createDiagram function."""
     string_description = "graph LR;A-->B;A-->C;B-->D;C-->D;"
     diagram_image = createDiagram(string_description)
     diagram_image.show()
```

### Comparing `pymermaiddiagram-0.0.1/src/pymermaiddiagram/pymermaid.py` & `pymermaiddiagram-0.0.2/src/pymermaiddiagram/pymermaid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import base64
-import requests, io
+import requests, io, os.path
 from PIL import Image
 
 def createDiagram(string_description):
     """Creates a diagram using mermaid.js image service from the given string description and returns an Image object.
     
     :param str string_description: containing the Mermaid code for the diagram
     :return: PIL.Image diagram_image: containing the generated diagram
@@ -22,7 +22,15 @@
     diagram_base64_string = diagram_base64_bytes.decode("ascii")
     mermaid_url = 'https://mermaid.ink/img/{}'.format(diagram_base64_string)
 
     diagram_image = Image.open(io.BytesIO(requests.get(mermaid_url).content))
 
     return diagram_image
 
+
+def saveDiagram(string_description, image_name, image_path = ""):
+
+    diagram_image = createDiagram(string_description)
+
+    image_name = image_name + ".jpg"
+    full_path = os.path.join(image_path, image_name)
+    diagram_image.save(full_path)
```

### Comparing `pymermaiddiagram-0.0.1/src/pymermaiddiagram.egg-info/PKG-INFO` & `pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymermaiddiagram
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to create mermaid.js diagrams using python
 Author-email: Gioele SL Fierro <hck@gslf.it>
 Project-URL: Homepage, https://github.com/gslf/PyMermade
 Project-URL: Bug Tracker, https://github.com/gslf/PyMermade/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,24 @@
 
 # PyMermaid
 ### A library to create mermaid.js diagrams using python
 ##### Gioele SL Fierro
 
 ---
 
+![pymermaiddiagram logo](/res/pymermaiddiagram.jpg)
+
 ### How to use pymermaiddiagrams
 
 ```python
 import base64
 import requests
 import io
 from PIL import Image
-from pymermaiddiagrams import createDiagram
+from pymermaiddiagram import createDiagram
 
 def main():
     """Example usage of the createDiagram function."""
     string_description = "graph LR;A-->B;A-->C;B-->D;C-->D;"
     diagram_image = createDiagram(string_description)
     diagram_image.show()
```

### Comparing `pymermaiddiagram-0.0.1/test/test_pymermaid.py` & `pymermaiddiagram-0.0.2/test/test_pymermaid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 sys.path.append(os.path.dirname(os.path.realpath(__file__)) + "/../src")
 
 
 import unittest
 import PIL
-from pymermaiddiagram.pymermaid import createDiagram
+from pymermaiddiagram.pymermaid import createDiagram, saveDiagram
 
 class TestPyMermade(unittest.TestCase):
     def test_diagram_creation(self):
         diagram_description = """
         graph LR;
             A--> B & C & D;
             B--> A & E;
@@ -22,14 +22,46 @@
 
     def test_error_diagram_creation(self):
         with self.assertRaises(Exception):
             diagram_description = ""
             result = createDiagram(diagram_description)
             self.assertRaises(Exception, result)
 
+    def test_diagram_saving(self):
+        diagram_description = """
+        graph LR;
+            A--> B & C & D;
+            B--> A & E;
+            C--> A & E;
+            D--> A & E;
+            E--> B & C & D;
+        """
+        saveDiagram(diagram_description, image_name = "test")
+        exist = os.path.isfile("test.jpg")
+        self.assertTrue(exist)
+        os.remove("test.jpg")
+
+    def test_diagram_saving_with_path(self):
+        diagram_description = """
+        graph LR;
+            A--> B & C & D;
+            B--> A & E;
+            C--> A & E;
+            D--> A & E;
+            E--> B & C & D;
+        """
+        
+        os.mkdir("res")
+        saveDiagram(diagram_description, image_name = "test", image_path = "res")
+        exist = os.path.isfile("res/test.jpg")
+        self.assertTrue(exist)
+        os.remove("res/test.jpg")
+        os.rmdir("res")
+
+
 
 if __name__ == "__main__":
     print("PyMermaid")
     print("Running tests . . .")
 
     unittest.main(verbosity=2)
```

