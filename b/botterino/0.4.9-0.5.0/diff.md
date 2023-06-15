# Comparing `tmp/botterino-0.4.9.tar.gz` & `tmp/botterino-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botterino-0.4.9.tar", last modified: Sun Apr 23 06:34:58 2023, max compression
+gzip compressed data, was "botterino-0.5.0.tar", last modified: Wed Jun 14 23:54:07 2023, max compression
```

## Comparing `botterino-0.4.9.tar` & `botterino-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.928062 botterino-0.4.9/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.4.9/LICENSE
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:34:58.928395 botterino-0.4.9/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.4.9/README.md
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.848723 botterino-0.4.9/botterino/
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.876918 botterino-0.4.9/botterino/Loader/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.4.9/botterino/Loader/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      868 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/Loader/loader.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.900572 botterino-0.4.9/botterino/Map/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:46:10.000000 botterino-0.4.9/botterino/Map/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1471 2023-04-23 06:15:24.000000 botterino-0.4.9/botterino/Map/map.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.924479 botterino-0.4.9/botterino/RedditPoller/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1368 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/RedditPoller/RedditPoller.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2443 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/RedditPoller/Retry.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.4.9/botterino/RedditPoller/__init__.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.926519 botterino-0.4.9/botterino/Utils/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.4.9/botterino/Utils/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3821 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/Utils/utils.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1508 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/__init__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       36 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/__main__.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     2673 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/botterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     3235 2023-04-23 06:32:23.000000 botterino-0.4.9/botterino/config.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      544 2023-04-23 04:36:39.000000 botterino-0.4.9/botterino/failure.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     6907 2023-04-23 06:15:17.000000 botterino-0.4.9/botterino/hosterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     1127 2023-04-23 04:36:40.000000 botterino-0.4.9/botterino/posterino.py
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     4615 2023-04-23 04:36:40.000000 botterino-0.4.9/botterino/ui.py
-drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 06:34:58.869334 botterino-0.4.9/botterino.egg-info/
--rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/PKG-INFO
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      638 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/SOURCES.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/dependency_links.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       70 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/requires.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-04-23 06:34:58.000000 botterino-0.4.9/botterino.egg-info/top_level.txt
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.4.9/pyproject.toml
--rw-r--r--   0 adarsharegmi   (501) staff       (20)      636 2023-04-23 06:34:58.932513 botterino-0.4.9/setup.cfg
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.672716 botterino-0.5.0/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1063 2021-06-10 02:59:26.000000 botterino-0.5.0/LICENSE
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-06-14 23:54:07.673268 botterino-0.5.0/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4566 2022-08-30 05:36:56.000000 botterino-0.5.0/README.md
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.628373 botterino-0.5.0/botterino/
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.640417 botterino-0.5.0/botterino/Loader/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-06-17 04:44:47.000000 botterino-0.5.0/botterino/Loader/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      868 2023-04-23 04:36:39.000000 botterino-0.5.0/botterino/Loader/loader.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.647278 botterino-0.5.0/botterino/Map/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2023-04-23 04:46:10.000000 botterino-0.5.0/botterino/Map/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1378 2023-04-30 02:55:00.000000 botterino-0.5.0/botterino/Map/map.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.659956 botterino-0.5.0/botterino/RedditPoller/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1368 2023-04-23 04:36:39.000000 botterino-0.5.0/botterino/RedditPoller/RedditPoller.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2443 2023-04-23 04:36:39.000000 botterino-0.5.0/botterino/RedditPoller/Retry.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2020-10-17 08:27:10.000000 botterino-0.5.0/botterino/RedditPoller/__init__.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.665265 botterino-0.5.0/botterino/Utils/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        0 2021-04-08 15:21:02.000000 botterino-0.5.0/botterino/Utils/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      639 2023-06-14 23:52:25.000000 botterino-0.5.0/botterino/Utils/color.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3379 2023-04-30 03:08:57.000000 botterino-0.5.0/botterino/Utils/utils.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1508 2023-04-23 04:36:39.000000 botterino-0.5.0/botterino/__init__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       36 2023-04-23 04:36:39.000000 botterino-0.5.0/botterino/__main__.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     2427 2023-06-11 05:23:46.000000 botterino-0.5.0/botterino/botterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     3197 2023-06-14 23:53:32.000000 botterino-0.5.0/botterino/config.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      509 2023-04-30 02:55:00.000000 botterino-0.5.0/botterino/failure.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     6485 2023-04-30 03:06:14.000000 botterino-0.5.0/botterino/hosterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     1118 2023-04-30 02:55:49.000000 botterino-0.5.0/botterino/posterino.py
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     4646 2023-04-30 02:55:01.000000 botterino-0.5.0/botterino/ui.py
+drwxr-xr-x   0 adarsharegmi   (501) staff       (20)        0 2023-06-14 23:54:07.639210 botterino-0.5.0/botterino.egg-info/
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)     5014 2023-06-14 23:54:07.000000 botterino-0.5.0/botterino.egg-info/PKG-INFO
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      663 2023-06-14 23:54:07.000000 botterino-0.5.0/botterino.egg-info/SOURCES.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)        1 2023-06-14 23:54:07.000000 botterino-0.5.0/botterino.egg-info/dependency_links.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       70 2023-06-14 23:54:07.000000 botterino-0.5.0/botterino.egg-info/requires.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)       10 2023-06-14 23:54:07.000000 botterino-0.5.0/botterino.egg-info/top_level.txt
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      103 2021-06-10 03:23:33.000000 botterino-0.5.0/pyproject.toml
+-rw-r--r--   0 adarsharegmi   (501) staff       (20)      636 2023-06-14 23:54:07.676350 botterino-0.5.0/setup.cfg
```

### Comparing `botterino-0.4.9/LICENSE` & `botterino-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/PKG-INFO` & `botterino-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.9
+Version: 0.5.0
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.9/README.md` & `botterino-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/botterino/Loader/loader.py` & `botterino-0.5.0/botterino/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/botterino/Map/map.py` & `botterino-0.5.0/botterino/Map/map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import folium
 import webbrowser
 import tempfile
 import os
 from sty import fg
