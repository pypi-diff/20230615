# Comparing `tmp/casho-0.0.13.tar.gz` & `tmp/Casho-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casho-0.0.13.tar", last modified: Thu Jun 15 06:57:26 2023, max compression
+gzip compressed data, was "Casho-1.0.0.tar", last modified: Thu Jun 15 20:11:44 2023, max compression
```

## Comparing `casho-0.0.13.tar` & `Casho-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:57:26.853045 casho-0.0.13/
--rw-rw-rw-   0        0        0      204 2023-06-15 06:57:26.851091 casho-0.0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 06:57:26.848041 casho-0.0.13/casho.egg-info/
--rw-rw-rw-   0        0        0      204 2023-06-15 06:57:26.000000 casho-0.0.13/casho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-06-15 06:57:26.000000 casho-0.0.13/casho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:57:26.000000 casho-0.0.13/casho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 06:57:26.000000 casho-0.0.13/casho.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:57:26.000000 casho-0.0.13/casho.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 06:57:26.854054 casho-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-06-15 06:57:22.000000 casho-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:11:44.260464 Casho-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-15 20:11:44.232871 Casho-1.0.0/Casho.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-06-15 20:11:44.000000 Casho-1.0.0/Casho.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-15 20:11:44.000000 Casho-1.0.0/Casho.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 20:11:44.000000 Casho-1.0.0/Casho.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 20:11:44.000000 Casho-1.0.0/Casho.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-15 20:11:44.000000 Casho-1.0.0/Casho.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      330 2023-06-15 20:11:44.259753 Casho-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 20:11:44.257753 Casho-1.0.0/py/
+-rw-rw-rw-   0        0        0       46 2023-06-15 19:58:50.000000 Casho-1.0.0/py/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-15 20:00:33.000000 Casho-1.0.0/py/admin.py
+-rw-rw-rw-   0        0        0      145 2023-06-15 20:00:30.000000 Casho-1.0.0/py/apps.py
+-rw-rw-rw-   0        0        0      619 2023-06-15 20:00:42.000000 Casho-1.0.0/py/custom_error.py
+-rw-rw-rw-   0        0        0      392 2023-06-15 20:00:45.000000 Casho-1.0.0/py/database_connection_error.py
+-rw-rw-rw-   0        0        0     2306 2023-06-15 20:00:48.000000 Casho-1.0.0/py/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:11:44.258753 Casho-1.0.0/py/migrations/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:48:05.000000 Casho-1.0.0/py/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-06-15 19:48:05.000000 Casho-1.0.0/py/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-15 19:48:05.000000 Casho-1.0.0/py/tests.py
+-rw-rw-rw-   0        0        0      289 2023-06-15 19:52:03.000000 Casho-1.0.0/py/views.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 20:11:44.260464 Casho-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-06-15 20:10:36.000000 Casho-1.0.0/setup.py
```

