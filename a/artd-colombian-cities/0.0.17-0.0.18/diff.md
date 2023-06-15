# Comparing `tmp/artd_colombian_cities-0.0.17.tar.gz` & `tmp/artd_colombian_cities-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_colombian_cities-0.0.17.tar", last modified: Tue Jun 13 23:29:04 2023, max compression
+gzip compressed data, was "artd_colombian_cities-0.0.18.tar", last modified: Thu Jun 15 18:50:17 2023, max compression
```

## Comparing `artd_colombian_cities-0.0.17.tar` & `artd_colombian_cities-0.0.18.tar`

### file list

```diff
@@ -1,49 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/artd_colombian_cities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/artd_colombian_cities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/artd_colombian_cities/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/artd_colombian_cities/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/artd_colombian_cities/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/artd_colombian_cities/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-13 23:29:04.000000 artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 23:29:04.000000 artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:29:04.000000 artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 23:29:04.000000 artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/colombian_cities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/colombian_cities/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/data/cities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/data/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/data/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/colombian_cities/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/generators/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.611211 artd_colombian_cities-0.0.17/colombian_cities/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/colombian_cities/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_colombian_cities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_colombian_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_countries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/colombian_cities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/colombian_cities/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/migrate/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:28:58.000000 artd_colombian_cities-0.0.17/migrate/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:29:04.615211 artd_colombian_cities-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 23:29:02.000000 artd_colombian_cities-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.343655 artd_colombian_cities-0.0.18/artd_colombian_cities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/artd_colombian_cities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/artd_colombian_cities/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/artd_colombian_cities/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/artd_colombian_cities/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/artd_colombian_cities/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.343655 artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 18:50:17.000000 artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-15 18:50:17.000000 artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:50:17.000000 artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 18:50:17.000000 artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.343655 artd_colombian_cities-0.0.18/colombian_cities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/__pycache__/tests.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)   197788 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/__pycache__/cities.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    25286 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/__pycache__/countries.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/__pycache__/regions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/data/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/generators/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.343655 artd_colombian_cities-0.0.18/colombian_cities/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__pycache__/create_colombian_cities.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__pycache__/create_colombian_regions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/__pycache__/create_countries.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_colombian_cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_colombian_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_countries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/colombian_cities/migrations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/colombian_cities/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/migrate/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 18:50:15.000000 artd_colombian_cities-0.0.18/migrate/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:50:17.347655 artd_colombian_cities-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-15 18:50:16.000000 artd_colombian_cities-0.0.18/setup.py
```

### Comparing `artd_colombian_cities-0.0.17/PKG-INFO` & `artd_colombian_cities-0.0.18/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd_colombian_cities
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Django app to create Colombian cities
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,15 +28,15 @@
 A Django app to create Colombian cities.
 
 Quick start
 -----------
 
 1. Add "colombian_cities" to your INSTALLED_APPS setting like this:
 
-2. Run ``python manage.py migrate`` to create the polls models.
+2. Run ``python manage.py migrate`` to create the colombian cities models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
```

### Comparing `artd_colombian_cities-0.0.17/README.rst` & `artd_colombian_cities-0.0.18/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Django app to create Colombian cities.
 
 Quick start
 -----------
 
 1. Add "colombian_cities" to your INSTALLED_APPS setting like this:
 
-2. Run ``python manage.py migrate`` to create the polls models.
+2. Run ``python manage.py migrate`` to create the colombian cities models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
```

### Comparing `artd_colombian_cities-0.0.17/artd_colombian_cities/settings.py` & `artd_colombian_cities-0.0.18/artd_colombian_cities/settings.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/artd_colombian_cities/urls.py` & `artd_colombian_cities-0.0.18/artd_colombian_cities/urls.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/artd_colombian_cities.egg-info/PKG-INFO` & `artd_colombian_cities-0.0.18/artd_colombian_cities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-colombian-cities
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Django app to create Colombian cities
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,15 +28,15 @@
 A Django app to create Colombian cities.
 
 Quick start
 -----------
 
 1. Add "colombian_cities" to your INSTALLED_APPS setting like this:
 
-2. Run ``python manage.py migrate`` to create the polls models.
+2. Run ``python manage.py migrate`` to create the colombian cities models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
```

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/admin.py` & `artd_colombian_cities-0.0.18/colombian_cities/admin.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/data/cities.py` & `artd_colombian_cities-0.0.18/colombian_cities/data/cities.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/data/countries.py` & `artd_colombian_cities-0.0.18/colombian_cities/data/countries.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/data/regions.py` & `artd_colombian_cities-0.0.18/colombian_cities/data/regions.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/generators/generators.py` & `artd_colombian_cities-0.0.18/colombian_cities/generators/generators.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_colombian_cities.py` & `artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_colombian_cities.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_colombian_regions.py` & `artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_colombian_regions.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/management/commands/create_countries.py` & `artd_colombian_cities-0.0.18/colombian_cities/management/commands/create_countries.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/migrations/0001_initial.py` & `artd_colombian_cities-0.0.18/colombian_cities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/models.py` & `artd_colombian_cities-0.0.18/colombian_cities/models.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/colombian_cities/tests.py` & `artd_colombian_cities-0.0.18/colombian_cities/tests.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.17/setup.py` & `artd_colombian_cities-0.0.18/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd_colombian_cities",
-    version="0.0.17",
+    version="0.0.18",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to create Colombian cities",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

