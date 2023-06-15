# Comparing `tmp/django-pam-2.1.1.tar.gz` & `tmp/django-pam-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pam-2.1.1.tar", last modified: Wed Jun 14 23:55:30 2023, max compression
+gzip compressed data, was "django-pam-2.1.2.tar", last modified: Thu Jun 15 02:37:40 2023, max compression
```

## Comparing `django-pam-2.1.1.tar` & `django-pam-2.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1081 2016-08-18 16:38:42.000000 django-pam-2.1.1/LICENSE.txt
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)      137 2016-08-18 16:38:42.000000 django-pam-2.1.1/MANIFEST.in
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-14 23:55:30.121690 django-pam-2.1.1/PKG-INFO
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2032 2023-06-14 23:40:14.000000 django-pam-2.1.1/README.rst
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/__init__.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/accounts/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/accounts/__init__.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2207 2018-12-26 17:37:54.000000 django-pam-2.1.1/django_pam/accounts/forms.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      489 2018-05-03 23:39:16.000000 django-pam-2.1.1/django_pam/accounts/urls.py
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     3818 2022-04-26 22:36:28.000000 django-pam-2.1.1/django_pam/accounts/view_mixins.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     8385 2022-04-26 22:00:49.000000 django-pam-2.1.1/django_pam/accounts/views.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/auth/
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/auth/__init__.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3567 2022-04-26 21:57:12.000000 django-pam-2.1.1/django_pam/auth/backends.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/static/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/static/django_pam/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/static/django_pam/css/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1508 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/css/auth.css
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1039 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/css/modal.css
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/static/django_pam/js/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      564 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/auth.js
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1918 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/inheritance.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3285 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2167 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     4075 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/modal.js
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/templates/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/accounts/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      882 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/_login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      585 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/_logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      171 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      245 2020-05-24 17:47:11.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      570 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/base.html
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/modals/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1261 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/modals/login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      796 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/modals/logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      335 2018-05-05 19:45:44.000000 django-pam-2.1.1/django_pam/urls.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam.egg-info/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/PKG-INFO
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1148 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/SOURCES.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/dependency_links.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       15 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/requires.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       11 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/top_level.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      151 2023-06-14 21:46:21.000000 django-pam-2.1.1/include.mk
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2023-06-14 23:55:30.121690 django-pam-2.1.1/setup.cfg
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     2203 2023-06-14 23:41:16.000000 django-pam-2.1.1/setup.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1081 2016-08-18 16:38:42.000000 django-pam-2.1.2/LICENSE.txt
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)      137 2016-08-18 16:38:42.000000 django-pam-2.1.2/MANIFEST.in
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-15 02:37:40.122449 django-pam-2.1.2/PKG-INFO
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2032 2023-06-14 23:40:14.000000 django-pam-2.1.2/README.rst
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/__init__.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/accounts/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/accounts/__init__.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2207 2018-12-26 17:37:54.000000 django-pam-2.1.2/django_pam/accounts/forms.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      489 2018-05-03 23:39:16.000000 django-pam-2.1.2/django_pam/accounts/urls.py
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     3818 2022-04-26 22:36:28.000000 django-pam-2.1.2/django_pam/accounts/view_mixins.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     8385 2022-04-26 22:00:49.000000 django-pam-2.1.2/django_pam/accounts/views.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/auth/
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/auth/__init__.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3567 2022-04-26 21:57:12.000000 django-pam-2.1.2/django_pam/auth/backends.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.118450 django-pam-2.1.2/django_pam/static/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.118450 django-pam-2.1.2/django_pam/static/django_pam/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/static/django_pam/css/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1508 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/css/auth.css
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1039 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/css/modal.css
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/static/django_pam/js/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      564 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/js/auth.js
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1918 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/js/inheritance.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3285 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/js/js.cookie-2.0.4.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2167 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     4075 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/static/django_pam/js/modal.js
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.118450 django-pam-2.1.2/django_pam/templates/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/templates/django_pam/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/templates/django_pam/accounts/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      882 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/accounts/_login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      585 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/accounts/_logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      171 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/accounts/login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      245 2020-05-24 17:47:11.000000 django-pam-2.1.2/django_pam/templates/django_pam/accounts/logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      570 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/base.html
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam/templates/django_pam/modals/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1261 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/modals/login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      796 2016-08-18 16:38:48.000000 django-pam-2.1.2/django_pam/templates/django_pam/modals/logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      335 2018-05-05 19:45:44.000000 django-pam-2.1.2/django_pam/urls.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-15 02:37:40.122449 django-pam-2.1.2/django_pam.egg-info/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-15 02:37:40.000000 django-pam-2.1.2/django_pam.egg-info/PKG-INFO
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1148 2023-06-15 02:37:40.000000 django-pam-2.1.2/django_pam.egg-info/SOURCES.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2023-06-15 02:37:40.000000 django-pam-2.1.2/django_pam.egg-info/dependency_links.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       15 2023-06-15 02:37:40.000000 django-pam-2.1.2/django_pam.egg-info/requires.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       11 2023-06-15 02:37:40.000000 django-pam-2.1.2/django_pam.egg-info/top_level.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      151 2023-06-15 02:35:24.000000 django-pam-2.1.2/include.mk
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2023-06-15 02:37:40.122449 django-pam-2.1.2/setup.cfg
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     2203 2023-06-14 23:41:16.000000 django-pam-2.1.2/setup.py
```

### Comparing `django-pam-2.1.1/LICENSE.txt` & `django-pam-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/PKG-INFO` & `django-pam-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pam
-Version: 2.1.1
+Version: 2.1.2
 Summary: Django PAM authentication backend implementation.
 Home-page: https://github.com/cnobile2012/django-pam
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
 Description: ==========
         Django PAM
