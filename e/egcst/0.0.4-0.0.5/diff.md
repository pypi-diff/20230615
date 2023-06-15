# Comparing `tmp/egcst-0.0.4.tar.gz` & `tmp/egcst-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcst-0.0.4.tar", last modified: Wed Jun 14 19:09:51 2023, max compression
+gzip compressed data, was "egcst-0.0.5.tar", last modified: Thu Jun 15 13:43:30 2023, max compression
```

## Comparing `egcst-0.0.4.tar` & `egcst-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.839719 egcst-0.0.4/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 19:09:51.839994 egcst-0.0.4/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.4/README.md
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.834608 egcst-0.0.4/egcst/
--rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.4/egcst/__init__.py
--rw-r--r--   0 sasha      (502) staff       (20)    12442 2023-06-14 18:59:37.000000 egcst-0.0.4/egcst/core.py
-drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-14 19:09:51.839026 egcst-0.0.4/egcst.egg-info/
--rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/PKG-INFO
--rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/SOURCES.txt
--rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/dependency_links.txt
--rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/requires.txt
--rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-14 19:09:51.000000 egcst-0.0.4/egcst.egg-info/top_level.txt
--rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-14 19:09:51.841619 egcst-0.0.4/setup.cfg
--rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-14 19:00:13.000000 egcst-0.0.4/setup.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:43:30.481930 egcst-0.0.5/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 13:43:30.482123 egcst-0.0.5/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)     2230 2023-06-14 19:06:51.000000 egcst-0.0.5/README.md
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:43:30.476991 egcst-0.0.5/egcst/
+-rw-r--r--   0 sasha      (502) staff       (20)       25 2023-06-13 23:54:54.000000 egcst-0.0.5/egcst/__init__.py
+-rw-r--r--   0 sasha      (502) staff       (20)    12448 2023-06-15 13:38:03.000000 egcst-0.0.5/egcst/core.py
+drwxr-xr-x   0 sasha      (502) staff       (20)        0 2023-06-15 13:43:30.481452 egcst-0.0.5/egcst.egg-info/
+-rw-r--r--   0 sasha      (502) staff       (20)      353 2023-06-15 13:43:30.000000 egcst-0.0.5/egcst.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (502) staff       (20)      204 2023-06-15 13:43:30.000000 egcst-0.0.5/egcst.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        1 2023-06-15 13:43:30.000000 egcst-0.0.5/egcst.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (502) staff       (20)       37 2023-06-15 13:43:30.000000 egcst-0.0.5/egcst.egg-info/requires.txt
+-rw-r--r--   0 sasha      (502) staff       (20)        6 2023-06-15 13:43:30.000000 egcst-0.0.5/egcst.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (502) staff       (20)      103 2023-06-15 13:43:30.482939 egcst-0.0.5/setup.cfg
+-rw-r--r--   0 sasha      (502) staff       (20)      571 2023-06-15 13:41:45.000000 egcst-0.0.5/setup.py
```

### Comparing `egcst-0.0.4/README.md` & `egcst-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `egcst-0.0.4/egcst/core.py` & `egcst-0.0.5/egcst/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,29 +65,29 @@
                     if (np.abs(delta_x) <= min_step) and (np.abs(delta_y) <= min_step):
                         continue
                     if delta_x:
                         slope = delta_y / delta_x
                         if np.abs(delta_x) > np.abs(delta_y):
                             n_steps = int(np.abs(delta_x) / min_step) + 1
                             i_step = delta_x / n_steps
-                            for i in range(n_steps):
+                            for i in range(n_steps-1):
                                 x_2 = x_0 + (i + 1) * i_step
                                 y_2 = y_0 + (x_2 - x_0) * slope
                                 entended_p.append([x_2, y_2])
                         else:
                             n_steps = int(np.abs(delta_y) / min_step) + 1
                             i_step = delta_y / n_steps
-                            for i in range(n_steps):
+                            for i in range(n_steps)-1:
                                 y_2 = y_0 + (i + 1) * i_step
                                 x_2 = x_0 + (y_2 - y_0) / slope
                                 entended_p.append([x_2, y_2])
                     else:
                         n_steps = int(np.abs(delta_y) / min_step) + 1
                         i_step = delta_y / n_steps
-                        for i in range(n_steps):
+                        for i in range(n_steps-1):
                             y_2 = y_0 + (i + 1) * i_step
                             if y_2 == y_1:
                                 continue
                             entended_p.append([x_0, y_2])
             entended_p.append(p[-1])
             self.polygons[i_p] = entended_p.copy()
```

### Comparing `egcst-0.0.4/setup.py` & `egcst-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name = 'egcst',
     packages = ['egcst'],
-    version = '0.0.4',
+    version = '0.0.5',
     license = 'MIT',
     description = 'This package performs triangulation for engineering geological cross-sections',
     url = 'https://github.com/yuryatin/egcst',
-    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.4.tar.gz',
+    download_url = 'https://github.com/yuryatin/egcst/archive/refs/tags/v0.0.5.tar.gz',
     keywords = ['engineering', 'geological', 'cross', 'sections', 'mapping', 'triangulation', 'delaunay'],
     classifiers = [],
     install_requires = ['numpy', 'matplotlib', 'shapely', 'ground', 'sect']
 )
```

