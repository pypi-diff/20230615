# Comparing `tmp/plover-stenograph-2.1.tar.gz` & `tmp/plover-stenograph-2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-stenograph-2.1.tar", last modified: Wed Jun 14 22:27:05 2023, max compression
+gzip compressed data, was "plover-stenograph-2.1.dev1.tar", last modified: Wed Jun 14 22:23:12 2023, max compression
```

## Comparing `plover-stenograph-2.1.tar` & `plover-stenograph-2.1.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:27:05.839922 plover-stenograph-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 22:27:05.839922 plover-stenograph-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 22:27:04.000000 plover-stenograph-2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:27:05.839922 plover-stenograph-2.1/plover_stenograph/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:27:04.000000 plover-stenograph-2.1/plover_stenograph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-14 22:27:04.000000 plover-stenograph-2.1/plover_stenograph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-14 22:27:04.000000 plover-stenograph-2.1/plover_stenograph/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 22:27:04.000000 plover-stenograph-2.1/plover_stenograph/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:27:05.839922 plover-stenograph-2.1/plover_stenograph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:27:05.000000 plover-stenograph-2.1/plover_stenograph.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-14 22:27:05.839922 plover-stenograph-2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-06-14 22:27:04.000000 plover-stenograph-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:27:05.839922 plover-stenograph-2.1/stenograph/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/stroke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/transport_libusb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/transport_wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-14 22:27:04.000000 plover-stenograph-2.1/stenograph/transport_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/plover_stenograph/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/plover_stenograph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/plover_stenograph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/plover_stenograph/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/plover_stenograph/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:23:12.000000 plover-stenograph-2.1.dev1/plover_stenograph.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:23:12.549781 plover-stenograph-2.1.dev1/stenograph/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/stroke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/transport_libusb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/transport_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-14 22:23:10.000000 plover-stenograph-2.1.dev1/stenograph/transport_windows.py
```

### Comparing `plover-stenograph-2.1/PKG-INFO` & `plover-stenograph-2.1.dev1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: plover-stenograph
-Version: 2.1
+Version: 2.1.dev1
 Summary: Plover plugin for Stenograph machines
 Home-page: https://github.com/sammdot/plover-stenograph
-License: UNKNOWN
 Keywords: plover plover_plugin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Plover Stenograph
 
 A Plover plugin for using newer Stenograph machines (Stentura Protégé and
 Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
 over USB or Wi-Fi.
 
 This is a work-in-progress rewrite of the
 [plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
 [plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
 plugins to reuse code and add more protocol functionality.
-
-
```

### Comparing `plover-stenograph-2.1/plover_stenograph/base.py` & `plover-stenograph-2.1.dev1/plover_stenograph/base.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/plover_stenograph.egg-info/PKG-INFO` & `plover-stenograph-2.1.dev1/plover_stenograph.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: plover-stenograph
-Version: 2.1
+Version: 2.1.dev1
 Summary: Plover plugin for Stenograph machines
 Home-page: https://github.com/sammdot/plover-stenograph
-License: UNKNOWN
 Keywords: plover plover_plugin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Plover Stenograph
 
 A Plover plugin for using newer Stenograph machines (Stentura Protégé and
 Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
 over USB or Wi-Fi.
 
 This is a work-in-progress rewrite of the
 [plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
 [plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
 plugins to reuse code and add more protocol functionality.
-
-
```

### Comparing `plover-stenograph-2.1/plover_stenograph.egg-info/SOURCES.txt` & `plover-stenograph-2.1.dev1/plover_stenograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/setup.cfg` & `plover-stenograph-2.1.dev1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-stenograph
-version = 2.1
+version = 2.1-dev1
 description = Plover plugin for Stenograph machines
 long_description = file:README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/sammdot/plover-stenograph
 keywords = plover plover_plugin
 classifiers = 
 	Programming Language :: Python :: 3.9
```

### Comparing `plover-stenograph-2.1/stenograph/exception.py` & `plover-stenograph-2.1.dev1/stenograph/exception.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/packet.py` & `plover-stenograph-2.1.dev1/stenograph/packet.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/stroke.py` & `plover-stenograph-2.1.dev1/stenograph/stroke.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/transport.py` & `plover-stenograph-2.1.dev1/stenograph/transport.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/transport_libusb.py` & `plover-stenograph-2.1.dev1/stenograph/transport_libusb.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/transport_wifi.py` & `plover-stenograph-2.1.dev1/stenograph/transport_wifi.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.1/stenograph/transport_windows.py` & `plover-stenograph-2.1.dev1/stenograph/transport_windows.py`

 * *Files identical despite different names*

