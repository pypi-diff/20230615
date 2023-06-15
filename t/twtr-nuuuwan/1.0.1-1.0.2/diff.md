# Comparing `tmp/twtr-nuuuwan-1.0.1.tar.gz` & `tmp/twtr-nuuuwan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtr-nuuuwan-1.0.1.tar", last modified: Thu Jun 15 06:30:25 2023, max compression
+gzip compressed data, was "twtr-nuuuwan-1.0.2.tar", last modified: Thu Jun 15 08:19:19 2023, max compression
```

## Comparing `twtr-nuuuwan-1.0.1.tar` & `twtr-nuuuwan-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr/core/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/Tweet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/Twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/tests/test_twitter_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.342001 twtr-nuuuwan-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 08:19:19.342001 twtr-nuuuwan-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:19:19.342001 twtr-nuuuwan-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.338001 twtr-nuuuwan-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.338001 twtr-nuuuwan-1.0.2/src/twtr/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/src/twtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/src/twtr/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.338001 twtr-nuuuwan-1.0.2/src/twtr/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/src/twtr/core/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/src/twtr/core/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/src/twtr/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.342001 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 08:19:19.000000 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 08:19:19.000000 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:19:19.000000 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 08:19:19.000000 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 08:19:19.000000 twtr-nuuuwan-1.0.2/src/twtr_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:19:19.342001 twtr-nuuuwan-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 08:18:21.000000 twtr-nuuuwan-1.0.2/tests/test_twitter_basic.py
```

### Comparing `twtr-nuuuwan-1.0.1/LICENSE` & `twtr-nuuuwan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twtr-nuuuwan-1.0.1/setup.py` & `twtr-nuuuwan-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'twtr'
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Wrapper library for the Twitter API and tweepy"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `twtr-nuuuwan-1.0.1/tests/test_twitter_basic.py` & `twtr-nuuuwan-1.0.2/tests/test_twitter_basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 import unittest
 
 from twtr import Tweet, Twitter
 
+TEST_TWEET_TEXT = "Hello World!"
 TEST_IMG_PATH = os.path.join("tests", "test.png")
+TEST_IMG_PATH2 = os.path.join("tests", "test2.png")
 TEST_TWITTER = Twitter()
 SKIP_REASON_TWITTER = "Calls Twitter API"
 
 
 class Test(unittest.TestCase):
     @unittest.skip(SKIP_REASON_TWITTER)
     def test_init_(self):
         self.assertIsNotNone(TEST_TWITTER)
 
     @unittest.skip(SKIP_REASON_TWITTER)
     def test_send_text_only(self):
-        tweet_id = TEST_TWITTER.send(Tweet("Hello World!"))
+        tweet_id = TEST_TWITTER.send(Tweet(TEST_TWEET_TEXT))
         self.assertIsNotNone(tweet_id)
 
     @unittest.skip(SKIP_REASON_TWITTER)
     def test_send_text_and_image(self):
         tweet_id = TEST_TWITTER.send(
-            Tweet("Hello World!").add_image(TEST_IMG_PATH)
+            Tweet(TEST_TWEET_TEXT).add_images([TEST_IMG_PATH, TEST_IMG_PATH2])
         )
         self.assertIsNotNone(tweet_id)
```

