# Comparing `tmp/solldex-api-client-0.1.0.tar.gz` & `tmp/solldex-api-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.0.tar", last modified: Thu Jun 15 16:51:28 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.1.tar", last modified: Thu Jun 15 16:55:49 2023, max compression
```

## Comparing `solldex-api-client-0.1.0.tar` & `solldex-api-client-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:51:28.392215 solldex-api-client-0.1.0/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.0/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     3122 2023-06-15 16:51:28.392069 solldex-api-client-0.1.0/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1901 2023-06-15 16:41:06.000000 solldex-api-client-0.1.0/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-15 16:51:28.392265 solldex-api-client-0.1.0/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-15 16:38:17.000000 solldex-api-client-0.1.0/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:51:28.390964 solldex-api-client-0.1.0/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.0/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2752 2023-06-15 16:48:47.000000 solldex-api-client-0.1.0/solldex_api/solldex_api.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:51:28.391862 solldex-api-client-0.1.0/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     3122 2023-06-15 16:51:28.000000 solldex-api-client-0.1.0/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      286 2023-06-15 16:51:28.000000 solldex-api-client-0.1.0/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-15 16:51:28.000000 solldex-api-client-0.1.0/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-15 16:51:28.000000 solldex-api-client-0.1.0/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-15 16:51:28.000000 solldex-api-client-0.1.0/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.104261 solldex-api-client-0.1.1/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.1/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 16:55:49.104104 solldex-api-client-0.1.1/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2023 2023-06-15 16:54:18.000000 solldex-api-client-0.1.1/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-15 16:55:49.104320 solldex-api-client-0.1.1/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-15 16:55:44.000000 solldex-api-client-0.1.1/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.102934 solldex-api-client-0.1.1/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.1/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2752 2023-06-15 16:48:47.000000 solldex-api-client-0.1.1/solldex_api/solldex_api.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.103868 solldex-api-client-0.1.1/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      286 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.0/LICENSE` & `solldex-api-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.0/PKG-INFO` & `solldex-api-client-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
         
@@ -16,17 +16,26 @@
         
         ## Features
         
         - Simple and intuitive interface for making requests to the Solldex API.
         - Built-in retry logic using the Tenacity library, with up to 3 retry attempts and a 2 second wait between each attempt.
         - Error logging for better debugging and maintenance.
         
+        ## Installation
+        
+        You can install the SolldexAPI Python Client via pip:
+        
+        ```bash
+        pip install solldex-api-client==0.1.0
+        ```
+        
+        
         ## Usage
         
-        To use the SolldexAPI client, you'll need to import the `SolldexAPI` class and initialize it with your API token:
+        To use the SolldexAPI client, you'll need to import the SolldexAPI class and initialize it with your API token:
         
         ```python
         from solldex_api import SolldexAPI
         
         api = SolldexAPI('your-token-here')
         ```
```

### Comparing `solldex-api-client-0.1.0/README.md` & `solldex-api-client-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,26 @@
 
 ## Features
 
 - Simple and intuitive interface for making requests to the Solldex API.
 - Built-in retry logic using the Tenacity library, with up to 3 retry attempts and a 2 second wait between each attempt.
 - Error logging for better debugging and maintenance.
 
+## Installation
+
+You can install the SolldexAPI Python Client via pip:
+
+```bash
+pip install solldex-api-client==0.1.0
+```
+
+
 ## Usage
 
-To use the SolldexAPI client, you'll need to import the `SolldexAPI` class and initialize it with your API token:
+To use the SolldexAPI client, you'll need to import the SolldexAPI class and initialize it with your API token:
 
 ```python
 from solldex_api import SolldexAPI
 
 api = SolldexAPI('your-token-here')
 ```
```

### Comparing `solldex-api-client-0.1.0/setup.py` & `solldex-api-client-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.0/solldex_api/solldex_api.py` & `solldex-api-client-0.1.1/solldex_api/solldex_api.py`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.0/solldex_api_client.egg-info/PKG-INFO` & `solldex-api-client-0.1.1/solldex_api_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
         
@@ -16,17 +16,26 @@
         
         ## Features
         
         - Simple and intuitive interface for making requests to the Solldex API.
         - Built-in retry logic using the Tenacity library, with up to 3 retry attempts and a 2 second wait between each attempt.
         - Error logging for better debugging and maintenance.
         
+        ## Installation
+        
+        You can install the SolldexAPI Python Client via pip:
+        
+        ```bash
+        pip install solldex-api-client==0.1.0
+        ```
+        
+        
         ## Usage
         
-        To use the SolldexAPI client, you'll need to import the `SolldexAPI` class and initialize it with your API token:
+        To use the SolldexAPI client, you'll need to import the SolldexAPI class and initialize it with your API token:
         
         ```python
         from solldex_api import SolldexAPI
         
         api = SolldexAPI('your-token-here')
         ```
```

