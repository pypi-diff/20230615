# Comparing `tmp/egcst-0.0.6.tar.gz` & `tmp/egcst-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.6.tar", last modified: Thu Jun 15 13:47:05 2023, max compression
+gzip compressed data, was "egcst-0.0.7.tar", last modified: Thu Jun 15 15:00:56 2023, max compression
```

## Comparing `egcst-0.0.6.tar` & `egcst-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:47:05.579977 egcst-0.0.6/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 13:47:05.580189 egcst-0.0.6/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.6/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:47:05.574319 egcst-0.0.6/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.6/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    12448 2023-06-15 13:45:14.000000 egcst-0.0.6/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:47:05.579511 egcst-0.0.6/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 13:47:05.000000 egcst-0.0.6/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-15 13:47:05.000000 egcst-0.0.6/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-15 13:47:05.000000 egcst-0.0.6/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-15 13:47:05.000000 egcst-0.0.6/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-15 13:47:05.000000 egcst-0.0.6/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-15 13:47:05.580943 egcst-0.0.6/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-15 13:46:10.000000 egcst-0.0.6/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:00:56.090927 egcst-0.0.7/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 15:00:56.091137 egcst-0.0.7/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.7/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:00:56.087754 egcst-0.0.7/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.7/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    12513 2023-06-15 14:57:46.000000 egcst-0.0.7/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 15:00:56.090466 egcst-0.0.7/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 15:00:55.000000 egcst-0.0.7/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-15 15:00:55.000000 egcst-0.0.7/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-15 15:00:55.000000 egcst-0.0.7/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-15 15:00:55.000000 egcst-0.0.7/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-15 15:00:55.000000 egcst-0.0.7/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-15 15:00:56.091885 egcst-0.0.7/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-15 14:59:21.000000 egcst-0.0.7/setup.py
```

### Comparing `egcst-0.0.6/README.md` & `egcst-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `egcst-0.0.6/egcst/core.py` & `egcst-0.0.7/egcst/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
         with open(self.input_file_name) as f:
             self.data = f.readlines()
 
         self.polygons = list()
         for p_n, row in enumerate(self.data):
             self.polygons.append(list())
             for item in row.strip().split('\t'):
-                items = item.split(',')
-                self.polygons[p_n].append([float(items[0]), float(items[1])])
+                if item.strip():
+                    items = item.strip().split(',')
+                    self.polygons[p_n].append([float(items[0].strip()), float(items[1].strip())])
 
         for i_p, p in enumerate(self.polygons):
             self.polygons[i_p].append(p[0])
 
         self.n_polygons = len(self.polygons)
         self.nesting_matrix = np.zeros(
             (self.n_polygons, self.n_polygons), dtype=np.int64)
```

### Comparing `egcst-0.0.6/setup.py` & `egcst-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name = 'egcst',
     packages = ['egcst'],
-    version = '0.0.6',
+    version = '0.0.7',
     license = 'MIT',
     description = 'This package performs triangulation for engineering geological cross-sections',
     url = 'https://github.com/yuryatin/egcst',
-    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.6.tar.gz',
+    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.7.tar.gz',
     keywords = ['engineering', 'geological', 'cross', 'sections', 'mapping', 'triangulation', 'delaunay'],
     classifiers = [],
     install_requires = ['numpy', 'matplotlib', 'shapely', 'ground', 'sect']
 )
```

