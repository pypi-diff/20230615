# Comparing `tmp/django-heartbeat-2.1.0.tar.gz` & `tmp/django-heartbeat-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-heartbeat-2.1.0.tar", last modified: Tue Oct  4 11:35:29 2022, max compression
+gzip compressed data, was "django-heartbeat-2.2.0.tar", last modified: Thu Jun 15 12:52:01 2023, max compression
```

## Comparing `django-heartbeat-2.1.0.tar` & `django-heartbeat-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 andrei.popescu (864884434) 1138207179        0 2022-10-04 11:35:29.398556 django-heartbeat-2.1.0/
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     1100 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/LICENSE
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      446 2022-10-04 11:35:29.397973 django-heartbeat-2.1.0/PKG-INFO
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     4034 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/README.md
--rw-r--r--   0 andrei.popescu (864884434) 1138207179       38 2022-10-04 11:35:29.398741 django-heartbeat-2.1.0/setup.cfg
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     1080 2022-10-04 09:06:48.000000 django-heartbeat-2.1.0/setup.py
-drwxr-xr-x   0 andrei.popescu (864884434) 1138207179        0 2022-10-04 11:35:29.374106 django-heartbeat-2.1.0/src/
-drwxr-xr-x   0 andrei.popescu (864884434) 1138207179        0 2022-10-04 11:35:29.381768 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      446 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/PKG-INFO
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      737 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/SOURCES.txt
--rw-r--r--   0 andrei.popescu (864884434) 1138207179        1 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/dependency_links.txt
--rw-r--r--   0 andrei.popescu (864884434) 1138207179        1 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/not-zip-safe
--rw-r--r--   0 andrei.popescu (864884434) 1138207179       19 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/requires.txt
--rw-r--r--   0 andrei.popescu (864884434) 1138207179       10 2022-10-04 11:35:29.000000 django-heartbeat-2.1.0/src/django_heartbeat.egg-info/top_level.txt
-drwxr-xr-x   0 andrei.popescu (864884434) 1138207179        0 2022-10-04 11:35:29.386647 django-heartbeat-2.1.0/src/heartbeat/
--rw-r--r--   0 andrei.popescu (864884434) 1138207179        0 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/__init__.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     3550 2022-10-04 09:06:48.000000 django-heartbeat-2.1.0/src/heartbeat/auth.py
-drwxr-xr-x   0 andrei.popescu (864884434) 1138207179        0 2022-10-04 11:35:29.396786 django-heartbeat-2.1.0/src/heartbeat/checkers/
--rw-r--r--   0 andrei.popescu (864884434) 1138207179        0 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/__init__.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      651 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/build.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     1872 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/databases.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179       81 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/debug_mode.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      196 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/distribution_list.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     1243 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/host.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179     2063 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/memcached_status.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      377 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/python.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      777 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/checkers/redis_status.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      791 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/settings.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      225 2022-10-04 09:06:48.000000 django-heartbeat-2.1.0/src/heartbeat/urls.py
--rw-r--r--   0 andrei.popescu (864884434) 1138207179      672 2022-09-20 14:03:55.000000 django-heartbeat-2.1.0/src/heartbeat/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:01.662672 django-heartbeat-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-15 12:52:01.662672 django-heartbeat-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:52:01.662672 django-heartbeat-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:01.658672 django-heartbeat-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:01.658672 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 12:52:01.000000 django-heartbeat-2.2.0/src/django_heartbeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:01.658672 django-heartbeat-2.2.0/src/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:52:01.662672 django-heartbeat-2.2.0/src/heartbeat/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/distribution_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/memcached_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/checkers/redis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 12:51:47.000000 django-heartbeat-2.2.0/src/heartbeat/views.py
```

### Comparing `django-heartbeat-2.1.0/LICENSE` & `django-heartbeat-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/README.md` & `django-heartbeat-2.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,141 @@
-# django-heartbeat  [![Build Status](https://travis-ci.org/pbs/django-heartbeat.svg?branch=master)](https://travis-ci.org/pbs/django-heartbeat) [![PyPI version](https://badge.fury.io/py/django-heartbeat.svg)](https://badge.fury.io/py/django-heartbeat)
-
 Django-heartbeat is a simple reusable app that checks and lists various information
 about your project and its dependencies
 
 # Requirements
 
-* Python >=2.7 (tested with Python 2.7, 3.5, 3.7, 3.8)
-* Django >=1.6 ( tested with >1.8 )
+* Python >=3.8 (tested with Python 3.8, 3.10)
+* Django >=3.2.19<=4.0
 
 # Installation
 
 Install using pip:
