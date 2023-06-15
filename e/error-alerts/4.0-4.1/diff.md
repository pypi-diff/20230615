# Comparing `tmp/error-alerts-4.0.tar.gz` & `tmp/error-alerts-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.0.tar", last modified: Wed Apr  5 17:26:07 2023, max compression
+gzip compressed data, was "error-alerts-4.1.tar", last modified: Thu Jun 15 14:36:34 2023, max compression
```

## Comparing `error-alerts-4.0.tar` & `error-alerts-4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 17:26:07.924097 error-alerts-4.0/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.0/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-04-05 17:26:07.924097 error-alerts-4.0/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 17:26:07.919100 error-alerts-4.0/error_alerts/
--rw-rw-rw-   0        0        0     2281 2023-04-05 17:25:52.000000 error-alerts-4.0/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 17:26:07.923097 error-alerts-4.0/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-04-05 17:26:06.000000 error-alerts-4.0/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-05 17:26:06.000000 error-alerts-4.0/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 17:26:06.000000 error-alerts-4.0/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-05 17:26:06.000000 error-alerts-4.0/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 17:26:06.000000 error-alerts-4.0/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-05 17:26:07.925096 error-alerts-4.0/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-04-05 17:26:02.000000 error-alerts-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.771242 error-alerts-4.1/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.1/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-15 14:36:34.771242 error-alerts-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.765246 error-alerts-4.1/error_alerts/
+-rw-rw-rw-   0        0        0     2280 2023-04-12 16:43:51.000000 error-alerts-4.1/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:36:34.770243 error-alerts-4.1/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 14:36:34.000000 error-alerts-4.1/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 14:36:34.771242 error-alerts-4.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-15 14:34:49.000000 error-alerts-4.1/setup.py
```

### Comparing `error-alerts-4.0/PKG-INFO` & `error-alerts-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.0
+Version: 4.1
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.0/README.md` & `error-alerts-4.1/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.0/error_alerts/__init__.py` & `error-alerts-4.1/error_alerts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import traceback
 from telegram import Bot
 
 class telegram:
-    def __init__(self, token=None, channel=None, logger=None, full_error=False, raise_error=False, resend_repeat_errors=True):
+    def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
         if token:
             self.bot = Bot(token=token)
         self.channel = channel
         self.logger = logger
         self.full_error = full_error
         self.raise_error = raise_error
         self.resend_repeat_errors = resend_repeat_errors
```

### Comparing `error-alerts-4.0/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.1/error_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.0
+Version: 4.1
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

