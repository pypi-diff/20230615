# Comparing `tmp/django-sweet-utils-1.4.0.tar.gz` & `tmp/django-sweet-utils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sweet-utils-1.4.0.tar", last modified: Tue Jun 13 12:00:11 2023, max compression
+gzip compressed data, was "django-sweet-utils-1.5.0.tar", last modified: Thu Jun 15 06:47:52 2023, max compression
```

## Comparing `django-sweet-utils-1.4.0.tar` & `django-sweet-utils-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.711107 django-sweet-utils-1.4.0/
--rw-r--r--   0 rustam     (501) staff       (20)     1063 2023-06-13 11:36:27.000000 django-sweet-utils-1.4.0/LICENSE
--rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     6484 2023-06-13 12:00:11.711296 django-sweet-utils-1.4.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     5119 2023-06-13 11:58:13.000000 django-sweet-utils-1.4.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.684834 django-sweet-utils-1.4.0/django_sweet_utils/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/__init__.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.687579 django-sweet-utils-1.4.0/django_sweet_utils/admin/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-05-25 16:24:12.000000 django-sweet-utils-1.4.0/django_sweet_utils/admin/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      253 2023-05-25 16:25:07.000000 django-sweet-utils-1.4.0/django_sweet_utils/admin/actions.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.689773 django-sweet-utils-1.4.0/django_sweet_utils/api/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/metadata.py
--rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/permissions.py
--rw-r--r--   0 rustam     (501) staff       (20)      962 2023-06-13 11:41:06.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/views.py
--rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/apps.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.690592 django-sweet-utils-1.4.0/django_sweet_utils/db/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/db/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     2232 2023-05-25 16:16:51.000000 django-sweet-utils-1.4.0/django_sweet_utils/db/models.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.692247 django-sweet-utils-1.4.0/django_sweet_utils/misc/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/json.py
--rw-r--r--   0 rustam     (501) staff       (20)     1462 2023-06-13 11:58:13.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/logging.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.693118 django-sweet-utils-1.4.0/django_sweet_utils/serializers/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.4.0/django_sweet_utils/serializers/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.4.0/django_sweet_utils/serializers/fields.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.710645 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/format_str.py
--rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/query_string.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.687003 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     6484 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      919 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       32 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       19 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1211 2023-06-13 12:00:11.712115 django-sweet-utils-1.4.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.962026 django-sweet-utils-1.5.0/
+-rw-r--r--   0 rustam     (501) staff       (20)     1063 2023-06-13 11:36:27.000000 django-sweet-utils-1.5.0/LICENSE
+-rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     6781 2023-06-15 06:47:52.962161 django-sweet-utils-1.5.0/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     5416 2023-06-15 06:47:10.000000 django-sweet-utils-1.5.0/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.936375 django-sweet-utils-1.5.0/django_sweet_utils/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/django_sweet_utils/__init__.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.940117 django-sweet-utils-1.5.0/django_sweet_utils/admin/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-05-25 16:24:12.000000 django-sweet-utils-1.5.0/django_sweet_utils/admin/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      253 2023-05-25 16:25:07.000000 django-sweet-utils-1.5.0/django_sweet_utils/admin/actions.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.943133 django-sweet-utils-1.5.0/django_sweet_utils/api/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/django_sweet_utils/api/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.5.0/django_sweet_utils/api/metadata.py
+-rw-r--r--   0 rustam     (501) staff       (20)      183 2023-06-15 06:47:10.000000 django-sweet-utils-1.5.0/django_sweet_utils/api/pagination.py
+-rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.5.0/django_sweet_utils/api/permissions.py
+-rw-r--r--   0 rustam     (501) staff       (20)      962 2023-06-13 11:41:06.000000 django-sweet-utils-1.5.0/django_sweet_utils/api/views.py
+-rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/django_sweet_utils/apps.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.944450 django-sweet-utils-1.5.0/django_sweet_utils/db/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/django_sweet_utils/db/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     2232 2023-05-25 16:16:51.000000 django-sweet-utils-1.5.0/django_sweet_utils/db/models.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.946058 django-sweet-utils-1.5.0/django_sweet_utils/misc/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/django_sweet_utils/misc/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.5.0/django_sweet_utils/misc/json.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1462 2023-06-13 11:58:13.000000 django-sweet-utils-1.5.0/django_sweet_utils/misc/logging.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.947280 django-sweet-utils-1.5.0/django_sweet_utils/serializers/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.5.0/django_sweet_utils/serializers/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.5.0/django_sweet_utils/serializers/fields.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.961561 django-sweet-utils-1.5.0/django_sweet_utils/templatetags/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.5.0/django_sweet_utils/templatetags/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.5.0/django_sweet_utils/templatetags/format_str.py
+-rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.5.0/django_sweet_utils/templatetags/query_string.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 06:47:52.939324 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     6781 2023-06-15 06:47:52.000000 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      956 2023-06-15 06:47:52.000000 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-15 06:47:52.000000 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       32 2023-06-15 06:47:52.000000 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       19 2023-06-15 06:47:52.000000 django-sweet-utils-1.5.0/django_sweet_utils.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1211 2023-06-15 06:47:52.962621 django-sweet-utils-1.5.0/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.5.0/setup.py
```

### Comparing `django-sweet-utils-1.4.0/LICENSE` & `django-sweet-utils-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/PKG-INFO` & `django-sweet-utils-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sweet-utils
-Version: 1.4.0
+Version: 1.5.0
 Summary: A little django code sugar.
 Home-page: https://github.com/AllYouZombies/django-sweet-utils
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -116,30 +116,45 @@
 
 You can get object or `None` if it does not exist with `get_or_none()` method on your model manager.
 
 ```python
 obj = MyModel.objects.get_or_none(pk=1)
 ```
 
