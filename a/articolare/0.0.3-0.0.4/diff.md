# Comparing `tmp/articolare-0.0.3.tar.gz` & `tmp/articolare-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articolare-0.0.3.tar", last modified: Thu Jun 15 19:13:35 2023, max compression
+gzip compressed data, was "articolare-0.0.4.tar", last modified: Thu Jun 15 19:39:31 2023, max compression
```

## Comparing `articolare-0.0.3.tar` & `articolare-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:13:35.099507 articolare-0.0.3/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1979 2023-06-15 19:13:35.098341 articolare-0.0.3/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1238 2023-06-15 18:53:21.000000 articolare-0.0.3/README.md
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:13:35.095234 articolare-0.0.3/art_api_client/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.3/art_api_client/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     3300 2023-06-15 18:56:46.000000 articolare-0.0.3/art_api_client/client.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:13:35.097020 articolare-0.0.3/articolare.egg-info/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1979 2023-06-15 19:13:35.000000 articolare-0.0.3/articolare.egg-info/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      278 2023-06-15 19:13:35.000000 articolare-0.0.3/articolare.egg-info/SOURCES.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 19:13:35.000000 articolare-0.0.3/articolare.egg-info/dependency_links.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 19:13:35.000000 articolare-0.0.3/articolare.egg-info/requires.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       21 2023-06-15 19:13:35.000000 articolare-0.0.3/articolare.egg-info/top_level.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 19:13:35.099688 articolare-0.0.3/setup.cfg
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1401 2023-06-15 19:12:09.000000 articolare-0.0.3/setup.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:13:35.097796 articolare-0.0.3/tests/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.3/tests/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      768 2023-06-15 19:04:45.000000 articolare-0.0.3/tests/test_client.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.069499 articolare-0.0.4/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:39:31.067862 articolare-0.0.4/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-0.0.4/README.md
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:30.876438 articolare-0.0.4/articolare/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.4/articolare/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     3300 2023-06-15 18:56:46.000000 articolare-0.0.4/articolare/translate.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.023364 articolare-0.0.4/articolare.egg-info/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/SOURCES.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/dependency_links.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/requires.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/top_level.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 19:39:31.069699 articolare-0.0.4/setup.cfg
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 19:25:49.000000 articolare-0.0.4/setup.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.024191 articolare-0.0.4/tests/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.4/tests/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-0.0.4/tests/test_client.py
```

### Comparing `articolare-0.0.3/PKG-INFO` & `articolare-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client for the Articolare API
-Home-page: https://github.com/youractualusername/articolare
 Author: Murilo Silvestre
-Author-email: info@articolare.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -28,37 +26,37 @@
 ```
   pip install articolare
 ```
 
 # Usage
 First, you need to initialize the ArticolareClient with your API key:
 ```
-from articolare import ArticolareClient 
+from articolare import create
 ```
 ```
-  client = ArticolareClient(api_key="your-api-key"))
+  client = create.ArticolareClient(api_key="your-api-key"))
 ```
 
-
 # Create
 You can then use the create method to make a request to the API:
 * languages available:
   * English
   * Portuguese
   * Spanish
   * Italian
 * Tokens:
   * Max Tokens = 1000 - If you require more tokens, please refer to our documentation on https://www.articolare.com/
 ```
 response = client.create(
     model="art-translator",
-    lang="English",
+    lang="english",
     style="conversation",
+    dialect="european"
     prompt="Enter your prompt here",
-    max_tokens=10
+    max_tokens=1000
 )
 ```
 
 * The create method returns a dictionary containing the response data from the API.
 
 # Testing
 This library includes a basic test suite, which you can run using pytest:
```

### Comparing `articolare-0.0.3/README.md` & `articolare-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 ```
   pip install articolare
 ```
 
 # Usage
 First, you need to initialize the ArticolareClient with your API key:
 ```
-from articolare import ArticolareClient 
+from articolare import create
 ```
 ```
-  client = ArticolareClient(api_key="your-api-key"))
+  client = create.ArticolareClient(api_key="your-api-key"))
 ```
 
-
 # Create
 You can then use the create method to make a request to the API:
 * languages available:
   * English
   * Portuguese
   * Spanish
   * Italian
 * Tokens:
   * Max Tokens = 1000 - If you require more tokens, please refer to our documentation on https://www.articolare.com/
 ```
 response = client.create(
     model="art-translator",
-    lang="English",
+    lang="english",
     style="conversation",
+    dialect="european"
     prompt="Enter your prompt here",
-    max_tokens=10
+    max_tokens=1000
 )
 ```
 
 * The create method returns a dictionary containing the response data from the API.
 
 # Testing
 This library includes a basic test suite, which you can run using pytest:
```

### Comparing `articolare-0.0.3/art_api_client/client.py` & `articolare-0.0.4/articolare/translate.py`

 * *Files identical despite different names*

### Comparing `articolare-0.0.3/articolare.egg-info/PKG-INFO` & `articolare-0.0.4/articolare.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client for the Articolare API
-Home-page: https://github.com/youractualusername/articolare
 Author: Murilo Silvestre
-Author-email: info@articolare.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -28,37 +26,37 @@
 ```
   pip install articolare
 ```
 
 # Usage
 First, you need to initialize the ArticolareClient with your API key:
 ```
-from articolare import ArticolareClient 
+from articolare import create
 ```
 ```
-  client = ArticolareClient(api_key="your-api-key"))
+  client = create.ArticolareClient(api_key="your-api-key"))
 ```
 
-
 # Create
 You can then use the create method to make a request to the API:
 * languages available:
   * English
   * Portuguese
   * Spanish
   * Italian
 * Tokens:
   * Max Tokens = 1000 - If you require more tokens, please refer to our documentation on https://www.articolare.com/
 ```
 response = client.create(
     model="art-translator",
-    lang="English",
+    lang="english",
     style="conversation",
+    dialect="european"
     prompt="Enter your prompt here",
-    max_tokens=10
+    max_tokens=1000
 )
 ```
 
 * The create method returns a dictionary containing the response data from the API.
 
 # Testing
 This library includes a basic test suite, which you can run using pytest:
```

### Comparing `articolare-0.0.3/setup.py` & `articolare-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="articolare",
-    version="0.0.3",
+    version="0.0.4",
     author="Murilo Silvestre",
-    author_email="info@articolare.com",
     description="Python client for the Articolare API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/youractualusername/articolare",
     packages=find_packages(),
     install_requires=[
         "requests",
         "certifi==2023.5.7",
         "charset-normalizer==3.1.0",
         "exceptiongroup==1.1.1",
         "idna==3.4",
```

### Comparing `articolare-0.0.3/tests/test_client.py` & `articolare-0.0.4/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
 from unittest.mock import patch
-from art_api_client import client as art
+from articolare import translate as art
 
 @patch('articolare.ArticolareClient._request')
 def test_create(mock_request):
     mock_request.return_value = {"success": True}
 
     client = art.ArticolareClient(api_key="testkey")
     response = client.create(
         model="testmodel",
-        lang="English",
-        style="Conversation Formal",
-        dialect="Latam",
+        lang="english",
+        style="conversation formal",
+        dialect="latam",
         prompt="testprompt",
         max_tokens=10
     )
 
     assert response == {"success": True}
     mock_request.assert_called_once_with("POST", "/create", json={
         "model": "testmodel",
-        "lang": "English",
+        "lang": "english",
         "style": "Conversation Formal",
-        "dialect": "Latam",
+        "dialect": "latam",
         "prompt": "testprompt",
         "max_tokens": 10
     })
```

