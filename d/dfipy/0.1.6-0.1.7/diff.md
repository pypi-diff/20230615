# Comparing `tmp/dfipy-0.1.6.tar.gz` & `tmp/dfipy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-0.1.6.tar", max compression
+gzip compressed data, was "dfipy-0.1.7.tar", max compression
```

## Comparing `dfipy-0.1.6.tar` & `dfipy-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      568 2023-06-14 14:08:25.746457 dfipy-0.1.6/LICENCE
--rw-r--r--   0        0        0     1753 2023-06-14 14:08:25.746457 dfipy-0.1.6/README.md
--rw-r--r--   0        0        0      194 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/__init__.py
--rw-r--r--   0        0        0    16347 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/analysis.py
--rw-r--r--   0        0        0     4631 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/connection.py
--rw-r--r--   0        0        0    26566 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/getters.py
--rw-r--r--   0        0        0    14461 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/show.py
--rw-r--r--   0        0        0     4845 2023-06-14 14:08:25.746457 dfipy-0.1.6/dfi/stream.py
--rw-r--r--   0        0        0     1970 2023-06-14 14:08:26.474473 dfipy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 dfipy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-06-15 14:41:39.080587 dfipy-0.1.7/LICENCE
+-rw-r--r--   0        0        0     1753 2023-06-15 14:41:39.080587 dfipy-0.1.7/README.md
+-rw-r--r--   0        0        0      194 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/__init__.py
+-rw-r--r--   0        0        0    16347 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/analysis.py
+-rw-r--r--   0        0        0     4631 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/connection.py
+-rw-r--r--   0        0        0    26566 2023-06-15 14:41:39.080587 dfipy-0.1.7/dfi/getters.py
+-rw-r--r--   0        0        0    14461 2023-06-15 14:41:39.084586 dfipy-0.1.7/dfi/show.py
+-rw-r--r--   0        0        0     4839 2023-06-15 14:41:39.084586 dfipy-0.1.7/dfi/stream.py
+-rw-r--r--   0        0        0     1970 2023-06-15 14:41:40.048603 dfipy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 dfipy-0.1.7/PKG-INFO
```

### Comparing `dfipy-0.1.6/LICENCE` & `dfipy-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/README.md` & `dfipy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/dfi/analysis.py` & `dfipy-0.1.7/dfi/analysis.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/dfi/connection.py` & `dfipy-0.1.7/dfi/connection.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/dfi/getters.py` & `dfipy-0.1.7/dfi/getters.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/dfi/show.py` & `dfipy-0.1.7/dfi/show.py`

 * *Files identical despite different names*

### Comparing `dfipy-0.1.6/dfi/stream.py` & `dfipy-0.1.7/dfi/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Auxiliary methods for streamed data.
 """
 
 import json
 import logging
+import warnings
 from time import sleep
 from typing import List
 
 import requests
 import sseclient  # pylint: disable=import-error
 from tqdm import tqdm
 
@@ -34,17 +35,17 @@
     msg = f"Unexpected event in bagging area: {event}"
     logger.error(msg)
     raise DFIResponseError(msg)
 
 
 def raise_message_event_not_reached() -> None:
     """helper to raise a warning if the "message" event was not reached."""
-    msg = "No response from DFI API for the given query"
+    msg = "DFI provided no 'message' events."
     logger.warning(msg)
-    raise DFIResponseWarning(msg)
+    warnings.warn(msg)
 
 
 def receive_entities(response: requests.models.Response, progress_bar: bool = False) -> List[any]:
     """
     Helper function to parse clients events as entities and optionally show the progress bar.
     """
     client = sseclient.SSEClient(response)
```

### Comparing `dfipy-0.1.6/pyproject.toml` & `dfipy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "0.1.6"
+version = "0.1.7"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@excession.co>",
   "Sebastiano Ferraris <sebastiano.ferraris@excession.co>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
```

### Comparing `dfipy-0.1.6/PKG-INFO` & `dfipy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 0.1.6
+Version: 0.1.7
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@excession.co
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

