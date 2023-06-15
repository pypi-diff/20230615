# Comparing `tmp/pymermaiddiagram-0.0.2.tar.gz` & `tmp/pymermaiddiagram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymermaiddiagram-0.0.2.tar", last modified: Thu Jun 15 15:47:35 2023, max compression
+gzip compressed data, was "pymermaiddiagram-0.0.3.tar", last modified: Thu Jun 15 15:59:36 2023, max compression
```

## Comparing `pymermaiddiagram-0.0.2.tar` & `pymermaiddiagram-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.011519 pymermaiddiagram-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:47:35.011519 pymermaiddiagram-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/pymermaiddiagram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram/pymermaid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 15:47:35.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 15:47:34.000000 pymermaiddiagram-0.0.2/src/pymermaiddiagram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:47:35.007519 pymermaiddiagram-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-15 15:47:21.000000 pymermaiddiagram-0.0.2/test/test_pymermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:36.985973 pymermaiddiagram-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 15:59:36.985973 pymermaiddiagram-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:59:36.985973 pymermaiddiagram-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:36.981973 pymermaiddiagram-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:36.981973 pymermaiddiagram-0.0.3/src/pymermaiddiagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram/pymermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:36.981973 pymermaiddiagram-0.0.3/src/pymermaiddiagram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-15 15:59:36.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 15:59:36.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:59:36.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 15:59:36.000000 pymermaiddiagram-0.0.3/src/pymermaiddiagram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:59:36.981973 pymermaiddiagram-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-15 15:59:25.000000 pymermaiddiagram-0.0.3/test/test_pymermaid.py
```

### Comparing `pymermaiddiagram-0.0.2/LICENSE.txt` & `pymermaiddiagram-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymermaiddiagram-0.0.2/pyproject.toml` & `pymermaiddiagram-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "pillow>=9", "requests>=2"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pymermaiddiagram"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gioele SL Fierro", email="hck@gslf.it" },
 ]
 description = "A library to create mermaid.js diagrams using python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pymermaiddiagram-0.0.2/src/pymermaiddiagram/pymermaid.py` & `pymermaiddiagram-0.0.3/src/pymermaiddiagram/pymermaid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import base64
 import requests, io, os.path
 from PIL import Image
 
 def createDiagram(string_description):
-    """Creates a diagram using mermaid.js image service from the given string description and returns an Image object.
+    """
+    Creates a diagram using mermaid.js image service from the given string description and returns an Image object.
     
     :param str string_description: containing the Mermaid code for the diagram
+
     :return: PIL.Image diagram_image: containing the generated diagram
 
     This function follows the steps:
         1. Encode the string_description to ASCII bytes.
         2. Convert the ASCII bytes to base64 bytes.
         3. Decode the base64 bytes to ASCII, creating a base64 string.
         4. Create the mermaid_url with the base64 string.
@@ -24,13 +26,21 @@
 
     diagram_image = Image.open(io.BytesIO(requests.get(mermaid_url).content))
 
     return diagram_image
 
 
 def saveDiagram(string_description, image_name, image_path = ""):
+    """
+    Saves the diagram image generated from the given string description.
+    
+    :param str tring_description: A textual description of the diagram to be created.
+    :param str image_name: The name of the image file (without file extension).
+    :param str,optional image_path: Path of the directory to save image in. Defaults to "" (current directory).
 
+    :return: None
+    """
     diagram_image = createDiagram(string_description)
 
     image_name = image_name + ".jpg"
     full_path = os.path.join(image_path, image_name)
     diagram_image.save(full_path)
```

### Comparing `pymermaiddiagram-0.0.2/test/test_pymermaid.py` & `pymermaiddiagram-0.0.3/test/test_pymermaid.py`

 * *Files identical despite different names*

