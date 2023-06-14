# Comparing `tmp/json-stream-2.3.0.tar.gz` & `tmp/json-stream-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-stream-2.3.0.tar", last modified: Wed Mar 29 21:42:05 2023, max compression
+gzip compressed data, was "json-stream-2.3.1.tar", last modified: Wed Jun 14 22:50:05 2023, max compression
```

## Comparing `json-stream-2.3.0.tar` & `json-stream-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.338929 json-stream-2.3.0/
--rw-r--r--   0 jamie      (501) staff       (20)     1058 2022-08-06 08:09:13.000000 json-stream-2.3.0/LICENSE.txt
--rw-r--r--   0 jamie      (501) staff       (20)    23966 2023-03-29 21:42:05.338768 json-stream-2.3.0/PKG-INFO
--rw-r--r--   0 jamie      (501) staff       (20)    21638 2023-02-21 10:49:10.000000 json-stream-2.3.0/README.md
--rw-r--r--   0 jamie      (501) staff       (20)     1452 2023-03-29 21:39:12.000000 json-stream-2.3.0/pyproject.toml
--rw-r--r--   0 jamie      (501) staff       (20)       38 2023-03-29 21:42:05.338960 json-stream-2.3.0/setup.cfg
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.330777 json-stream-2.3.0/src/
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.334357 json-stream-2.3.0/src/json_stream/
--rw-r--r--   0 jamie      (501) staff       (20)      227 2023-02-21 10:49:10.000000 json-stream-2.3.0/src/json_stream/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     8908 2023-03-29 21:41:45.000000 json-stream-2.3.0/src/json_stream/base.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.335579 json-stream-2.3.0/src/json_stream/dump/
--rw-r--r--   0 jamie      (501) staff       (20)      569 2023-02-21 10:49:10.000000 json-stream-2.3.0/src/json_stream/dump/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.335925 json-stream-2.3.0/src/json_stream/dump/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.0/src/json_stream/dump/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1533 2023-02-21 10:49:10.000000 json-stream-2.3.0/src/json_stream/dump/tests/test_dump.py
--rw-r--r--   0 jamie      (501) staff       (20)     1476 2022-08-06 08:09:13.000000 json-stream-2.3.0/src/json_stream/dump/threading.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.336103 json-stream-2.3.0/src/json_stream/httpx/
--rw-r--r--   0 jamie      (501) staff       (20)      602 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/httpx/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.336433 json-stream-2.3.0/src/json_stream/httpx/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/httpx/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1876 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/httpx/tests/test_httpx.py
--rw-r--r--   0 jamie      (501) staff       (20)      728 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/iterators.py
--rw-r--r--   0 jamie      (501) staff       (20)      483 2023-03-29 21:41:45.000000 json-stream-2.3.0/src/json_stream/loader.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.336665 json-stream-2.3.0/src/json_stream/requests/
--rw-r--r--   0 jamie      (501) staff       (20)      604 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/requests/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.336924 json-stream-2.3.0/src/json_stream/requests/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.0/src/json_stream/requests/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1940 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/requests/tests/test_requests.py
--rw-r--r--   0 jamie      (501) staff       (20)      387 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/select_tokenizer.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.338563 json-stream-2.3.0/src/json_stream/tests/
--rw-r--r--   0 jamie      (501) staff       (20)     3053 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)      500 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/tests/test_iterators.py
--rw-r--r--   0 jamie      (501) staff       (20)     9984 2023-03-29 21:39:12.000000 json-stream-2.3.0/src/json_stream/tests/test_loader.py
--rw-r--r--   0 jamie      (501) staff       (20)     7209 2023-03-17 22:41:52.000000 json-stream-2.3.0/src/json_stream/tests/test_tokenizer.py
--rw-r--r--   0 jamie      (501) staff       (20)     1454 2023-03-17 22:41:52.000000 json-stream-2.3.0/src/json_stream/tests/test_tokenizer_integration.py
--rw-r--r--   0 jamie      (501) staff       (20)      440 2023-02-21 10:49:10.000000 json-stream-2.3.0/src/json_stream/tests/test_util.py
--rw-r--r--   0 jamie      (501) staff       (20)      884 2022-08-06 08:09:13.000000 json-stream-2.3.0/src/json_stream/tests/test_visitor.py
--rw-r--r--   0 jamie      (501) staff       (20)     1132 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/tests/test_writer.py
--rw-r--r--   0 jamie      (501) staff       (20)    13422 2023-03-17 22:41:52.000000 json-stream-2.3.0/src/json_stream/tokenizer.py
--rw-r--r--   0 jamie      (501) staff       (20)     2071 2023-02-21 10:49:10.000000 json-stream-2.3.0/src/json_stream/util.py
--rw-r--r--   0 jamie      (501) staff       (20)      902 2023-03-29 21:41:45.000000 json-stream-2.3.0/src/json_stream/visitor.py
--rw-r--r--   0 jamie      (501) staff       (20)     1775 2023-02-11 10:45:16.000000 json-stream-2.3.0/src/json_stream/writer.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-03-29 21:42:05.335251 json-stream-2.3.0/src/json_stream.egg-info/
--rw-r--r--   0 jamie      (501) staff       (20)    23966 2023-03-29 21:42:05.000000 json-stream-2.3.0/src/json_stream.egg-info/PKG-INFO
--rw-r--r--   0 jamie      (501) staff       (20)     1182 2023-03-29 21:42:05.000000 json-stream-2.3.0/src/json_stream.egg-info/SOURCES.txt
--rw-r--r--   0 jamie      (501) staff       (20)        1 2023-03-29 21:42:05.000000 json-stream-2.3.0/src/json_stream.egg-info/dependency_links.txt
--rw-r--r--   0 jamie      (501) staff       (20)       69 2023-03-29 21:42:05.000000 json-stream-2.3.0/src/json_stream.egg-info/requires.txt
--rw-r--r--   0 jamie      (501) staff       (20)       12 2023-03-29 21:42:05.000000 json-stream-2.3.0/src/json_stream.egg-info/top_level.txt
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.467652 json-stream-2.3.1/
+-rw-r--r--   0 jamie      (501) staff       (20)     1058 2022-08-06 08:09:13.000000 json-stream-2.3.1/LICENSE.txt
+-rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-14 22:50:05.467490 json-stream-2.3.1/PKG-INFO
+-rw-r--r--   0 jamie      (501) staff       (20)    21632 2023-06-13 15:55:51.000000 json-stream-2.3.1/README.md
+-rw-r--r--   0 jamie      (501) staff       (20)     1452 2023-06-13 16:26:36.000000 json-stream-2.3.1/pyproject.toml
+-rw-r--r--   0 jamie      (501) staff       (20)       38 2023-06-14 22:50:05.467689 json-stream-2.3.1/setup.cfg
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.460083 json-stream-2.3.1/src/
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.463400 json-stream-2.3.1/src/json_stream/
+-rw-r--r--   0 jamie      (501) staff       (20)      227 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     8908 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/base.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464447 json-stream-2.3.1/src/json_stream/dump/
+-rw-r--r--   0 jamie      (501) staff       (20)      569 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/dump/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464774 json-stream-2.3.1/src/json_stream/dump/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/dump/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1533 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/dump/tests/test_dump.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1476 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/dump/threading.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464950 json-stream-2.3.1/src/json_stream/httpx/
+-rw-r--r--   0 jamie      (501) staff       (20)      602 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465306 json-stream-2.3.1/src/json_stream/httpx/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1876 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/tests/test_httpx.py
+-rw-r--r--   0 jamie      (501) staff       (20)      728 2023-06-07 13:57:08.000000 json-stream-2.3.1/src/json_stream/iterators.py
+-rw-r--r--   0 jamie      (501) staff       (20)      483 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/loader.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465560 json-stream-2.3.1/src/json_stream/requests/
+-rw-r--r--   0 jamie      (501) staff       (20)      604 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/requests/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465803 json-stream-2.3.1/src/json_stream/requests/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/requests/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1940 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/requests/tests/test_requests.py
+-rw-r--r--   0 jamie      (501) staff       (20)      387 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/select_tokenizer.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.467275 json-stream-2.3.1/src/json_stream/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)     3053 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)      500 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/test_iterators.py
+-rw-r--r--   0 jamie      (501) staff       (20)    10284 2023-06-13 15:56:01.000000 json-stream-2.3.1/src/json_stream/tests/test_loader.py
+-rw-r--r--   0 jamie      (501) staff       (20)    10353 2023-06-14 22:48:01.000000 json-stream-2.3.1/src/json_stream/tests/test_tokenizer.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1454 2023-03-17 22:41:52.000000 json-stream-2.3.1/src/json_stream/tests/test_tokenizer_integration.py
+-rw-r--r--   0 jamie      (501) staff       (20)      440 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/tests/test_util.py
+-rw-r--r--   0 jamie      (501) staff       (20)      884 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/tests/test_visitor.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1132 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/test_writer.py
+-rw-r--r--   0 jamie      (501) staff       (20)    14198 2023-06-14 22:48:01.000000 json-stream-2.3.1/src/json_stream/tokenizer.py
+-rw-r--r--   0 jamie      (501) staff       (20)     2071 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/util.py
+-rw-r--r--   0 jamie      (501) staff       (20)      902 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/visitor.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1775 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/writer.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464154 json-stream-2.3.1/src/json_stream.egg-info/
+-rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/PKG-INFO
+-rw-r--r--   0 jamie      (501) staff       (20)     1182 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie      (501) staff       (20)        1 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie      (501) staff       (20)       69 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/requires.txt
+-rw-r--r--   0 jamie      (501) staff       (20)       12 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/top_level.txt
```

### Comparing `json-stream-2.3.0/LICENSE.txt` & `json-stream-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/PKG-INFO` & `json-stream-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream
-Version: 2.3.0
+Version: 2.3.1
 Summary: Streaming JSON encoder and decoder
 Author-email: Jamie Cockburn <jamie_cockburn@hotmail.co.uk>
 License: Copyright (c) 2020 Jamie Cockburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -105,16 +105,16 @@
 
 It is also possible to "mix" the modes as you consume the data.
 
 #### Transient mode (default)
 
 This mode is appropriate if you can consume the data iteratively. You cannot 
 move backwards through the stream to read data that has already been skipped
