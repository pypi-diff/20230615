# Comparing `tmp/promptlayer-0.1.87.tar.gz` & `tmp/promptlayer-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.87.tar", last modified: Tue Jun 13 15:19:18 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.88.tar", last modified: Thu Jun 15 15:39:26 2023, max compression
```

## Comparing `promptlayer-0.1.87.tar` & `promptlayer-0.1.88.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.895920 promptlayer-0.1.87/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.87/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-13 15:19:18.894665 promptlayer-0.1.87/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.87/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.886705 promptlayer-0.1.87/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-13 14:07:07.000000 promptlayer-0.1.87/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.889840 promptlayer-0.1.87/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.87/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.890887 promptlayer-0.1.87/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.87/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.87/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.87/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.892556 promptlayer-0.1.87/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.87/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.87/promptlayer/prompts/chat.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.87/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.893828 promptlayer-0.1.87/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.87/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.87/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.87/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 15:19:18.889428 promptlayer-0.1.87/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-13 15:19:18.000000 promptlayer-0.1.87/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-13 15:19:18.000000 promptlayer-0.1.87/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-13 15:19:18.000000 promptlayer-0.1.87/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-13 15:19:18.000000 promptlayer-0.1.87/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-13 15:19:18.000000 promptlayer-0.1.87/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-13 15:19:18.896048 promptlayer-0.1.87/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-13 15:17:47.000000 promptlayer-0.1.87/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.652189 promptlayer-0.1.88/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.88/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-15 15:39:26.651540 promptlayer-0.1.88/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.88/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.642641 promptlayer-0.1.88/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-13 14:07:07.000000 promptlayer-0.1.88/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.645072 promptlayer-0.1.88/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.88/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.646030 promptlayer-0.1.88/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.88/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.88/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.88/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.648919 promptlayer-0.1.88/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.88/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1839 2023-06-13 15:17:41.000000 promptlayer-0.1.88/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.88/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.650685 promptlayer-0.1.88/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.88/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.88/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13502 2023-06-15 15:39:19.000000 promptlayer-0.1.88/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-15 15:39:26.644634 promptlayer-0.1.88/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-15 15:39:26.000000 promptlayer-0.1.88/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-15 15:39:26.000000 promptlayer-0.1.88/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-15 15:39:26.000000 promptlayer-0.1.88/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-15 15:39:26.000000 promptlayer-0.1.88/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-15 15:39:26.000000 promptlayer-0.1.88/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-15 15:39:26.652314 promptlayer-0.1.88/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-15 15:39:19.000000 promptlayer-0.1.88/setup.py
```

### Comparing `promptlayer-0.1.87/LICENSE` & `promptlayer-0.1.88/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/PKG-INFO` & `promptlayer-0.1.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.87
+Version: 0.1.88
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.87 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.88 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.87/README.md` & `promptlayer-0.1.88/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/__init__.py` & `promptlayer-0.1.88/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.88/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/promptlayer.py` & `promptlayer-0.1.88/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/prompts/chat.py` & `promptlayer-0.1.88/promptlayer/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/prompts/prompts.py` & `promptlayer-0.1.88/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/track/track.py` & `promptlayer-0.1.88/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/promptlayer/utils.py` & `promptlayer-0.1.88/promptlayer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     kwargs,
     tags,
     response,
     request_start_time,
     request_end_time,
     api_key,
     return_pl_id=False,
+    metadata=None,
 ):
     if type(response) != dict and hasattr(response, "to_dict_recursive"):
         response = response.to_dict_recursive()
     try:
         request_response = requests.post(
             f"{URL_API_PROMPTLAYER}/track-request",
             json={
@@ -121,14 +122,15 @@
                 "provider_type": provider_type,
                 "args": args,
                 "kwargs": kwargs,
                 "tags": tags,
                 "request_response": response,
                 "request_start_time": request_start_time,
                 "request_end_time": request_end_time,
+                "metadata": metadata,
                 "api_key": api_key,
             },
         )
         if request_response.status_code != 200:
             if hasattr(request_response, "json"):
                 print(
                     f"WARNING: While logging your request PromptLayer had the following error: {request_response.json().get('message')}",
```

### Comparing `promptlayer-0.1.87/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.88/promptlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.87
+Version: 0.1.88
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.87 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.88 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.87/promptlayer.egg-info/SOURCES.txt` & `promptlayer-0.1.88/promptlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.87/setup.py` & `promptlayer-0.1.88/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.87",
+    version="0.1.88",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

