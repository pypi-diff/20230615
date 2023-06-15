# Comparing `tmp/numerical_py-0.0.8.tar.gz` & `tmp/numerical_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-0.0.8.tar", last modified: Thu Jun 15 09:36:43 2023, max compression
+gzip compressed data, was "numerical_py-0.0.9.tar", last modified: Thu Jun 15 09:41:59 2023, max compression
```

## Comparing `numerical_py-0.0.8.tar` & `numerical_py-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:36:43.450496 numerical_py-0.0.8/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:36:43.450496 numerical_py-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 09:36:43.426475 numerical_py-0.0.8/numerical_py/
--rw-rw-rw-   0        0        0       38 2023-06-15 09:30:13.000000 numerical_py-0.0.8/numerical_py/__init__.py
--rw-rw-rw-   0        0        0      506 2023-06-15 09:36:33.000000 numerical_py-0.0.8/numerical_py/integrals.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:36:43.442496 numerical_py-0.0.8/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:36:43.000000 numerical_py-0.0.8/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-06-15 09:36:43.000000 numerical_py-0.0.8/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:36:43.000000 numerical_py-0.0.8/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 09:36:43.000000 numerical_py-0.0.8/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:36:43.450496 numerical_py-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 09:36:39.000000 numerical_py-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:41:59.390175 numerical_py-0.0.9/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:41:59.390175 numerical_py-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 09:41:59.390175 numerical_py-0.0.9/numerical_py.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:41:59.000000 numerical_py-0.0.9/numerical_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:41:59.390175 numerical_py-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-15 09:41:56.000000 numerical_py-0.0.9/setup.py
```