-### API Views
+### API
+
+#### Views
 
 Inherit your DRF API views from `django_sweet_utils.api.views`:  
   
 ```
 from django_sweet_utils.api.views import UpdateAPIView, DestroyAPIView
 
 
 class MyUpdateView(UpdateAPIView):
    ...
 
 
 class MyDestroyView(DestroyAPIView):
    ...
 ```
-   
+  
+#### Pagination
+
+There is `PageNumberPagination` class that adds `page_size` query parameter to `PageNumberPagination` class.  
+  
+```python
+REST_FRAMEWORK = {
+   ...
+   'DEFAULT_PAGINATION_CLASS': 'django_sweet_utils.api.pagination.PageNumberPagination',
+   'PAGE_SIZE': 10,
+   ...
+}
+```
+  
 From now your views supports `POST` request method instead of `PATCH` and `DELETE`
 DestroyAPIView does not perform actual database deletion, but only marks file as deleted with `is_deleted=True`
   
 ### Permissions
 
 #### There is `DjangoModelPermissions` class that adds `view` permission to `DjangoModelPermissions` class on `GET` request method.
```

### Comparing `django-sweet-utils-1.4.0/README.md` & `django-sweet-utils-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -81,30 +81,45 @@
 
 You can get object or `None` if it does not exist with `get_or_none()` method on your model manager.
 
 ```python
 obj = MyModel.objects.get_or_none(pk=1)
 ```
 
-### API Views
+### API
+
+#### Views
 
 Inherit your DRF API views from `django_sweet_utils.api.views`:  
   
 ```
 from django_sweet_utils.api.views import UpdateAPIView, DestroyAPIView
 
 
 class MyUpdateView(UpdateAPIView):
    ...
 
 
 class MyDestroyView(DestroyAPIView):
    ...
 ```
