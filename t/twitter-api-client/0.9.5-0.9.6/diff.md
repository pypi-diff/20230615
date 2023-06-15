# Comparing `tmp/twitter-api-client-0.9.5.tar.gz` & `tmp/twitter-api-client-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.5.tar", last modified: Fri Jun  9 19:55:08 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.6.tar", last modified: Thu Jun 15 18:23:06 2023, max compression
```

## Comparing `twitter-api-client-0.9.5.tar` & `twitter-api-client-0.9.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.049420 twitter-api-client-0.9.5/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.5/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-09 19:55:08.049420 twitter-api-client-0.9.5/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-09 19:54:08.000000 twitter-api-client-0.9.5/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.5/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23626 2023-06-09 19:50:48.000000 twitter-api-client-0.9.5/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28718 2023-06-09 19:44:07.000000 twitter-api-client-0.9.5/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7382 2023-06-07 19:06:40.000000 twitter-api-client-0.9.5/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    33526 2023-06-09 19:47:45.000000 twitter-api-client-0.9.5/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6225 2023-06-09 19:50:48.000000 twitter-api-client-0.9.5/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-07 19:04:37.000000 twitter-api-client-0.9.5/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-09 19:55:08.048420 twitter-api-client-0.9.5/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-09 19:55:08.000000 twitter-api-client-0.9.5/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    11479 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    13412 2023-06-15 18:22:46.000000 twitter-api-client-0.9.6/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.604269 twitter-api-client-0.9.6/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.6/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    26861 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    30104 2023-06-15 18:20:32.000000 twitter-api-client-0.9.6/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-15 17:28:10.000000 twitter-api-client-0.9.6/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-15 17:31:50.000000 twitter-api-client-0.9.6/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.604269 twitter-api-client-0.9.6/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    11479 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.5/LICENSE` & `twitter-api-client-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.5/PKG-INFO` & `twitter-api-client-0.9.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.5
+Version: 0.9.6
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -37,16 +37,24 @@
 ```
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
+## sign-in with credentials
 email, username, password = ..., ..., ...
-account = Account(email, username, password, debug=2, save=True)
+account = Account(email, username, password)
+
+## or, resume session using cookies
+# account = Account(cookies={"ct0": ..., "auth_token": ...})
+
+## or, resume session using cookies (JSON file)
+# account = Account(cookies='twitter.cookies')
+
 
 account.tweet('test 123')
 account.untweet(123456)
 account.retweet(123456)
 account.unretweet(123456)
 account.reply('foo', tweet_id=123456)
 account.quote('bar', tweet_id=123456)
@@ -91,15 +99,15 @@
 account.unblock(1234)
 
 # user profile
 account.update_profile_image('test.jpg')
 account.update_profile_banner('test.png')
 account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
 
-#  topics
+# topics
 account.follow_topic(111)
 account.unfollow_topic(111)
 
 # lists
 account.create_list('My List', 'description of my list', private=False)
 account.update_list(222, 'My Updated List', 'some updated description', private=False)
 account.update_list_banner(222, 'test.png')
@@ -119,14 +127,23 @@
 # get timelines
 timeline = account.home_timeline()
 latest_timeline = account.home_latest_timeline(limit=500)
 
 # get bookmarks
 bookmarks = account.bookmarks()
 
+# get all dms
+dms = account.dm_history(['12345-67890'])
+
+# search dms
+dms = account.dm_search('test')
+
+# delete conversation
+account.dm_delete('12345-67890')
+
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
     "allow_dms_from": "following",
@@ -182,16 +199,27 @@
 ### Scraping
 
 #### Get all user/tweet data
 
 ```python
 from twitter.scraper import Scraper
 
+## sign-in with credentials
 email, username, password = ..., ..., ...
