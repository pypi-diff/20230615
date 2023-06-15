# Comparing `tmp/django-pam-2.1.0.tar.gz` & `tmp/django-pam-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pam-2.1.0.tar", last modified: Tue Apr 26 23:00:29 2022, max compression
+gzip compressed data, was "django-pam-2.1.1.tar", last modified: Wed Jun 14 23:55:30 2023, max compression
```

## Comparing `django-pam-2.1.0.tar` & `django-pam-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1081 2016-08-18 16:38:42.000000 django-pam-2.1.0/LICENSE.txt
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)      137 2016-08-18 16:38:42.000000 django-pam-2.1.0/MANIFEST.in
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3147 2022-04-26 23:00:28.997279 django-pam-2.1.0/PKG-INFO
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2029 2022-04-26 22:51:32.000000 django-pam-2.1.0/README.rst
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/__init__.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/accounts/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/accounts/__init__.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2207 2018-12-26 17:37:54.000000 django-pam-2.1.0/django_pam/accounts/forms.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      489 2018-05-03 23:39:16.000000 django-pam-2.1.0/django_pam/accounts/urls.py
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     3818 2022-04-26 22:36:28.000000 django-pam-2.1.0/django_pam/accounts/view_mixins.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     8385 2022-04-26 22:00:49.000000 django-pam-2.1.0/django_pam/accounts/views.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/auth/
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/auth/__init__.py
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3567 2022-04-26 21:57:12.000000 django-pam-2.1.0/django_pam/auth/backends.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.993278 django-pam-2.1.0/django_pam/static/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.993278 django-pam-2.1.0/django_pam/static/django_pam/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/static/django_pam/css/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1508 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/css/auth.css
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1039 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/css/modal.css
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/static/django_pam/js/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      564 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/js/auth.js
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1918 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/js/inheritance.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3285 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/js/js.cookie-2.0.4.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2167 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     4075 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/static/django_pam/js/modal.js
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.993278 django-pam-2.1.0/django_pam/templates/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/templates/django_pam/
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/templates/django_pam/accounts/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      882 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/accounts/_login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      585 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/accounts/_logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      171 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/accounts/login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      245 2020-05-24 17:47:11.000000 django-pam-2.1.0/django_pam/templates/django_pam/accounts/logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      570 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/base.html
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam/templates/django_pam/modals/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1261 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/modals/login.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      796 2016-08-18 16:38:48.000000 django-pam-2.1.0/django_pam/templates/django_pam/modals/logout.html
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      335 2018-05-05 19:45:44.000000 django-pam-2.1.0/django_pam/urls.py
-drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2022-04-26 23:00:28.997279 django-pam-2.1.0/django_pam.egg-info/
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3147 2022-04-26 23:00:28.000000 django-pam-2.1.0/django_pam.egg-info/PKG-INFO
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1148 2022-04-26 23:00:28.000000 django-pam-2.1.0/django_pam.egg-info/SOURCES.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2022-04-26 23:00:28.000000 django-pam-2.1.0/django_pam.egg-info/dependency_links.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       15 2022-04-26 23:00:28.000000 django-pam-2.1.0/django_pam.egg-info/requires.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       11 2022-04-26 23:00:28.000000 django-pam-2.1.0/django_pam.egg-info/top_level.txt
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      151 2022-04-26 22:22:08.000000 django-pam-2.1.0/include.mk
--rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2022-04-26 23:00:28.997279 django-pam-2.1.0/setup.cfg
--rw-r--r--   0 cnobile   (1000) cnobile   (1000)     2150 2022-04-26 22:31:17.000000 django-pam-2.1.0/setup.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1081 2016-08-18 16:38:42.000000 django-pam-2.1.1/LICENSE.txt
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)      137 2016-08-18 16:38:42.000000 django-pam-2.1.1/MANIFEST.in
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-14 23:55:30.121690 django-pam-2.1.1/PKG-INFO
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2032 2023-06-14 23:40:14.000000 django-pam-2.1.1/README.rst
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/__init__.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/accounts/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/accounts/__init__.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2207 2018-12-26 17:37:54.000000 django-pam-2.1.1/django_pam/accounts/forms.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      489 2018-05-03 23:39:16.000000 django-pam-2.1.1/django_pam/accounts/urls.py
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     3818 2022-04-26 22:36:28.000000 django-pam-2.1.1/django_pam/accounts/view_mixins.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     8385 2022-04-26 22:00:49.000000 django-pam-2.1.1/django_pam/accounts/views.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/auth/
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)        0 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/auth/__init__.py
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3567 2022-04-26 21:57:12.000000 django-pam-2.1.1/django_pam/auth/backends.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/static/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/static/django_pam/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/static/django_pam/css/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1508 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/css/auth.css
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1039 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/css/modal.css
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/static/django_pam/js/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      564 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/auth.js
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     1918 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/inheritance.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3285 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     2167 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     4075 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/static/django_pam/js/modal.js
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam/templates/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/accounts/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      882 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/_login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      585 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/_logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      171 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      245 2020-05-24 17:47:11.000000 django-pam-2.1.1/django_pam/templates/django_pam/accounts/logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      570 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/base.html
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.121690 django-pam-2.1.1/django_pam/templates/django_pam/modals/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1261 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/modals/login.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      796 2016-08-18 16:38:48.000000 django-pam-2.1.1/django_pam/templates/django_pam/modals/logout.html
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      335 2018-05-05 19:45:44.000000 django-pam-2.1.1/django_pam/urls.py
+drwxrwxr-x   0 cnobile   (1000) cnobile   (1000)        0 2023-06-14 23:55:30.117690 django-pam-2.1.1/django_pam.egg-info/
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     3795 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/PKG-INFO
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)     1148 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/SOURCES.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)        1 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/dependency_links.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       15 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/requires.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       11 2023-06-14 23:55:30.000000 django-pam-2.1.1/django_pam.egg-info/top_level.txt
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)      151 2023-06-14 21:46:21.000000 django-pam-2.1.1/include.mk
+-rw-rw-r--   0 cnobile   (1000) cnobile   (1000)       38 2023-06-14 23:55:30.121690 django-pam-2.1.1/setup.cfg
+-rw-r--r--   0 cnobile   (1000) cnobile   (1000)     2203 2023-06-14 23:41:16.000000 django-pam-2.1.1/setup.py
```

### Comparing `django-pam-2.1.0/LICENSE.txt` & `django-pam-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/PKG-INFO` & `django-pam-2.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,105 @@
 Metadata-Version: 2.1
 Name: django-pam
