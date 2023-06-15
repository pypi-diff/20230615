# Comparing `tmp/django-persistent-filters-0.2.tar.gz` & `tmp/django-persistent-filters-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-persistent-filters-0.2.tar", last modified: Tue Dec  7 14:54:09 2021, max compression
+gzip compressed data, was "dist/django-persistent-filters-0.21.tar", last modified: Tue Dec  7 14:57:34 2021, max compression
```

## Comparing `django-persistent-filters-0.2.tar` & `django-persistent-filters-0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:54:09.267584 django-persistent-filters-0.2/
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2021-12-07 14:15:56.000000 django-persistent-filters-0.2/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2021-12-07 14:54:09.267584 django-persistent-filters-0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      916 2021-12-07 14:51:00.000000 django-persistent-filters-0.2/README.rst
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:54:09.267584 django-persistent-filters-0.2/django_persistent_filters.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2021-12-07 14:54:09.000000 django-persistent-filters-0.2/django_persistent_filters.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      372 2021-12-07 14:54:09.000000 django-persistent-filters-0.2/django_persistent_filters.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-12-07 14:54:09.000000 django-persistent-filters-0.2/django_persistent_filters.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2021-12-07 14:54:09.000000 django-persistent-filters-0.2/django_persistent_filters.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       19 2021-12-07 14:54:09.000000 django-persistent-filters-0.2/django_persistent_filters.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:54:09.267584 django-persistent-filters-0.2/persistent_filters/
--rw-rw-r--   0 user      (1000) user      (1000)      188 2021-12-07 13:45:23.000000 django-persistent-filters-0.2/persistent_filters/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      150 2021-12-07 13:24:31.000000 django-persistent-filters-0.2/persistent_filters/apps.py
--rw-rw-r--   0 user      (1000) user      (1000)     1221 2021-12-07 14:51:00.000000 django-persistent-filters-0.2/persistent_filters/middleware.py
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2021-12-07 14:54:09.271584 django-persistent-filters-0.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-12-07 13:18:24.000000 django-persistent-filters-0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/
+-rw-rw-r--   0 user      (1000) user      (1000)     1057 2021-12-07 14:15:56.000000 django-persistent-filters-0.21/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2020 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      916 2021-12-07 14:51:00.000000 django-persistent-filters-0.21/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/django_persistent_filters.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2020 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      371 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       19 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/persistent_filters/
+-rw-rw-r--   0 user      (1000) user      (1000)      189 2021-12-07 14:56:12.000000 django-persistent-filters-0.21/persistent_filters/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      150 2021-12-07 13:24:31.000000 django-persistent-filters-0.21/persistent_filters/apps.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1221 2021-12-07 14:51:00.000000 django-persistent-filters-0.21/persistent_filters/middleware.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2021-12-07 13:18:24.000000 django-persistent-filters-0.21/setup.py
```

### Comparing `django-persistent-filters-0.2/LICENSE` & `django-persistent-filters-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `django-persistent-filters-0.2/README.rst` & `django-persistent-filters-0.21/README.md`

 * *Files identical despite different names*

### Comparing `django-persistent-filters-0.2/persistent_filters/middleware.py` & `django-persistent-filters-0.21/persistent_filters/middleware.py`

 * *Files identical despite different names*

### Comparing `django-persistent-filters-0.2/setup.cfg` & `django-persistent-filters-0.21/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = django-persistent-filters
 version = attr: persistent_filters.__version__
 description = Provide a django middleware that take care to persist the querystring in the browser cookies.
 long_description = file: README.md
+long_description_content_type = text/markdown
 url = https://github.com/LorenzoProd/django-persistent-filters
 author = Lorenzo Prodon
 author_email = lorenzo.prodon@gmail.com
 license = BSD-3-Clause  # Example license
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