-   
+  
+#### Pagination
+
+There is `PageNumberPagination` class that adds `page_size` query parameter to `PageNumberPagination` class.  
+  
+```python
+REST_FRAMEWORK = {
+   ...
+   'DEFAULT_PAGINATION_CLASS': 'django_sweet_utils.api.pagination.PageNumberPagination',
+   'PAGE_SIZE': 10,
+   ...
+}
+```
+  
 From now your views supports `POST` request method instead of `PATCH` and `DELETE`
 DestroyAPIView does not perform actual database deletion, but only marks file as deleted with `is_deleted=True`
   
 ### Permissions
 
 #### There is `DjangoModelPermissions` class that adds `view` permission to `DjangoModelPermissions` class on `GET` request method.
```

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/api/metadata.py` & `django-sweet-utils-1.5.0/django_sweet_utils/api/metadata.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/api/views.py` & `django-sweet-utils-1.5.0/django_sweet_utils/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/db/models.py` & `django-sweet-utils-1.5.0/django_sweet_utils/db/models.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/misc/logging.py` & `django-sweet-utils-1.5.0/django_sweet_utils/misc/logging.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/serializers/fields.py` & `django-sweet-utils-1.5.0/django_sweet_utils/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils/templatetags/query_string.py` & `django-sweet-utils-1.5.0/django_sweet_utils/templatetags/query_string.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils.egg-info/PKG-INFO` & `django-sweet-utils-1.5.0/django_sweet_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sweet-utils
-Version: 1.4.0
+Version: 1.5.0
 Summary: A little django code sugar.
 Home-page: https://github.com/AllYouZombies/django-sweet-utils
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -116,30 +116,45 @@
 
 You can get object or `None` if it does not exist with `get_or_none()` method on your model manager.
 
 ```python
 obj = MyModel.objects.get_or_none(pk=1)
 ```
 
-### API Views
+### API
+
+#### Views
 
 Inherit your DRF API views from `django_sweet_utils.api.views`:  
   
 ```
 from django_sweet_utils.api.views import UpdateAPIView, DestroyAPIView
 
 
 class MyUpdateView(UpdateAPIView):
    ...
 
 
 class MyDestroyView(DestroyAPIView):
    ...
 ```
-   
+  
+#### Pagination
+
+There is `PageNumberPagination` class that adds `page_size` query parameter to `PageNumberPagination` class.  
+  
+```python
+REST_FRAMEWORK = {
+   ...
+   'DEFAULT_PAGINATION_CLASS': 'django_sweet_utils.api.pagination.PageNumberPagination',
+   'PAGE_SIZE': 10,
+   ...
+}
+```
+  
 From now your views supports `POST` request method instead of `PATCH` and `DELETE`
 DestroyAPIView does not perform actual database deletion, but only marks file as deleted with `is_deleted=True`
   
 ### Permissions
 
 #### There is `DjangoModelPermissions` class that adds `view` permission to `DjangoModelPermissions` class on `GET` request method.
```

### Comparing `django-sweet-utils-1.4.0/django_sweet_utils.egg-info/SOURCES.txt` & `django-sweet-utils-1.5.0/django_sweet_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 django_sweet_utils.egg-info/dependency_links.txt
 django_sweet_utils.egg-info/requires.txt
 django_sweet_utils.egg-info/top_level.txt
 django_sweet_utils/admin/__init__.py
 django_sweet_utils/admin/actions.py
 django_sweet_utils/api/__init__.py
 django_sweet_utils/api/metadata.py
+django_sweet_utils/api/pagination.py
 django_sweet_utils/api/permissions.py
 django_sweet_utils/api/views.py
 django_sweet_utils/db/__init__.py
 django_sweet_utils/db/models.py
 django_sweet_utils/misc/__init__.py
 django_sweet_utils/misc/json.py
 django_sweet_utils/misc/logging.py
```

### Comparing `django-sweet-utils-1.4.0/setup.cfg` & `django-sweet-utils-1.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-sweet-utils
-version = 1.4.0
+version = 1.5.0
 description = A little django code sugar.
 url = https://github.com/AllYouZombies/django-sweet-utils
 author = Astafeev Rustam
 author_email = rustam@astafeev.dev
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
```

