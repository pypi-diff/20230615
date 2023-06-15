# Comparing `tmp/pymino-1.1.9.5.tar.gz` & `tmp/pymino-1.1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.9.4\dist\.tmp-2z2baa8d\pymino-1.1.9.5.tar", last modified: Thu Jun 15 01:42:13 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.9.4\dist\.tmp-jkpe4sap\pymino-1.1.9.6.tar", last modified: Thu Jun 15 01:48:57 2023, max compression
```

## Comparing `pymino-1.1.9.5.tar` & `pymino-1.1.9.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.827297 pymino-1.1.9.5/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.5/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-06-15 01:42:13.827793 pymino-1.1.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.761824 pymino-1.1.9.5/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-15 01:41:46.000000 pymino-1.1.9.5/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.5/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30128 2023-06-11 20:06:18.000000 pymino-1.1.9.5/pymino/bot.py
--rw-rw-rw-   0        0        0    52073 2023-06-13 03:02:06.000000 pymino-1.1.9.5/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.793596 pymino-1.1.9.5/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.5/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.5/pymino/ext/account.py
--rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.5/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.5/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24041 2023-06-15 01:41:25.000000 pymino-1.1.9.5/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.5/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.5/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.5/pymino/ext/console.py
--rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.5/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.5/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.811425 pymino-1.1.9.5/pymino/ext/entities/
--rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.5/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.5/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.5/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.5/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.5/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.5/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.5/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.5/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.5/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.5/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.5/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.5/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.5/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.5/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.5/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.825809 pymino-1.1.9.5/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.5/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.5/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.5/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.5/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.5/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.5/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.5/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.5/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.5/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:42:13.777722 pymino-1.1.9.5/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-06-15 01:42:13.000000 pymino-1.1.9.5/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1323 2023-06-15 01:42:13.000000 pymino-1.1.9.5/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:42:13.000000 pymino-1.1.9.5/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-15 01:42:13.000000 pymino-1.1.9.5/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 01:42:13.000000 pymino-1.1.9.5/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-15 01:42:13.829777 pymino-1.1.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.083114 pymino-1.1.9.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.9.6/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-15 01:48:57.083610 pymino-1.1.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.021114 pymino-1.1.9.6/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-15 01:48:31.000000 pymino-1.1.9.6/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-11 13:46:02.000000 pymino-1.1.9.6/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-15 01:47:51.000000 pymino-1.1.9.6/pymino/bot.py
+-rw-rw-rw-   0        0        0    52073 2023-06-13 03:02:06.000000 pymino-1.1.9.6/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.053354 pymino-1.1.9.6/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-11 16:50:39.000000 pymino-1.1.9.6/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.9.6/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.9.6/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-10 00:59:39.000000 pymino-1.1.9.6/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24041 2023-06-15 01:41:25.000000 pymino-1.1.9.6/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-11 14:03:00.000000 pymino-1.1.9.6/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   292004 2023-06-11 18:06:25.000000 pymino-1.1.9.6/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-11 22:20:09.000000 pymino-1.1.9.6/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    41963 2023-06-11 20:52:12.000000 pymino-1.1.9.6/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.9.6/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.070218 pymino-1.1.9.6/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.9.6/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.9.6/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.9.6/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.9.6/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.9.6/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-06-10 00:36:20.000000 pymino-1.1.9.6/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.9.6/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-11 21:21:53.000000 pymino-1.1.9.6/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.9.6/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.9.6/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.9.6/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.9.6/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.9.6/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.9.6/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-11 14:02:47.000000 pymino-1.1.9.6/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.082123 pymino-1.1.9.6/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-11 17:31:29.000000 pymino-1.1.9.6/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.9.6/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-13 04:27:21.000000 pymino-1.1.9.6/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.9.6/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-11 22:22:27.000000 pymino-1.1.9.6/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.9.6/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-11 21:47:35.000000 pymino-1.1.9.6/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-13 03:31:19.000000 pymino-1.1.9.6/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.9.6/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:48:57.037978 pymino-1.1.9.6/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1323 2023-06-15 01:48:57.000000 pymino-1.1.9.6/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 01:48:56.000000 pymino-1.1.9.6/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-15 01:48:57.089562 pymino-1.1.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.9.6/setup.py
```

### Comparing `pymino-1.1.9.5/LICENSE` & `pymino-1.1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/PKG-INFO` & `pymino-1.1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.5
+Version: 1.1.9.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.5/README.md` & `pymino-1.1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/__init__.py` & `pymino-1.1.9.6/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.5'
+__version__ = '1.1.9.6'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.5/pymino/async_bot.py` & `pymino-1.1.9.6/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/bot.py` & `pymino-1.1.9.6/pymino/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class Bot(WSClient):
     """
     `Bot` - This is the main client.
 
     `**Parameters**``
     - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
     - `community_id` - The community id to use for the bot. `Defaults` to `None`.
+    - `console_enabled` - Whether to enable the console. `Defaults` to `True`.
     - `device_id` - The device id to use for the bot. `Defaults` to `None`.
     - `intents` - Avoids receiving events that you do not need. `Defaults` to `False`.
     - `online_status` - Whether to set the bot's online status to `online`. `Defaults` to `True`.
     - `proxy` - The proxy to use for the bot. `Defaults` to `None`.
 
     ----------------------------
     When should I use `Bot` instead of `Client`?
@@ -206,16 +207,16 @@
         bot.run(email="email", password="password")
         ```
     """
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
-        device_id: str = None,
         console_enabled: bool = False,
