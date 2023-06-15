# Comparing `tmp/ango-1.1.3.tar.gz` & `tmp/ango-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.1.3.tar", last modified: Wed Jun 14 14:32:46 2023, max compression
+gzip compressed data, was "ango-1.1.4.tar", last modified: Thu Jun 15 11:28:03 2023, max compression
```

## Comparing `ango-1.1.3.tar` & `ango-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:46.008013 ango-1.1.3/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-14 14:32:46.008013 ango-1.1.3/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.3/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:46.004013 ango-1.1.3/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:03.000000 ango-1.1.3/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:46.008013 ango-1.1.3/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:03.000000 ango-1.1.3/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-14 14:32:03.000000 ango-1.1.3/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-14 14:32:03.000000 ango-1.1.3/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-14 14:32:03.000000 ango-1.1.3/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5771 2023-06-14 14:32:37.000000 ango-1.1.3/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-14 14:32:03.000000 ango-1.1.3/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-14 14:32:46.008013 ango-1.1.3/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-14 14:32:45.000000 ango-1.1.3/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-14 14:32:46.000000 ango-1.1.3/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-14 14:32:45.000000 ango-1.1.3/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-14 14:32:45.000000 ango-1.1.3/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-14 14:32:45.000000 ango-1.1.3/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-14 14:32:46.008013 ango-1.1.3/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-14 14:32:37.000000 ango-1.1.3/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:28:03.019157 ango-1.1.4/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-15 11:28:03.019157 ango-1.1.4/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.4/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:28:03.019157 ango-1.1.4/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:27:31.000000 ango-1.1.4/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:28:03.019157 ango-1.1.4/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:27:31.000000 ango-1.1.4/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-15 11:27:31.000000 ango-1.1.4/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-15 11:27:31.000000 ango-1.1.4/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-15 11:27:31.000000 ango-1.1.4/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5786 2023-06-15 11:27:47.000000 ango-1.1.4/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-15 11:27:31.000000 ango-1.1.4/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-15 11:28:03.019157 ango-1.1.4/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-15 11:28:02.000000 ango-1.1.4/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-15 11:28:03.000000 ango-1.1.4/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-15 11:28:02.000000 ango-1.1.4/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-15 11:28:02.000000 ango-1.1.4/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-15 11:28:02.000000 ango-1.1.4/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-15 11:28:03.019157 ango-1.1.4/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-15 11:27:57.000000 ango-1.1.4/setup.py
```

### Comparing `ango-1.1.3/PKG-INFO` & `ango-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.3/README.md` & `ango-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.1.3/ango/models/label_category.py` & `ango-1.1.4/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.3/ango/plugin_logger.py` & `ango-1.1.4/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.3/ango/plugins.py` & `ango-1.1.4/ango/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 class Plugin(socketio.ClientNamespace):
 
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__('/plugin')
         self.id = id
         self.secret = secret
-        scheduler = BackgroundScheduler()
-        scheduler.add_job(self.heartbeat, 'interval', seconds=60)
-        scheduler.start()
+        self.scheduler = BackgroundScheduler()
+        self.scheduler.add_job(self.heartbeat, 'interval', seconds=60)
+        self.scheduler.start()
         self.logger = logging.getLogger()
         self.callback = callback
         self.loop = asyncio.get_event_loop()
 
     def on_connect(self):
         self.logger.warning("Connected")
         self.heartbeat()
```

### Comparing `ango-1.1.3/ango/sdk.py` & `ango-1.1.4/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.3/ango.egg-info/PKG-INFO` & `ango-1.1.4/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.3/setup.py` & `ango-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.1.3",
+    version="1.1.4",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