+
 ```
 pip install django-heartbeat
 ```
 
 Next, add 'heartbeat' to your settings.py INSTALLED_APPS:
+
 ```
 INSTALLED_APPS = (
   ...
   'heartbeat',
 )
 ```
 
 Configure urls.py
 
 ```Python
 if 'heartbeat' in settings.INSTALLED_APPS:
-  from heartbeat.urls import urlpatterns as heartbeat_urls
+    from heartbeat.urls import urlpatterns as heartbeat_urls
 
-  urlpatterns += [
-    url(r'^heartbeat/', include(heartbeat_urls))
-  ]
+    urlpatterns += [
+        url(r'^heartbeat/', include(heartbeat_urls))
+    ]
 ```
 
 # Usage
+
 - `/heartbeat/`
 
   After this point you can access the /heartbeat/ endpoint and receive a 200 OK.
 
 
 - `/heartbeat/1337/`
 
   If you want a more detailed view of some custom checkers you MUST configure a
-custom profile for heartbeat in your settings.py. The profile should be
-a dictionary containing at least the basic auth credentials or the key `disable`
-set to `True` to disable basic authentication.
+  custom profile for heartbeat in your settings.py. The profile should be
+  a dictionary containing at least the basic auth credentials or the key `disable`
+  set to `True` to disable basic authentication.
 
 e.g.:
 
   ```Python
   HEARTBEAT = {
-      'package_name': 'foo_project',
-      'checkers': [
-          'heartbeat.checkers.build',
-          'heartbeat.checkers.distribution_list',
-          'heartbeat.checkers.debug_mode',
-      ],
-      'auth': {
-          'username': 'foo',
-          'password': 'bar',
-      },
-  }
+    'package_name': 'foo_project',
+    'checkers': [
+        'heartbeat.checkers.build',
+        'heartbeat.checkers.distribution_list',
+        'heartbeat.checkers.debug_mode',
+    ],
+    'auth': {
+        'username': 'foo',
+        'password': 'bar',
+    },
+}
   ```
 
 If no checkers are defined, heartbeat will default to the following:
+
 - `heartbeat.checkers.distribution_list`
 - `heartbeat.checkers.debug_mode`
 - `heartbeat.checkers.python`
 
-
 # Available checkers
 
-Please make sure you have the latest version of django-heartbeat since checker names changed in versions 1.0.8 and 2.0.0.
-If for some reason you cannot install the latest version, read the release notes for the version you have and the versions mentioned above.
+Please make sure you have the latest version of django-heartbeat since checker names changed in versions 1.0.8 and
+2.0.0.
+If for some reason you cannot install the latest version, read the release notes for the version you have and the
+versions mentioned above.
 
 `heartbeat.checkers.build`
-  - lists information about installed package
-  - Please be aware that in order for this checker to work you have to add the
+
+- lists information about installed package
+- Please be aware that in order for this checker to work you have to add the
   'package_name': 'foo_package' key, value pair in the HEARTBEAT settings
 
 `heartbeat.checkers.databases`
-  - displays information about the connection with your configured databases
+
+- displays information about the connection with your configured databases
 
 `heartbeat.checkers.debug_mode`
-  - displays whether the DEBUG mode is set to True or False
+
+- displays whether the DEBUG mode is set to True or False
 
 `heartbeat.checkers.distribution_list`
-  - lists all installed dependencies
-  
+
+- lists all installed dependencies
+
 `heartbeat.checkers.host`
-  - displays various information about your system
+
+- displays various information about your system
   (e.g. hostname, number of CPUs, uptime, used/free memory, etc.)
 
 `heartbeat.checkers.memcached_status`
