# Comparing `tmp/solldex-api-client-0.1.1.tar.gz` & `tmp/solldex-api-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.1.tar", last modified: Thu Jun 15 16:55:49 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.2.tar", last modified: Thu Jun 15 17:06:19 2023, max compression
```

## Comparing `solldex-api-client-0.1.1.tar` & `solldex-api-client-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.104261 solldex-api-client-0.1.1/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.1/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 16:55:49.104104 solldex-api-client-0.1.1/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     2023 2023-06-15 16:54:18.000000 solldex-api-client-0.1.1/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-15 16:55:49.104320 solldex-api-client-0.1.1/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-15 16:55:44.000000 solldex-api-client-0.1.1/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.102934 solldex-api-client-0.1.1/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.1/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2752 2023-06-15 16:48:47.000000 solldex-api-client-0.1.1/solldex_api/solldex_api.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 16:55:49.103868 solldex-api-client-0.1.1/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      286 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-15 16:55:49.000000 solldex-api-client-0.1.1/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.509449 solldex-api-client-0.1.2/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.2/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 17:06:19.509290 solldex-api-client-0.1.2/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2023 2023-06-15 16:54:18.000000 solldex-api-client-0.1.2/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-15 17:06:19.509572 solldex-api-client-0.1.2/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-15 17:05:13.000000 solldex-api-client-0.1.2/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.508129 solldex-api-client-0.1.2/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       35 2023-06-15 16:49:58.000000 solldex-api-client-0.1.2/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2734 2023-06-15 17:05:51.000000 solldex-api-client-0.1.2/solldex_api/solldex_api.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-15 17:06:19.508978 solldex-api-client-0.1.2/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3316 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      286 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-15 17:06:19.000000 solldex-api-client-0.1.2/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.1/LICENSE` & `solldex-api-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.1/PKG-INFO` & `solldex-api-client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

### Comparing `solldex-api-client-0.1.1/README.md` & `solldex-api-client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.1/setup.py` & `solldex-api-client-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.1/solldex_api/solldex_api.py` & `solldex-api-client-0.1.2/solldex_api/solldex_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,65 +19,65 @@
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             'Authorization': f'Bearer {token}'
         }
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def recepcionar_lote(self, data: Dict[str, Union[str, int, Dict]]) -> requests.Response:
+    def recepcionar_lote(self, data: Dict[str, Union[str, int, Dict]]) -> Dict:
         """
         Makes a POST request to the 'recepcionar-lote-rps' endpoint of the Solldex API.
 
         Args:
             data: The request body data.
 
         Returns:
             The response from the Solldex API.
         """
         url = f'{self.base_url}/recepcionar-lote-rps'
         try:
             response = requests.post(url, headers=self.headers, json=data)
             response.raise_for_status()
-            return response
+            return response.json()
         except requests.RequestException as e:
             logging.error(f'Request to {url} failed: {e}')
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def consultar_lote(self, data: Dict[str, Union[str, int]]) -> requests.Response:
+    def consultar_lote(self, data: Dict[str, Union[str, int]]) -> Dict:
         """
         Makes a GET request to the 'consulta-lote' endpoint of the Solldex API.
 
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f'{self.base_url}/consulta-lote'
         try:
             response = requests.get(url, headers=self.headers, json=data)
             response.raise_for_status()
-            return response
+            return response.json()
         except requests.RequestException as e:
             logging.error(f'Request to {url} failed: {e}')
             raise
 
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2))
-    def consultar_rps(self, data: Dict[str, Union[str, int]]) -> requests.Response:
+    def consultar_rps(self, data: Dict[str, Union[str, int]]) -> Dict:
         """
         Makes a GET request to the 'consulta-rps' endpoint of the Solldex API.
 
         Args:
             data: The request parameters.
 
         Returns:
             The response from the Solldex API.
         """
         url = f'{self.base_url}/consulta-rps'
         try:
             response = requests.get(url, headers=self.headers, json=data)
             response.raise_for_status()
-            return response
+            return response.json()
         except requests.RequestException as e:
             logging.error(f'Request to {url} failed: {e}')
             raise
```

### Comparing `solldex-api-client-0.1.1/solldex_api_client.egg-info/PKG-INFO` & `solldex-api-client-0.1.2/solldex_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

