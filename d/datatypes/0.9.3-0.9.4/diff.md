# Comparing `tmp/datatypes-0.9.3.tar.gz` & `tmp/datatypes-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatypes-0.9.3.tar", last modified: Mon Mar 20 20:45:03 2023, max compression
+gzip compressed data, was "datatypes-0.9.4.tar", last modified: Thu Jun 15 04:30:59 2023, max compression
```

## Comparing `datatypes-0.9.3.tar` & `datatypes-0.9.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:45:03.977558 datatypes-0.9.3/
--rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.3/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-03-20 20:45:03.977418 datatypes-0.9.3/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.3/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:45:03.975520 datatypes-0.9.3/datatypes/
--rw-r--r--   0 jaymon     (501) staff       (20)     2270 2023-03-20 20:44:47.000000 datatypes-0.9.3/datatypes/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.3/datatypes/collections.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.3/datatypes/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.3/datatypes/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.3/datatypes/copy.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.3/datatypes/csv.py
--rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.3/datatypes/datetime.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:45:03.977126 datatypes-0.9.3/datatypes/decorators/
--rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.3/datatypes/decorators/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.3/datatypes/decorators/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.3/datatypes/decorators/descriptor.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.3/datatypes/decorators/misc.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.3/datatypes/email.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.3/datatypes/enum.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.3/datatypes/environ.py
--rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.3/datatypes/event.py
--rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.3/datatypes/html.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.3/datatypes/http.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11257 2023-03-08 19:50:47.000000 datatypes-0.9.3/datatypes/logging.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3793 2023-03-04 00:19:04.000000 datatypes-0.9.3/datatypes/number.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3739 2023-02-27 22:36:06.000000 datatypes-0.9.3/datatypes/parse.py
--rw-r--r--   0 jaymon     (501) staff       (20)   123959 2023-02-07 08:03:33.000000 datatypes-0.9.3/datatypes/path.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.3/datatypes/profile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35861 2023-03-15 19:55:58.000000 datatypes-0.9.3/datatypes/reflection.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11167 2023-02-18 01:09:49.000000 datatypes-0.9.3/datatypes/server.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.3/datatypes/service.py
--rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.3/datatypes/string.py
--rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.3/datatypes/token.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.3/datatypes/url.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.3/datatypes/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-03-20 20:45:03.976162 datatypes-0.9.3/datatypes.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-03-20 20:45:03.000000 datatypes-0.9.3/datatypes.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-03-20 20:45:03.000000 datatypes-0.9.3/datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-03-20 20:45:03.000000 datatypes-0.9.3/datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-03-20 20:45:03.000000 datatypes-0.9.3/datatypes.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-03-20 20:45:03.977600 datatypes-0.9.3/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.3/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.400069 datatypes-0.9.4/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1083 2020-07-08 22:29:16.000000 datatypes-0.9.4/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-06-15 04:30:59.399937 datatypes-0.9.4/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      408 2020-07-08 22:45:30.000000 datatypes-0.9.4/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.398208 datatypes-0.9.4/datatypes/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2287 2023-06-15 04:29:18.000000 datatypes-0.9.4/datatypes/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    33663 2023-02-18 01:09:36.000000 datatypes-0.9.4/datatypes/collections.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5556 2023-02-18 01:09:45.000000 datatypes-0.9.4/datatypes/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7749 2023-02-16 23:56:47.000000 datatypes-0.9.4/datatypes/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4902 2023-01-15 22:38:58.000000 datatypes-0.9.4/datatypes/copy.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11028 2021-09-01 07:52:59.000000 datatypes-0.9.4/datatypes/csv.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    22349 2023-03-04 08:31:34.000000 datatypes-0.9.4/datatypes/datetime.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.399647 datatypes-0.9.4/datatypes/decorators/
+-rw-r--r--   0 jaymon     (501) staff       (20)      389 2023-01-20 01:17:21.000000 datatypes-0.9.4/datatypes/decorators/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    14105 2023-02-01 23:11:59.000000 datatypes-0.9.4/datatypes/decorators/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13007 2023-01-30 19:17:34.000000 datatypes-0.9.4/datatypes/decorators/descriptor.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3551 2023-02-01 23:14:06.000000 datatypes-0.9.4/datatypes/decorators/misc.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11912 2022-12-23 00:30:10.000000 datatypes-0.9.4/datatypes/email.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5747 2020-08-06 08:36:37.000000 datatypes-0.9.4/datatypes/enum.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7575 2023-02-16 08:34:44.000000 datatypes-0.9.4/datatypes/environ.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     7339 2023-01-26 00:06:46.000000 datatypes-0.9.4/datatypes/event.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    15804 2023-01-21 21:27:07.000000 datatypes-0.9.4/datatypes/html.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23175 2023-02-27 22:34:26.000000 datatypes-0.9.4/datatypes/http.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11306 2023-06-15 04:11:55.000000 datatypes-0.9.4/datatypes/logging.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5758 2023-06-13 23:17:08.000000 datatypes-0.9.4/datatypes/number.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3739 2023-02-27 22:36:06.000000 datatypes-0.9.4/datatypes/parse.py
+-rw-r--r--   0 jaymon     (501) staff       (20)   124391 2023-06-13 20:01:59.000000 datatypes-0.9.4/datatypes/path.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6236 2023-03-18 21:36:58.000000 datatypes-0.9.4/datatypes/profile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35861 2023-03-15 19:55:58.000000 datatypes-0.9.4/datatypes/reflection.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11167 2023-02-18 01:09:49.000000 datatypes-0.9.4/datatypes/server.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6612 2023-02-16 00:02:52.000000 datatypes-0.9.4/datatypes/service.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    42752 2023-02-21 19:23:11.000000 datatypes-0.9.4/datatypes/string.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    12955 2023-01-06 07:52:19.000000 datatypes-0.9.4/datatypes/token.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23472 2023-01-24 22:20:57.000000 datatypes-0.9.4/datatypes/url.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2828 2023-02-18 01:11:42.000000 datatypes-0.9.4/datatypes/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-15 04:30:59.398772 datatypes-0.9.4/datatypes.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1013 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      784 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       10 2023-06-15 04:30:59.000000 datatypes-0.9.4/datatypes.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-15 04:30:59.400108 datatypes-0.9.4/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1950 2020-07-08 22:29:00.000000 datatypes-0.9.4/setup.py
```

### Comparing `datatypes-0.9.3/LICENSE.txt` & `datatypes-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/PKG-INFO` & `datatypes-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.3
+Version: 0.9.4
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.3/datatypes/__init__.py` & `datatypes-0.9.4/datatypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     HTMLTokenizer,
 )
 from .number import (
     Shorten,
     Integer,
     Hex,
     Binary,
+    Exponential,
 )
 from .collections import (
     Pool,
     PriorityQueue,
     Dict,
     NormalizeDict,
     idict, IDict, Idict, iDict,
@@ -126,14 +127,14 @@
 from .server import (
     PathServer,
     CallbackServer,
     WSGIServer,
 )
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 
 # get rid of "No handler found" warnings (cribbed from requests)
 # DEPRECATED 7-15-2022, doesn't seem to be needed in python3
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `datatypes-0.9.3/datatypes/collections.py` & `datatypes-0.9.4/datatypes/collections.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/compat.py` & `datatypes-0.9.4/datatypes/compat.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/config.py` & `datatypes-0.9.4/datatypes/config.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/copy.py` & `datatypes-0.9.4/datatypes/copy.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/csv.py` & `datatypes-0.9.4/datatypes/csv.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/datetime.py` & `datatypes-0.9.4/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/decorators/base.py` & `datatypes-0.9.4/datatypes/decorators/base.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/decorators/descriptor.py` & `datatypes-0.9.4/datatypes/decorators/descriptor.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/decorators/misc.py` & `datatypes-0.9.4/datatypes/decorators/misc.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/email.py` & `datatypes-0.9.4/datatypes/email.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/enum.py` & `datatypes-0.9.4/datatypes/enum.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/environ.py` & `datatypes-0.9.4/datatypes/environ.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/event.py` & `datatypes-0.9.4/datatypes/event.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/html.py` & `datatypes-0.9.4/datatypes/html.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/http.py` & `datatypes-0.9.4/datatypes/http.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/logging.py` & `datatypes-0.9.4/datatypes/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 from logging import * # allow using this module as a passthrough for builtin logging
 import logging
+import logging.config
+from logging import config
 import sys
 
 
 def null_config(name):
     """This will configure a null logger for name, it is meant to avoid the "no handler found"
     warnings when libraries would use logging that hadn't been configured, but it
     seems like it is no longer needed in python 3
```

### Comparing `datatypes-0.9.3/datatypes/parse.py` & `datatypes-0.9.4/datatypes/parse.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/path.py` & `datatypes-0.9.4/datatypes/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1838,15 +1838,14 @@
         except OSError as e:
             if e.errno == errno.EACCES or e.errno == errno.EAGAIN:
                 yield None
 
             else:
                 raise
 
-
     def flock_text(self, mode="", **kwargs):
         kwargs.setdefault("encoding", self.encoding)
         kwargs.setdefault("errors", self.errors)
         return self.flock(mode, **kwargs)
 
     def open(self, mode="", buffering=-1, encoding=None, errors=None, newline=None):
         """Open the file pointed to by the path, like the built-in open() function does
@@ -1934,14 +1933,34 @@
         https://docs.python.org/3/library/pathlib.html#pathlib.Path.read_text
         """
         encoding = encoding or self.encoding
         errors = errors or self.errors
         with self.open(encoding=encoding, errors=errors) as fp:
             return fp.read()
 
+    def splitlines(self, keepends=False, encoding=None, errors=None):
+        """iterate through all the lines"""
+        encoding = encoding or self.encoding
+        errors = errors or self.errors
+        with self.open("r", encoding=encoding, errors=errors) as f:
+            for line in f:
+                yield line if keepends else line.rstrip()
+
+    def __iter__(self):
+        for line in self.splitlines():
+            yield line
+
+    def chunklines(self, linecount=1, keepends=False, encoding=None, errors=None):
+        chunk = []
+        for i, line in enumerate(self.splitlines(keepends=keepends, encoding=encoding, errors=errors), 1):
+            chunk.append(line)
+            if i % linecount == 0:
+                yield chunk
+                chunk = []
+
     def prepare_bytes(self, data, **kwargs):
         """Internal method used to prepare the data to be written
 
         :param data: str, the text that will be written
         :param **kwargs: keywords, you can pass in encoding here
         :returns: tuple, (data, encoding, errors)
         """
@@ -2164,24 +2183,14 @@
         """
         if count == 0:
             ret = self.splitlines()
         else:
             ret = deque(self.splitlines(), maxlen=count)
         return ret
 
-    def splitlines(self, keepends=False):
-        """iterate through all the lines"""
-        with self.open("r", encoding=self.encoding, errors=self.errors) as f:
-            for line in f:
-                yield line if keepends else line.rstrip()
-
-    def __iter__(self):
-        for line in self.splitlines():
-            yield line
-
     def has(self, pattern=""):
         """Check for pattern in the body of the file
 
         :Example:
             d = Filepath("foo.txt")
 
             d.has("<TEXT>") # True
```

### Comparing `datatypes-0.9.3/datatypes/profile.py` & `datatypes-0.9.4/datatypes/profile.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/reflection.py` & `datatypes-0.9.4/datatypes/reflection.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/server.py` & `datatypes-0.9.4/datatypes/server.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/service.py` & `datatypes-0.9.4/datatypes/service.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/string.py` & `datatypes-0.9.4/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/token.py` & `datatypes-0.9.4/datatypes/token.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/url.py` & `datatypes-0.9.4/datatypes/url.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes/utils.py` & `datatypes-0.9.4/datatypes/utils.py`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/datatypes.egg-info/PKG-INFO` & `datatypes-0.9.4/datatypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatypes
-Version: 0.9.3
+Version: 0.9.4
 Summary: Utility Classes and Functions that are handy across multiple projects
 Home-page: http://github.com/Jaymon/datatypes
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `datatypes-0.9.3/datatypes.egg-info/SOURCES.txt` & `datatypes-0.9.4/datatypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatypes-0.9.3/setup.py` & `datatypes-0.9.4/setup.py`

 * *Files identical despite different names*

