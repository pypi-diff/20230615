# Comparing `tmp/svgecko-0.3.2.tar.gz` & `tmp/svgecko-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgecko-0.3.2.tar", last modified: Thu Jun  1 13:58:44 2023, max compression
+gzip compressed data, was "svgecko-0.3.4.tar", last modified: Thu Jun 15 13:25:20 2023, max compression
```

## Comparing `svgecko-0.3.2.tar` & `svgecko-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 13:58:44.041228 svgecko-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 13:58:32.000000 svgecko-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:58:44.041228 svgecko-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 13:58:32.000000 svgecko-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.037228 svgecko-0.3.2/svgecko/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/svgecko/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/resources/cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/resources/python-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/svg_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/svgecko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:32.000000 svgecko-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 13:58:32.000000 svgecko-0.3.2/tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:20.045393 svgecko-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 13:25:20.041393 svgecko-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-15 13:25:07.000000 svgecko-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:25:20.045393 svgecko-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 13:25:07.000000 svgecko-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:20.041393 svgecko-0.3.4/svgecko/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:20.041393 svgecko-0.3.4/svgecko/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/resources/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/resources/python-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/svg_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 13:25:07.000000 svgecko-0.3.4/svgecko/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:20.041393 svgecko-0.3.4/svgecko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 13:25:20.000000 svgecko-0.3.4/svgecko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 13:25:20.000000 svgecko-0.3.4/svgecko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:25:20.000000 svgecko-0.3.4/svgecko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 13:25:20.000000 svgecko-0.3.4/svgecko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 13:25:20.000000 svgecko-0.3.4/svgecko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:20.041393 svgecko-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:25:07.000000 svgecko-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 13:25:07.000000 svgecko-0.3.4/tests/test_svg.py
```

### Comparing `svgecko-0.3.2/README.md` & `svgecko-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.2/setup.py` & `svgecko-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='svgecko',
-    version='0.3.2',
+    version='0.3.4',
     author='Josef Ondrej',
     author_email='josef.ondrej@outlook.com',
     description='Lightweight library for arbitrary geometric SVG transformations',
     long_description='Lightweight library for arbitrary geometric SVG transformations',
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'svgecko': ['resources/*.svg']},
```

### Comparing `svgecko-0.3.2/svgecko/resources/python-logo.svg` & `svgecko-0.3.4/svgecko/resources/python-logo.svg`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.2/svgecko/svg.py` & `svgecko-0.3.4/svgecko/svg.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,20 @@
 
     def __copy__(self):
         return SVG(self._xml)
 
     def __deepcopy__(self, memodict={}):
         return SVG(deepcopy(self._xml))
 
+    def __getstate__(self):
+        return {'xml': self.to_string()}
+
+    def __setstate__(self, state):
+        self._xml = self.from_string(state['xml']).xml
+
     @property
     def shape(self):
         raw_width, raw_height = self.xml.attrib['width'], self.xml.attrib['height']
         width = float(''.join([c for c in raw_width if c.isdigit() or c == '.']))
         height = float(''.join([c for c in raw_height if c.isdigit() or c == '.']))
         return width, height
```

### Comparing `svgecko-0.3.2/svgecko/svg_path.py` & `svgecko-0.3.4/svgecko/svg_path.py`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.2/tests/test_svg.py` & `svgecko-0.3.4/tests/test_svg.py`

 * *Files identical despite different names*

