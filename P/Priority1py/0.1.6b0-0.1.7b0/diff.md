# Comparing `tmp/Priority1py-0.1.6-beta.tar.gz` & `tmp/Priority1py-0.1.7-beta.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Priority1py-0.1.6-beta.tar", last modified: Thu Jun 15 01:45:58 2023, max compression
+gzip compressed data, was "dist\Priority1py-0.1.7-beta.tar", last modified: Thu Jun 15 01:49:40 2023, max compression
```

## Comparing `Priority1py-0.1.6-beta.tar` & `Priority1py-0.1.7-beta.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:45:58.000000 Priority1py-0.1.6-beta/
--rw-rw-rw-   0        0        0      779 2023-06-15 01:45:58.000000 Priority1py-0.1.6-beta/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 01:45:58.000000 Priority1py-0.1.6-beta/Priority1py/
--rw-rw-rw-   0        0        0     2126 2023-06-15 01:30:52.000000 Priority1py-0.1.6-beta/Priority1py/Priority1py.py
--rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-0.1.6-beta/Priority1py/__init__.py
--rw-rw-rw-   0        0        0       37 2023-06-14 03:02:08.000000 Priority1py-0.1.6-beta/Priority1py/json.py
--rw-rw-rw-   0        0        0     1225 2023-06-14 03:47:26.000000 Priority1py-0.1.6-beta/Priority1py/request.py
--rw-rw-rw-   0        0        0      795 2023-06-15 01:44:58.000000 Priority1py-0.1.6-beta/Priority1py/strings.py
--rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-0.1.6-beta/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-06-15 01:45:22.000000 Priority1py-0.1.6-beta/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/
+-rw-rw-rw-   0        0        0      779 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/Priority1py/
+-rw-rw-rw-   0        0        0     2127 2023-06-15 01:48:44.000000 Priority1py-0.1.7-beta/Priority1py/Priority1py.py
+-rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-0.1.7-beta/Priority1py/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-06-14 03:02:08.000000 Priority1py-0.1.7-beta/Priority1py/json.py
+-rw-rw-rw-   0        0        0     1225 2023-06-14 03:47:26.000000 Priority1py-0.1.7-beta/Priority1py/request.py
+-rw-rw-rw-   0        0        0      795 2023-06-15 01:44:58.000000 Priority1py-0.1.7-beta/Priority1py/strings.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-0.1.7-beta/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-06-15 01:48:59.000000 Priority1py-0.1.7-beta/setup.py
```

### Comparing `Priority1py-0.1.6-beta/PKG-INFO` & `Priority1py-0.1.7-beta/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Priority1py
-Version: 0.1.6-beta
+Version: 0.1.7-beta
 Summary: Priority 1 web API python library
 Home-page: https://github.com/reid10305/Priority1py
 Author: Daniel Pifer
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.6-beta.tar.gz
+Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.7-beta.tar.gz
 Description: UNKNOWN
 Keywords: API,Priority1
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Priority1py-0.1.6-beta/Priority1py/Priority1py.py` & `Priority1py-0.1.7-beta/Priority1py/Priority1py.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return list
     
 
     def get_latest_tracking(self, identifier:str, identifiertype:str):
         ''' get the latest tracking update '''
 
         # get tracking statuses
-        status_list = self.__get_items_from_tracking(identifer=identifier, identifiertype=identifiertype, target='trackingStatuses')
+        status_list = self.__get_items_from_tracking(identifier=identifier, identifiertype=identifiertype, target='trackingStatuses')
 
         latest_status = status_list[0]
         
         return {
             'timestamp' : latest_status['timeStamp'],
             'status' : latest_status['status'],
             'statusreason' : latest_status['statusReason'],
```

### Comparing `Priority1py-0.1.6-beta/Priority1py/request.py` & `Priority1py-0.1.7-beta/Priority1py/request.py`

 * *Files identical despite different names*

### Comparing `Priority1py-0.1.6-beta/Priority1py/strings.py` & `Priority1py-0.1.7-beta/Priority1py/strings.py`

 * *Files identical despite different names*

### Comparing `Priority1py-0.1.6-beta/setup.py` & `Priority1py-0.1.7-beta/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from distutils.core import setup
 setup(
   name = 'Priority1py',         # How you named your package folder (MyLib)
   packages = ['Priority1py'],   # Chose the same as "name"
-  version = '0.1.6-beta',      # Start with a small number and increase it with every change you make
+  version = '0.1.7-beta',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Priority 1 web API python library',   # Give a short description about your library
   author = 'Daniel Pifer',                   # Type in your name
   author_email = '',      # Type in your E-Mail
   url = 'https://github.com/reid10305/Priority1py',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.6-beta.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.7-beta.tar.gz',    # I explain this later on
   keywords = ['API', 'Priority1'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

