# Comparing `tmp/glaceon-1.2.0.tar.gz` & `tmp/glaceon-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glaceon-1.2.0.tar", last modified: Sun May 14 11:53:19 2023, max compression
+gzip compressed data, was "glaceon-1.30.0.tar", last modified: Wed Jun 14 22:41:52 2023, max compression
```

## Comparing `glaceon-1.2.0.tar` & `glaceon-1.30.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.359317 glaceon-1.2.0/
--rw-rw-rw-   0        0        0      230 2023-05-14 11:53:19.358317 glaceon-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.341364 glaceon-1.2.0/glaceon/
--rw-rw-rw-   0        0        0     2194 2023-05-14 11:52:50.000000 glaceon-1.2.0/glaceon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:53:19.357353 glaceon-1.2.0/glaceon.egg-info/
--rw-rw-rw-   0        0        0      230 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 11:53:19.000000 glaceon-1.2.0/glaceon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 11:53:19.359317 glaceon-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-05-14 11:52:59.000000 glaceon-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.859710 glaceon-1.30.0/
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.850513 glaceon-1.30.0/GLACEON/
+-rw-rw-rw-   0        0        0      325 2023-06-14 22:40:02.000000 glaceon-1.30.0/GLACEON/__init__.py
+-rw-rw-rw-   0        0        0     2421 2023-05-20 18:37:28.000000 glaceon-1.30.0/GLACEON/cli.py
+-rw-rw-rw-   0        0        0      573 2023-05-20 18:41:33.000000 glaceon-1.30.0/GLACEON/gflask.py
+-rw-rw-rw-   0        0        0     3137 2023-06-14 22:41:52.859710 glaceon-1.30.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-05-20 18:14:31.000000 glaceon-1.30.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.858713 glaceon-1.30.0/glaceon.egg-info/
+-rw-rw-rw-   0        0        0     3137 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:41:52.860704 glaceon-1.30.0/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-06-14 22:40:40.000000 glaceon-1.30.0/setup.py
```

### Comparing `glaceon-1.2.0/glaceon/__init__.py` & `glaceon-1.30.0/GLACEON/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 import time
 
 
 class cli:
-    def __init__(self, speed=1, debug=False):
+
+    def __init__(self, speed=None, debug=None):
         self.speed = speed
         self.last_timestamp = time.time()
         self.debug = debug
-        self.initialized = True
+        self.initialized = speed is not None and debug is not None
 
     def getTimestamp(self):
         current_time = datetime.now().strftime("%H:%M:%S")
         return f"[{current_time}]"
 
     def fade(self, text, start_color, end_color):
         fade_steps = 10
@@ -24,40 +25,45 @@
             r += r_step
             g += g_step
             b += b_step
             faded_text += f"\033[38;2;{int(r)};{int(g)};{int(b)}m{letter}\033[0m"
         return faded_text
 
     def print(self, tag, message):
+        timestamp = self.getTimestamp()
+        inittag = self.fade("ERROR", (255, 0, 0), (128, 0, 0))
+
         if not self.initialized:
-            print(f"[ERR] Glaceon Not Initialized!")
-            return
+            if not self.debug:
+                print(f"{timestamp} [{inittag}] Not initialized!")
+                input()
+                exit()
+                return
+            else:
+                print(f"{timestamp} [{inittag}] Not initialized correctly!")
+                return
 
-        # split the tag and message
         tag_text = f"{tag}"
         message_text = message
 
-        # fade the tag colors
         if tag == "INFO":
             tag_text = self.fade(tag_text, (148, 0, 211), (0, 191, 255))
         elif tag == "WARNING":
             tag_text = self.fade(tag_text, (255, 215, 0), (255, 69, 0))
         elif tag == "ERROR":
             tag_text = self.fade(tag_text, (255, 0, 0), (128, 0, 0))
         elif tag == "SUCCESS":
-            tag_text = self.fade(tag, (0, 255, 0), (255, 255, 255))
+            tag_text = self.fade(tag_text, (0, 255, 0), (255, 255, 255))
         elif tag == "DEBUG":
             if not self.debug:
                 return
             tag_text = self.fade(tag_text, (0, 0, 255), (0, 191, 255))
+        else:
+            print(f"{timestamp} [{inittag}] Invalid Tag: {tag}")
+            input()
+            exit()
 
-        # get the current timestamp
-        current_time = time.time()
-        time_elapsed = current_time - self.last_timestamp
-        self.last_timestamp = current_time
-
-        # delay the output based on the specified speed
-        time.sleep(max(1 / self.speed - time_elapsed, 0))
+        current_time = datetime.now().strftime("%H:%M:%S")
+        time_elapsed = time.time() - self.last_timestamp
+        self.last_timestamp += max(1 / self.speed - time_elapsed, 0)
 
-        # print the timestamp, tag, and message
-        timestamp = self.getTimestamp()
-        print(f"{timestamp} [{tag_text}] {message_text}")
+        print(f"{timestamp} [{tag_text}] {message_text}")
```

