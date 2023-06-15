# Comparing `tmp/selis-2.1.tar.gz` & `tmp/selis-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.1.tar", last modified: Wed Jun 14 16:31:01 2023, max compression
+gzip compressed data, was "selis-2.2.tar", last modified: Thu Jun 15 16:17:50 2023, max compression
```

## Comparing `selis-2.1.tar` & `selis-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:31:01.632518 selis-2.1/
--rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:31:01.632393 selis-2.1/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:31:01.631367 selis-2.1/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.1/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3935 2023-06-14 16:30:42.000000 selis-2.1/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.1/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-14 16:31:01.632210 selis-2.1/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)       47 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       43 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-14 16:31:01.000000 selis-2.1/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-14 16:31:01.632564 selis-2.1/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      254 2023-06-14 16:30:51.000000 selis-2.1/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:17:50.354521 selis-2.2/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:17:50.354400 selis-2.2/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:17:50.353043 selis-2.2/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.2/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4863 2023-06-15 16:17:22.000000 selis-2.2/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)     1472 2023-06-14 16:21:18.000000 selis-2.2/selis/selis.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-15 16:17:50.354177 selis-2.2/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      233 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-15 16:17:50.000000 selis-2.2/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-15 16:17:50.354569 selis-2.2/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      254 2023-06-15 16:17:39.000000 selis-2.2/setup.py
```

### Comparing `selis-2.1/selis/client.py` & `selis-2.2/selis/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 import socket
 import threading
 import sys
 import getpass
 import webbrowser
 import random
+import requests
 
 from optparse import OptionParser
+from bs4 import BeautifulSoup
 
 
 class Client:
     def __init__(self, ip, port, nickname, admin_mode):
         self.admin_mode = admin_mode
         self.nickname = nickname
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             self.connection.connect((ip, port))
         except:
             print(f"[-] Sever not found")
             sys.exit()
-        self.send_nickname_to_sever()
+        self.send_info_user_to_sever()
         self.is_running = True
 
 
-    def send_nickname_to_sever(self):
-        self.connection.send((self.nickname).encode())
+    def return_info_response(self, url):
+        headers = {"User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"}
+        response = requests.get(url, headers=headers)
+        soup = BeautifulSoup(response.content, "html.parser")
+        return soup
+    
+
+    def get_info_user(self, soup):
+        content = soup.find_all("td")
+        for i, element in enumerate(content):
+            if i == 4:
+                ip = element.get_text()
+            elif i == 5:
+                device = element.get_text()
+            elif i == 6:
+                operation_system = element.get_text()
+
+        return ip + "/" + device + "/" + operation_system
+
+
+    def send_info_user_to_sever(self):
+        response = self.return_info_response("https://www.iplocation.net/find-ip-address")
+        info = self.get_info_user(response)
+        msg = self.nickname + "/" + info
+        self.send_message(msg)
 
 
     def send_message(self, message):
         try:
             self.connection.send(message.encode())
         except:
             exit()
```

### Comparing `selis-2.1/selis/selis.py` & `selis-2.2/selis/selis.py`

 * *Files identical despite different names*

