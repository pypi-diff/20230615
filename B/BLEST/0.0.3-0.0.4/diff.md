# Comparing `tmp/BLEST-0.0.3.tar.gz` & `tmp/BLEST-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-0.0.3.tar", last modified: Sun Jun 11 22:08:05 2023, max compression
+gzip compressed data, was "BLEST-0.0.4.tar", last modified: Thu Jun 15 16:05:10 2023, max compression
```

## Comparing `BLEST-0.0.3.tar` & `BLEST-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 22:08:05.829306 BLEST-0.0.3/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-11 22:08:05.828570 BLEST-0.0.3/BLEST.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     3124 2023-06-11 22:08:05.000000 BLEST-0.0.3/BLEST.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-11 22:08:05.000000 BLEST-0.0.3/BLEST.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 22:08:05.000000 BLEST-0.0.3/BLEST.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)        8 2023-06-11 22:08:05.000000 BLEST-0.0.3/BLEST.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-11 22:08:05.000000 BLEST-0.0.3/BLEST.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.3/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     3124 2023-06-11 22:08:05.828976 BLEST-0.0.3/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     2513 2023-06-11 22:07:20.000000 BLEST-0.0.3/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-11 22:08:05.829400 BLEST-0.0.3/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)      877 2023-06-11 22:06:07.000000 BLEST-0.0.3/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:05:10.194595 BLEST-0.0.4/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:05:10.193759 BLEST-0.0.4/BLEST.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     3911 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)       29 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:05:10.000000 BLEST-0.0.4/BLEST.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.4/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     3911 2023-06-15 16:05:10.194189 BLEST-0.0.4/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3318 2023-06-15 15:01:11.000000 BLEST-0.0.4/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-15 16:05:10.194734 BLEST-0.0.4/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)      941 2023-06-15 15:50:24.000000 BLEST-0.0.4/setup.py
```

### Comparing `BLEST-0.0.3/BLEST.egg-info/PKG-INFO` & `BLEST-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: BLEST
-Version: 0.0.3
-Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
-Home-page: https://github.com/jhuntdev/blest-py
-Author: JHunt
-Author-email: blest@jhunt.dev
-License: UNKNOWN
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BLEST Python
 
 The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST. It includes examples for Django, FastAPI, and Flask.
 
 To learn more about BLEST, please refer to the white paper: https://jhunt.dev/BLEST%20White%20Paper.pdf
 
 ## Features
 
-- JSON Payloads - Reduce parsing time and overhead
+- Built on JSON - Reduce parsing time and overhead
 - Request Batching - Save bandwidth and reduce load times
 - Compact Payloads - Save more bandwidth
 - Selective Returns - Save even more bandwidth
 - Single Endpoint - Reduce complexity and improve data privacy
 - Fully Encrypted - Improve data privacy
 
 ## Installation
@@ -39,28 +21,65 @@
 pip install blest
 ```
 
 ## Usage
 
 ### Server-side
 
-Use the `create_request_handler` function to create a request handler suitable for use in a Python application. The following example uses Flask, but you can find examples with other frameworks [here](/examples).
+Use the `create_server` function to create a standalone HTTP server, or use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Both functions allow you to define middleware in your router.
+
+### create_server
+
+```python
+from blest import create_server
+
+# Create some middleware (optional)
+def auth_middleware(params, context):
+  if params.name:
+    context.user = {
+      'name': params.name
+    }
+  else:
+    raise Exception('Unauthorized')
+
+# Create a route controller
+def greet_controller(params, context):
+  return {
+    'greeting': f'Hi, {context.user.name}!'
+  }
+
+# Define your router
+router = {
+  'greet': [auth_middleware, greet_controller]
+}
+
+run = create_server(router)
+
+if __name__ == '__main__':
+  run()
+```
+
+### create_request_handler
+
+The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
 from blest import create_request_handler
 
 async def greet(params, context):
   return {
     'geeting': 'Hi, ' + params.get('name') + '!'
   }
 
-router = create_request_handler({
+routes = {
   'greet': greet
-})
+}
+
+router = create_request_handler(routes)
 
 app = Flask(__name__)
 
 @app.post('/')
 async def index():
   result, error = await router(request.json)
   if error:
@@ -75,35 +94,40 @@
 ### Client-side
 
 Client-side libraries assist in batching and processing requests and commands. Currently available for React with other frameworks coming soon.
 
 #### React
 
 ```javascript