-  - displays stats about your Memcached.
-  - Before enabling this checker please make sure that you have installed the appropriate Memcached binding (the two most common are [python-memcached](https://pypi.python.org/pypi/python-memcached) and [pylibmc](https://pypi.python.org/pypi/pylibmc))
 
-`heartbeat.checkers.python`
-  - lists the current python version
+- displays stats about your Memcached.
+- Before enabling this checker please make sure that you have installed the appropriate Memcached binding (the two most
+  common are [python-memcached](https://pypi.python.org/pypi/python-memcached)
+  and [pylibmc](https://pypi.python.org/pypi/pylibmc))
 
-`heartbeat.checkers.redis_status`
-  - checks your connection with the Redis server
-  - Make sure that you have CACHEOPS_REDIS configured properly in your settings.py
+`heartbeat.checkers.python`
 
+- lists the current python version
 
+`heartbeat.checkers.redis_status`
 
+- checks your connection with the Redis server
+- Make sure that you have CACHEOPS_REDIS configured properly in your settings.py
 
 # Implementing your own checker
+
 - my_checker.py:
   ```Python
   def check(request):
     """
     :param request: HttpRequest object
     :return: dict
     """
 
     # Checker logic goes here
 
     return {'ping': 'pong'}
   ```
+
 Note: The function name of your checker MUST be 'check' and has to return a JSON-serializable object
 
 - add it to the settings.HEARTBEAT config
   ```Python
   HEARTBEAT = {
       'checkers': [
           'heartbeat.checkers.distribution_list',
@@ -136,11 +148,11 @@
   ```
 
 Simple, huh?
 
 If you would like to contribute to this library with a new checker(or any other
 functionality), feel free to make a pull request.
 
-
 # Contributors
+
 - Andrei Prădan
 - Dan Claudiu Pop
```

### Comparing `django-heartbeat-2.1.0/src/django_heartbeat.egg-info/SOURCES.txt` & `django-heartbeat-2.2.0/src/django_heartbeat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 src/django_heartbeat.egg-info/PKG-INFO
 src/django_heartbeat.egg-info/SOURCES.txt
 src/django_heartbeat.egg-info/dependency_links.txt
 src/django_heartbeat.egg-info/not-zip-safe
 src/django_heartbeat.egg-info/requires.txt
 src/django_heartbeat.egg-info/top_level.txt
 src/heartbeat/__init__.py
```

### Comparing `django-heartbeat-2.1.0/src/heartbeat/auth.py` & `django-heartbeat-2.2.0/src/heartbeat/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                         password == HEARTBEAT['auth']['password']):
                     return func(request, *args, **kwargs)
 
         response = HttpResponse(
             "Authentication failed", status=401)
         response['WWW-Authenticate'] = 'Basic realm="Welcome to 1337"'
         return response
+
     return _decorator
 
 
 def get_auth():
     auth = HEARTBEAT.get('auth')
     if not auth:
         raise ImproperlyConfigured('Missing auth configuration for heartbeat')
@@ -63,24 +64,24 @@
 
 
 def get_client_ip(request):
     access_route = get_access_route(request)
 
     if len(access_route) == 1:
         return access_route[0]
-    expression = """
+    expression = r"""
         (^(?!(?:[0-9]{1,3}\.){3}[0-9]{1,3}$).*$)|  # will match non valid ipV4
         (^127\.0\.0\.1)|  # will match 127.0.0.1
         (^10\.)|  # will match 10.0.0.0 - 10.255.255.255 IP-s
         (^172\.1[6-9]\.)|  # will match 172.16.0.0 - 172.19.255.255 IP-s
         (^172\.2[0-9]\.)|  # will match 172.20.0.0 - 172.29.255.255 IP-s
         (^172\.3[0-1]\.)|  # will match 172.30.0.0 - 172.31.255.255 IP-s
         (^192\.168\.)  # will match 192.168.0.0 - 192.168.255.255 IP-s
     """
-    regex = re.compile(repr(expression), re.X)
+    regex = re.compile(expression, re.X)
     for ip in access_route:
         if not ip:
             # it's possible that the first value from X_FORWARDED_FOR
             # will be null, so we need to pass that value
             continue
         if regex.search(ip):
             continue
```

### Comparing `django-heartbeat-2.1.0/src/heartbeat/checkers/build.py` & `django-heartbeat-2.2.0/src/heartbeat/checkers/build.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/checkers/databases.py` & `django-heartbeat-2.2.0/src/heartbeat/checkers/databases.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/checkers/host.py` & `django-heartbeat-2.2.0/src/heartbeat/checkers/host.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/checkers/memcached_status.py` & `django-heartbeat-2.2.0/src/heartbeat/checkers/memcached_status.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/checkers/redis_status.py` & `django-heartbeat-2.2.0/src/heartbeat/checkers/redis_status.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/settings.py` & `django-heartbeat-2.2.0/src/heartbeat/settings.py`

 * *Files identical despite different names*

### Comparing `django-heartbeat-2.1.0/src/heartbeat/views.py` & `django-heartbeat-2.2.0/src/heartbeat/views.py`

 * *Files identical despite different names*

