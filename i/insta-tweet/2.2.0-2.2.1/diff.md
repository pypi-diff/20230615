# Comparing `tmp/insta-tweet-2.2.0.tar.gz` & `tmp/insta-tweet-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insta-tweet-2.2.0.tar", last modified: Tue May  9 03:37:56 2023, max compression
+gzip compressed data, was "insta-tweet-2.2.1.tar", last modified: Thu Jun 15 09:05:16 2023, max compression
```

## Comparing `insta-tweet-2.2.0.tar` & `insta-tweet-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/
-drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.869286 insta-tweet-2.2.0/InstaTweet/
--rw-rw-rw-   0        0        0      325 2023-05-09 03:33:58.000000 insta-tweet-2.2.0/InstaTweet/__init__.py
--rw-rw-rw-   0        0        0     5070 2023-05-09 03:04:05.000000 insta-tweet-2.2.0/InstaTweet/db.py
--rw-rw-rw-   0        0        0     6775 2023-05-09 03:18:47.000000 insta-tweet-2.2.0/InstaTweet/instaclient.py
--rw-rw-rw-   0        0        0     6257 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instapage.py
--rw-rw-rw-   0        0        0     4852 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instapost.py
--rw-rw-rw-   0        0        0     6084 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/instatweet.py
--rw-rw-rw-   0        0        0    15926 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/profile.py
--rw-rw-rw-   0        0        0     7454 2023-05-09 03:04:21.000000 insta-tweet-2.2.0/InstaTweet/tweetclient.py
--rw-rw-rw-   0        0        0     1695 2023-05-04 08:44:04.000000 insta-tweet-2.2.0/InstaTweet/utils.py
--rw-rw-rw-   0        0        0     1084 2023-04-27 09:24:17.000000 insta-tweet-2.2.0/LICENSE
--rw-rw-rw-   0        0        0     7764 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6812 2023-05-09 03:36:31.000000 insta-tweet-2.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/insta_tweet.egg-info/
--rw-rw-rw-   0        0        0     7764 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 03:37:56.000000 insta-tweet-2.2.0/insta_tweet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 03:37:56.884994 insta-tweet-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-09 03:32:35.000000 insta-tweet-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:05:16.598057 insta-tweet-2.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-15 09:05:16.598057 insta-tweet-2.2.1/InstaTweet/
+-rw-rw-rw-   0        0        0      325 2023-06-15 09:01:54.000000 insta-tweet-2.2.1/InstaTweet/__init__.py
+-rw-rw-rw-   0        0        0     5070 2023-05-09 03:04:05.000000 insta-tweet-2.2.1/InstaTweet/db.py
+-rw-rw-rw-   0        0        0     7652 2023-06-15 08:55:58.000000 insta-tweet-2.2.1/InstaTweet/instaclient.py
+-rw-rw-rw-   0        0        0     6257 2023-05-09 03:04:21.000000 insta-tweet-2.2.1/InstaTweet/instapage.py
+-rw-rw-rw-   0        0        0     4976 2023-06-15 08:51:27.000000 insta-tweet-2.2.1/InstaTweet/instapost.py
+-rw-rw-rw-   0        0        0     6084 2023-05-09 03:04:21.000000 insta-tweet-2.2.1/InstaTweet/instatweet.py
+-rw-rw-rw-   0        0        0    15926 2023-05-09 03:04:21.000000 insta-tweet-2.2.1/InstaTweet/profile.py
+-rw-rw-rw-   0        0        0     7454 2023-05-09 03:04:21.000000 insta-tweet-2.2.1/InstaTweet/tweetclient.py
+-rw-rw-rw-   0        0        0     1695 2023-05-04 08:44:04.000000 insta-tweet-2.2.1/InstaTweet/utils.py
+-rw-rw-rw-   0        0        0     1084 2023-04-27 09:24:17.000000 insta-tweet-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7764 2023-06-15 09:05:16.598057 insta-tweet-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6812 2023-06-15 09:01:21.000000 insta-tweet-2.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 09:05:16.598057 insta-tweet-2.2.1/insta_tweet.egg-info/
+-rw-rw-rw-   0        0        0     7764 2023-06-15 09:05:16.000000 insta-tweet-2.2.1/insta_tweet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-06-15 09:05:16.000000 insta-tweet-2.2.1/insta_tweet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:05:16.000000 insta-tweet-2.2.1/insta_tweet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-15 09:05:16.000000 insta-tweet-2.2.1/insta_tweet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 09:05:16.000000 insta-tweet-2.2.1/insta_tweet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:05:16.598057 insta-tweet-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-09 04:01:05.000000 insta-tweet-2.2.1/setup.py
```

### Comparing `insta-tweet-2.2.0/InstaTweet/db.py` & `insta-tweet-2.2.1/InstaTweet/db.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/InstaTweet/instaclient.py` & `insta-tweet-2.2.1/InstaTweet/instaclient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import requests
 from requests import Response
 from typing import Type, Union, Optional, Dict
 from json.decoder import JSONDecodeError
 from . import InstaPage, InstaUser, InstaPost, Hashtag
 
 