-Version: 2.1.0
+Version: 2.1.1
 Summary: Django PAM authentication backend implementation.
 Home-page: https://github.com/cnobile2012/django-pam
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
+Description: ==========
+        Django PAM
+        ==========
+        
+        .. image:: http://img.shields.io/pypi/v/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: PyPI Version
+        
+        .. image:: http://img.shields.io/pypi/wheel/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: PyPI Wheel
+        
+        .. image:: http://img.shields.io/pypi/pyversions/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: Python Versions
+        
+        .. image:: http://img.shields.io/pypi/l/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: License
+        
+        A Django PAM authentication backend implementation.
+        
+        The MIT License (MIT)
+        
+        Overview
+        --------
+        
+        This is a simple authentication backend that uses the
+        `python-pam <https://github.com/FirefighterBlu3/python-pam>`_
+        package. Django PAM can be used in an SSO (Single Sign On) environment
+        or just with a single box where you want to log into a Django app with
+        your UNIX login.
+        
+        Updated for Django 4.2.x and Python 3.11.
+        
+        Python 2.x has been depricated. If you need a version of Django PAM use
+        version 2.0.1.
+        
+        Provides
+        --------
+        
+        1. PAM Authentication Backend
+        
+        2. Login and Logout Views
+        
+        3. Templates for both standard and modal authentication.
+        
+        4. Supporting JavaScript and CSS.
+        
+        Quick Start
+        -----------
+        
+        You will need to add Django PAM to your ``INSTALLED_APPS``::
+        
+          INSTALLED_APPS = [
+              ...
+              'django_pam',
+          ]
+        
+        Next you will need to add the Django PAM backend to the ``AUTHENTICATION_BACKENDS``::
+        
+          AUTHENTICATION_BACKENDS = [
+              'django_pam.auth.backends.PAMBackend',
+              'django.contrib.auth.backends.ModelBackend',
+          ]
+        
+        The user that runs the application needs to be a member of the
+        ``/etc/shadow`` file group, this is usually the web server user. This
+        is necessary so the web server can authenticate other users. To do
+        this run the command below with the proper user::
+        
+          $ sudo usermod -a -G shadow <user>
+        
+        Complete Documentation can be found on
+        `Read the Docs <https://readthedocs.org/>`_ at:
+        `Django PAM <http://django-pam.readthedocs.io/en/latest/>`_
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-==========
-Django PAM
-==========
-
-.. image:: http://img.shields.io/pypi/v/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: PyPI Version
-
-.. image:: http://img.shields.io/pypi/wheel/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: PyPI Wheel
-
-.. image:: http://img.shields.io/pypi/pyversions/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: Python Versions
-
-.. image:: http://img.shields.io/pypi/l/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: License
-
-A Django PAM authentication backend implementation.
-
-The MIT License (MIT)
-
-Overview
---------
-
-This is a simple authentication backend that uses the
-`python-pam <https://github.com/FirefighterBlu3/python-pam>`_
-package. Django PAM can be used in an SSO (Single Sign On) environment
-or just with a single box where you want to log into a Django app with
-your UNIX login.
-
-Updated for Django 4.x and Python 3.9.
-
-Python 2.x has been depricated. If you need a version of Django PAM use
-version 2.0.1.
-
-Provides
---------
-
-1. PAM Authentication Backend
-
-2. Login and Logout Views
-
-3. Templates for both standard and modal authentication.
-
-4. Supporting JavaScript and CSS.
-
-Quick Start
------------
-
-You will need to add Django PAM to your ``INSTALLED_APPS``::
-
-  INSTALLED_APPS = [
-      ...
-      'django_pam',
-  ]
-
-Next you will need to add the Django PAM backend to the ``AUTHENTICATION_BACKENDS``::
-
-  AUTHENTICATION_BACKENDS = [
-      'django_pam.auth.backends.PAMBackend',
-      'django.contrib.auth.backends.ModelBackend',
-  ]
-
-The user that runs the application needs to be a member of the
-``/etc/shadow`` file group, this is usually the web server user. This
-is necessary so the web server can authenticate other users. To do
-this run the command below with the proper user::
-
-  $ sudo usermod -a -G shadow <user>
-
-Complete Documentation can be found on
-`Read the Docs <https://readthedocs.org/>`_ at:
-`Django PAM <http://django-pam.readthedocs.io/en/latest/>`_
-
-
```

### Comparing `django-pam-2.1.0/README.rst` & `django-pam-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 This is a simple authentication backend that uses the
 `python-pam <https://github.com/FirefighterBlu3/python-pam>`_
 package. Django PAM can be used in an SSO (Single Sign On) environment
 or just with a single box where you want to log into a Django app with
 your UNIX login.
 
