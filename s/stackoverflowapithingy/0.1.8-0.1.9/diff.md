# Comparing `tmp/stackoverflowapithingy-0.1.8.tar.gz` & `tmp/stackoverflowapithingy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.8.tar", last modified: Thu Jun 15 12:02:32 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.9.tar", last modified: Thu Jun 15 13:09:39 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.8.tar` & `stackoverflowapithingy-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.780705 stackoverflowapithingy-0.1.8/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 12:02:32.780598 stackoverflowapithingy-0.1.8/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 12:02:32.780750 stackoverflowapithingy-0.1.8/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 12:02:15.000000 stackoverflowapithingy-0.1.8/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.779882 stackoverflowapithingy-0.1.8/stackoverflowapithingy/
--rw-r--r--   0 benjamin   (501) staff       (20)      140 2023-06-15 11:41:43.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1625 2023-06-15 12:00:52.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy/stackoverflow.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.780453 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      312 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 13:09:39.784897 stackoverflowapithingy-0.1.9/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 13:09:39.784789 stackoverflowapithingy-0.1.9/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 13:09:39.784939 stackoverflowapithingy-0.1.9/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 13:09:26.000000 stackoverflowapithingy-0.1.9/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 13:09:39.784101 stackoverflowapithingy-0.1.9/stackoverflowapithingy/
+-rw-r--r--   0 benjamin   (501) staff       (20)      140 2023-06-15 11:41:43.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2153 2023-06-15 12:33:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy/stackoverflow.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 13:09:39.784639 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 13:09:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      312 2023-06-15 13:09:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 13:09:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 13:09:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 13:09:39.000000 stackoverflowapithingy-0.1.9/stackoverflowapithingy.egg-info/top_level.txt
```

### Comparing `stackoverflowapithingy-0.1.8/stackoverflowapithingy/stackoverflow.py` & `stackoverflowapithingy-0.1.9/stackoverflowapithingy/stackoverflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 import requests
+import re
+
+def remove_html_tags(text): #this is literally from google ai
+  clean_text = re.sub('<[^>]+>', '', text)
+  return clean_text
 
 #settings = {"q_per_page":1,"accepted":True,"sort":3,"default_tags":["python"]}
 def whatIsSettings():
     return "settings = {\"q_per_page\":1,\"accepted\":True,\"sort\":3,\"default_tags\":[\"python\"]}\noh and sort order is activity, votes, creation, relevance\nalso tags should be an array :)"
 
 
 def getQuestionByTags(tags=["python"],settings={"q_per_page":1,"accepted":True,"sort":3,"default_tags":["python"]}): #tags is array
@@ -21,7 +26,19 @@
     return requests.get(url).json()
 
 
 def getAnswerById(answer_id):
     url = "https://api.stackexchange.com/2.3/answers/{0}?order=desc&site=stackoverflow&filter=withbody".format(answer_id)
     return requests.get(url).json()
 
+def formatResponse(response,isQuestion=True): #False if it is an answer
+    try:
+        title = ""
+        if isQuestion:
+            title = response['items'][0]['title']
+            
+        body = remove_html_tags(response['items'][0]['body'])
+        raw = response['items'][0]['body']
+        return [title,body,raw]
+    except:
+        raise ValueError("Invalid response passed")
+
```

