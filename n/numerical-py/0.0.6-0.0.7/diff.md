# Comparing `tmp/numerical_py-0.0.6.tar.gz` & `tmp/numerical_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-0.0.6.tar", last modified: Thu Jun 15 09:27:49 2023, max compression
+gzip compressed data, was "numerical_py-0.0.7.tar", last modified: Thu Jun 15 09:30:28 2023, max compression
```

## Comparing `numerical_py-0.0.6.tar` & `numerical_py-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:27:49.528816 numerical_py-0.0.6/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:27:49.528816 numerical_py-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 09:27:49.520758 numerical_py-0.0.6/numerical_py/
--rw-rw-rw-   0        0        0       23 2023-06-15 09:27:29.000000 numerical_py-0.0.6/numerical_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:27:49.528816 numerical_py-0.0.6/numerical_py/integrals/
--rw-rw-rw-   0        0        0       38 2023-06-15 09:24:04.000000 numerical_py-0.0.6/numerical_py/integrals/__init__.py
--rw-rw-rw-   0        0        0      210 2023-06-15 09:00:45.000000 numerical_py-0.0.6/numerical_py/integrals/trapezoid.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:27:49.528816 numerical_py-0.0.6/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:27:49.000000 numerical_py-0.0.6/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-15 09:27:49.000000 numerical_py-0.0.6/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:27:49.000000 numerical_py-0.0.6/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 09:27:49.000000 numerical_py-0.0.6/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:27:49.528816 numerical_py-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 09:27:35.000000 numerical_py-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:30:28.786962 numerical_py-0.0.7/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:30:28.786962 numerical_py-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 09:30:28.770932 numerical_py-0.0.7/numerical_py/
+-rw-rw-rw-   0        0        0       38 2023-06-15 09:30:13.000000 numerical_py-0.0.7/numerical_py/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-06-15 09:30:22.000000 numerical_py-0.0.7/numerical_py/integrals.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:30:28.786962 numerical_py-0.0.7/numerical_py.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:30:28.000000 numerical_py-0.0.7/numerical_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-15 09:30:28.000000 numerical_py-0.0.7/numerical_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:30:28.000000 numerical_py-0.0.7/numerical_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 09:30:28.000000 numerical_py-0.0.7/numerical_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:30:28.794960 numerical_py-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-15 09:30:26.000000 numerical_py-0.0.7/setup.py
```