-Updated for Django 4.x and Python 3.9.
+Updated for Django 4.2.x and Python 3.11.
 
 Python 2.x has been depricated. If you need a version of Django PAM use
 version 2.0.1.
 
 Provides
 --------
```

### Comparing `django-pam-2.1.0/django_pam/accounts/forms.py` & `django-pam-2.1.1/django_pam/accounts/forms.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/accounts/view_mixins.py` & `django-pam-2.1.1/django_pam/accounts/view_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/accounts/views.py` & `django-pam-2.1.1/django_pam/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/auth/backends.py` & `django-pam-2.1.1/django_pam/auth/backends.py`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/css/auth.css` & `django-pam-2.1.1/django_pam/static/django_pam/css/auth.css`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/css/modal.css` & `django-pam-2.1.1/django_pam/static/django_pam/css/modal.css`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/js/auth.js` & `django-pam-2.1.1/django_pam/static/django_pam/js/auth.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/js/inheritance.js` & `django-pam-2.1.1/django_pam/static/django_pam/js/inheritance.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/js/js.cookie-2.0.4.js` & `django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js` & `django-pam-2.1.1/django_pam/static/django_pam/js/js.cookie-2.0.4.min.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/static/django_pam/js/modal.js` & `django-pam-2.1.1/django_pam/static/django_pam/js/modal.js`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/templates/django_pam/accounts/_login.html` & `django-pam-2.1.1/django_pam/templates/django_pam/accounts/_login.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/templates/django_pam/accounts/_logout.html` & `django-pam-2.1.1/django_pam/templates/django_pam/accounts/_logout.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/templates/django_pam/base.html` & `django-pam-2.1.1/django_pam/templates/django_pam/base.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/templates/django_pam/modals/login.html` & `django-pam-2.1.1/django_pam/templates/django_pam/modals/login.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam/templates/django_pam/modals/logout.html` & `django-pam-2.1.1/django_pam/templates/django_pam/modals/logout.html`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/django_pam.egg-info/PKG-INFO` & `django-pam-2.1.1/django_pam.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,105 @@
 Metadata-Version: 2.1
 Name: django-pam
-Version: 2.1.0
+Version: 2.1.1
 Summary: Django PAM authentication backend implementation.
 Home-page: https://github.com/cnobile2012/django-pam
 Author: Carl J. Nobile
 Author-email: carl.nobile@gmail.com
 License: MIT
+Description: ==========
+        Django PAM
+        ==========
+        
+        .. image:: http://img.shields.io/pypi/v/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: PyPI Version
+        
+        .. image:: http://img.shields.io/pypi/wheel/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: PyPI Wheel
+        
+        .. image:: http://img.shields.io/pypi/pyversions/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: Python Versions
+        
+        .. image:: http://img.shields.io/pypi/l/django-pam.svg
+           :target: https://pypi.python.org/pypi/django-pam
+           :alt: License
+        
+        A Django PAM authentication backend implementation.
+        
+        The MIT License (MIT)
+        
+        Overview
+        --------
+        
+        This is a simple authentication backend that uses the
+        `python-pam <https://github.com/FirefighterBlu3/python-pam>`_
+        package. Django PAM can be used in an SSO (Single Sign On) environment
+        or just with a single box where you want to log into a Django app with
+        your UNIX login.
+        
+        Updated for Django 4.2.x and Python 3.11.
+        
+        Python 2.x has been depricated. If you need a version of Django PAM use
+        version 2.0.1.
+        
+        Provides
+        --------
+        
+        1. PAM Authentication Backend
+        
+        2. Login and Logout Views
+        
+        3. Templates for both standard and modal authentication.
+        
+        4. Supporting JavaScript and CSS.
+        
+        Quick Start
+        -----------
+        
+        You will need to add Django PAM to your ``INSTALLED_APPS``::
+        
+          INSTALLED_APPS = [
+              ...
+              'django_pam',
+          ]
+        
+        Next you will need to add the Django PAM backend to the ``AUTHENTICATION_BACKENDS``::
+        
+          AUTHENTICATION_BACKENDS = [
+              'django_pam.auth.backends.PAMBackend',
+              'django.contrib.auth.backends.ModelBackend',
+          ]
+        
+        The user that runs the application needs to be a member of the
+        ``/etc/shadow`` file group, this is usually the web server user. This
+        is necessary so the web server can authenticate other users. To do
+        this run the command below with the proper user::
+        
+          $ sudo usermod -a -G shadow <user>
+        
+        Complete Documentation can be found on
+        `Read the Docs <https://readthedocs.org/>`_ at:
+        `Django PAM <http://django-pam.readthedocs.io/en/latest/>`_
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-==========
-Django PAM
-==========
-
-.. image:: http://img.shields.io/pypi/v/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: PyPI Version
-
-.. image:: http://img.shields.io/pypi/wheel/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: PyPI Wheel
-
-.. image:: http://img.shields.io/pypi/pyversions/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: Python Versions
-
-.. image:: http://img.shields.io/pypi/l/django-pam.svg
-   :target: https://pypi.python.org/pypi/django-pam
-   :alt: License
-
-A Django PAM authentication backend implementation.
-
-The MIT License (MIT)
-
-Overview
---------
-
-This is a simple authentication backend that uses the
-`python-pam <https://github.com/FirefighterBlu3/python-pam>`_
-package. Django PAM can be used in an SSO (Single Sign On) environment
-or just with a single box where you want to log into a Django app with
-your UNIX login.
-
-Updated for Django 4.x and Python 3.9.
-
-Python 2.x has been depricated. If you need a version of Django PAM use
-version 2.0.1.
-
-Provides
---------
-
-1. PAM Authentication Backend
-
-2. Login and Logout Views
-
-3. Templates for both standard and modal authentication.
-
-4. Supporting JavaScript and CSS.
-
-Quick Start
------------
-
-You will need to add Django PAM to your ``INSTALLED_APPS``::
-
-  INSTALLED_APPS = [
-      ...
-      'django_pam',
-  ]
-
-Next you will need to add the Django PAM backend to the ``AUTHENTICATION_BACKENDS``::
-
-  AUTHENTICATION_BACKENDS = [
-      'django_pam.auth.backends.PAMBackend',
-      'django.contrib.auth.backends.ModelBackend',
-  ]
-
-The user that runs the application needs to be a member of the
-``/etc/shadow`` file group, this is usually the web server user. This
-is necessary so the web server can authenticate other users. To do
-this run the command below with the proper user::
-
-  $ sudo usermod -a -G shadow <user>
-
-Complete Documentation can be found on
-`Read the Docs <https://readthedocs.org/>`_ at:
-`Django PAM <http://django-pam.readthedocs.io/en/latest/>`_
-
-
```

### Comparing `django-pam-2.1.0/django_pam.egg-info/SOURCES.txt` & `django-pam-2.1.1/django_pam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pam-2.1.0/setup.py` & `django-pam-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from setuptools import setup
 
 # Allow setup.py to be run from any path.
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 def version():
-    regex = r'^(?m){}[\s]*=[\s]*(?P<ver>\d*)$'
+    regex = r'(?m)(^{}[\s]*=[\s]*(?P<ver>\d*)$)'
 
     with open(os.path.join(os.path.dirname(__file__), 'include.mk')) as f:
         ver = f.read()
 
     major = re.search(regex.format('MAJORVERSION'), ver).group('ver')
     minor = re.search(regex.format('MINORVERSION'), ver).group('ver')
     patch = re.search(regex.format('PATCHLEVEL'), ver).group('ver')
@@ -33,25 +33,26 @@
     url='https://github.com/cnobile2012/django-pam',
     author='Carl J. Nobile',
     author_email='carl.nobile@gmail.com',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.0',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Build Tools',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         ],
     install_requires=[
         'python-pam',
         'six',
```