```

### Comparing `django-pam-2.1.1/README.rst` & `django-pam-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/accounts/forms.py` & `django-pam-2.1.2/django_pam/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/accounts/view_mixins.py` & `django-pam-2.1.2/django_pam/accounts/view_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/accounts/views.py` & `django-pam-2.1.2/django_pam/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/auth/backends.py` & `django-pam-2.1.2/django_pam/auth/backends.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/css/auth.css` & `django-pam-2.1.2/django_pam/static/django_pam/css/auth.css`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/css/modal.css` & `django-pam-2.1.2/django_pam/static/django_pam/css/modal.css`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/js/auth.js` & `django-pam-2.1.2/django_pam/static/django_pam/js/auth.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/js/inheritance.js` & `django-pam-2.1.2/django_pam/static/django_pam/js/inheritance.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.js` & `django-pam-2.1.2/django_pam/static/django_pam/js/js.cookie-2.0.4.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js` & `django-pam-2.1.2/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/static/django_pam/js/modal.js` & `django-pam-2.1.2/django_pam/static/django_pam/js/modal.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/templates/django_pam/accounts/_login.html` & `django-pam-2.1.2/django_pam/templates/django_pam/accounts/_login.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/templates/django_pam/accounts/_logout.html` & `django-pam-2.1.2/django_pam/templates/django_pam/accounts/_logout.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/templates/django_pam/base.html` & `django-pam-2.1.2/django_pam/templates/django_pam/base.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/templates/django_pam/modals/login.html` & `django-pam-2.1.2/django_pam/templates/django_pam/modals/login.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam/templates/django_pam/modals/logout.html` & `django-pam-2.1.2/django_pam/templates/django_pam/modals/logout.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/django_pam.egg-info/PKG-INFO` & `django-pam-2.1.2/django_pam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pam
-Version: 2.1.1
+Version: 2.1.2
 Summary: Django PAM authentication backend implementation.
 Home-page: https://github.com/cnobile2012/django-pam
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
 Description: ==========
         Django PAM
```

### Comparing `django-pam-2.1.1/django_pam.egg-info/SOURCES.txt` & `django-pam-2.1.2/django_pam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.1/setup.py` & `django-pam-2.1.2/setup.py`

 * *Files identical despite different names*

