# Comparing `tmp/BLEST-0.0.4.tar.gz` & `tmp/BLEST-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-0.0.4.tar", last modified: Thu Jun 15 16:05:10 2023, max compression
+gzip compressed data, was "BLEST-0.0.5.tar", last modified: Thu Jun 15 16:12:24 2023, max compression
```

## Comparing `BLEST-0.0.4.tar` & `BLEST-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:05:10.194595 BLEST-0.0.4/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:05:10.193759 BLEST-0.0.4/BLEST.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     3911 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)       29 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.4/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     3911 2023-06-15 16:05:10.194189 BLEST-0.0.4/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3318 2023-06-15 15:01:11.000000 BLEST-0.0.4/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-15 16:05:10.194734 BLEST-0.0.4/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)      941 2023-06-15 15:50:24.000000 BLEST-0.0.4/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:12:24.430933 BLEST-0.0.5/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:12:24.430106 BLEST-0.0.5/BLEST.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     3926 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)       29 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.5/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     3926 2023-06-15 16:12:24.430576 BLEST-0.0.5/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3333 2023-06-15 16:11:07.000000 BLEST-0.0.5/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-15 16:12:24.431021 BLEST-0.0.5/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)      941 2023-06-15 16:11:50.000000 BLEST-0.0.5/setup.py
```

### Comparing `BLEST-0.0.4/BLEST.egg-info/PKG-INFO` & `BLEST-0.0.5/BLEST.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -47,25 +47,25 @@
 ### create_server
 
 ```python
 from blest import create_server
 
 # Create some middleware (optional)
 def auth_middleware(params, context):
-  if params.name:
-    context.user = {
-      'name': params.name
+  if params['name']:
+    context['user'] = {
+      'name': params['name']
     }
   else:
     raise Exception('Unauthorized')
 
 # Create a route controller
 def greet_controller(params, context):
   return {
-    'greeting': f'Hi, {context.user.name}!'
+    'greeting': f"Hi, {context['user']['name']}!"
   }
 
 # Define your router
 router = {
   'greet': [auth_middleware, greet_controller]
 }
```

### Comparing `BLEST-0.0.4/LICENSE` & `BLEST-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.4/PKG-INFO` & `BLEST-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -47,25 +47,25 @@
 ### create_server
 
 ```python
 from blest import create_server
 
 # Create some middleware (optional)
 def auth_middleware(params, context):
-  if params.name:
-    context.user = {
-      'name': params.name
+  if params['name']:
+    context['user'] = {
+      'name': params['name']
     }
   else:
     raise Exception('Unauthorized')
 
 # Create a route controller
 def greet_controller(params, context):
   return {
-    'greeting': f'Hi, {context.user.name}!'
+    'greeting': f"Hi, {context['user']['name']}!"
   }
 
 # Define your router
 router = {
   'greet': [auth_middleware, greet_controller]
 }
```

### Comparing `BLEST-0.0.4/README.md` & `BLEST-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 ### create_server
 
 ```python
 from blest import create_server
 
 # Create some middleware (optional)
 def auth_middleware(params, context):
-  if params.name:
-    context.user = {
-      'name': params.name
+  if params['name']:
+    context['user'] = {
+      'name': params['name']
     }
   else:
     raise Exception('Unauthorized')
 
 # Create a route controller
 def greet_controller(params, context):
   return {
-    'greeting': f'Hi, {context.user.name}!'
+    'greeting': f"Hi, {context['user']['name']}!"
   }
 
 # Define your router
 router = {
   'greet': [auth_middleware, greet_controller]
 }
```

### Comparing `BLEST-0.0.4/setup.py` & `BLEST-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="BLEST",
-    version="0.0.4",
+    version="0.0.5",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/jhuntdev/blest-py",
     packages=find_packages(),
```

