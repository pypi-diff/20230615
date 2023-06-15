# Comparing `tmp/Priority1py-0.1.7-beta.tar.gz` & `tmp/Priority1py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Priority1py-0.1.7-beta.tar", last modified: Thu Jun 15 01:49:40 2023, max compression
+gzip compressed data, was "dist\Priority1py-1.0.0.tar", last modified: Thu Jun 15 02:50:07 2023, max compression
```

## Comparing `Priority1py-0.1.7-beta.tar` & `Priority1py-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/
--rw-rw-rw-   0        0        0      779 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 01:49:40.000000 Priority1py-0.1.7-beta/Priority1py/
--rw-rw-rw-   0        0        0     2127 2023-06-15 01:48:44.000000 Priority1py-0.1.7-beta/Priority1py/Priority1py.py
--rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-0.1.7-beta/Priority1py/__init__.py
--rw-rw-rw-   0        0        0       37 2023-06-14 03:02:08.000000 Priority1py-0.1.7-beta/Priority1py/json.py
--rw-rw-rw-   0        0        0     1225 2023-06-14 03:47:26.000000 Priority1py-0.1.7-beta/Priority1py/request.py
--rw-rw-rw-   0        0        0      795 2023-06-15 01:44:58.000000 Priority1py-0.1.7-beta/Priority1py/strings.py
--rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-0.1.7-beta/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-06-15 01:48:59.000000 Priority1py-0.1.7-beta/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:50:07.000000 Priority1py-1.0.0/
+-rw-rw-rw-   0        0        0      769 2023-06-15 02:50:07.000000 Priority1py-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 02:50:07.000000 Priority1py-1.0.0/Priority1py/
+-rw-rw-rw-   0        0        0     2334 2023-06-15 02:46:50.000000 Priority1py-1.0.0/Priority1py/Priority1py.py
+-rw-rw-rw-   0        0        0      148 2023-06-15 01:29:14.000000 Priority1py-1.0.0/Priority1py/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-06-15 02:44:19.000000 Priority1py-1.0.0/Priority1py/request.py
+-rw-rw-rw-   0        0        0      797 2023-06-15 02:12:42.000000 Priority1py-1.0.0/Priority1py/strings.py
+-rw-rw-rw-   0        0        0      241 2023-06-15 02:14:29.000000 Priority1py-1.0.0/Priority1py/test.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-06-15 02:49:40.000000 Priority1py-1.0.0/setup.py
```

### Comparing `Priority1py-0.1.7-beta/PKG-INFO` & `Priority1py-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Priority1py
-Version: 0.1.7-beta
+Version: 1.0.0
 Summary: Priority 1 web API python library
 Home-page: https://github.com/reid10305/Priority1py
 Author: Daniel Pifer
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.7-beta.tar.gz
+Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.0.tar.gz
 Description: UNKNOWN
 Keywords: API,Priority1
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Priority1py-0.1.7-beta/Priority1py/Priority1py.py` & `Priority1py-1.0.0/Priority1py/Priority1py.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from Priority1py.request import req_send
 from Priority1py.strings import Endpoint, Crud, Accessorial, IDType
+# from request import req_send
+# from strings import Endpoint, Crud, Accessorial, IDType
 import json
 
 class Priority1py():
     ''' API helper class '''
 
     def __init__(self, key:str):
         self.key = key
@@ -17,30 +19,35 @@
             'identifierType' : identifiertype,
             'identifierValue' : identifier
         }
 
         # send request and convert to json 
         res_str = self.req.send_req(endpoint=Endpoint.LTL_SHIPMENT_STATUS, payload=payload, request=Crud.POST)
         res_json = json.loads(res_str)
+        print(res_json)
 
         # test for no shipments found
         if 'No shipments found' in res_json:
             raise Exception('No shipments found matching that ID')
 
         # parse json for status list
-        list = res_json['shipments'][0][target]
+        try:
+            list = res_json['shipments'][0][target]
 
-        return list
+            return list
+        
+        except KeyError:
+            return 'Bad '
     
 
     def get_latest_tracking(self, identifier:str, identifiertype:str):
         ''' get the latest tracking update '''
 
         # get tracking statuses
-        status_list = self.__get_items_from_tracking(identifier=identifier, identifiertype=identifiertype, target='trackingStatuses')
+        status_list = self.__get_items_from_tracking(identifier=identifier, identifiertype=identifiertype.value, target='trackingStatuses')
 
         latest_status = status_list[0]
         
         return {
             'timestamp' : latest_status['timeStamp'],
             'status' : latest_status['status'],
             'statusreason' : latest_status['statusReason'],
```

### Comparing `Priority1py-0.1.7-beta/Priority1py/request.py` & `Priority1py-1.0.0/Priority1py/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 ''' classes used for sending requests to P1 API '''
 import requests, json
 
 class req_send():
     ''' class to send url '''
-    def __init__(self, key:str, base_url:str='https://api.priority1.com/') -> json:
+    def __init__(self, key:str, base_url:str='https://api.priority1.com'):
         self.base_url = base_url
         self.key = key
 
     
-    def send_req(self, endpoint:str, payload:json, request:str) -> str:
+    def send_req(self, endpoint:str, payload:dict, request:str) -> str:
         ''' sends a request to P1 and return the string
             takes in endpoint string and json data for
             request body '''
         
         headers = {
             'X-API-KEY' : self.key,
             'accept' : 'application/json',
             'Content-type' : 'application/json'
         }
+        
+        # print(headers)
+        # print(payload)
+
+        url = self.base_url + endpoint.value
+
+        data = json.dumps(payload)
 
-        url = self.base_url + endpoint
+        # print(url)
 
         try:
-            result = requests.request(request, url, headers=headers, data=payload)
+            result = requests.request(request.value, url=url, headers=headers, data=data)
             return result.text
         
         except requests.exceptions.HTTPError as e:
             raise Exception('HTTP Error occurred.')
         
 
     def set_base_url(self, url:str) -> str:
```

### Comparing `Priority1py-0.1.7-beta/Priority1py/strings.py` & `Priority1py-1.0.0/Priority1py/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ''' constant strings used '''
 from enum import Enum
 
 class Endpoint(Enum):
     def __str__(self):
         return self.value
-    LTL_RATE_QUOTE = '/v2/ltl/quotes/rates'
-    LTL_SHIPMENT_STATUS = '/v2/ltl/shipments/status'
+    LTL_RATE_QUOTE = '/v2/ltl/quotes/rates/'
+    LTL_SHIPMENT_STATUS = '/v2/ltl/shipments/status/'
 
 
 class Crud(Enum):
     def __str__(self):
         return self.value
     POST = 'POST'
     GET = 'GET'
```

### Comparing `Priority1py-0.1.7-beta/setup.py` & `Priority1py-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from distutils.core import setup
 setup(
   name = 'Priority1py',         # How you named your package folder (MyLib)
   packages = ['Priority1py'],   # Chose the same as "name"
-  version = '0.1.7-beta',      # Start with a small number and increase it with every change you make
+  version = '1.0.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Priority 1 web API python library',   # Give a short description about your library
   author = 'Daniel Pifer',                   # Type in your name
   author_email = '',      # Type in your E-Mail
   url = 'https://github.com/reid10305/Priority1py',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.7-beta.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v1.0.0.tar.gz',    # I explain this later on
   keywords = ['API', 'Priority1'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

