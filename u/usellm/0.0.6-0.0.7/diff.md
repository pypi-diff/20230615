# Comparing `tmp/usellm-0.0.6.tar.gz` & `tmp/usellm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usellm-0.0.6.tar", last modified: Mon Jun 12 12:31:30 2023, max compression
+gzip compressed data, was "usellm-0.0.7.tar", last modified: Thu Jun 15 13:43:50 2023, max compression
```

## Comparing `usellm-0.0.6.tar` & `usellm-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.434120 usellm-0.0.6/
--rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.6/LICENSE
--rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-12 12:31:30.433895 usellm-0.0.6/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.6/README.md
--rw-r--r--   0 jovian     (501) staff       (20)       38 2023-06-12 12:31:30.434210 usellm-0.0.6/setup.cfg
--rw-r--r--   0 jovian     (501) staff       (20)      583 2023-06-12 12:30:45.000000 usellm-0.0.6/setup.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.432275 usellm-0.0.6/usellm/
--rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.6/usellm/__init__.py
--rw-r--r--   0 jovian     (501) staff       (20)     7470 2023-06-12 12:30:45.000000 usellm-0.0.6/usellm/use_llm.py
--rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.6/usellm/utils.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.433185 usellm-0.0.6/usellm.egg-info/
--rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)      228 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/SOURCES.txt
--rw-r--r--   0 jovian     (501) staff       (20)        1 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/dependency_links.txt
--rw-r--r--   0 jovian     (501) staff       (20)       17 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/requires.txt
--rw-r--r--   0 jovian     (501) staff       (20)        7 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/top_level.txt
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-15 13:43:50.951489 usellm-0.0.7/
+-rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.7/LICENSE
+-rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-15 13:43:50.951338 usellm-0.0.7/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.7/README.md
+-rw-r--r--   0 jovian     (501) staff       (20)       38 2023-06-15 13:43:50.951529 usellm-0.0.7/setup.cfg
+-rw-r--r--   0 jovian     (501) staff       (20)      583 2023-06-15 13:43:31.000000 usellm-0.0.7/setup.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-15 13:43:50.950376 usellm-0.0.7/usellm/
+-rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.7/usellm/__init__.py
+-rw-r--r--   0 jovian     (501) staff       (20)     8374 2023-06-15 13:43:20.000000 usellm-0.0.7/usellm/use_llm.py
+-rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.7/usellm/utils.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-15 13:43:50.951132 usellm-0.0.7/usellm.egg-info/
+-rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-15 13:43:50.000000 usellm-0.0.7/usellm.egg-info/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)      228 2023-06-15 13:43:50.000000 usellm-0.0.7/usellm.egg-info/SOURCES.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        1 2023-06-15 13:43:50.000000 usellm-0.0.7/usellm.egg-info/dependency_links.txt
+-rw-r--r--   0 jovian     (501) staff       (20)       17 2023-06-15 13:43:50.000000 usellm-0.0.7/usellm.egg-info/requires.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        7 2023-06-15 13:43:50.000000 usellm-0.0.7/usellm.egg-info/top_level.txt
```

### Comparing `usellm-0.0.6/LICENSE` & `usellm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `usellm-0.0.6/PKG-INFO` & `usellm-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usellm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Use Large Language Models in Python App
 Home-page: https://github.com/usellm/usellm-py
 Author: Siddhant
 Author-email: siddhant@jovian.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `usellm-0.0.6/README.md` & `usellm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `usellm-0.0.6/setup.py` & `usellm-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode('utf-8', errors='ignore')
 
 setup(
     name='usellm',
-    version='0.0.6',
+    version='0.0.7',
     author='Siddhant',
     author_email='siddhant@jovian.com',
     url='https://github.com/usellm/usellm-py',
     description='Use Large Language Models in Python App',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=["usellm"], exclude=["examples"]),
```

### Comparing `usellm-0.0.6/usellm/use_llm.py` & `usellm-0.0.7/usellm/use_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Optional
 import json
 import requests
+import numpy as np
 
 
 class Message:
     def __init__(self, role: str, content: str):
         self.role = role
         self.content = content
 
@@ -122,14 +123,24 @@
         self.n = n
         self.size = size
         self.embed_input = embed_input
         self.embed_user = embed_user
         self.text = text
         self.audio_url = audio_url
 
+class EmbeddingOptions:
+    def __init__(
+        self,
+        embeddings:list[list[any]],
+        query:list[float],
+        top
+    ):
+        self.embeddings = embeddings
+        self.query = query 
+        self.top = top
 
 class UseLLM:
     def __init__(self, service_url: str):
         self.service_url = service_url
 
     def chat(self, options: Options) -> Message:
         if options.stream:
@@ -186,14 +197,15 @@
             }
         )
 
         response = requests.post(
             self.service_url,
             headers={"Content-Type": "application/json"},
             data=data,
+            timeout=5000
         )
 
         if response.status_code != 200:
             raise Exception(response.text)
         else:
             json_response = response.json()
             res = GenerateImageResponse(images=json_response["images"])
@@ -273,7 +285,24 @@
         
         if response.status_code != 200:
             raise Exception(response.text)
         else:
             json_response = response.json() 
             res = TranscribeResponse(text = json_response['text'])
             return res
+
+    def cosineSimilarity(self, vecA, vecB):
+        dot_product = np.dot(vecA, vecB)
+        magnitude = np.linalg.norm(vecA) * np.linalg.norm(vecB)
+        return dot_product / magnitude
+    
+    
+    def scoreEmbeddings(self, options:EmbeddingOptions) -> List[float]:
+        scores = [self.cosineSimilarity(options.query, vector) for vector in options.embeddings]
+        sorted_scores = sorted([(score, index) for index, score in enumerate(scores)], key=lambda x: x[0], reverse=True)
+        
+        
+        if options.top is not None:
+            sorted_scores = sorted_scores[:options.top]
+    
+        return sorted_scores
+
```

### Comparing `usellm-0.0.6/usellm.egg-info/PKG-INFO` & `usellm-0.0.7/usellm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usellm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Use Large Language Models in Python App
 Home-page: https://github.com/usellm/usellm-py
 Author: Siddhant
 Author-email: siddhant@jovian.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