-import React from 'react';
-import { useBlestRequest, useBlestCommand } from 'blest-react';
+import React from 'react'
+import { useBlestRequest, useBlestCommand } from 'blest-react'
 
 // Use the useBlestRequest hook for fetching data
 const MyComponent = () => {
-  const { data, loading, error } = useBlestRequest('listItems', { limit: 24 });
+  const { data, loading, error } = useBlestRequest('listItems', { limit: 24 })
 
-  // Render your component
-  // ...
-};
+  return (
+    // Render your component
+  )
+}
 
 // Use the useBlestCommand hook for sending data
 const MyForm = () => {
-  const [submitMyForm, { data, loading, error }] = useBlestCommand('submitForm');
+  const [submitMyForm, { data, loading, error }] = useBlestCommand('submitForm')
+  
+  const handleSubmit = (values) => {
+    return submitMyForm(values)
+  }
 
-  // Render your form
-  // ...
-};
+  return (
+    // Render your form
+  )
+}
 ```
 
 ## Contributing
 
 We actively welcome pull requests. Learn how to [contribute](CONTRIBUTING.md) for more information.
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
-
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `BLEST-0.0.3/LICENSE` & `BLEST-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.3/PKG-INFO` & `BLEST-0.0.4/BLEST.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
-License: UNKNOWN
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -20,15 +19,15 @@
 
 The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST. It includes examples for Django, FastAPI, and Flask.
 
 To learn more about BLEST, please refer to the white paper: https://jhunt.dev/BLEST%20White%20Paper.pdf
 
 ## Features
 
-- JSON Payloads - Reduce parsing time and overhead
+- Built on JSON - Reduce parsing time and overhead
 - Request Batching - Save bandwidth and reduce load times
 - Compact Payloads - Save more bandwidth
 - Selective Returns - Save even more bandwidth
 - Single Endpoint - Reduce complexity and improve data privacy
 - Fully Encrypted - Improve data privacy
 
 ## Installation
@@ -39,28 +38,65 @@
 pip install blest
 ```
 
 ## Usage
 
 ### Server-side
 
-Use the `create_request_handler` function to create a request handler suitable for use in a Python application. The following example uses Flask, but you can find examples with other frameworks [here](/examples).
+Use the `create_server` function to create a standalone HTTP server, or use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Both functions allow you to define middleware in your router.
+
+### create_server
+
+```python
+from blest import create_server
+
+# Create some middleware (optional)
+def auth_middleware(params, context):
+  if params.name:
+    context.user = {
+      'name': params.name
+    }
+  else:
+    raise Exception('Unauthorized')
+
+# Create a route controller
+def greet_controller(params, context):
+  return {
+    'greeting': f'Hi, {context.user.name}!'
+  }
+
+# Define your router
+router = {
+  'greet': [auth_middleware, greet_controller]
+}
+
+run = create_server(router)
+
+if __name__ == '__main__':
+  run()
+```
+
+### create_request_handler
+
+The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
 from blest import create_request_handler
 
 async def greet(params, context):
   return {
     'geeting': 'Hi, ' + params.get('name') + '!'
   }
 
-router = create_request_handler({
+routes = {
   'greet': greet
-})
+}
+
+router = create_request_handler(routes)
 
 app = Flask(__name__)
 
 @app.post('/')
 async def index():
   result, error = await router(request.json)
   if error:
@@ -75,35 +111,40 @@
 ### Client-side
 
 Client-side libraries assist in batching and processing requests and commands. Currently available for React with other frameworks coming soon.
 
 #### React
 
 ```javascript
-import React from 'react';
-import { useBlestRequest, useBlestCommand } from 'blest-react';
+import React from 'react'
+import { useBlestRequest, useBlestCommand } from 'blest-react'
 
 // Use the useBlestRequest hook for fetching data
 const MyComponent = () => {
-  const { data, loading, error } = useBlestRequest('listItems', { limit: 24 });
+  const { data, loading, error } = useBlestRequest('listItems', { limit: 24 })
 
-  // Render your component
-  // ...
-};
+  return (
+    // Render your component
+  )
+}
 
 // Use the useBlestCommand hook for sending data
 const MyForm = () => {
-  const [submitMyForm, { data, loading, error }] = useBlestCommand('submitForm');
+  const [submitMyForm, { data, loading, error }] = useBlestCommand('submitForm')
+  
+  const handleSubmit = (values) => {
+    return submitMyForm(values)
+  }
 
-  // Render your form
-  // ...
-};
+  return (
+    // Render your form
+  )
+}
 ```
 
 ## Contributing
 
 We actively welcome pull requests. Learn how to [contribute](CONTRIBUTING.md) for more information.
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
-
```

### Comparing `BLEST-0.0.3/setup.py` & `BLEST-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="BLEST",
-    version="0.0.3",
+    version="0.0.4",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/jhuntdev/blest-py",
     packages=find_packages(),
@@ -18,11 +18,15 @@
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "asyncio",
+        "aiohttp",
+        "json",
+        "copy",
+        "os"
     ],
     python_requires=">=3.6",
     platforms="any",
 )
```

