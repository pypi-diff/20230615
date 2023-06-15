# Comparing `tmp/django-persistent-filters-0.21.tar.gz` & `tmp/django-persistent-filters-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-persistent-filters-0.21.tar", last modified: Tue Dec  7 14:57:34 2021, max compression
+gzip compressed data, was "django-persistent-filters-1.0.tar", last modified: Thu Jun 15 13:34:26 2023, max compression
```

## Comparing `django-persistent-filters-0.21.tar` & `django-persistent-filters-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2021-12-07 14:15:56.000000 django-persistent-filters-0.21/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2020 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      916 2021-12-07 14:51:00.000000 django-persistent-filters-0.21/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/django_persistent_filters.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2020 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      371 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       19 2021-12-07 14:57:33.000000 django-persistent-filters-0.21/django_persistent_filters.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/persistent_filters/
--rw-rw-r--   0 user      (1000) user      (1000)      189 2021-12-07 14:56:12.000000 django-persistent-filters-0.21/persistent_filters/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      150 2021-12-07 13:24:31.000000 django-persistent-filters-0.21/persistent_filters/apps.py
--rw-rw-r--   0 user      (1000) user      (1000)     1221 2021-12-07 14:51:00.000000 django-persistent-filters-0.21/persistent_filters/middleware.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2021-12-07 14:57:34.004359 django-persistent-filters-0.21/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-12-07 13:18:24.000000 django-persistent-filters-0.21/setup.py
+drwxr-xr-x   0 lorenzoprodon   (501) staff       (20)        0 2023-06-15 13:34:26.292478 django-persistent-filters-1.0/
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     1057 2023-06-15 13:22:54.000000 django-persistent-filters-1.0/LICENSE
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     2213 2023-06-15 13:34:26.292532 django-persistent-filters-1.0/PKG-INFO
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     1098 2023-06-15 13:22:54.000000 django-persistent-filters-1.0/README.md
+drwxr-xr-x   0 lorenzoprodon   (501) staff       (20)        0 2023-06-15 13:34:26.291807 django-persistent-filters-1.0/django_persistent_filters.egg-info/
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     2213 2023-06-15 13:34:26.000000 django-persistent-filters-1.0/django_persistent_filters.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)      371 2023-06-15 13:34:26.000000 django-persistent-filters-1.0/django_persistent_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)        1 2023-06-15 13:34:26.000000 django-persistent-filters-1.0/django_persistent_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)       12 2023-06-15 13:34:26.000000 django-persistent-filters-1.0/django_persistent_filters.egg-info/requires.txt
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)       19 2023-06-15 13:34:26.000000 django-persistent-filters-1.0/django_persistent_filters.egg-info/top_level.txt
+drwxr-xr-x   0 lorenzoprodon   (501) staff       (20)        0 2023-06-15 13:34:26.292272 django-persistent-filters-1.0/persistent_filters/
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)      188 2023-06-15 13:33:25.000000 django-persistent-filters-1.0/persistent_filters/__init__.py
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)      150 2023-06-15 11:57:18.000000 django-persistent-filters-1.0/persistent_filters/apps.py
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     2169 2023-06-15 13:20:44.000000 django-persistent-filters-1.0/persistent_filters/middleware.py
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)     1150 2023-06-15 13:34:26.292763 django-persistent-filters-1.0/setup.cfg
+-rw-r--r--   0 lorenzoprodon   (501) staff       (20)       38 2023-06-15 11:57:18.000000 django-persistent-filters-1.0/setup.py
```

### Comparing `django-persistent-filters-0.21/LICENSE` & `django-persistent-filters-1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Lorenzo Prodon
+Copyright (c) 2023 Lorenzo Prodon
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-persistent-filters-0.21/PKG-INFO` & `django-persistent-filters-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-persistent-filters
-Version: 0.21
-Summary: Provide a django middleware that take care to persist the querystring in the browser cookies.
+Version: 1.0
+Summary: Provide a django middleware that take care to persist the querystring in the browser cookies or in the Django Request object.
 Home-page: https://github.com/LorenzoProd/django-persistent-filters
 Author: Lorenzo Prodon
 Author-email: lorenzo.prodon@gmail.com
 License: BSD-3-Clause  # Example license
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,15 +23,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Persistent Filters
 
 Django Persistent Filters is a Python package which provide a django middleware that take care to persist the
-querystring in the browser cookies.
+querystring in the browser cookies or in the Django Request object.
 
 If you have a ListView with a Form for filter the objects, this package is perfect for you!
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install:
 
@@ -47,14 +46,18 @@
 ```python
 MIDDLEWARE = [
     ...,
     "persistent_filters.middleware.PersistentFiltersMiddleware"
 ]
 ```
 
+If you want to store filters in the Request object instead Cookies, add in the `settings.py` file:
+```python
+PERSISTENT_FILTERS_IN_REQUEST = True
+```
 Add the urls with a filter form in `settings.py` file:
 
 ```python
 PERSISTENT_FILTERS_URLS = [
     # You can use name urls
     reverse_lazy("user:list"),
 
@@ -64,9 +67,7 @@
 ```
 
 Add in the form the button for reset filters:
 
 ```html
 <button type="submit" name="reset-filters">Reset</button>
 ```
-
-
```

### Comparing `django-persistent-filters-0.21/django_persistent_filters.egg-info/PKG-INFO` & `django-persistent-filters-1.0/django_persistent_filters.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-persistent-filters
-Version: 0.21
-Summary: Provide a django middleware that take care to persist the querystring in the browser cookies.
+Version: 1.0
+Summary: Provide a django middleware that take care to persist the querystring in the browser cookies or in the Django Request object.
 Home-page: https://github.com/LorenzoProd/django-persistent-filters
 Author: Lorenzo Prodon
 Author-email: lorenzo.prodon@gmail.com
 License: BSD-3-Clause  # Example license
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,15 +23,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Persistent Filters
 
 Django Persistent Filters is a Python package which provide a django middleware that take care to persist the
-querystring in the browser cookies.
+querystring in the browser cookies or in the Django Request object.
 
 If you have a ListView with a Form for filter the objects, this package is perfect for you!
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install:
 
@@ -47,14 +46,18 @@
 ```python
 MIDDLEWARE = [
     ...,
     "persistent_filters.middleware.PersistentFiltersMiddleware"
 ]
 ```
 
+If you want to store filters in the Request object instead Cookies, add in the `settings.py` file:
+```python
+PERSISTENT_FILTERS_IN_REQUEST = True
+```
 Add the urls with a filter form in `settings.py` file:
 
 ```python
 PERSISTENT_FILTERS_URLS = [
     # You can use name urls
     reverse_lazy("user:list"),
 
@@ -64,9 +67,7 @@
 ```
 
 Add in the form the button for reset filters:
 
 ```html
 <button type="submit" name="reset-filters">Reset</button>
 ```
-
-
```

### Comparing `django-persistent-filters-0.21/setup.cfg` & `django-persistent-filters-1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = django-persistent-filters
 version = attr: persistent_filters.__version__
-description = Provide a django middleware that take care to persist the querystring in the browser cookies.
+description = Provide a django middleware that take care to persist the querystring in the browser cookies or in the Django Request object.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LorenzoProd/django-persistent-filters
 author = Lorenzo Prodon
 author_email = lorenzo.prodon@gmail.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