-over. It is the mode you **must** use if you want process large amounts of
-JSON data without consuming large amounts of memory required.
+over. It is the mode you **must** use if you want to process large amounts of
+JSON data without consuming large amounts of memory.
 
 In transient mode, only the data currently being read is stored in memory. Any
 data previously read from the stream is discarded (it's up to you what to do 
 with it) and attempting to access this data results in a
 `TransientAccessException`.
 
 ```python
```

### Comparing `json-stream-2.3.0/README.md` & `json-stream-2.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 
 It is also possible to "mix" the modes as you consume the data.
 
 #### Transient mode (default)
 
 This mode is appropriate if you can consume the data iteratively. You cannot 
 move backwards through the stream to read data that has already been skipped
-over. It is the mode you **must** use if you want process large amounts of
-JSON data without consuming large amounts of memory required.
+over. It is the mode you **must** use if you want to process large amounts of
+JSON data without consuming large amounts of memory.
 
 In transient mode, only the data currently being read is stored in memory. Any
 data previously read from the stream is discarded (it's up to you what to do 
 with it) and attempting to access this data results in a
 `TransientAccessException`.
 
 ```python
```

### Comparing `json-stream-2.3.0/pyproject.toml` & `json-stream-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "json-stream"
-version = "2.3.0"
+version = "2.3.1"
 authors = [
     {name = "Jamie Cockburn", email="jamie_cockburn@hotmail.co.uk"},
 ]
 license = {file = "LICENSE.txt"}
 description = "Streaming JSON encoder and decoder"
 keywords = ["json", "stream", "decoder", "encoder", "parsing"]
 classifiers = [
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.5,<4"
-dependencies = ["json-stream-rs-tokenizer >= 0.4.16"]
+dependencies = ["json-stream-rs-tokenizer >= 0.4.17"]
 dynamic = ["readme"]
 
 [project.urls]
 Homepage = "https://github.com/daggaz/json-stream"
 Repository = "https://github.com/daggaz/json-stream"
 Tracker = "https://github.com/daggaz/json-stream/issues"
 Funding = "https://www.buymeacoffee.com/daggaz"
```

### Comparing `json-stream-2.3.0/src/json_stream/base.py` & `json-stream-2.3.1/src/json_stream/base.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/dump/__init__.py` & `json-stream-2.3.1/src/json_stream/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/dump/tests/test_dump.py` & `json-stream-2.3.1/src/json_stream/dump/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/dump/threading.py` & `json-stream-2.3.1/src/json_stream/dump/threading.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/httpx/__init__.py` & `json-stream-2.3.1/src/json_stream/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/httpx/tests/test_httpx.py` & `json-stream-2.3.1/src/json_stream/httpx/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/iterators.py` & `json-stream-2.3.1/src/json_stream/iterators.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/requests/__init__.py` & `json-stream-2.3.1/src/json_stream/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/requests/tests/test_requests.py` & `json-stream-2.3.1/src/json_stream/requests/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/tests/__init__.py` & `json-stream-2.3.1/src/json_stream/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/tests/test_loader.py` & `json-stream-2.3.1/src/json_stream/tests/test_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import json
 from io import StringIO
 
 from json_stream import load
 from json_stream.base import (
     TransientAccessException,
     PersistentStreamingJSONObject,
     TransientStreamingJSONList,
@@ -102,16 +103,16 @@
         self.assertTrue(data[1])
         self.assertEqual(data[2], "")
         with self.assertRaises(IndexError):
             _ = data[3]
 
         # Access out of order
         data = load(StringIO(json_str), persistent=True)
-        self.assertEqual(data[0], 1)
         self.assertTrue(data[1])
+        self.assertEqual(data[0], 1)
         self.assertEqual(data[2], "")
         with self.assertRaises(IndexError):
             _ = data[3]
 
     def test_load_list_get_transient(self):
         json_str = '[1, true, ""]'
 
@@ -242,7 +243,17 @@
             load(StringIO('{"x"')).read_all()
         with self.assertRaisesRegex(ValueError, "Unterminated object at end of file"):
             load(StringIO('{"x":')).read_all()
         with self.assertRaisesRegex(ValueError, "Unterminated object at end of file"):
             load(StringIO('{"x": 1')).read_all()
         with self.assertRaisesRegex(ValueError, "Unterminated object at end of file"):
             load(StringIO('{"x": 1,')).read_all()
+
+    def test_unicode(self):
+        data = json.dumps('Ä')
+        result = load(StringIO(data))
+        self.assertEqual(result, 'Ä')
+
+    def test_non_bmp_unicode(self):
+        data = json.dumps('𝄞')
+        result = load(StringIO(data))
+        self.assertEqual(result, '𝄞')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `json-stream-2.3.0/src/json_stream/tests/test_tokenizer_integration.py` & `json-stream-2.3.1/src/json_stream/tests/test_tokenizer_integration.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/tests/test_visitor.py` & `json-stream-2.3.1/src/json_stream/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/tests/test_writer.py` & `json-stream-2.3.1/src/json_stream/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/tokenizer.py` & `json-stream-2.3.1/src/json_stream/tokenizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 Taken from the NAYA project
 
 https://github.com/danielyule/naya
 
 Copyright (c) 2019 Daniel Yule
 """
 import io
+import unicodedata
+
+SURROGATE = 'Cs'
 
 
 class TokenType:
     OPERATOR = 0
     STRING = 1
     NUMBER = 2
     BOOLEAN = 3
@@ -34,18 +37,18 @@
     FALSE_1 = 15
     FALSE_2 = 16
     FALSE_3 = 17
     FALSE_4 = 18
     NULL_1 = 19
     NULL_2 = 20
     NULL_3 = 21
-    UNICODE_1 = 22
-    UNICODE_2 = 23
-    UNICODE_3 = 24
-    UNICODE_4 = 25
+    UNICODE = 22
+    UNICODE_SURROGATE_START = 23
+    UNICODE_SURROGATE_STRING_ESCAPE = 24
+    UNICODE_SURROGATE = 25
 
 
 class SpecialChar:
     # Kind of a hack but simple: if we used the empty string "" to represent
     # EOF, expressions like `char in "0123456789"` would be true for EOF, which
     # is confusing. If we used a non-string, they would result in TypeErrors.
     # By using the string "EOF", they work as expected. The only thing we have
@@ -78,20 +81,20 @@
 def tokenize(stream):
     stream = _ensure_text(stream)
 
     def is_delimiter(char):
         return char.isspace() or char in "{}[]:," or char == SpecialChar.EOF
 
     token = []
-    charcode = 0
+    unicode_buffer = ""
     completed = False
     now_token = ""
 
-    def process_char(char, charcode):
-        nonlocal token, completed, now_token
+    def process_char(char):
+        nonlocal token, completed, now_token, unicode_buffer
         advance = True
         add_char = False
         next_state = state
         if state == State.WHITESPACE:
             if char == "{":
                 completed = True
                 now_token = (TokenType.OPERATOR, "{")
@@ -271,15 +274,15 @@
             else:
                 add_char = True
         elif state == State.STRING_END:
             if is_delimiter(char):
                 advance = False
                 next_state = State.WHITESPACE
             else:
-                raise ValueError("Expected whitespace or an operator after strin.  Got '{}'".format(char))
+                raise ValueError("Expected whitespace or an operator after string.  Got '{}'".format(char))
         elif state == State.STRING_ESCAPE:
             next_state = State.STRING
             if char == "\\" or char == "\"":
                 add_char = True
             elif char == "b":
                 char = "\b"
                 add_char = True
@@ -295,79 +298,87 @@
             elif char == "r":
                 char = "\r"
                 add_char = True
             elif char == "/":
                 char = "/"
                 add_char = True
             elif char == "u":
-                next_state = State.UNICODE_1
-                charcode = 0
+                next_state = State.UNICODE
+                unicode_buffer = ""
             else:
                 raise ValueError("Invalid string escape: {}".format(char))
-        elif state == State.UNICODE_1:
-            if char in "0123456789":
-                charcode = (ord(char) - 48) * 4096
-            elif char in "abcdef":
-                charcode = (ord(char) - 87) * 4096
-            elif char in "ABCDEF":
-                charcode = (ord(char) - 55) * 4096
-            else:
-                raise ValueError("Invalid character code: {}".format(char))
-            next_state = State.UNICODE_2
-            char = ""
-        elif state == State.UNICODE_2:
-            if char in "0123456789":
-                charcode += (ord(char) - 48) * 256
-            elif char in "abcdef":
-                charcode += (ord(char) - 87) * 256
-            elif char in "ABCDEF":
-                charcode += (ord(char) - 55) * 256
-            else:
-                raise ValueError("Invalid character code: {}".format(char))
-            next_state = State.UNICODE_3
-            char = ""
-        elif state == State.UNICODE_3:
-            if char in "0123456789":
-                charcode += (ord(char) - 48) * 16
-            elif char in "abcdef":
-                charcode += (ord(char) - 87) * 16
-            elif char in "ABCDEF":
-                charcode += (ord(char) - 55) * 16
-            else:
-                raise ValueError("Invalid character code: {}".format(char))
-            next_state = State.UNICODE_4
-            char = ""
-        elif state == State.UNICODE_4:
-            if char in "0123456789":
-                charcode += ord(char) - 48
-            elif char in "abcdef":
-                charcode += ord(char) - 87
-            elif char in "ABCDEF":
-                charcode += ord(char) - 55
+        elif state == State.UNICODE:
+            if char == SpecialChar.EOF:
+                raise ValueError('Unterminated unicode literal at end of file')
+            unicode_buffer += char
+            if len(unicode_buffer) == 4:
+                try:
+                    code_point = int(unicode_buffer, 16)
+                except ValueError:
+                    raise ValueError(f"Invalid unicode literal: \\u{unicode_buffer}")
+                char = chr(code_point)
+                if unicodedata.category(char) == SURROGATE:
+                    next_state = State.UNICODE_SURROGATE_START
+                else:
+                    next_state = State.STRING
+                    add_char = True
+        elif state == State.UNICODE_SURROGATE_START:
+            if char == "\\":
+                next_state = State.UNICODE_SURROGATE_STRING_ESCAPE
+            elif char == SpecialChar.EOF:
+                raise ValueError("Unpaired UTF-16 surrogate at end of file")
             else:
-                raise ValueError("Invalid character code: {}".format(char))
-            next_state = State.STRING
-            char = chr(charcode)
-            add_char = True
+                raise ValueError(f"Unpaired UTF-16 surrogate")
+
+        elif state == State.UNICODE_SURROGATE_STRING_ESCAPE:
+            if char == "u":
+                next_state = State.UNICODE_SURROGATE
+            elif char == SpecialChar.EOF:
+                raise ValueError("Unpaired UTF-16 surrogate at end of file")
+            else:
+                raise ValueError(f"Unpaired UTF-16 surrogate")
+
+        elif state == State.UNICODE_SURROGATE:
+            if char == SpecialChar.EOF:
+                raise ValueError('Unterminated unicode literal at end of file')
+            unicode_buffer += char
+            if len(unicode_buffer) == 8:
+                code_point_1 = int(unicode_buffer[:4], 16)
+                try:
+                    code_point_2 = int(unicode_buffer[4:], 16)
+                except ValueError:
+                    raise ValueError(f"Invalid unicode literal: \\u{unicode_buffer[4:]}")
+                char = chr(code_point_2)
+                if unicodedata.category(char) != SURROGATE:
+                    raise ValueError(f"Second half of UTF-16 surrogate pair is not a surrogate!")
+                try:
+                    pair = int.to_bytes(code_point_1, 2, 'little') + int.to_bytes(code_point_2, 2, 'little')
+                    char = pair.decode('utf-16-le')
+                except ValueError:
+                    raise ValueError(
+                        f"Error decoding UTF-16 surrogate pair \\u{unicode_buffer[:4]}\\u{unicode_buffer[4:]}"
+                    )
+                next_state = State.STRING
+                add_char = True
 
         if add_char:
             token.append(char)
 
-        return advance, next_state, charcode
+        return advance, next_state
     state = State.WHITESPACE
-    char = stream.read(1)
+    c = stream.read(1)
     index = 0
-    while char:
+    while c:
         try:
-            advance, state, charcode = process_char(char, charcode)
+            advance, state = process_char(c)
         except ValueError as e:
             raise ValueError("".join([e.args[0], " at index {}".format(index)]))
         if completed:
             completed = False
             token = []
             yield now_token
         if advance:
-            char = stream.read(1)
+            c = stream.read(1)
             index += 1
-    process_char(SpecialChar.EOF, charcode)
+    process_char(SpecialChar.EOF)
     if completed:
         yield now_token
```

### Comparing `json-stream-2.3.0/src/json_stream/util.py` & `json-stream-2.3.1/src/json_stream/util.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/visitor.py` & `json-stream-2.3.1/src/json_stream/visitor.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream/writer.py` & `json-stream-2.3.1/src/json_stream/writer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.0/src/json_stream.egg-info/PKG-INFO` & `json-stream-2.3.1/src/json_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream
-Version: 2.3.0
+Version: 2.3.1
 Summary: Streaming JSON encoder and decoder
 Author-email: Jamie Cockburn <jamie_cockburn@hotmail.co.uk>
 License: Copyright (c) 2020 Jamie Cockburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -105,16 +105,16 @@
 
 It is also possible to "mix" the modes as you consume the data.
 
 #### Transient mode (default)
 
 This mode is appropriate if you can consume the data iteratively. You cannot 
 move backwards through the stream to read data that has already been skipped
-over. It is the mode you **must** use if you want process large amounts of
-JSON data without consuming large amounts of memory required.
+over. It is the mode you **must** use if you want to process large amounts of
+JSON data without consuming large amounts of memory.
 
 In transient mode, only the data currently being read is stored in memory. Any
 data previously read from the stream is discarded (it's up to you what to do 
 with it) and attempting to access this data results in a
 `TransientAccessException`.
 
 ```python
```

### Comparing `json-stream-2.3.0/src/json_stream.egg-info/SOURCES.txt` & `json-stream-2.3.1/src/json_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

