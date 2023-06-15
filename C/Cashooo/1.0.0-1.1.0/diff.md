# Comparing `tmp/Cashooo-1.0.0.tar.gz` & `tmp/Cashooo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cashooo-1.0.0.tar", last modified: Thu Jun 15 20:55:05 2023, max compression
+gzip compressed data, was "Cashooo-1.1.0.tar", last modified: Thu Jun 15 21:01:30 2023, max compression
```

## Comparing `Cashooo-1.0.0.tar` & `Cashooo-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 20:55:05.794144 Cashooo-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-15 20:55:05.666140 Cashooo-1.0.0/Cashooo/
--rw-rw-rw-   0        0        0       66 2023-06-15 20:50:02.000000 Cashooo-1.0.0/Cashooo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:55:05.783146 Cashooo-1.0.0/Cashooo/mylibrary/
--rw-rw-rw-   0        0        0      211 2023-06-15 20:55:00.000000 Cashooo-1.0.0/Cashooo/mylibrary/__init__.py
--rw-rw-rw-   0        0        0       66 2023-06-15 20:00:33.000000 Cashooo-1.0.0/Cashooo/mylibrary/admin.py
--rw-rw-rw-   0        0        0      167 2023-06-15 20:54:48.000000 Cashooo-1.0.0/Cashooo/mylibrary/apps.py
--rw-rw-rw-   0        0        0      619 2023-06-15 20:00:42.000000 Cashooo-1.0.0/Cashooo/mylibrary/custom_error.py
--rw-rw-rw-   0        0        0      392 2023-06-15 20:00:45.000000 Cashooo-1.0.0/Cashooo/mylibrary/database_connection_error.py
--rw-rw-rw-   0        0        0     2306 2023-06-15 20:00:48.000000 Cashooo-1.0.0/Cashooo/mylibrary/middleware.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:55:05.787153 Cashooo-1.0.0/Cashooo/mylibrary/migrations/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:48:05.000000 Cashooo-1.0.0/Cashooo/mylibrary/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-06-15 19:48:05.000000 Cashooo-1.0.0/Cashooo/mylibrary/models.py
--rw-rw-rw-   0        0        0       63 2023-06-15 19:48:05.000000 Cashooo-1.0.0/Cashooo/mylibrary/tests.py
--rw-rw-rw-   0        0        0      289 2023-06-15 19:52:03.000000 Cashooo-1.0.0/Cashooo/mylibrary/views.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:55:05.730135 Cashooo-1.0.0/Cashooo.egg-info/
--rw-rw-rw-   0        0        0      332 2023-06-15 20:55:05.000000 Cashooo-1.0.0/Cashooo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-15 20:55:05.000000 Cashooo-1.0.0/Cashooo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 20:55:05.000000 Cashooo-1.0.0/Cashooo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 20:55:05.000000 Cashooo-1.0.0/Cashooo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 20:55:05.000000 Cashooo-1.0.0/Cashooo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      332 2023-06-15 20:55:05.792148 Cashooo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-15 20:55:05.794144 Cashooo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-15 20:54:57.000000 Cashooo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:01:30.474139 Cashooo-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:01:30.373571 Cashooo-1.1.0/Cashooo/
+-rw-rw-rw-   0        0        0       66 2023-06-15 20:50:02.000000 Cashooo-1.1.0/Cashooo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:01:30.464165 Cashooo-1.1.0/Cashooo/mylibrary/
+-rw-rw-rw-   0        0        0      251 2023-06-15 20:59:53.000000 Cashooo-1.1.0/Cashooo/mylibrary/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-15 20:00:33.000000 Cashooo-1.1.0/Cashooo/mylibrary/admin.py
+-rw-rw-rw-   0        0        0      167 2023-06-15 20:54:48.000000 Cashooo-1.1.0/Cashooo/mylibrary/apps.py
+-rw-rw-rw-   0        0        0      619 2023-06-15 20:00:42.000000 Cashooo-1.1.0/Cashooo/mylibrary/custom_error.py
+-rw-rw-rw-   0        0        0      392 2023-06-15 20:00:45.000000 Cashooo-1.1.0/Cashooo/mylibrary/database_connection_error.py
+-rw-rw-rw-   0        0        0     2306 2023-06-15 20:00:48.000000 Cashooo-1.1.0/Cashooo/mylibrary/middleware.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:01:30.468136 Cashooo-1.1.0/Cashooo/mylibrary/migrations/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:48:05.000000 Cashooo-1.1.0/Cashooo/mylibrary/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-06-15 19:48:05.000000 Cashooo-1.1.0/Cashooo/mylibrary/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-15 19:48:05.000000 Cashooo-1.1.0/Cashooo/mylibrary/tests.py
+-rw-rw-rw-   0        0        0      289 2023-06-15 19:52:03.000000 Cashooo-1.1.0/Cashooo/mylibrary/views.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:01:30.412138 Cashooo-1.1.0/Cashooo.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-06-15 21:01:30.000000 Cashooo-1.1.0/Cashooo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-15 21:01:30.000000 Cashooo-1.1.0/Cashooo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:01:30.000000 Cashooo-1.1.0/Cashooo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 21:01:30.000000 Cashooo-1.1.0/Cashooo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 21:01:30.000000 Cashooo-1.1.0/Cashooo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      332 2023-06-15 21:01:30.472142 Cashooo-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:01:30.475153 Cashooo-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-15 21:01:25.000000 Cashooo-1.1.0/setup.py
```

### Comparing `Cashooo-1.0.0/Cashooo/mylibrary/custom_error.py` & `Cashooo-1.1.0/Cashooo/mylibrary/custom_error.py`

 * *Files identical despite different names*

### Comparing `Cashooo-1.0.0/Cashooo/mylibrary/middleware.py` & `Cashooo-1.1.0/Cashooo/mylibrary/middleware.py`

 * *Files identical despite different names*

