# Comparing `tmp/negar-gui-0.7.7.tar.gz` & `tmp/negar-gui-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negar-gui-0.7.7.tar", last modified: Tue Jun 13 07:38:06 2023, max compression
+gzip compressed data, was "negar-gui-0.7.8.tar", last modified: Thu Jun 15 08:25:54 2023, max compression
```

## Comparing `negar-gui-0.7.7.tar` & `negar-gui-0.7.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/
--rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.7/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.7/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-13 07:38:06.074695 negar-gui-0.7.7/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.7/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/
--rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/Ui_hwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.7/negar_gui/Ui_mwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.7/negar_gui/Ui_uwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)      161 2023-06-13 07:28:43.000000 negar-gui-0.7.7/negar_gui/constants.py
--rw-r--r--   0 javad     (1000) javad     (1000)    14819 2023-06-13 06:56:14.000000 negar-gui-0.7.7/negar_gui/gui.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/icons/
--rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.7/negar_gui/icons/logo.png
--rw-r--r--   0 javad     (1000) javad     (1000)    25555 2023-06-13 07:07:34.000000 negar-gui-0.7.7/negar_gui/main.py
--rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-06-13 07:26:58.000000 negar-gui-0.7.7/negar_gui/resource_rc.py
--rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.7/negar_gui/style.qss
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui/ts/
--rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.7/negar_gui/ts/fa.qm
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-13 07:38:06.074695 negar-gui-0.7.7/negar_gui.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       91 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-06-13 07:38:06.000000 negar-gui-0.7.7/negar_gui.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-06-13 07:38:06.074695 negar-gui-0.7.7/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1171 2023-06-13 07:27:29.000000 negar-gui-0.7.7/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:25:54.551813 negar-gui-0.7.8/
+-rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.7.8/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.7.8/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-15 08:25:54.551813 negar-gui-0.7.8/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     2399 2023-04-01 17:16:18.000000 negar-gui-0.7.8/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:25:54.548480 negar-gui-0.7.8/negar_gui/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.7.8/negar_gui/Ui_hwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-04-07 20:19:39.000000 negar-gui-0.7.8/negar_gui/Ui_mwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.7.8/negar_gui/Ui_uwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.7.8/negar_gui/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)      161 2023-06-15 08:21:01.000000 negar-gui-0.7.8/negar_gui/constants.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    14819 2023-06-13 06:56:14.000000 negar-gui-0.7.8/negar_gui/gui.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:25:54.548480 negar-gui-0.7.8/negar_gui/icons/
+-rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.7.8/negar_gui/icons/logo.png
+-rw-r--r--   0 javad     (1000) javad     (1000)    25555 2023-06-13 07:07:34.000000 negar-gui-0.7.8/negar_gui/main.py
+-rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-06-15 08:18:56.000000 negar-gui-0.7.8/negar_gui/resource_rc.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.7.8/negar_gui/style.qss
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:25:54.548480 negar-gui-0.7.8/negar_gui/ts/
+-rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.7.8/negar_gui/ts/fa.qm
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:25:54.548480 negar-gui-0.7.8/negar_gui.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2781 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       91 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-06-15 08:25:54.000000 negar-gui-0.7.8/negar_gui.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-06-15 08:25:54.551813 negar-gui-0.7.8/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1171 2023-06-15 08:19:45.000000 negar-gui-0.7.8/setup.py
```

### Comparing `negar-gui-0.7.7/LICENSE` & `negar-gui-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/PKG-INFO` & `negar-gui-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.7
+Version: 0.7.8
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
```

### Comparing `negar-gui-0.7.7/README.md` & `negar-gui-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/Ui_hwin.py` & `negar-gui-0.7.8/negar_gui/Ui_hwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/Ui_mwin.py` & `negar-gui-0.7.8/negar_gui/Ui_mwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/Ui_uwin.py` & `negar-gui-0.7.8/negar_gui/Ui_uwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/gui.py` & `negar-gui-0.7.8/negar_gui/gui.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/icons/logo.png` & `negar-gui-0.7.8/negar_gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/main.py` & `negar-gui-0.7.8/negar_gui/main.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/resource_rc.py` & `negar-gui-0.7.8/negar_gui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/style.qss` & `negar-gui-0.7.8/negar_gui/style.qss`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui/ts/fa.qm` & `negar-gui-0.7.8/negar_gui/ts/fa.qm`

 * *Files identical despite different names*

### Comparing `negar-gui-0.7.7/negar_gui.egg-info/PKG-INFO` & `negar-gui-0.7.8/negar_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negar-gui
-Version: 0.7.7
+Version: 0.7.8
 Summary: Graphical User Interface for Negar -- Persian Text Editor
 Home-page: http://github.com/javadr/negar-gui
 Author: Javad Razavian
 Author-email: javadr@gmail.com
 License: GPLv3
 Keywords: Spellcheck Persian Text-Editor
 Platform: UNKNOWN
```

### Comparing `negar-gui-0.7.7/setup.py` & `negar-gui-0.7.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     name="negar-gui",
     version=version,
     author="Javad Razavian",
     author_email="javadr@gmail.com",
     include_package_data=True,
     packages=['negar_gui',],
     install_requires=[
-        'python-negar>=1.2.2',
+        'python-negar>=1.2.4',
         'PyQt5',
         'pyperclip',
         'pyuca',
         'regex',
         'requests',
         'qrcode',
         'docopt',
```