-scraper = Scraper(email, username, password, debug=1, save=True)
+scraper = Scraper(email, username, password)
+
+## or, resume session using cookies
+# scraper = Scraper(cookies={"ct0": ..., "auth_token": ...})
+
+## or, resume session using cookies (JSON file)
+# scraper = Scraper(cookies='twitter.cookies')
+
+## or, initialize guest session (limited endpoints)
+# from twitter.util import init_session
+# scraper = Scraper(session=init_session())
 
 # user data
 users = scraper.users(['foo', 'bar', 'hello', 'world'])
 users = scraper.users_by_ids([123, 234, 345])  # batch-request
 tweets = scraper.tweets([123, 234, 345])
 likes = scraper.likes([123, 234, 345])
 tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
@@ -223,15 +251,15 @@
 
 #### Resume Pagination
 **Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ...,...,...
-scraper = Scraper(email, username, password, debug=1, save=True)
+scraper = Scraper(email, username, password)
 
 user_id = 44196397
 cursor = '1767341853908517597|1663601806447476672'  # example cursor
 limit = 100  # arbitrary limit for demonstration
 follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
 
 # use last_cursor to resume pagination
@@ -240,15 +268,15 @@
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 # default output directory is `data/raw` if save=True
-search = Search(email, username, password, debug=1, save=True)
+search = Search(email, username, password)
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
@@ -281,56 +309,56 @@
 Capture live audio for up to 500 streams per IP
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 rooms = [...]
 scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
 ```
 
 #### Live Transcript Capture
 
 **Raw transcript chunks**
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # room must be live, i.e. in "Running" state
 scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
 ```
 
 **Processed (final) transcript chunks**
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # room must be live, i.e. in "Running" state
 scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
 ```
 
 #### Search and Metadata
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 from twitter.constants import SpaceCategory
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # download audio and chat-log from space
 spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
 
 # pull metadata only
 spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
 
@@ -361,10 +389,10 @@
 E.g.
 
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ..., ..., ...
 proton_email, proton_password = ..., ...
-account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+account = Scraper(email, username, password, protonmail={'email':proton_email, 'password':proton_password})
 ```
```

### Comparing `twitter-api-client-0.9.5/setup.py` & `twitter-api-client-0.9.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.5",
+    version="0.9.6",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
     
@@ -44,16 +44,24 @@
     ```
     
     ### Automation
     
     ```python
     from twitter.account import Account
     
+    ## sign-in with credentials
     email, username, password = ..., ..., ...
-    account = Account(email, username, password, debug=2, save=True)
+    account = Account(email, username, password)
+    
+    ## or, resume session using cookies
+    # account = Account(cookies={"ct0": ..., "auth_token": ...})
+    
+    ## or, resume session using cookies (JSON file)
+    # account = Account(cookies='twitter.cookies')
+    
     
     account.tweet('test 123')
     account.untweet(123456)
     account.retweet(123456)
     account.unretweet(123456)
     account.reply('foo', tweet_id=123456)
     account.quote('bar', tweet_id=123456)
@@ -98,15 +106,15 @@
     account.unblock(1234)
     
     # user profile
     account.update_profile_image('test.jpg')
     account.update_profile_banner('test.png')
     account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
     
-    #  topics
+    # topics
     account.follow_topic(111)
     account.unfollow_topic(111)
     
     # lists
     account.create_list('My List', 'description of my list', private=False)
     account.update_list(222, 'My Updated List', 'some updated description', private=False)
     account.update_list_banner(222, 'test.png')
@@ -126,14 +134,23 @@
     # get timelines
     timeline = account.home_timeline()
     latest_timeline = account.home_latest_timeline(limit=500)
     
     # get bookmarks
     bookmarks = account.bookmarks()
     