-'''
-A class for plotting guesses on a map relative to a "correct" guess
-'''
+from ..Utils.color import colormsg
 
+"""
+A class for plotting guesses on a map relative to a "correct" guess
+"""
 
-class Map():
 
+class Map:
     def __init__(self, latitude, longitude, zoomLevel=10):
         # TODO: we might want to center the map about the center of all points instead of the correct answer
-        self.map = folium.Map(location=[latitude, longitude],
-                              zoom_start=zoomLevel)
-        self.filePath = ''
+        self.map = folium.Map(location=[latitude, longitude], zoom_start=zoomLevel)
+        self.filePath = ""
 
     def addPoint(self, latitude, longitude, user, distance, link, color):
-        description = '''
+        description = """
         {username}
 
         {distance}m away
 
         {link}
-        '''
-        folium.Marker(location=[latitude, longitude],
-                      popup=description.format(username=user,
-                                               distance=distance,
-                                               link=link),
-                      icon=folium.Icon(color=color)).add_to(self.map)
+        """
+        folium.Marker(
+            location=[latitude, longitude],
+            popup=description.format(username=user, distance=distance, link=link),
+            icon=folium.Icon(color=color),
+        ).add_to(self.map)
 
     def saveMap(self):
-        tempFile = tempfile.NamedTemporaryFile(suffix='.html', delete=False)
+        tempFile = tempfile.NamedTemporaryFile(suffix=".html", delete=False)
         try:
             self.map.save(tempFile)
         except Exception as e:
-            print(f'{fg.red}Could not save map: {e} {fg.rs}')
+            colormsg(f"Could not save map: {e}", fg.red)
             return
         self.filePath = tempFile.name
 
     def getFilePath(self):
         return self.filePath
 
     def openMapInBrowser(self):
         if not self.filePath:
             return
-        webbrowser.open(f'file://{os.path.realpath(self.filePath)}')
+        webbrowser.open(f"file://{os.path.realpath(self.filePath)}")
```

### Comparing `botterino-0.4.9/botterino/RedditPoller/RedditPoller.py` & `botterino-0.5.0/botterino/RedditPoller/RedditPoller.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/botterino/RedditPoller/Retry.py` & `botterino-0.5.0/botterino/RedditPoller/Retry.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/botterino/Utils/utils.py` & `botterino-0.5.0/botterino/Utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from ..config import pg, username, debug, reddit, donotreply, api
 from ..RedditPoller.RedditPoller import RedditPoller, CommentWrapper
 from ..RedditPoller.Retry import retry
 from geopy.point import Point
 from geopy.distance import distance
-from sty import fg
-from random import randrange
 from halo import Halo
 import re
 import requests
 import json
 import time
 import warnings
 import random
@@ -23,44 +21,26 @@
 # google earth formats, other formats
 everything_else = re.compile(
     """(^| )(-?\d{1,2}(\.\d+)?(?=\s*,?\s*)[\s,]+-?\d{1,3}(\.\d+)?|\d{1,2}(\.\d+°|°(\d{1,2}(\.\d+'|'(\d{1,2}(\.\d+)?\")?))?)[NS](?=\s*,?\s*)[\s,]+\d{1,3}(\.\d+°|°(\d{1,2}(\.\d+'|'(\d{1,2}(\.\d+)?\")?))?)[EW])"""
 )
 
 MAPS_URL = "https://maps.google.com/maps?t=k&q=loc:{},{}"
 
-badColors = [0, 16, 17, 18, 22, 52, 88, 90] + list(range(232, 256))
-
 
 def submissions():
     """
     returns a generator of titles of submissions to pg
     newest submissions first
     """
     for submission in reddit.user.me().submissions.new(limit=200):
         if submission.subreddit != pg:
             continue
         yield submission.title
 
 
-def randomColorWithAuthor(author):
-    seed = hash(author)
-    random.seed(seed)
-    color = randrange(256)
-    while color in badColors:
-        color = (color + 1) % 256
-    return fg(color)
-
-
-def randomColor():
-    color = randrange(256)
-    while color in badColors:
-        color = randrange(256)
-    return fg(color)
-
-
 def postDelay():
     if debug:
         return -1
 
     r = requests.get(f"{api}/current")
     data = json.loads(r.content)
     tries = 1
```

### Comparing `botterino-0.4.9/botterino/__init__.py` & `botterino-0.5.0/botterino/__init__.py`

 * *Files identical despite different names*

### Comparing `botterino-0.4.9/botterino/botterino.py` & `botterino-0.5.0/botterino/botterino.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from .config import pg, username, hints
 from .posterino import submitRound
 from .hosterino import checkAnswers, checkHints
-from .Utils.utils import waitForApproval, approved, postDelay, randomColor
+from .Utils.utils import waitForApproval, approved, postDelay
+from .Utils.color import colormsg
 from .Loader.loader import getRound
 from sty import fg
 from importlib.metadata import version
 from update_checker import UpdateChecker
 from threading import Thread
 import time
 
 v = version("botterino")
 checker = UpdateChecker()
 result = checker.check("botterino", v)
 if result:
-    print(f"{fg.yellow}{result}")
-    print(f'{fg.yellow}run "pip install --upgrade botterino" to update')
+    colormsg(result, fg.yellow)
+    colormsg('run "pip install --upgrade botterino" to update', fg.yellow)
 
 
 def checkType(r):
     types = []
     if "tolerance" in r and "answer" in r:
         types.append("coordinates")
     if "tolerances" in r and "answers" in r:
@@ -32,48 +33,37 @@
     if "manual" not in r:
         types.append("automatic")
     return ",".join(types)
 
 
 def main(stop=None):
     while True:
-        print(
-            f"{fg.yellow}Waiting for {username} to win a round... 🐌", end=f"{fg.rs}\n"
-        )
+        colormsg(f"Waiting for {username} to win a round... 🐌", fg.yellow)
         stopped = waitForApproval(stop)
         if stopped or stop:
-            print(f"{fg.red}Stopped botterino{fg.rs}")
+            colormsg("Stopped botterino", fg.red)
             return
-        print(
-            f"{fg.blue}Congrats on a well deserved win {username}! ⭐", end=f"{fg.rs}\n"
-        )
+        colormsg(f"Congrats on a well deserved win {username}! ⭐", fg.blue)
         r = getRound()
         while not r:
-            print(f"{fg.red}No rounds in round file! checking again in 10s")
+            colormsg(f"No rounds in round file! checking again in 10s", fg.red)
             time.sleep(10)
             r = getRound()
         submission = submitRound(r)
-        print(
-            f"{randomColor()}Your round was posted to https://reddit.com{submission.permalink}",
-            end=f"{fg.rs}\n",
-        )
-        print(
-            f'{fg.magenta}Round \'{r["title"]}\' posted in {postDelay()}s',
-            end=f"{fg.rs}\n",
+        colormsg(
+            f"Your round was posted to https://reddit.com{submission.permalink}",
         )
-        print(f"{fg.cyan}Checking Answers: {checkType(r)}...{fg.rs}", end=f"{fg.rs}\n")
+        colormsg(f'Round \'{r["title"]}\' posted in {postDelay()}s', fg.magenta)
+        colormsg(f"Checking Answers: {checkType(r)}...", fg.cyan)
         H = hints if not r.get("hints") else r.get("hints")
         CheckAnswers = Thread(target=checkAnswers, args=(r, submission))
         CheckHints = Thread(target=checkHints, args=(H, submission))
         CheckAnswers.start()
         CheckHints.start()
         CheckAnswers.join()
         CheckHints.join()
         while approved():
             continue
         after = r.get("after")
         if after:
             submission.reply(after)
-            print(
-                f"{randomColor()}Posted your message after the round: {after}",
-                end=f"{fg.rs}\n",
-            )
+            colormsg(f"Posted your message after the round: {after}")
```

### Comparing `botterino-0.4.9/botterino/config.py` & `botterino-0.5.0/botterino/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import praw
 import os
 import sys
+from .Utils.color import colormsg
 from . import botfiles, correctMessage, incorrectMessage, hints
 from sty import fg
 import random
 import webbrowser
 import socket
 
 
@@ -38,65 +39,58 @@
 archivefile = botfiles.archive
 cwd = os.getcwd()
 # FIXME: clean this up
 try:
     os.chdir(botfiles.botconfig)
     reddit = praw.Reddit("botterino")
     if reddit.user.me():
-        print(
-            f"{fg.green}Successfully logged into reddit as {reddit.user.me()}",
-            end=f"{fg.rs}\n",
-        )
+        colormsg(f"Successfully logged into reddit as {reddit.user.me()}", fg.green)
     else:
-        print(
-            f"{fg.yellow}Unable to login with username/password. If your account has 2fa continue in browser. Otherwise check {botfiles.prawconfig}",
-            end=f"{fg.rs}\n",
+        colormsg(
+            f"Unable to login with username/password. If your account has 2fa continue in browser. Otherwise check {botfiles.prawconfig}",
+            fg.yellow,
         )
         os.chdir(botfiles.botconfig)
         reddit = praw.Reddit("botterino", redirect_uri="http://localhost:8080")
         state = str(random.randint(0, 65000))
-        scopes = [
-            "identity", "history", "read", "edit", "submit", "privatemessages"
-        ]
+        scopes = ["identity", "history", "read", "edit", "submit", "privatemessages"]
         url = reddit.auth.url(scopes, state, "permanent")
-        print(
+        colormsg(
             "A window will be opened in the browser to complete the login process to reddit."
         )
         webbrowser.open(url)
 
         client = receive_connection()
         data = client.recv(1024).decode("utf-8")
         param_tokens = data.split(" ", 2)[1].split("?", 1)[1].split("&")
         params = {
-            key: value
-            for (key, value) in [token.split("=") for token in param_tokens]
+            key: value for (key, value) in [token.split("=") for token in param_tokens]
         }
 
         if state != params["state"]:
             send_message(
                 client,
                 "State mismatch. Expected: {} Received: {}".format(
-                    state, params["state"]),
+                    state, params["state"]
+                ),
             )
         elif "error" in params:
             send_message(client, params["error"])
 
         refresh_token = reddit.auth.authorize(params["code"])
         send_message(client, "Refresh token: {}".format(refresh_token))
-        print(refresh_token)
+        colormsg(refresh_token, fg.blue)
         if not reddit.user.me():
-            print(
-                f"{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}"
+            colormsg(
+                f"Unable to login to reddit. Please check {botfiles.prawconfig}", fg.red
             )
             exit(1)
 except Exception as e:
-    print(
-        f"{fg.red}Unable to login to reddit. Please check {botfiles.prawconfig}"
-    )
-    print(f"{fg.red}{e}")
+    colormsg(f"Unable to login to reddit. Please check {botfiles.prawconfig}", fg.red)
+    colormsg(f"{e}", fg.red)
 finally:
     os.chdir(cwd)
 
 pg = reddit.subreddit("itoxtestingfacility" if debug else "picturegame")
 
 username = str(reddit.user.me())
```

### Comparing `botterino-0.4.9/botterino/hosterino.py` & `botterino-0.5.0/botterino/hosterino.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,20 @@
     correctMessage,
     incorrectMessage,
     botfiles,
 )
 from itertools import permutations
 import re
 from sty import fg
+from .Utils.color import colormsg, getColorFromAuthor
 from .Utils.utils import (
     approved,
     decimal,
     getComments,
     getDistance,
-    randomColor,
-    randomColorWithAuthor,
     MAPS_URL,
     hyperlink,
 )
 from difflib import SequenceMatcher
 from .Map.map import Map
 import time
 
@@ -29,103 +28,98 @@
 
 def checkMultipleCoordinates(guess, answers, tolerances):
     guesser = guess.author.name
     answers = [Point(a) for a in answers]
     match = re.findall(decimal, guess.body)
     if len(match) != len(answers):
         # TODO print a message here
-        print(
-            f"{randomColorWithAuthor(guesser)}{guesser}'s guess {guess.body} was incorrect",
-            end=f"{fg.rs}\n",
-        )
-        return False
-    try:
-        points = [Point(f"{lat},{lon}") for lat, lon in match]
-        points = permutations(points)
-    except Exception as e:
-        print(f"{randomColor()}Something happened: ", e,
-              "it probably does not matter")
+        colormsg(f"{guesser}'s guess {guess.body} was incorrect", author=guesser)
         return False
+    points = [Point(f"{lat},{lon}") for lat, lon in match]
+    points = permutations(points)
 
-    results = [[
-        withinTolerance(p, a, t) for p, a, t in zip(ps, answers, tolerances)
-    ] for ps in points]
+    results = [
+        [withinTolerance(p, a, t) for p, a, t in zip(ps, answers, tolerances)]
+        for ps in points
+    ]
     results = [all(r) for r in results]
     result = any(results)
     if not result:
-        print(
-            f"{randomColorWithAuthor(guesser)}{guesser}'s guess {guess.body} was incorrect"
-        )
+        colormsg(f"{guesser}'s guess {guess.body} was incorrect", author=guesser)
     return result
 
 
 def checkCoordinates(guess, answer, tolerance, map):
     guesser = guess.author.name
     answer = Point(answer)
     errorAndPoint = getDistance(guess.body, answer)
     error, point = errorAndPoint if errorAndPoint else (None, None)
     if error is None:
-        print(
-            f"{randomColorWithAuthor(guesser)}Could not find a coordinate in guess '{guess.body}' by {guesser}",
-            end=f"{fg.rs}\n",
+        colormsg(
+            f"Could not find a coordinate in guess '{guess.body}' by {guesser}",
+            author=guesser,
         )
         return "ignore"
     error = round(error, 2)
     mapslink = MAPS_URL.format(point.latitude, point.longitude)
-    color = fg.green if error <= tolerance else randomColorWithAuthor(guesser)
+    color = fg.green if error <= tolerance else getColorFromAuthor(guesser)
     pl = ""
     if hasattr(guess, "context"):
         pl = guess.context
     elif hasattr(guess, "permalink"):
         pl = guess.permalink
     commentLink = f"https://reddit.com{pl}"
     if error < 1000:
-        print(
-            f'{color}{guesser}\'s {hyperlink("guess", commentLink)} was {error}m {hyperlink("off", mapslink)}',
-            end=f"{fg.rs}\n",
+        colormsg(
+            f'{guesser}\'s {hyperlink("guess", commentLink)} was {error}m {hyperlink("off", mapslink)}',
+            color,
         )
     else:
-        print(
-            f'{color}{guesser}\'s {hyperlink("guess", commentLink)} was {round(error/1000,2)}km {hyperlink("off", mapslink)}',
-            end=f"{fg.rs}\n",
+        colormsg(
+            f'{guesser}\'s {hyperlink("guess", commentLink)} was {round(error/1000,2)}km {hyperlink("off", mapslink)}',
+            color,
         )
 
     if map:
         # TODO: try to give different users differnt colors
-        map.addPoint(point.latitude, point.longitude, guesser, error,
-                     commentLink, "red" if error > tolerance else "green")
+        map.addPoint(
+            point.latitude,
+            point.longitude,
+            guesser,
+            error,
+            commentLink,
+            "red" if error > tolerance else "green",
+        )
 
     return error <= tolerance
 
 
 def checkText(guess, answer, tolerance, ignorecase):
     guesser = guess.author.name
     text = guess.body.strip().replace("\\", "")
 
     if ignorecase:
         text, answer = text.lower(), answer.lower()
 
     similarity = SequenceMatcher(None, text, answer).ratio()
-    print(
-        f"{randomColorWithAuthor(guesser)}{guesser}'s guess was {round(similarity * 100, 3)}% similar to the correct answer",
-        end=f"{fg.rs}\n",
+    colormsg(
+        f"{guesser}'s guess was {round(similarity * 100, 3)}% similar to the correct answer",
+        author=guesser,
     )
     return similarity >= tolerance
 
 
 def postHint(submission, time):
     with open(botfiles.hintfile, "r") as F:
         hintText = F.read()
     if not hintText:
-        print(f"{fg.yellow}Skipping {time}m hint: hints.txt is empty")
+        colormsg(f"Skipping {time}m hint: hints.txt is empty", fg.yellow)
         return
     hint = submission.reply(f"Hint({time}m): {hintText}")
-    print(
-        f"{fg.green}Posted hint ({time}m) to https://reddit.com{hint.permalink}"
-    )
+    colormsg(f"Posted hint ({time}m) to https://reddit.com{hint.permalink}", fg.green)
     open(botfiles.hintfile, "w").close()
 
 
 def checkHints(hints, submission):
     hints = list(hints)
     hints += [60, 120, 180, 240]
     hints = sorted(list(set(hints)))
@@ -179,49 +173,45 @@
             r = checkCoordinates(c, answer, tolerance, answerPlot)
             if r == "ignore":
                 continue
             result = result and r
         elif tolerances:
             tolerances = [float(t) for t in r["tolerances"]]
             if len(answers) != len(tolerances):
-                print(
-                    "{fg.red}Refusing to check answers, number of tolerances must equal number of answers.",
-                    end=f"{fg.rs}\n",
+                colormsg(
+                    f"Refusing to check answers, number of tolerances must equal number of answers.",
+                    fg.red
                 )
-            result = result and checkMultipleCoordinates(
-                c, answers, tolerances)
+            result = result and checkMultipleCoordinates(c, answers, tolerances)
 
         if text and similarity is None:
             continue
 
         if ignorecase is None:
             ignorecase = True
 
         if text:
             result = result and checkText(c, text, similarity, ignorecase)
 
         if not result:
             c.reply(incorrectMessage)
         if result:
             if manual:
-                print(
-                    f"{randomColor()}Guess '{c.body}' looks correct, but you will have to check it out.",
-                    end=f"{fg.rs}\n",
+                colormsg(
+                    f"Guess '{c.body}' looks correct, but you will have to check it out.",
                 )
             else:
                 plusCorrect = c.reply(correctMessage)
                 guesser = c.author.name
-                print(
-                    f"{fg.green}Corrected {guesser} in {plusCorrect.created_utc - c.created_utc}s",
-                    end=f"{fg.rs}\n",
+                colormsg(
+                    f"Corrected {guesser} in {plusCorrect.created_utc - c.created_utc}s",
+                    fg.green,
                 )
                 break
 
     # TODO: show the map on every guess instead of only when the round is over
     if answerPlot:
         answerPlot.saveMap()
         outputFile = answerPlot.getFilePath()
         if outputFile:
-            print(
-                f'{fg.green}Answers to your round plotted at {outputFile}{fg.rs}'
-            )
-            answerPlot.openMapInBrowser()
+            colormsg(f"Answers to your round plotted at {outputFile}", fg.cyan)
+            answerPlot.openMapInBrowser()
```

### Comparing `botterino-0.4.9/botterino/posterino.py` & `botterino-0.5.0/botterino/posterino.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 from .config import pg
-from .Utils.utils import randomColor, getRoundPrefix, submissions
+from .Utils.utils import getRoundPrefix, submissions
+from .Utils.color import colormsg
 from sty import fg
 import time
 import re
 
 
 def getSeriesPrefix(name):
     if not name:
@@ -28,10 +29,10 @@
     submission = pg.submit(title=title, url=r["url"].strip())
 
     message = r.get("message")
     if message is not None:
         time.sleep(15)
         submission.reply(message)
 
-        print(f"{randomColor()}Message posted to thread: {message}", end=f"{fg.rs}\n")
+        colormsg(f"Message posted to thread: {message}")
 
     return submission
```

### Comparing `botterino-0.4.9/botterino/ui.py` & `botterino-0.5.0/botterino/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from tkinter import *
 from tkinter import ttk
 from .config import roundfile
 from .Loader.loader import append, load
 from .botterino import main
 from sty import fg
 from threading import Thread
+from .Utils.color import colormsg
 
 root = Tk()
 root.title("Botterino")
 
+
 # Todo: place this in a sensible place
 class Stopper:
     def __init__(self):
         self.stopped = False
 
     def __bool__(self):
         return self.stopped
@@ -81,15 +83,15 @@
     if url_input:
         inner["url"] = url_input
     if manual_input:
         inner["manual"] = manual_input
     data[name_input] = inner
     append(data, roundfile)
     clear_entries()
-    print(f"{fg.green}Added round {name_input} to rounds.yaml{fg.rs}")
+    colormsg(f"Added round {name_input} to rounds.yaml", fg.green)
 
 
 def clear_entries():
     name_entry.delete(0, END)
     title_entry.delete(0, END)
     answer_entry.delete(0, END)
     tolerance_entry.delete(0, END)
```

### Comparing `botterino-0.4.9/botterino.egg-info/PKG-INFO` & `botterino-0.5.0/botterino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botterino
-Version: 0.4.9
+Version: 0.5.0
 Summary: Automate posting and hosting of rounds on /r/picturegame
 Home-page: https://github.com/pgitox/botterino
 Author: itoxici
 Author-email: itox@picturegame.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `botterino-0.4.9/botterino.egg-info/SOURCES.txt` & `botterino-0.5.0/botterino.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 botterino/Loader/loader.py
 botterino/Map/__init__.py
 botterino/Map/map.py
 botterino/RedditPoller/RedditPoller.py
 botterino/RedditPoller/Retry.py
 botterino/RedditPoller/__init__.py
 botterino/Utils/__init__.py
+botterino/Utils/color.py
 botterino/Utils/utils.py
```

### Comparing `botterino-0.4.9/setup.cfg` & `botterino-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = botterino
-version = 0.4.9
+version = 0.5.0
 author = itoxici
 author_email = itox@picturegame.co
 description = Automate posting and hosting of rounds on /r/picturegame
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pgitox/botterino
 classifiers =
```

