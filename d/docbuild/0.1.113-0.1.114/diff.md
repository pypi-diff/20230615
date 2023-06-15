# Comparing `tmp/docbuild-0.1.113.tar.gz` & `tmp/docbuild-0.1.114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.113.tar", last modified: Wed Jun 14 18:54:00 2023, max compression
+gzip compressed data, was "docbuild-0.1.114.tar", last modified: Thu Jun 15 12:30:09 2023, max compression
```

## Comparing `docbuild-0.1.113.tar` & `docbuild-0.1.114.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 18:54:00.869682 docbuild-0.1.113/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-14 18:54:00.869470 docbuild-0.1.113/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.113/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 18:54:00.864450 docbuild-0.1.113/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-14 18:53:51.000000 docbuild-0.1.113/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.113/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.113/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.113/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     7390 2023-06-14 18:50:34.000000 docbuild-0.1.113/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 18:54:00.867009 docbuild-0.1.113/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.113/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.113/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.113/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.113/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.113/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.113/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      832 2023-06-14 17:33:33.000000 docbuild-0.1.113/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 18:54:00.868950 docbuild-0.1.113/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.113/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    15947 2023-06-14 17:47:23.000000 docbuild-0.1.113/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)    24827 2023-06-14 14:41:31.000000 docbuild-0.1.113/docbuild/visual_detection/borderless_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.113/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16336 2023-06-14 18:46:35.000000 docbuild-0.1.113/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-14 18:54:00.865428 docbuild-0.1.113/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-14 18:54:00.000000 docbuild-0.1.113/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-14 18:54:00.000000 docbuild-0.1.113/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-14 18:54:00.000000 docbuild-0.1.113/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-14 18:54:00.000000 docbuild-0.1.113/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-14 18:54:00.000000 docbuild-0.1.113/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-14 18:54:00.869738 docbuild-0.1.113/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-14 18:53:57.000000 docbuild-0.1.113/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.801814 docbuild-0.1.114/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-15 12:30:09.801577 docbuild-0.1.114/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.114/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.789097 docbuild-0.1.114/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-15 12:30:03.000000 docbuild-0.1.114/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.114/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.114/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.114/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7390 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.797883 docbuild-0.1.114/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.114/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.114/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.114/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.114/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.114/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.114/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      832 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.800983 docbuild-0.1.114/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.114/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    15947 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)    24827 2023-06-15 12:29:48.000000 docbuild-0.1.114/docbuild/visual_detection/borderless_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.114/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16336 2023-06-15 12:27:28.000000 docbuild-0.1.114/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-15 12:30:09.794365 docbuild-0.1.114/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-15 12:30:09.000000 docbuild-0.1.114/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-15 12:30:09.801982 docbuild-0.1.114/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-15 12:29:57.000000 docbuild-0.1.114/setup.py
```

### Comparing `docbuild-0.1.113/PKG-INFO` & `docbuild-0.1.114/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.113
+Version: 0.1.114
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.113/docbuild/graph.py` & `docbuild-0.1.114/docbuild/graph.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/hocr_parser.py` & `docbuild-0.1.114/docbuild/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/page_creator.py` & `docbuild-0.1.114/docbuild/page_creator.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.114/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.114/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.114/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/textract_parser.py` & `docbuild-0.1.114/docbuild/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/utils.py` & `docbuild-0.1.114/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.114/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/visual_detection/borderless_table_extraction.py` & `docbuild-0.1.114/docbuild/visual_detection/borderless_table_extraction.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.114/docbuild/visual_detection/vis_line_detection.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.114/docbuild.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.113
+Version: 0.1.114
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.113/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.114/docbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.113/setup.py` & `docbuild-0.1.114/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.113",
+    version="0.1.114",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
```

