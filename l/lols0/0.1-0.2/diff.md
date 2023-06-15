# Comparing `tmp/lols0-0.1.tar.gz` & `tmp/lols0-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lols0-0.1.tar", last modified: Thu Jun 15 04:30:18 2023, max compression
+gzip compressed data, was "lols0-0.2.tar", last modified: Thu Jun 15 04:46:33 2023, max compression
```

## Comparing `lols0-0.1.tar` & `lols0-0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 04:30:18.575271 lols0-0.1/
--rw-rw-rw-   0        0        0      165 2023-06-15 04:30:18.576271 lols0-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 04:30:18.495308 lols0-0.1/cosa/
--rw-rw-rw-   0        0        0       84 2023-06-15 04:19:09.000000 lols0-0.1/cosa/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-06-15 03:08:15.000000 lols0-0.1/cosa/actu.py
--rw-rw-rw-   0        0        0     1354 2023-06-14 23:50:18.000000 lols0-0.1/cosa/agregar.py
--rw-rw-rw-   0        0        0      560 2023-06-14 23:49:12.000000 lols0-0.1/cosa/borrar.py
--rw-rw-rw-   0        0        0     2095 2023-06-14 23:47:21.000000 lols0-0.1/cosa/buscar.py
--rw-rw-rw-   0        0        0       26 2023-06-15 00:28:48.000000 lols0-0.1/cosa/mian.py
--rw-rw-rw-   0        0        0     2839 2023-06-15 00:40:21.000000 lols0-0.1/cosa/principal.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:30:18.518292 lols0-0.1/cosa/prog/
--rw-rw-rw-   0        0        0       84 2023-06-15 04:19:09.000000 lols0-0.1/cosa/prog/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-06-15 03:08:15.000000 lols0-0.1/cosa/prog/actu.py
--rw-rw-rw-   0        0        0     1354 2023-06-14 23:50:18.000000 lols0-0.1/cosa/prog/agregar.py
--rw-rw-rw-   0        0        0      560 2023-06-14 23:49:12.000000 lols0-0.1/cosa/prog/borrar.py
--rw-rw-rw-   0        0        0     2095 2023-06-14 23:47:21.000000 lols0-0.1/cosa/prog/buscar.py
--rw-rw-rw-   0        0        0       26 2023-06-15 00:28:48.000000 lols0-0.1/cosa/prog/mian.py
--rw-rw-rw-   0        0        0     2839 2023-06-15 00:40:21.000000 lols0-0.1/cosa/prog/principal.py
--rw-rw-rw-   0        0        0      448 2023-06-14 23:48:15.000000 lols0-0.1/cosa/prog/ver_datos.py
--rw-rw-rw-   0        0        0      448 2023-06-14 23:48:15.000000 lols0-0.1/cosa/ver_datos.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:30:18.573271 lols0-0.1/lols0.egg-info/
--rw-rw-rw-   0        0        0      165 2023-06-15 04:30:18.000000 lols0-0.1/lols0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-15 04:30:18.000000 lols0-0.1/lols0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 04:30:18.000000 lols0-0.1/lols0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-15 04:30:18.000000 lols0-0.1/lols0.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 04:30:18.579269 lols0-0.1/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-15 04:29:05.000000 lols0-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:33.884055 lols0-0.2/
+-rw-rw-rw-   0        0        0      165 2023-06-15 04:46:33.884055 lols0-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:33.832086 lols0-0.2/cosa/
+-rw-rw-rw-   0        0        0      161 2023-06-15 04:44:26.000000 lols0-0.2/cosa/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-06-15 03:08:15.000000 lols0-0.2/cosa/actu.py
+-rw-rw-rw-   0        0        0     1354 2023-06-14 23:50:18.000000 lols0-0.2/cosa/agregar.py
+-rw-rw-rw-   0        0        0      560 2023-06-14 23:49:12.000000 lols0-0.2/cosa/borrar.py
+-rw-rw-rw-   0        0        0     2095 2023-06-14 23:47:21.000000 lols0-0.2/cosa/buscar.py
+-rw-rw-rw-   0        0        0       26 2023-06-15 00:28:48.000000 lols0-0.2/cosa/mian.py
+-rw-rw-rw-   0        0        0     2839 2023-06-15 00:40:21.000000 lols0-0.2/cosa/principal.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:33.853073 lols0-0.2/cosa/prog/
+-rw-rw-rw-   0        0        0      161 2023-06-15 04:44:58.000000 lols0-0.2/cosa/prog/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-06-15 03:08:15.000000 lols0-0.2/cosa/prog/actu.py
+-rw-rw-rw-   0        0        0     1354 2023-06-14 23:50:18.000000 lols0-0.2/cosa/prog/agregar.py
+-rw-rw-rw-   0        0        0      560 2023-06-14 23:49:12.000000 lols0-0.2/cosa/prog/borrar.py
+-rw-rw-rw-   0        0        0     2095 2023-06-14 23:47:21.000000 lols0-0.2/cosa/prog/buscar.py
+-rw-rw-rw-   0        0        0       26 2023-06-15 00:28:48.000000 lols0-0.2/cosa/prog/mian.py
+-rw-rw-rw-   0        0        0     2839 2023-06-15 00:40:21.000000 lols0-0.2/cosa/prog/principal.py
+-rw-rw-rw-   0        0        0      448 2023-06-14 23:48:15.000000 lols0-0.2/cosa/prog/ver_datos.py
+-rw-rw-rw-   0        0        0      448 2023-06-14 23:48:15.000000 lols0-0.2/cosa/ver_datos.py
+drwxrwxrwx   0        0        0        0 2023-06-15 04:46:33.881059 lols0-0.2/lols0.egg-info/
+-rw-rw-rw-   0        0        0      165 2023-06-15 04:46:33.000000 lols0-0.2/lols0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-15 04:46:33.000000 lols0-0.2/lols0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 04:46:33.000000 lols0-0.2/lols0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-15 04:46:33.000000 lols0-0.2/lols0.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 04:46:33.886054 lols0-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-15 04:45:42.000000 lols0-0.2/setup.py
```

### Comparing `lols0-0.1/cosa/actu.py` & `lols0-0.2/cosa/actu.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/agregar.py` & `lols0-0.2/cosa/agregar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/borrar.py` & `lols0-0.2/cosa/borrar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/buscar.py` & `lols0-0.2/cosa/buscar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/principal.py` & `lols0-0.2/cosa/principal.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/prog/actu.py` & `lols0-0.2/cosa/prog/actu.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/prog/agregar.py` & `lols0-0.2/cosa/prog/agregar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/prog/borrar.py` & `lols0-0.2/cosa/prog/borrar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/prog/buscar.py` & `lols0-0.2/cosa/prog/buscar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.1/cosa/prog/principal.py` & `lols0-0.2/cosa/prog/principal.py`

 * *Files identical despite different names*

