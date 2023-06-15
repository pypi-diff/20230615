# Comparing `tmp/rubpy-6.2.2.tar.gz` & `tmp/rubpy-6.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.2.2.tar", last modified: Wed Jun 14 19:18:24 2023, max compression
+gzip compressed data, was "rubpy-6.2.3.tar", last modified: Thu Jun 15 19:40:27 2023, max compression
```

## Comparing `rubpy-6.2.2.tar` & `rubpy-6.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/
--rw-rw-rw-   0        0        0     3378 2023-06-14 19:18:24.262907 rubpy-6.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.236270 rubpy-6.2.2/rubpy/
--rw-rw-rw-   0        0        0      240 2023-06-14 19:18:12.000000 rubpy-6.2.2/rubpy/__init__.py
--rw-rw-rw-   0        0        0    42576 2023-06-14 18:57:48.000000 rubpy-6.2.2/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.247281 rubpy-6.2.2/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.2/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.2/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.2/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    26944 2023-06-14 18:58:42.000000 rubpy-6.2.2/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.2/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    11374 2023-06-14 11:44:44.000000 rubpy-6.2.2/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.2/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.262907 rubpy-6.2.2/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.2/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.2/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:18:24.247281 rubpy-6.2.2/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 19:18:24.000000 rubpy-6.2.2/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 19:18:24.262907 rubpy-6.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-06-14 19:18:00.000000 rubpy-6.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.927990 rubpy-6.2.3/
+-rw-rw-rw-   0        0        0     3378 2023-06-15 19:40:27.927014 rubpy-6.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.881141 rubpy-6.2.3/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-06-15 19:34:03.000000 rubpy-6.2.3/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    42819 2023-06-15 19:40:07.000000 rubpy-6.2.3/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.906520 rubpy-6.2.3/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.3/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.917255 rubpy-6.2.3/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.3/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.3/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.3/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.3/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.921161 rubpy-6.2.3/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11374 2023-06-14 11:44:44.000000 rubpy-6.2.3/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.923111 rubpy-6.2.3/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.3/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.927014 rubpy-6.2.3/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.3/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.3/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:40:27.904565 rubpy-6.2.3/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-06-15 19:40:27.000000 rubpy-6.2.3/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-06-15 19:40:27.000000 rubpy-6.2.3/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:40:27.000000 rubpy-6.2.3/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-15 19:40:27.000000 rubpy-6.2.3/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 19:40:27.000000 rubpy-6.2.3/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:40:27.927990 rubpy-6.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-06-15 19:33:52.000000 rubpy-6.2.3/setup.py
```

### Comparing `rubpy-6.2.2/PKG-INFO` & `rubpy-6.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.2
+Version: 6.2.3
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.2 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.3 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.2/README.md` & `rubpy-6.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/client.py` & `rubpy-6.2.3/rubpy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -835,14 +835,19 @@
 
     async def get_messages(self, object_guid: str, min_id: int, max_id: int, sort: str = 'FromMin', limit: int = 10):
         return await self(methods.messages.GetMessages(object_guid, min_id, max_id, sort, limit))
 
     async def get_messages_interval(self, object_guid: str, middle_message_id: str):
         return await self(methods.messages.GetMessagesInterval(object_guid, middle_message_id))
 
+    async def get_message_url(self, object_guid: str, message_id: int):
+        if type(message_id) == str:
+            message_id = int(message_id)
+        return await self(methods.messages.GetMessageShareUrl(object_guid, message_id))
+
 # ---------------- Channels Methods ----------------
 
     async def add_channel(self, title: str, description: str = None):
         return await self(methods.channels.AddChannel(title, description))
 
     async def remove_channel(self, channel_guid: str):
         return await self(methods.channels.RemoveChannel(channel_guid))
```

### Comparing `rubpy-6.2.2/rubpy/crypto/crypto.py` & `rubpy-6.2.3/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/gadgets/classino.py` & `rubpy-6.2.3/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/gadgets/exceptions.py` & `rubpy-6.2.3/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/gadgets/grouping.py` & `rubpy-6.2.3/rubpy/gadgets/grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,14 +373,20 @@
             }
         },
         "GetMessagesInterval": {
             "params": {
                 "object_guid": {"types": "str"},
                 "middle_message_id": {"types": ["str", "int"], "func": "to_string"},
             }
+        },
+        "GetMessageShareUrl": {
+            "params": {
+                "object_guid": {"types": "str"},
+                "message_id": {"types": ["str", "int"]},
+            }
         }
     },
     "channels": {
         "Values": ["Join", "Remove", "Archive", "Set", "Unset"],
         "AddChannel": {
             "params": {
                 "title": {"types": "str"},
```

### Comparing `rubpy-6.2.2/rubpy/gadgets/methods.py` & `rubpy-6.2.3/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/gadgets/thumbnail.py` & `rubpy-6.2.3/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/network/connection.py` & `rubpy-6.2.3/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/network/proxies.py` & `rubpy-6.2.3/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.3/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/sessions/stringSession.py` & `rubpy-6.2.3/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/structs/handlers.py` & `rubpy-6.2.3/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/structs/models.py` & `rubpy-6.2.3/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/structs/results.py` & `rubpy-6.2.3/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy/structs/struct.py` & `rubpy-6.2.3/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.3/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.2
+Version: 6.2.3
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.2 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.3 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.2/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.3/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.2/setup.py` & `rubpy-6.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.2.2',
+    version = '6.2.3',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

