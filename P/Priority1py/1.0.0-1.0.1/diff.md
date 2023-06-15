# Comparing `tmp/Priority1py-1.0.0.tar.gz` & `tmp/Priority1py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Priority1py-1.0.0.tar", last modified: Thu Jun 15 02:50:07 2023, max compression
+gzip compressed data, was "dist\Priority1py-1.0.1.tar", last modified: Thu Jun 15 02:53:40 2023, max compression
```

## Comparing `Priority1py-1.0.0.tar` & `Priority1py-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:50:07.000000 Priority1py-1.0.0/
--rw-rw-rw-   0        0        0      769 2023-06-15 02:50:07.000000 Priority1py-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 02:50:07.000000 Priority1py-1.0.0/Priority1py/
--rw-rw-rw-   0        0        0     2334 2023-06-15 02:46:50.000000 Priority1py-1.0.0/Priority1py/Priority1py.py
--rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-1.0.0/Priority1py/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-06-15 02:44:19.000000 Priority1py-1.0.0/Priority1py/request.py
--rw-rw-rw-   0        0        0      797 2023-06-15 02:12:42.000000 Priority1py-1.0.0/Priority1py/strings.py
--rw-rw-rw-   0        0        0      241 2023-06-15 02:14:29.000000 Priority1py-1.0.0/Priority1py/test.py
--rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1646 2023-06-15 02:49:40.000000 Priority1py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:53:40.000000 Priority1py-1.0.1/
+-rw-rw-rw-   0        0        0      769 2023-06-15 02:53:40.000000 Priority1py-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 02:53:40.000000 Priority1py-1.0.1/Priority1py/
+-rw-rw-rw-   0        0        0     2309 2023-06-15 02:52:27.000000 Priority1py-1.0.1/Priority1py/Priority1py.py
+-rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-1.0.1/Priority1py/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-06-15 02:44:19.000000 Priority1py-1.0.1/Priority1py/request.py
+-rw-rw-rw-   0        0        0      797 2023-06-15 02:12:42.000000 Priority1py-1.0.1/Priority1py/strings.py
+-rw-rw-rw-   0        0        0      241 2023-06-15 02:14:29.000000 Priority1py-1.0.1/Priority1py/test.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-06-15 02:53:33.000000 Priority1py-1.0.1/setup.py
```

### Comparing `Priority1py-1.0.0/PKG-INFO` & `Priority1py-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Priority1py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Priority 1 web API python library
 Home-page: https://github.com/reid10305/Priority1py
 Author: Daniel Pifer
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.1.tar.gz
 Description: UNKNOWN
 Keywords: API,Priority1
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Priority1py-1.0.0/Priority1py/Priority1py.py` & `Priority1py-1.0.1/Priority1py/Priority1py.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
             'identifierType' : identifiertype,
             'identifierValue' : identifier
         }
 
         # send request and convert to json 
         res_str = self.req.send_req(endpoint=Endpoint.LTL_SHIPMENT_STATUS, payload=payload, request=Crud.POST)
         res_json = json.loads(res_str)
-        print(res_json)
 
         # test for no shipments found
         if 'No shipments found' in res_json:
             raise Exception('No shipments found matching that ID')
 
         # parse json for status list
         try:
```

### Comparing `Priority1py-1.0.0/Priority1py/request.py` & `Priority1py-1.0.1/Priority1py/request.py`

 * *Files identical despite different names*

### Comparing `Priority1py-1.0.0/Priority1py/strings.py` & `Priority1py-1.0.1/Priority1py/strings.py`

 * *Files identical despite different names*

### Comparing `Priority1py-1.0.0/setup.py` & `Priority1py-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from distutils.core import setup
 setup(
   name = 'Priority1py',         # How you named your package folder (MyLib)
   packages = ['Priority1py'],   # Chose the same as "name"
-  version = '1.0.0',      # Start with a small number and increase it with every change you make
+  version = '1.0.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Priority 1 web API python library',   # Give a short description about your library
   author = 'Daniel Pifer',                   # Type in your name
   author_email = '',      # Type in your E-Mail
   url = 'https://github.com/reid10305/Priority1py',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.0.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.1.tar.gz',    # I explain this later on
   keywords = ['API', 'Priority1'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

