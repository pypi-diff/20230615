# Comparing `tmp/articolare-1.1.1.tar.gz` & `tmp/articolare-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articolare-1.1.1.tar", last modified: Thu Jun 15 20:36:04 2023, max compression
+gzip compressed data, was "articolare-1.1.2.tar", last modified: Thu Jun 15 20:56:38 2023, max compression
```

## Comparing `articolare-1.1.1.tar` & `articolare-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:36:04.808620 articolare-1.1.1/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:36:04.807384 articolare-1.1.1/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-1.1.1/README.md
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:36:04.784079 articolare-1.1.1/articolare/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-1.1.1/articolare/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     3371 2023-06-15 20:34:14.000000 articolare-1.1.1/articolare/translate.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:36:04.798020 articolare-1.1.1/articolare.egg-info/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:36:04.000000 articolare-1.1.1/articolare.egg-info/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 20:36:04.000000 articolare-1.1.1/articolare.egg-info/SOURCES.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 20:36:04.000000 articolare-1.1.1/articolare.egg-info/dependency_links.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 20:36:04.000000 articolare-1.1.1/articolare.egg-info/requires.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 20:36:04.000000 articolare-1.1.1/articolare.egg-info/top_level.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 20:36:04.808746 articolare-1.1.1/setup.cfg
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 20:34:36.000000 articolare-1.1.1/setup.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:36:04.798839 articolare-1.1.1/tests/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-1.1.1/tests/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-1.1.1/tests/test_client.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:56:38.808452 articolare-1.1.2/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:56:38.807574 articolare-1.1.2/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-1.1.2/README.md
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:56:38.805115 articolare-1.1.2/articolare/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-1.1.2/articolare/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     3396 2023-06-15 20:54:13.000000 articolare-1.1.2/articolare/translate.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:56:38.806647 articolare-1.1.2/articolare.egg-info/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:56:38.000000 articolare-1.1.2/articolare.egg-info/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 20:56:38.000000 articolare-1.1.2/articolare.egg-info/SOURCES.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 20:56:38.000000 articolare-1.1.2/articolare.egg-info/dependency_links.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 20:56:38.000000 articolare-1.1.2/articolare.egg-info/requires.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 20:56:38.000000 articolare-1.1.2/articolare.egg-info/top_level.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 20:56:38.808553 articolare-1.1.2/setup.cfg
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 20:56:26.000000 articolare-1.1.2/setup.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:56:38.807195 articolare-1.1.2/tests/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-1.1.2/tests/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-1.1.2/tests/test_client.py
```

### Comparing `articolare-1.1.1/PKG-INFO` & `articolare-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-1.1.1/README.md` & `articolare-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `articolare-1.1.1/articolare/translate.py` & `articolare-1.1.2/articolare/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class ArticolareClient:
     BASE_URL = "https://articolare-translator-api-yr2dhc67qa-uc.a.run.app"
 
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('API_KEY')
         self.session = requests.Session()
         self.session.headers.update({
-            "Authorization": f"Bearer {self.api_key}"
+            "x-api-key": self.api_key  # Change "Authorization" to "x-api-key"
         })
 
         # Set up retry mechanism
         retries = Retry(total=5, backoff_factor=1, status_forcelist=[429, 502, 503, 504])
         self.session.mount('http://', HTTPAdapter(max_retries=retries))
         self.session.mount('https://', HTTPAdapter(max_retries=retries))
```

### Comparing `articolare-1.1.1/articolare.egg-info/PKG-INFO` & `articolare-1.1.2/articolare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-1.1.1/setup.py` & `articolare-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="articolare",
-    version="1.1.1",
+    version="1.1.2",
     author="Murilo Silvestre",
     description="Python client for the Articolare API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `articolare-1.1.1/tests/test_client.py` & `articolare-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