@@ -79,14 +80,34 @@
         :param username: the username of the IG user to scrape
         """
         username = username.lstrip('@')
         endpoint = f"https://i.instagram.com/api/v1/users/web_profile_info/?username={username}"
         response = self.request(endpoint)
         return self._wrap(username, response, InstaUser)
 
+    def get_post(self, shortcode: str) -> Optional[InstaPost]:
+        """Scrapes an Instagram post by shortcode or URL
+
+        :param shortcode: the shortcode or URL of the post
+        """
+        if shortcode.startswith('http'):
+            match = re.match(
+                pattern=r"(?:https?://)?w{0,3}\.?instagram\.com/\w+/([\w-]+)/?",
+                string=shortcode
+            )
+            if match:
+                shortcode = match.group(1)
+            else:
+                return print(f"{shortcode} is not a valid Instagram shortcode or URL")
+
+        endpoint = f'https://www.instagram.com/graphql/query?query_hash=2b0673e0dc4580674a88d426fe00ea90' \
+                   f'&variables=%7B%22shortcode%22%3A%22{shortcode}%22%7D'
+        response = self.request(endpoint)
+        return self._wrap(shortcode, response, InstaPost)
+
     def _wrap(self, page: str, response: Response, Wrapper: Type[InstaPage]) -> InstaPage:
         """Validates and wraps the API response from an Instagram page
         """
         page = f'user @{page}' if Wrapper is InstaUser else f'hashtag #{page}'
         if response.ok:
             try:
                 return Wrapper(response.json(), self)
```

### Comparing `insta-tweet-2.2.0/InstaTweet/instapage.py` & `insta-tweet-2.2.1/InstaTweet/instapage.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/InstaTweet/instapost.py` & `insta-tweet-2.2.1/InstaTweet/instapost.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     """Minimalistic API response wrapper for an Instagram post"""
 
     def __init__(self, data: dict, client: Optional["InstaClient"] = None):
         """Initialize an :class:`~InstaPost`
 
         :param data: the JSON response data of a single Instagram post, found within the :attr:`~.InstaUser.user_data`
         """
+        if 'data' in data:  # If scraped from ``get_post()``
+            data = data['data'].get('shortcode_media', {})
+
         #: Source data from API response
         self.json = data
         self.client = client
         #: The post id
         self.id = data['id']
         self.dimensions: dict = data.get('dimensions', {})
         self.is_video: bool = data.get('is_video', False)
```

### Comparing `insta-tweet-2.2.0/InstaTweet/instatweet.py` & `insta-tweet-2.2.1/InstaTweet/instatweet.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/InstaTweet/profile.py` & `insta-tweet-2.2.1/InstaTweet/profile.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/InstaTweet/tweetclient.py` & `insta-tweet-2.2.1/InstaTweet/tweetclient.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/InstaTweet/utils.py` & `insta-tweet-2.2.1/InstaTweet/utils.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/LICENSE` & `insta-tweet-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.2.0/PKG-INFO` & `insta-tweet-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-tweet
-Version: 2.2.0
+Version: 2.2.1
 Summary: Automatically Repost Content From Instagram to Twitter
 Home-page: https://www.github.com/TDKorn/insta-tweet/
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT
 Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
 Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
@@ -13,23 +13,23 @@
 License-File: LICENSE
 
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
 .. |.InstaTweet| replace:: InstaTweet
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L5-L147
 .. |.add_pages| replace:: add_pages()
-.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L132-L165
 .. |.Profile| replace:: Profile
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L11-L382
 .. |.start| replace:: start()
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L71-L121
 .. |.InstaClient| replace:: InstaClient
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instaclient.py#L17-L180
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
```

### Comparing `insta-tweet-2.2.0/README.rst` & `insta-tweet-2.2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
 .. |.InstaTweet| replace:: ``InstaTweet``
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L5-L147
 .. |.add_pages| replace:: ``add_pages()``
-.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L132-L165
 .. |.Profile| replace:: ``Profile``
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L11-L382
 .. |.start| replace:: ``start()``
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L71-L121
 .. |.InstaClient| replace:: ``InstaClient``
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instaclient.py#L17-L180
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 .. meta:: :title: InstaTweet - Automatically Repost Content From Instagram to
 Twitter :description: A Python package to automatically repost content from
 Instagram to Twitter .. |.InstaTweet| replace:: ``InstaTweet`` .. _.InstaTweet:
-https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-
+https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L5-
 L147 .. |.add_pages| replace:: ``add_pages()`` .. _.add_pages: https://
-github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165 ..
+github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L132-L165 ..
 |.Profile| replace:: ``Profile`` .. _.Profile: https://github.com/tdkorn/insta-
-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382 .. |.start| replace:: ``start
-()`` .. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/
+tweet/blob/v2.2.1/InstaTweet/profile.py#L11-L382 .. |.start| replace:: ``start
+()`` .. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/
 instatweet.py#L71-L121 .. |.InstaClient| replace:: ``InstaClient`` ..
-_.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/
-instaclient.py#L16-L159 .. |mandatory-settings| replace:: mandatory settings ..
+_.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/
+instaclient.py#L17-L180 .. |mandatory-settings| replace:: mandatory settings ..
 _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/
 getting-started.html#mandatory-settings .. _about-insta-tweet: â¨ð¥
 InstaTweet ð¤â¨ ----------------------- .. image:: https://img.shields.io/
 pypi/v/insta-tweet :target: https://pypi.org/project/insta-tweet/ :alt: PyPI
 Version .. image:: https://img.shields.io/badge/GitHub-insta--tweet-4f1abc :
 target: https://github.com/tdkorn/insta-tweet :alt: GitHub Repository ..
 image:: https://static.pepy.tech/personalized-badge/insta-
```

### Comparing `insta-tweet-2.2.0/insta_tweet.egg-info/PKG-INFO` & `insta-tweet-2.2.1/insta_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-tweet
-Version: 2.2.0
+Version: 2.2.1
 Summary: Automatically Repost Content From Instagram to Twitter
 Home-page: https://www.github.com/TDKorn/insta-tweet/
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT
 Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
 Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
@@ -13,23 +13,23 @@
 License-File: LICENSE
 
 .. meta::
    :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
    :description: A Python package to automatically repost content from Instagram to Twitter
 
 .. |.InstaTweet| replace:: InstaTweet
-.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L5-L147
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L5-L147
 .. |.add_pages| replace:: add_pages()
-.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L132-L165
+.. _.add_pages: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L132-L165
 .. |.Profile| replace:: Profile
-.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/profile.py#L11-L382
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/profile.py#L11-L382
 .. |.start| replace:: start()
-.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instatweet.py#L71-L121
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instatweet.py#L71-L121
 .. |.InstaClient| replace:: InstaClient
-.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.0/InstaTweet/instaclient.py#L16-L159
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/v2.2.1/InstaTweet/instaclient.py#L17-L180
 .. |mandatory-settings| replace:: mandatory settings
 .. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
 
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
```

### Comparing `insta-tweet-2.2.0/setup.py` & `insta-tweet-2.2.1/setup.py`

 * *Files identical despite different names*

