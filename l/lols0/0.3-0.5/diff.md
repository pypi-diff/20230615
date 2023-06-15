# Comparing `tmp/lols0-0.3.tar.gz` & `tmp/lols0-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lols0-0.3.tar", last modified: Thu Jun 15 05:22:57 2023, max compression
+gzip compressed data, was "lols0-0.5.tar", last modified: Thu Jun 15 05:54:36 2023, max compression
```

## Comparing `lols0-0.3.tar` & `lols0-0.5.tar`

### file list

```diff
@@ -1,27 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 05:22:57.393158 lols0-0.3/
--rw-rw-rw-   0        0        0      224 2023-06-15 05:22:57.394155 lols0-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 05:22:57.282454 lols0-0.3/cosa/
--rw-rw-rw-   0        0        0       27 2023-06-15 05:15:17.000000 lols0-0.3/cosa/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-06-15 05:10:28.000000 lols0-0.3/cosa/actu.py
--rw-rw-rw-   0        0        0     1354 2023-06-15 05:10:28.000000 lols0-0.3/cosa/agregar.py
--rw-rw-rw-   0        0        0      560 2023-06-15 05:10:28.000000 lols0-0.3/cosa/borrar.py
--rw-rw-rw-   0        0        0     2095 2023-06-15 05:10:28.000000 lols0-0.3/cosa/buscar.py
--rw-rw-rw-   0        0        0       26 2023-06-15 05:10:28.000000 lols0-0.3/cosa/mian.py
--rw-rw-rw-   0        0        0     2839 2023-06-15 05:10:28.000000 lols0-0.3/cosa/principal.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:22:57.343292 lols0-0.3/cosa/prog/
--rw-rw-rw-   0        0        0       86 2023-06-15 05:16:54.000000 lols0-0.3/cosa/prog/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-06-15 05:10:28.000000 lols0-0.3/cosa/prog/actu.py
--rw-rw-rw-   0        0        0     1354 2023-06-15 05:10:28.000000 lols0-0.3/cosa/prog/agregar.py
--rw-rw-rw-   0        0        0      560 2023-06-15 05:10:28.000000 lols0-0.3/cosa/prog/borrar.py
--rw-rw-rw-   0        0        0     2095 2023-06-15 05:10:28.000000 lols0-0.3/cosa/prog/buscar.py
--rw-rw-rw-   0        0        0       26 2023-06-15 05:10:28.000000 lols0-0.3/cosa/prog/mian.py
--rw-rw-rw-   0        0        0     2839 2023-06-15 05:10:29.000000 lols0-0.3/cosa/prog/principal.py
--rw-rw-rw-   0        0        0      448 2023-06-15 05:10:29.000000 lols0-0.3/cosa/prog/ver_datos.py
--rw-rw-rw-   0        0        0      448 2023-06-15 05:10:28.000000 lols0-0.3/cosa/ver_datos.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:22:57.392162 lols0-0.3/lols0.egg-info/
--rw-rw-rw-   0        0        0      224 2023-06-15 05:22:57.000000 lols0-0.3/lols0.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-15 05:22:57.000000 lols0-0.3/lols0.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 05:22:57.000000 lols0-0.3/lols0.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-15 05:22:57.000000 lols0-0.3/lols0.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 05:22:57.402421 lols0-0.3/setup.cfg
--rw-rw-rw-   0        0        0      249 2023-06-15 05:22:11.000000 lols0-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:54:36.346540 lols0-0.5/
+-rw-rw-rw-   0        0        0      224 2023-06-15 05:54:36.347536 lols0-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 05:54:36.324597 lols0-0.5/cosa/
+-rw-rw-rw-   0        0        0       42 2023-06-15 05:37:16.000000 lols0-0.5/cosa/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-06-15 05:10:28.000000 lols0-0.5/cosa/actu.py
+-rw-rw-rw-   0        0        0     1354 2023-06-15 05:10:28.000000 lols0-0.5/cosa/agregar.py
+-rw-rw-rw-   0        0        0      560 2023-06-15 05:10:28.000000 lols0-0.5/cosa/borrar.py
+-rw-rw-rw-   0        0        0     2095 2023-06-15 05:10:28.000000 lols0-0.5/cosa/buscar.py
+-rw-rw-rw-   0        0        0     2839 2023-06-15 05:10:28.000000 lols0-0.5/cosa/principal.py
+-rw-rw-rw-   0        0        0      448 2023-06-15 05:10:28.000000 lols0-0.5/cosa/ver_datos.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:54:36.345541 lols0-0.5/lols0.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-06-15 05:54:36.000000 lols0-0.5/lols0.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-15 05:54:36.000000 lols0-0.5/lols0.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 05:54:36.000000 lols0-0.5/lols0.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-15 05:54:36.000000 lols0-0.5/lols0.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 05:54:36.351526 lols0-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      250 2023-06-15 05:54:17.000000 lols0-0.5/setup.py
```

### Comparing `lols0-0.3/cosa/actu.py` & `lols0-0.5/cosa/actu.py`

 * *Files identical despite different names*

### Comparing `lols0-0.3/cosa/agregar.py` & `lols0-0.5/cosa/agregar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.3/cosa/borrar.py` & `lols0-0.5/cosa/borrar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.3/cosa/buscar.py` & `lols0-0.5/cosa/buscar.py`

 * *Files identical despite different names*

### Comparing `lols0-0.3/cosa/principal.py` & `lols0-0.5/cosa/principal.py`

 * *Files identical despite different names*

