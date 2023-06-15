# Comparing `tmp/twtr-nuuuwan-1.0.3.tar.gz` & `tmp/twtr-nuuuwan-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtr-nuuuwan-1.0.3.tar", last modified: Thu Jun 15 08:46:58 2023, max compression
+gzip compressed data, was "twtr-nuuuwan-1.0.6.tar", last modified: Thu Jun 15 12:12:07 2023, max compression
```

## Comparing `twtr-nuuuwan-1.0.3.tar` & `twtr-nuuuwan-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.420510 twtr-nuuuwan-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/src/twtr/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/src/twtr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/src/twtr/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/src/twtr/core/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/src/twtr/core/Tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/src/twtr/core/Twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/src/twtr/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 08:46:58.000000 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 08:46:58.000000 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:46:58.000000 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 08:46:58.000000 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 08:46:58.000000 twtr-nuuuwan-1.0.3/src/twtr_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:46:58.424510 twtr-nuuuwan-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 08:46:02.000000 twtr-nuuuwan-1.0.3/tests/test_twitter_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/twtr/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.194621 twtr-nuuuwan-1.0.6/src/twtr/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/src/twtr/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 12:12:07.000000 twtr-nuuuwan-1.0.6/src/twtr_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:12:07.198622 twtr-nuuuwan-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-15 12:11:04.000000 twtr-nuuuwan-1.0.6/tests/test_twitter_basic.py
```

### Comparing `twtr-nuuuwan-1.0.3/LICENSE` & `twtr-nuuuwan-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twtr-nuuuwan-1.0.3/setup.py` & `twtr-nuuuwan-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'twtr'
-VERSION = "1.0.3"
+VERSION = "1.0.6"
 DESCRIPTION = "Wrapper library for the Twitter API and tweepy"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `twtr-nuuuwan-1.0.3/src/twtr/core/Twitter.py` & `twtr-nuuuwan-1.0.6/src/twtr/core/Twitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,79 +2,82 @@
 import os
 
 import tweepy
 
 from twtr.common import log
 from twtr.core.Tweet import Tweet
 
+MIN_TOKEN_LEN = 8
+TOKENS = [
+    'TWTR_BEARER_TOKEN',
+    'TWTR_API_KEY',
+    'TWTR_API_KEY_SECRET',
+    'TWTR_ACCESS_TOKEN',
+    'TWTR_ACCESS_TOKEN_SECRET',
+]
+
 
 class Twitter:
     @staticmethod
-    def get_vars_from_argparse():
+    def validate(token: str, var: str):
+        if var is None or len(var) < MIN_TOKEN_LEN:
+            log.error(f'❌ {token} ("{var}") is not valid')
+            return False
+        log.debug(f'✅ {token} is valid')
+        return True
+
+    @staticmethod
+    def get_args():
         parser = argparse.ArgumentParser()
-        parser.add_argument('--TWTR_BEARER_TOKEN')
-        parser.add_argument('--TWTR_API_KEY')
-        parser.add_argument('--TWTR_API_KEY_SECRET')
-        parser.add_argument('--TWTR_ACCESS_TOKEN')
-        parser.add_argument('--TWTR_ACCESS_TOKEN_SECRET')
+        for token in TOKENS:
+            parser.add_argument(f'--{token}')
+        return parser.parse_args()
 
-        args = parser.parse_args()
-        return (
+    @staticmethod
+    def get_vars_from_argparse():
+        args = Twitter.get_args()
+        vars = (
             args.TWTR_BEARER_TOKEN,
             args.TWTR_API_KEY,
             args.TWTR_API_KEY_SECRET,
             args.TWTR_ACCESS_TOKEN,
             args.TWTR_ACCESS_TOKEN_SECRET,
         )
+        has_errors = False
+        for token, var in zip(TOKENS, vars):
+            if not Twitter.validate(token, var):
+                has_errors = True
+        if has_errors:
+            raise ValueError('Contains Invalid Twitter tokens')
+        return vars
 
-    @staticmethod
-    def get_vars_from_env():
-        return (
-            os.environ.get('TWTR_BEARER_TOKEN'),
-            os.environ.get('TWTR_API_KEY'),
-            os.environ.get('TWTR_API_KEY_SECRET'),
-            os.environ.get('TWTR_ACCESS_TOKEN'),
-            os.environ.get('TWTR_ACCESS_TOKEN_SECRET'),
+    def __init__(self):
+        (
+            bearer_token,
+            consumer_key,
+            consumer_secret,
+            access_token,
+            access_token_secret,
+        ) = self.get_vars_from_argparse()
+
+        self.__client__ = tweepy.Client(
+            bearer_token=bearer_token,
+            consumer_key=consumer_key,
+            consumer_secret=consumer_secret,
+            access_token=access_token,
+            access_token_secret=access_token_secret,
         )
 
-    def __init__(self):
-        vars_argparse = self.get_vars_from_argparse()
-        vars_env = self.get_vars_from_env()
-        
-        bearer_token = vars_argparse[0] or vars_env[0]
-        consumer_key = vars_argparse[1] or vars_env[1]
-        consumer_secret = vars_argparse[2] or vars_env[2]
-        access_token = vars_argparse[3] or vars_env[3]
-        access_token_secret = vars_argparse[4] or vars_env[4]
-
-        if (
-            bearer_token is None
-            or consumer_key is None
-            or consumer_secret is None
-            or access_token is None
-            or access_token_secret is None
-        ):
-            self.__client__ = None
-            self.__api__ = None
-        else:
-            self.__client__ = tweepy.Client(
-                bearer_token=bearer_token,
-                consumer_key=consumer_key,
-                consumer_secret=consumer_secret,
-                access_token=access_token,
-                access_token_secret=access_token_secret,
-            )
-
-            auth = tweepy.OAuth1UserHandler(
-                consumer_key=consumer_key,
-                consumer_secret=consumer_secret,
-                access_token=access_token,
-                access_token_secret=access_token_secret,
-            )
-            self.__api__ = tweepy.API(auth)
+        auth = tweepy.OAuth1UserHandler(
+            consumer_key=consumer_key,
+            consumer_secret=consumer_secret,
+            access_token=access_token,
+            access_token_secret=access_token_secret,
+        )
+        self.__api__ = tweepy.API(auth)
 
     def check_api_and_client(self):
         if self.__client__ is None:
             raise ValueError('Client is not valid')
 
     def __media_upload__(self, image_path: str) -> int:
         if not os.path.exists(image_path):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

