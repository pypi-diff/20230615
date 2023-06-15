# Comparing `tmp/aiogram-ext-0.7.0.tar.gz` & `tmp/aiogram-ext-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.7.0.tar", last modified: Mon May  1 14:41:16 2023, max compression
+gzip compressed data, was "aiogram-ext-0.8.0.tar", last modified: Thu Jun 15 19:54:11 2023, max compression
```

## Comparing `aiogram-ext-0.7.0.tar` & `aiogram-ext-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1686 2023-05-01 14:40:34.383545 aiogram-ext-0.7.0/botty/__init__.py
--rw-r--r--   0        0        0      825 2023-04-30 16:54:40.161145 aiogram-ext-0.7.0/botty/bot.py
--rw-r--r--   0        0        0     1752 2023-04-30 07:58:02.593722 aiogram-ext-0.7.0/botty/broadcast.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.7.0/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.7.0/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.7.0/botty/context.py
--rw-r--r--   0        0        0     1763 2023-04-30 08:48:22.035344 aiogram-ext-0.7.0/botty/deps.py
--rw-r--r--   0        0        0     6646 2023-05-01 07:28:28.745994 aiogram-ext-0.7.0/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.7.0/botty/env.py
--rw-r--r--   0        0        0      240 2023-04-30 16:18:41.592946 aiogram-ext-0.7.0/botty/errors.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.7.0/botty/filters.py
--rw-r--r--   0        0        0     1631 2023-04-30 07:30:17.108202 aiogram-ext-0.7.0/botty/helpers.py
--rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.7.0/botty/html.py
--rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.7.0/botty/keyboards.py
--rw-r--r--   0        0        0      510 2023-05-01 14:40:34.367037 aiogram-ext-0.7.0/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.7.0/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.7.0/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.7.0/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.7.0/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.7.0/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.7.0/botty/r.py
--rw-r--r--   0        0        0      481 2023-05-01 14:41:11.144787 aiogram-ext-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.7.0/README.md
--rw-r--r--   0        0        0      315 2023-04-28 05:22:40.926562 aiogram-ext-0.7.0/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-05-01 14:40:34.383545 aiogram-ext-0.8.0/botty/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-30 16:54:40.161145 aiogram-ext-0.8.0/botty/bot.py
+-rw-r--r--   0        0        0     1752 2023-04-30 07:58:02.593722 aiogram-ext-0.8.0/botty/broadcast.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.8.0/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.8.0/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.8.0/botty/context.py
+-rw-r--r--   0        0        0     1763 2023-04-30 08:48:22.035344 aiogram-ext-0.8.0/botty/deps.py
+-rw-r--r--   0        0        0     6767 2023-06-15 19:32:00.933012 aiogram-ext-0.8.0/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.8.0/botty/env.py
+-rw-r--r--   0        0        0      240 2023-04-30 16:18:41.592946 aiogram-ext-0.8.0/botty/errors.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.8.0/botty/filters.py
+-rw-r--r--   0        0        0     1631 2023-04-30 07:30:17.108202 aiogram-ext-0.8.0/botty/helpers.py
+-rw-r--r--   0        0        0      129 2023-04-28 11:17:12.416217 aiogram-ext-0.8.0/botty/html.py
+-rw-r--r--   0        0        0      784 2023-04-28 11:05:50.359926 aiogram-ext-0.8.0/botty/keyboards.py
+-rw-r--r--   0        0        0      510 2023-05-01 14:40:34.367037 aiogram-ext-0.8.0/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.8.0/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.8.0/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.8.0/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.8.0/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.8.0/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      472 2023-04-30 07:10:43.133852 aiogram-ext-0.8.0/botty/r.py
+-rw-r--r--   0        0        0      481 2023-06-15 19:53:52.858739 aiogram-ext-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.8.0/README.md
+-rw-r--r--   0        0        0      583 2023-06-15 19:43:33.829144 aiogram-ext-0.8.0/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.8.0/PKG-INFO
```

### Comparing `aiogram-ext-0.7.0/botty/__init__.py` & `aiogram-ext-0.8.0/botty/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/bot.py` & `aiogram-ext-0.8.0/botty/bot.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/broadcast.py` & `aiogram-ext-0.8.0/botty/broadcast.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/buttons.py` & `aiogram-ext-0.8.0/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/context.py` & `aiogram-ext-0.8.0/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/deps.py` & `aiogram-ext-0.8.0/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/dispatcher.py` & `aiogram-ext-0.8.0/botty/dispatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,16 +83,19 @@
 
     def document(self):
         return DocumentHandler(self)
 
     def photo(self):
         return PhotoHandler(self)
 
-    def message(self):
-        return MessageHandler(self)
+    def message(self, content_types: str | list[str] = "any"):
+        return MessageHandler(self, content_types)
+
+    def sticker(self):
+        return self.message("sticker")
 
     def error(self, exc: Exception = Exception):
         return self.errors_handler(exception=exc)
 
     @property
     def CONTACT(self):  # noqa
         return self.contact()
```

### Comparing `aiogram-ext-0.7.0/botty/env.py` & `aiogram-ext-0.8.0/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/filters.py` & `aiogram-ext-0.8.0/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/helpers.py` & `aiogram-ext-0.8.0/botty/helpers.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/keyboards.py` & `aiogram-ext-0.8.0/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/middlewares/_conversation.py` & `aiogram-ext-0.8.0/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/middlewares/_membership.py` & `aiogram-ext-0.8.0/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/middlewares/misc.py` & `aiogram-ext-0.8.0/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.7.0/botty/middlewares/throttling.py` & `aiogram-ext-0.8.0/botty/middlewares/throttling.py`

 * *Files identical despite different names*