+    # get all dms
+    dms = account.dm_history(['12345-67890'])
+    
+    # search dms
+    dms = account.dm_search('test')
+    
+    # delete conversation
+    account.dm_delete('12345-67890')
+    
     # example configuration
     account.update_settings({
         "address_book_live_sync_enabled": False,
         "allow_ads_personalization": False,
         "allow_authenticated_periscope_requests": True,
         "allow_dm_groups_from": "following",
         "allow_dms_from": "following",
@@ -189,16 +206,27 @@
     ### Scraping
     
     #### Get all user/tweet data
     
     ```python
     from twitter.scraper import Scraper
     
+    ## sign-in with credentials
     email, username, password = ..., ..., ...
-    scraper = Scraper(email, username, password, debug=1, save=True)
+    scraper = Scraper(email, username, password)
+    
+    ## or, resume session using cookies
+    # scraper = Scraper(cookies={"ct0": ..., "auth_token": ...})
+    
+    ## or, resume session using cookies (JSON file)
+    # scraper = Scraper(cookies='twitter.cookies')
+    
+    ## or, initialize guest session (limited endpoints)
+    # from twitter.util import init_session
+    # scraper = Scraper(session=init_session())
     
     # user data
     users = scraper.users(['foo', 'bar', 'hello', 'world'])
     users = scraper.users_by_ids([123, 234, 345])  # batch-request
     tweets = scraper.tweets([123, 234, 345])
     likes = scraper.likes([123, 234, 345])
     tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
@@ -230,15 +258,15 @@
     
     #### Resume Pagination
     **Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
     ```python
     from twitter.scraper import Scraper
     
     email, username, password = ...,...,...
-    scraper = Scraper(email, username, password, debug=1, save=True)
+    scraper = Scraper(email, username, password)
     
     user_id = 44196397
     cursor = '1767341853908517597|1663601806447476672'  # example cursor
     limit = 100  # arbitrary limit for demonstration
     follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
     
     # use last_cursor to resume pagination
@@ -247,15 +275,15 @@
     #### Search
     
     ```python   
     from twitter.search import Search
     
     email, username, password = ..., ..., ...
     # default output directory is `data/raw` if save=True
-    search = Search(email, username, password, debug=1, save=True)
+    search = Search(email, username, password)
     
     latest_results = search.run(
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'ios android',
         limit=100,
         latest=True,  # get latest tweets only
@@ -288,56 +316,56 @@
     Capture live audio for up to 500 streams per IP
     
     ```python
     from twitter.scraper import Scraper
     from twitter.util import init_session
     
     session = init_session() # initialize guest session, no login required
-    scraper = Scraper(session=session, debug=1, save=True)
+    scraper = Scraper(session=session)
     
     rooms = [...]
     scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
     ```
     
     #### Live Transcript Capture
     
     **Raw transcript chunks**
     
     ```python
     from twitter.scraper import Scraper
     from twitter.util import init_session
     
     session = init_session() # initialize guest session, no login required
-    scraper = Scraper(session=session, debug=1, save=True)
+    scraper = Scraper(session=session)
     
     # room must be live, i.e. in "Running" state
     scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
     ```
     
     **Processed (final) transcript chunks**
     
     ```python
     from twitter.scraper import Scraper
     from twitter.util import init_session
     
     session = init_session() # initialize guest session, no login required
-    scraper = Scraper(session=session, debug=1, save=True)
+    scraper = Scraper(session=session)
     
     # room must be live, i.e. in "Running" state
     scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
     ```
     
     #### Search and Metadata
     ```python
     from twitter.scraper import Scraper
     from twitter.util import init_session
     from twitter.constants import SpaceCategory
     
     session = init_session() # initialize guest session, no login required
-    scraper = Scraper(session=session, debug=1, save=True)
+    scraper = Scraper(session=session)
     
     # download audio and chat-log from space
     spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
     
     # pull metadata only
     spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
     
@@ -368,15 +396,15 @@
     E.g.
     
     ```python
     from twitter.scraper import Scraper
     
     email, username, password = ..., ..., ...
     proton_email, proton_password = ..., ...
-    account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+    account = Scraper(email, username, password, protonmail={'email':proton_email, 'password':proton_password})
     ```
     
     '''),
     long_description_content_type='text/markdown',
     author="Trevor Hobenshield",
     author_email="trevorhobenshield@gmail.com",
     url="https://github.com/trevorhobenshield/twitter-api-client",
```

### Comparing `twitter-api-client-0.9.5/twitter/account.py` & `twitter-api-client-0.9.6/twitter/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import asyncio
 import hashlib
 import logging.config
 import math
 import mimetypes
 import platform
 import random
 from copy import deepcopy
 from datetime import datetime
 from string import ascii_letters
 from uuid import uuid1, getnode
 
+from httpx import AsyncClient, Limits
 from tqdm import tqdm
+from tqdm.asyncio import tqdm_asyncio
 
 from .constants import *
 from .login import login
 from .util import *
 
 try:
     if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
@@ -572,15 +575,92 @@
                 logging.getLogger(name).setLevel(logging.ERROR)
 
         return logging.getLogger(logger_name)
 
     @staticmethod
     def _validate_session(*args, **kwargs):
         email, username, password, session = args
+
+        # validate credentials
+        if all((email, username, password)):
+            return login(email, username, password, **kwargs)
+
+        # invalid credentials, try validating session
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
             return session
-        if not session:
-            # no session provided, login to authenticate
-            return login(email, username, password, **kwargs)
+
+        # invalid credentials and session
+        cookies = kwargs.get('cookies')
+
+        # try validating cookies dict
+        if isinstance(cookies, dict) and all(cookies.get(c) for c in {'ct0', 'auth_token'}):
+            _session = Client(cookies=cookies, follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
+        # try validating cookies from file
+        if isinstance(cookies, str):
+            _session = Client(cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
         raise Exception('Session not authenticated. '
                         'Please use an authenticated session or remove the `session` argument and try again.')
+
+    def dm_history(self, conversation_ids: list[str]) -> list[dict]:
+        async def get(session: AsyncClient, conversation_id: str):
+            params = deepcopy(dm_history_params)
+            r = await session.get(
+                f'{self.v1_api}/dm/conversation/{conversation_id}.json',
+                params=params,
+            )
+            res = r.json().get('conversation_timeline', {})
+            data = [x['message'] for x in res.get('entries', [])]
+            entry_id = res.get('min_entry_id')
+            while entry_id:
+                params['max_id'] = entry_id
+                r = await session.get(
+                    f'{self.v1_api}/dm/conversation/{conversation_id}.json',
+                    params=params,
+                )
+                res = r.json().get('conversation_timeline', {})
+                data.extend(x['message'] for x in res.get('entries', []))
+                entry_id = res.get('min_entry_id')
+            return data
+
+        async def process():
+            limits = Limits(max_connections=100)
+            headers, cookies = get_headers(self.session), self.session.cookies
+            async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
+                return await tqdm_asyncio.gather(*(get(c, _id) for _id in conversation_ids), desc="Getting DMs")
+
+        return asyncio.run(process())
+
+    def dm_delete(self, conversation_id: str):
+        return self.session.post(
+            f'{self.v1_api}/dm/conversation/{conversation_id}/delete.json',
+            headers=get_headers(self.session),
+        )
+
+    def dm_search(self, query: str):
+        def get(cursor=None):
+            if cursor:
+                params['variables']['cursor'] = cursor.pop()
+            _id, op = Operation.DmAllSearchSlice
+            r = self.session.get(
+                f'https://twitter.com/i/api/graphql/{_id}/{op}',
+                params=build_params(params)
+            )
+            res = r.json()
+            cursor = find_key(res, 'next_cursor')
+            return res, cursor
+
+        variables = deepcopy(Operation.default_variables)
+        variables['count'] = 50  # strict limit, errors thrown if exceeded
+        variables['query'] = query
+        params = {'variables': variables, 'features': Operation.default_features}
+        res, cursor = get()
+        data = [res]
+        while cursor:
+            res, cursor = get(cursor)
+            data.append(res)
+        return {'query': query, 'data': data}
```

### Comparing `twitter-api-client-0.9.5/twitter/constants.py` & `twitter-api-client-0.9.6/twitter/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     DeleteDraftTweet = 'bkh9G3FGgTldS9iTKWWYYw', 'DeleteDraftTweet'
     DeletePaymentMethod = 'VaaLGwK5KNLoc7wsOmp4uw', 'DeletePaymentMethod'
     DeleteTweetDownvote = 'VNEvEGXaUAMfiExP8Tbezw', 'DeleteTweetDownvote'
     DeleteTweetReaction = 'GKwK0Rj4EdkfwdHQMZTpuw', 'DeleteTweetReaction'
     DisableUserAccountLabel = '_ckHEj05gan2VfNHG6thBA', 'DisableUserAccountLabel'
     DisableVerifiedPhoneLabel = 'g2m0pAOamawNtVIfjXNMJg', 'DisableVerifiedPhoneLabel'
     DismissRitoSuggestedAction = 'jYvwa61cv3NwNP24iUru6g', 'DismissRitoSuggestedAction'
-    DmAllSearchSlice = '9qd2xqJkMURKSyXVJ33xBw', 'DmAllSearchSlice'
+    DmAllSearchSlice = 'U-QXVRZ6iddb1QuZweh5DQ', 'DmAllSearchSlice'
     DmGroupSearchSlice = '5zpY1dCR-8NyxQJS_CFJoQ', 'DmGroupSearchSlice'
     DmMutedTimeline = 'lrcWa13oyrQc7L33wRdLAQ', 'DmMutedTimeline'
     DmNsfwMediaFilterUpdate = 'of_N6O33zfyD4qsFJMYFxA', 'DmNsfwMediaFilterUpdate'
     DmPeopleSearchSlice = 'xYSm8m5kJnzm_gFCn5GH-w', 'DmPeopleSearchSlice'
     EditBookmarkFolder = 'a6kPp1cS1Dgbsjhapz1PNw', 'EditBookmarkFolder'
     EditDraftTweet = 'JIeXE-I6BZXHfxsgOkyHYQ', 'EditDraftTweet'
     EditScheduledTweet = '_mHkQ5LHpRRjSXKOcG6eZw', 'EditScheduledTweet'
@@ -340,14 +340,18 @@
         'withSuperFollowsUserFields': True,
         'withReactionsMetadata': False,
         'withReactionsPerspective': False,
         'withSuperFollowsTweetFields': True,
         'isMetatagsQuery': False,
         'withReplays': True,
         'withClientEventToken': False,
+        'withAttachments': True,
+        'withConversationQueryHighlights': True,
+        'withMessageQueryHighlights': True,
+        'withMessages': True,
     }
     default_features = {
         "blue_business_profile_image_shape_enabled": True,
         "creator_subscriptions_tweet_preview_api_enabled": True,
         "freedom_of_speech_not_reach_fetch_enabled": False,
         "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
         "graphql_timeline_v2_bookmark_timeline": True,
@@ -552,7 +556,41 @@
     'q': '',
     'requestContext': 'launch',
     'pc': 1,
     'spelling_corrections': 1,
     'include_ext_edit_control': 'true',
     'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe'
 }
+
+dm_history_params = {
+    'context': 'FETCH_DM_CONVERSATION',
+    'include_profile_interstitial_type': '1',
+    'include_blocking': '1',
+    'include_blocked_by': '1',
+    'include_followed_by': '1',
+    'include_want_retweets': '1',
+    'include_mute_edge': '1',
+    'include_can_dm': '1',
+    'include_can_media_tag': '1',
+    'include_ext_has_nft_avatar': '1',
+    'include_ext_is_blue_verified': '1',
+    'include_ext_verified_type': '1',
+    'include_ext_profile_image_shape': '1',
+    'skip_status': '1',
+    'dm_secret_conversations_enabled': 'false',
+    'krs_registration_enabled': 'true',
+    'cards_platform': 'Web-12',
+    'include_cards': '1',
+    'include_ext_alt_text': 'true',
+    'include_ext_limited_action_results': 'false',
+    'include_quote_count': 'true',
+    'include_reply_count': '1',
+    'tweet_mode': 'extended',
+    'include_ext_views': 'true',
+    'dm_users': 'false',
+    'include_groups': 'true',
+    'include_inbox_timelines': 'true',
+    'include_ext_media_color': 'true',
+    'supports_reactions': 'true',
+    'include_conversation_info': 'true',
+    'ext': 'mediaColor,altText,mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,superFollowMetadata,unmentionInfo,editControl',
+}
```

### Comparing `twitter-api-client-0.9.5/twitter/login.py` & `twitter-api-client-0.9.6/twitter/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,17 @@
         },
         headers={
             'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             'content-type': 'application/json',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'en',
-        })
+        },
+        follow_redirects=True
+    )
 
     # client.protonmail = kwargs.get('protonmail')
 
     client = execute_login_flow(client)
     if kwargs.get('debug'):
         if not client or client.cookies.get('flow_errors') == 'true':
             print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
```

### Comparing `twitter-api-client-0.9.5/twitter/scraper.py` & `twitter-api-client-0.9.6/twitter/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,16 +785,35 @@
             if name != logger_name:
                 logging.getLogger(name).setLevel(logging.ERROR)
 
         return logging.getLogger(logger_name)
 
     def _validate_session(self, *args, **kwargs):
         email, username, password, session = args
+
+        # validate credentials
+        if all((email, username, password)):
+            return login(email, username, password, **kwargs)
+
+        # invalid credentials, try validating session
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
             return session
-        if not session:
-            # no session provided, log-in to authenticate
-            return login(email, username, password, **kwargs)
+
+        # invalid credentials and session
+        cookies = kwargs.get('cookies')
+
+        # try validating cookies dict
+        if isinstance(cookies, dict) and all(cookies.get(c) for c in {'ct0', 'auth_token'}):
+            _session = Client(cookies=cookies, follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
+        # try validating cookies from file
+        if isinstance(cookies, str):
+            _session = Client(cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
+        # no session, credentials, or cookies provided. use guest session.
         self.logger.warning(f'{RED}This is a guest session, some endpoints cannot be accessed.{RESET}\n')
         self.guest = True
         return session
```

### Comparing `twitter-api-client-0.9.5/twitter/search.py` & `twitter-api-client-0.9.6/twitter/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,15 +150,33 @@
                 logging.getLogger(name).setLevel(logging.ERROR)
 
         return logging.getLogger(logger_name)
 
     @staticmethod
     def _validate_session(*args, **kwargs):
         email, username, password, session = args
+
+        # validate credentials
+        if all((email, username, password)):
+            return login(email, username, password, **kwargs)
+
+        # invalid credentials, try validating session
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
             return session
-        if not session:
-            # no session provided, log-in to authenticate
-            return login(email, username, password, **kwargs)
+
+        # invalid credentials and session
+        cookies = kwargs.get('cookies')
+
+        # try validating cookies dict
+        if isinstance(cookies, dict) and all(cookies.get(c) for c in {'ct0', 'auth_token'}):
+            _session = Client(cookies=cookies, follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
+        # try validating cookies from file
+        if isinstance(cookies, str):
+            _session = Client(cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True)
+            _session.headers.update(get_headers(_session))
+            return _session
+
         raise Exception('Session not authenticated. '
                         'Please use an authenticated session or remove the `session` argument and try again.')
```

### Comparing `twitter-api-client-0.9.5/twitter/util.py` & `twitter-api-client-0.9.6/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.5/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.6/twitter_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.5
+Version: 0.9.6
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -37,16 +37,24 @@
 ```
 
 ### Automation
 
 ```python
 from twitter.account import Account
 
+## sign-in with credentials
 email, username, password = ..., ..., ...
-account = Account(email, username, password, debug=2, save=True)
+account = Account(email, username, password)
+
+## or, resume session using cookies
+# account = Account(cookies={"ct0": ..., "auth_token": ...})
+
+## or, resume session using cookies (JSON file)
+# account = Account(cookies='twitter.cookies')
+
 
 account.tweet('test 123')
 account.untweet(123456)
 account.retweet(123456)
 account.unretweet(123456)
 account.reply('foo', tweet_id=123456)
 account.quote('bar', tweet_id=123456)
@@ -91,15 +99,15 @@
 account.unblock(1234)
 
 # user profile
 account.update_profile_image('test.jpg')
 account.update_profile_banner('test.png')
 account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
 
-#  topics
+# topics
 account.follow_topic(111)
 account.unfollow_topic(111)
 
 # lists
 account.create_list('My List', 'description of my list', private=False)
 account.update_list(222, 'My Updated List', 'some updated description', private=False)
 account.update_list_banner(222, 'test.png')
@@ -119,14 +127,23 @@
 # get timelines
 timeline = account.home_timeline()
 latest_timeline = account.home_latest_timeline(limit=500)
 
 # get bookmarks
 bookmarks = account.bookmarks()
 
+# get all dms
+dms = account.dm_history(['12345-67890'])
+
+# search dms
+dms = account.dm_search('test')
+
+# delete conversation
+account.dm_delete('12345-67890')
+
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
     "allow_dms_from": "following",
@@ -182,16 +199,27 @@
 ### Scraping
 
 #### Get all user/tweet data
 
 ```python
 from twitter.scraper import Scraper
 
+## sign-in with credentials
 email, username, password = ..., ..., ...
-scraper = Scraper(email, username, password, debug=1, save=True)
+scraper = Scraper(email, username, password)
+
+## or, resume session using cookies
+# scraper = Scraper(cookies={"ct0": ..., "auth_token": ...})
+
+## or, resume session using cookies (JSON file)
+# scraper = Scraper(cookies='twitter.cookies')
+
+## or, initialize guest session (limited endpoints)
+# from twitter.util import init_session
+# scraper = Scraper(session=init_session())
 
 # user data
 users = scraper.users(['foo', 'bar', 'hello', 'world'])
 users = scraper.users_by_ids([123, 234, 345])  # batch-request
 tweets = scraper.tweets([123, 234, 345])
 likes = scraper.likes([123, 234, 345])
 tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
@@ -223,15 +251,15 @@
 
 #### Resume Pagination
 **Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ...,...,...
-scraper = Scraper(email, username, password, debug=1, save=True)
+scraper = Scraper(email, username, password)
 
 user_id = 44196397
 cursor = '1767341853908517597|1663601806447476672'  # example cursor
 limit = 100  # arbitrary limit for demonstration
 follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
 
 # use last_cursor to resume pagination
@@ -240,15 +268,15 @@
 #### Search
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 # default output directory is `data/raw` if save=True
-search = Search(email, username, password, debug=1, save=True)
+search = Search(email, username, password)
 
 latest_results = search.run(
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'ios android',
     limit=100,
     latest=True,  # get latest tweets only
@@ -281,56 +309,56 @@
 Capture live audio for up to 500 streams per IP
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 rooms = [...]
 scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
 ```
 
 #### Live Transcript Capture
 
 **Raw transcript chunks**
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # room must be live, i.e. in "Running" state
 scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
 ```
 
 **Processed (final) transcript chunks**
 
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # room must be live, i.e. in "Running" state
 scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
 ```
 
 #### Search and Metadata
 ```python
 from twitter.scraper import Scraper
 from twitter.util import init_session
 from twitter.constants import SpaceCategory
 
 session = init_session() # initialize guest session, no login required
-scraper = Scraper(session=session, debug=1, save=True)
+scraper = Scraper(session=session)
 
 # download audio and chat-log from space
 spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
 
 # pull metadata only
 spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
 
@@ -361,10 +389,10 @@
 E.g.
 
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ..., ..., ...
 proton_email, proton_password = ..., ...
-account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
+account = Scraper(email, username, password, protonmail={'email':proton_email, 'password':proton_password})
 ```
```

