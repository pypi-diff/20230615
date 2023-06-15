# Comparing `tmp/numerical_py-0.0.2.tar.gz` & `tmp/numerical_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-0.0.2.tar", last modified: Thu Jun 15 09:01:47 2023, max compression
+gzip compressed data, was "numerical_py-0.0.3.tar", last modified: Thu Jun 15 09:09:40 2023, max compression
```

## Comparing `numerical_py-0.0.2.tar` & `numerical_py-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:01:47.136067 numerical_py-0.0.2/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:01:47.136067 numerical_py-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 09:01:47.112029 numerical_py-0.0.2/numerical_py/
--rw-rw-rw-   0        0        0        0 2023-06-15 08:39:04.000000 numerical_py-0.0.2/numerical_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:01:47.128062 numerical_py-0.0.2/numerical_py/integrals/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:00:43.000000 numerical_py-0.0.2/numerical_py/integrals/__init__.py
--rw-rw-rw-   0        0        0      210 2023-06-15 09:00:45.000000 numerical_py-0.0.2/numerical_py/integrals/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:01:47.128062 numerical_py-0.0.2/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 09:01:46.000000 numerical_py-0.0.2/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-15 09:01:46.000000 numerical_py-0.0.2/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:01:46.000000 numerical_py-0.0.2/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 09:01:46.000000 numerical_py-0.0.2/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:01:47.136067 numerical_py-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 09:01:44.000000 numerical_py-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:09:40.004671 numerical_py-0.0.3/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:09:40.004671 numerical_py-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 09:09:39.988638 numerical_py-0.0.3/numerical_py/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:07:48.000000 numerical_py-0.0.3/numerical_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:09:40.004671 numerical_py-0.0.3/numerical_py/integrals/
+-rw-rw-rw-   0        0        0       33 2023-06-15 09:07:50.000000 numerical_py-0.0.3/numerical_py/integrals/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-06-15 09:00:45.000000 numerical_py-0.0.3/numerical_py/integrals/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:09:39.996655 numerical_py-0.0.3/numerical_py.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-06-15 09:09:39.000000 numerical_py-0.0.3/numerical_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-15 09:09:39.000000 numerical_py-0.0.3/numerical_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:09:39.000000 numerical_py-0.0.3/numerical_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 09:09:39.000000 numerical_py-0.0.3/numerical_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:09:40.004671 numerical_py-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-06-15 09:09:37.000000 numerical_py-0.0.3/setup.py
```

