# Comparing `tmp/drf-simplejwt-additions-1.1.2.tar.gz` & `tmp/drf-simplejwt-additions-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-simplejwt-additions-1.1.2.tar", last modified: Wed Jun 14 07:33:33 2023, max compression
+gzip compressed data, was "drf-simplejwt-additions-1.1.3.tar", last modified: Thu Jun 15 10:52:18 2023, max compression
```

## Comparing `drf-simplejwt-additions-1.1.2.tar` & `drf-simplejwt-additions-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.109520 drf-simplejwt-additions-1.1.2/
--rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.2/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:33:33.109635 drf-simplejwt-additions-1.1.2/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     2601 2023-06-14 07:17:24.000000 drf-simplejwt-additions-1.1.2/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.107266 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1459 2023-06-14 06:59:58.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/middleware.py
--rw-r--r--   0 rustam     (501) staff       (20)      552 2023-06-14 07:33:25.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/serializers.py
--rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/views.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.109109 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      420 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-14 07:33:33.110301 drf-simplejwt-additions-1.1.2/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.2/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 10:52:18.618543 drf-simplejwt-additions-1.1.3/
+-rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.3/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-15 10:52:18.619222 drf-simplejwt-additions-1.1.3/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     2601 2023-06-14 07:17:24.000000 drf-simplejwt-additions-1.1.3/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 10:52:18.609209 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1577 2023-06-15 10:15:53.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/middleware.py
+-rw-r--r--   0 rustam     (501) staff       (20)      597 2023-06-15 10:52:09.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/serializers.py
+-rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/views.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-15 10:52:18.617197 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-15 10:52:18.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      420 2023-06-15 10:52:18.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-15 10:52:18.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-15 10:52:18.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-15 10:52:18.000000 drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-15 10:52:18.622326 drf-simplejwt-additions-1.1.3/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.3/setup.py
```

### Comparing `drf-simplejwt-additions-1.1.2/PKG-INFO` & `drf-simplejwt-additions-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-simplejwt-additions
-Version: 1.1.2
+Version: 1.1.3
 Summary: Additions for Django Rest Framework Simple JWT
 Home-page: https://github.com/AllYouZombies/drf-simplejwt-additions
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-simplejwt-additions-1.1.2/README.md` & `drf-simplejwt-additions-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/middleware.py` & `drf-simplejwt-additions-1.1.3/drf_simplejwt_additions/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.contrib.auth import get_user_model
 from django.conf import settings
 from django.utils.deprecation import MiddlewareMixin
 from jwt import decode as jwt_decode
+from jwt.exceptions import InvalidSignatureError, ExpiredSignatureError
 from rest_framework_simplejwt.exceptions import InvalidToken, TokenError
 
 import logging
 
 
 User = get_user_model()
 
@@ -24,15 +25,15 @@
             return self.get_response(request)
         token = request.META.get('HTTP_AUTHORIZATION', '').split(' ')[-1]
         if not token:
             return self.get_response(request)
         try:
             algorithm = settings.SIMPLE_JWT['ALGORITHM']
             user_data = jwt_decode(token, settings.SECRET_KEY, algorithms=[algorithm])['user']
-        except (InvalidToken, TokenError) as e:
+        except (InvalidToken, TokenError, InvalidSignatureError, ExpiredSignatureError) as e:
             logging.error(e)
             return self.get_response(request)
         else:
             defaults = user_data
             user, user_created = get_user_model().objects.update_or_create(
                 id=user_data['id'],
                 defaults=defaults
```

### Comparing `drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/PKG-INFO` & `drf-simplejwt-additions-1.1.3/drf_simplejwt_additions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-simplejwt-additions
-Version: 1.1.2
+Version: 1.1.3
 Summary: Additions for Django Rest Framework Simple JWT
 Home-page: https://github.com/AllYouZombies/drf-simplejwt-additions
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-simplejwt-additions-1.1.2/setup.cfg` & `drf-simplejwt-additions-1.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-simplejwt-additions
-version = 1.1.2
+version = 1.1.3
 description = Additions for Django Rest Framework Simple JWT
 url = https://github.com/AllYouZombies/drf-simplejwt-additions
 author = Astafeev Rustam
 author_email = rustam@astafeev.dev
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
```