+        device_id: str = None,
         intents: bool = False,
         online_status: bool = False,
         proxy: str = None
         ):
 
         self._debug:            bool = check_debugger()
         self._console_enabled:  bool = console_enabled
```

### Comparing `pymino-1.1.9.5/pymino/client.py` & `pymino-1.1.9.6/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/account.py` & `pymino-1.1.9.6/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/async_community.py` & `pymino-1.1.9.6/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/async_context.py` & `pymino-1.1.9.6/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/async_event_handler.py` & `pymino-1.1.9.6/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/async_socket.py` & `pymino-1.1.9.6/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/community.py` & `pymino-1.1.9.6/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/console.py` & `pymino-1.1.9.6/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/context.py` & `pymino-1.1.9.6/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/dispatcher.py` & `pymino-1.1.9.6/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/api_response.py` & `pymino-1.1.9.6/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/chat_threads.py` & `pymino-1.1.9.6/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/comments.py` & `pymino-1.1.9.6/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/enums.py` & `pymino-1.1.9.6/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/exceptions.py` & `pymino-1.1.9.6/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/general.py` & `pymino-1.1.9.6/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/handlers.py` & `pymino-1.1.9.6/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/link_info.py` & `pymino-1.1.9.6/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/messages.py` & `pymino-1.1.9.6/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/notification.py` & `pymino-1.1.9.6/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/userprofile.py` & `pymino-1.1.9.6/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/entities/wsevents.py` & `pymino-1.1.9.6/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/handle_queue.py` & `pymino-1.1.9.6/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/socket.py` & `pymino-1.1.9.6/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.9.6/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/chat_console.py` & `pymino-1.1.9.6/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/commands.py` & `pymino-1.1.9.6/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/community_console.py` & `pymino-1.1.9.6/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/generate.py` & `pymino-1.1.9.6/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/menu.py` & `pymino-1.1.9.6/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/profile_console.py` & `pymino-1.1.9.6/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino/ext/utilities/request_handler.py` & `pymino-1.1.9.6/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/pymino.egg-info/PKG-INFO` & `pymino-1.1.9.6/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.5
+Version: 1.1.9.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.9.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.9.5/pymino.egg-info/SOURCES.txt` & `pymino-1.1.9.6/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.5/setup.cfg` & `pymino-1.1.9.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e35 0d0a 6175  on = 1.1.9.5..au
+00000020: 6f6e 203d 2031 2e31 2e39 2e36 0d0a 6175  on = 1.1.9.6..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.5/setup.py` & `pymino-1.1.9.6/setup.py`

 * *Files identical despite different names*

