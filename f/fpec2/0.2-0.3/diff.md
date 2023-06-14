# Comparing `tmp/fpec2-0.2.tar.gz` & `tmp/fpec2-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpec2-0.2.tar", last modified: Wed Jun 14 22:52:43 2023, max compression
+gzip compressed data, was "fpec2-0.3.tar", last modified: Wed Jun 14 23:11:12 2023, max compression
```

## Comparing `fpec2-0.2.tar` & `fpec2-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:43.571784 fpec2-0.2/
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:43.535881 fpec2-0.2/J/
--rw-rw-rw-   0        0        0     2640 2023-06-14 19:51:11.000000 fpec2-0.2/J/Numpy.py
--rw-rw-rw-   0        0        0     3091 2023-06-14 19:51:18.000000 fpec2-0.2/J/Simpy.py
--rw-rw-rw-   0        0        0       24 2023-06-14 22:48:28.000000 fpec2-0.2/J/__init__.py
--rw-rw-rw-   0        0        0     2398 2023-06-14 19:51:32.000000 fpec2-0.2/J/calculo.py
--rw-rw-rw-   0        0        0     3150 2023-06-14 22:51:44.000000 fpec2-0.2/J/ejemplox.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:43.546849 fpec2-0.2/J/m/
--rw-rw-rw-   0        0        0     2640 2023-06-14 19:51:11.000000 fpec2-0.2/J/m/Numpy.py
--rw-rw-rw-   0        0        0     3091 2023-06-14 19:51:18.000000 fpec2-0.2/J/m/Simpy.py
--rw-rw-rw-   0        0        0       49 2023-06-14 22:40:23.000000 fpec2-0.2/J/m/__init__.py
--rw-rw-rw-   0        0        0     2398 2023-06-14 19:51:32.000000 fpec2-0.2/J/m/calculo.py
--rw-rw-rw-   0        0        0     3150 2023-06-14 22:51:36.000000 fpec2-0.2/J/m/ejemplox.py
--rw-rw-rw-   0        0        0      280 2023-06-14 22:52:43.571784 fpec2-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:43.567793 fpec2-0.2/fpec2.egg-info/
--rw-rw-rw-   0        0        0      280 2023-06-14 22:52:43.000000 fpec2-0.2/fpec2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-14 22:52:43.000000 fpec2-0.2/fpec2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:52:43.000000 fpec2-0.2/fpec2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 22:52:43.000000 fpec2-0.2/fpec2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 22:52:43.575772 fpec2-0.2/setup.cfg
--rw-rw-rw-   0        0        0      318 2023-06-14 22:51:40.000000 fpec2-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:12.970788 fpec2-0.3/
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:12.944857 fpec2-0.3/J/
+-rw-rw-rw-   0        0        0     2640 2023-06-14 19:51:11.000000 fpec2-0.3/J/Numpy.py
+-rw-rw-rw-   0        0        0     3091 2023-06-14 19:51:18.000000 fpec2-0.3/J/Simpy.py
+-rw-rw-rw-   0        0        0       24 2023-06-14 22:48:28.000000 fpec2-0.3/J/__init__.py
+-rw-rw-rw-   0        0        0     2398 2023-06-14 19:51:32.000000 fpec2-0.3/J/calculo.py
+-rw-rw-rw-   0        0        0     3150 2023-06-14 22:51:44.000000 fpec2-0.3/J/ejemplox.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:12.953835 fpec2-0.3/J/m/
+-rw-rw-rw-   0        0        0     2640 2023-06-14 19:51:11.000000 fpec2-0.3/J/m/Numpy.py
+-rw-rw-rw-   0        0        0     3091 2023-06-14 19:51:18.000000 fpec2-0.3/J/m/Simpy.py
+-rw-rw-rw-   0        0        0       49 2023-06-14 22:40:23.000000 fpec2-0.3/J/m/__init__.py
+-rw-rw-rw-   0        0        0     2398 2023-06-14 19:51:32.000000 fpec2-0.3/J/m/calculo.py
+-rw-rw-rw-   0        0        0     3150 2023-06-14 22:51:36.000000 fpec2-0.3/J/m/ejemplox.py
+-rw-rw-rw-   0        0        0      284 2023-06-14 23:11:12.970788 fpec2-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:12.969791 fpec2-0.3/fpec2.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-06-14 23:11:12.000000 fpec2-0.3/fpec2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-14 23:11:12.000000 fpec2-0.3/fpec2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:11:12.000000 fpec2-0.3/fpec2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 23:11:12.000000 fpec2-0.3/fpec2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-14 23:11:12.974777 fpec2-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      321 2023-06-14 23:05:58.000000 fpec2-0.3/setup.py
```

### Comparing `fpec2-0.2/J/Numpy.py` & `fpec2-0.3/J/Numpy.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/Simpy.py` & `fpec2-0.3/J/Simpy.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/calculo.py` & `fpec2-0.3/J/calculo.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/ejemplox.py` & `fpec2-0.3/J/ejemplox.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/m/Numpy.py` & `fpec2-0.3/J/m/Numpy.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/m/Simpy.py` & `fpec2-0.3/J/m/Simpy.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/m/calculo.py` & `fpec2-0.3/J/m/calculo.py`

 * *Files identical despite different names*

### Comparing `fpec2-0.2/J/m/ejemplox.py` & `fpec2-0.3/J/m/ejemplox.py`

 * *Files identical despite different names*

