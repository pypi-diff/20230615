# Comparing `tmp/stackoverflowapithingy-0.1.7.tar.gz` & `tmp/stackoverflowapithingy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoverflowapithingy-0.1.7.tar", last modified: Thu Jun 15 11:53:33 2023, max compression
+gzip compressed data, was "stackoverflowapithingy-0.1.8.tar", last modified: Thu Jun 15 12:02:32 2023, max compression
```

## Comparing `stackoverflowapithingy-0.1.7.tar` & `stackoverflowapithingy-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.653395 stackoverflowapithingy-0.1.7/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:53:33.653291 stackoverflowapithingy-0.1.7/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 11:53:33.653437 stackoverflowapithingy-0.1.7/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 11:53:30.000000 stackoverflowapithingy-0.1.7/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.652588 stackoverflowapithingy-0.1.7/stackoverflowapithingy/
--rw-r--r--   0 benjamin   (501) staff       (20)      140 2023-06-15 11:41:43.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1485 2023-06-15 11:19:18.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy/stackoverflow.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 11:53:33.653136 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      312 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 11:53:33.000000 stackoverflowapithingy-0.1.7/stackoverflowapithingy.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.780705 stackoverflowapithingy-0.1.8/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 12:02:32.780598 stackoverflowapithingy-0.1.8/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-06-15 12:02:32.780750 stackoverflowapithingy-0.1.8/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      276 2023-06-15 12:02:15.000000 stackoverflowapithingy-0.1.8/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.779882 stackoverflowapithingy-0.1.8/stackoverflowapithingy/
+-rw-r--r--   0 benjamin   (501) staff       (20)      140 2023-06-15 11:41:43.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1625 2023-06-15 12:00:52.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy/stackoverflow.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-06-15 12:02:32.780453 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)      247 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      312 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        9 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       23 2023-06-15 12:02:32.000000 stackoverflowapithingy-0.1.8/stackoverflowapithingy.egg-info/top_level.txt
```

### Comparing `stackoverflowapithingy-0.1.7/stackoverflowapithingy/stackoverflow.py` & `stackoverflowapithingy-0.1.8/stackoverflowapithingy/stackoverflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import requests
 
 #settings = {"q_per_page":1,"accepted":True,"sort":3,"default_tags":["python"]}
 def whatIsSettings():
     return "settings = {\"q_per_page\":1,\"accepted\":True,\"sort\":3,\"default_tags\":[\"python\"]}\noh and sort order is activity, votes, creation, relevance\nalso tags should be an array :)"
 
 
-def getQuestionByTags(tags,settings): #tags is array
+def getQuestionByTags(tags=["python"],settings={"q_per_page":1,"accepted":True,"sort":3,"default_tags":["python"]}): #tags is array
     formattedtags = ";".join(tags)
     url = "https://api.stackexchange.com/2.2/questions?pagesize={0}&order=desc&sort=votes&tagged={1}&site=stackoverflow&filter=withbody".format(str(settings["q_per_page"]),formattedtags)
     return requests.get(url).json() #returns question object(s)
 
 
-def getQuestionBySearch(query,tags,settings):
+def getQuestionBySearch(query,tags=["python"],settings={"q_per_page":1,"accepted":True,"sort":3,"default_tags":["python"]}):
     formattedtags = ";".join(tags)
     url = "https://api.stackexchange.com/2.3/search/advanced?pagesize={0}&order=desc&sort={1}&q={2}&accepted={3}&tagged={4}&site=stackoverflow&filter=withbody".format(settings["q_per_page"],["activity","votes","creation","relevance"][settings["sort"]],query,settings["accepted"],formattedtags)
     return requests.get(url).json()
 
-def getAnswerByQuestion(question_id,settings):
+def getAnswerByQuestion(question_id):
     url = "https://api.stackexchange.com/2.3/questions/{0}/answers?order=desc&site=stackoverflow&filter=withbody".format(question_id)
     return requests.get(url).json()
 
 
-def getAnswerById(answer_id,settings):
+def getAnswerById(answer_id):
     url = "https://api.stackexchange.com/2.3/answers/{0}?order=desc&site=stackoverflow&filter=withbody".format(answer_id)
     return requests.get(url).json()
```

