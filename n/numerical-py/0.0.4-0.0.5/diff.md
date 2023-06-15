# Comparing `tmp/numerical_py-0.0.4.tar.gz` & `tmp/numerical_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-0.0.4.tar", last modified: Thu Jun 15 09:19:16 2023, max compression
+gzip compressed data, was "numerical_py-0.0.5.tar", last modified: Thu Jun 15 09:24:17 2023, max compression
```

## Comparing `numerical_py-0.0.4.tar` & `numerical_py-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:16.216791 numerical_py-0.0.4/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:19:16.216791 numerical_py-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:16.200779 numerical_py-0.0.4/numerical_py/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:07:48.000000 numerical_py-0.0.4/numerical_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:16.216791 numerical_py-0.0.4/numerical_py/integrals/
--rw-rw-rw-   0        0        0       33 2023-06-15 09:19:08.000000 numerical_py-0.0.4/numerical_py/integrals/__init__.py
--rw-rw-rw-   0        0        0      210 2023-06-15 09:00:45.000000 numerical_py-0.0.4/numerical_py/integrals/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:16.208793 numerical_py-0.0.4/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:19:15.000000 numerical_py-0.0.4/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-15 09:19:16.000000 numerical_py-0.0.4/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:19:15.000000 numerical_py-0.0.4/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 09:19:16.000000 numerical_py-0.0.4/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:19:16.216791 numerical_py-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 09:19:13.000000 numerical_py-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:24:17.416372 numerical_py-0.0.5/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:24:17.416372 numerical_py-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 09:24:17.400366 numerical_py-0.0.5/numerical_py/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:24:02.000000 numerical_py-0.0.5/numerical_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:24:17.408366 numerical_py-0.0.5/numerical_py/integrals/
+-rw-rw-rw-   0        0        0       38 2023-06-15 09:24:04.000000 numerical_py-0.0.5/numerical_py/integrals/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-06-15 09:00:45.000000 numerical_py-0.0.5/numerical_py/integrals/trapezoid.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:24:17.408366 numerical_py-0.0.5/numerical_py.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:24:17.000000 numerical_py-0.0.5/numerical_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-15 09:24:17.000000 numerical_py-0.0.5/numerical_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:24:17.000000 numerical_py-0.0.5/numerical_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 09:24:17.000000 numerical_py-0.0.5/numerical_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:24:17.416372 numerical_py-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-15 09:24:06.000000 numerical_py-0.0.5/setup.py
```

