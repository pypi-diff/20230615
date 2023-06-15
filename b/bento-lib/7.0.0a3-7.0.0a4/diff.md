# Comparing `tmp/bento_lib-7.0.0a3.tar.gz` & `tmp/bento_lib-7.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.0.0a3.tar", last modified: Wed Jun 14 18:10:38 2023, max compression
+gzip compressed data, was "bento_lib-7.0.0a4.tar", last modified: Thu Jun 15 18:42:59 2023, max compression
```

## Comparing `bento_lib-7.0.0a3.tar` & `bento_lib-7.0.0a4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:10:38.466480 bento_lib-7.0.0a3/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 18:10:38.000000 bento_lib-7.0.0a3/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:10:38.470480 bento_lib-7.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 18:10:24.000000 bento_lib-7.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.059838 bento_lib-7.0.0a4/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:42:59.055838 bento_lib-7.0.0a4/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 18:42:59.000000 bento_lib-7.0.0a4/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:42:59.063838 bento_lib-7.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-15 18:42:48.000000 bento_lib-7.0.0a4/setup.py
```

### Comparing `bento_lib-7.0.0a3/LICENSE` & `bento_lib-7.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/PKG-INFO` & `bento_lib-7.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.0.0a3
+Version: 7.0.0a4
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a3/README.md` & `bento_lib-7.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/auth/middleware/base.py` & `bento_lib-7.0.0a4/bento_lib/auth/middleware/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import aiohttp
 import logging
 import requests
 
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Callable
 
 from ..exceptions import BentoAuthException
 
 __all__ = ["BaseAuthMiddleware"]
 
 
 class BaseAuthMiddleware(ABC):
@@ -44,42 +44,64 @@
         if require_token:
             if token is None:
                 raise BentoAuthException("No token provided")
 
     def mk_authz_url(self, path: str) -> str:
         return f"{self._bento_authz_service_url.rstrip('/')}{path}"
 
-    def _extract_token_and_build_headers(self, request: Any, require_token: bool) -> dict:
+    def _extract_token_and_build_headers(
+        self,
+        request: Any,
+        require_token: bool,
+        headers_getter: Callable[[Any], dict[str, str]] | None = None,
+    ) -> dict[str, str]:
+        if headers_getter:
+            return headers_getter(request)
+
         tkn_header = self.get_authz_header_value(request)
         self.check_require_token(require_token, tkn_header)
         return {"Authorization": tkn_header} if tkn_header else {}
 
     def _gen_exc_non_200_error_from_authz(self, code: int, content: bytes):
         self._logger.error(f"Got non-200 response from authorization service: {code} {content}")
         # Generic error - don't leak errors from authz service!
         raise BentoAuthException("Error from authz service", status_code=500)
 
-    def authz_post(self, request: Any, path: str, body: dict, require_token: bool = False) -> dict:
+    def authz_post(
+        self,
+        request: Any,
+        path: str,
+        body: dict,
+        require_token: bool = False,
+        headers_getter: Callable[[Any], dict[str, str]] | None = None,
+    ) -> dict:
         res = requests.post(
             self.mk_authz_url(path),
             json=body,
-            headers=self._extract_token_and_build_headers(request, require_token),
+            headers=self._extract_token_and_build_headers(request, require_token, headers_getter),
             verify=self._verify_ssl)
 
         if res.status_code != 200:  # Invalid authorization service response
             raise self._gen_exc_non_200_error_from_authz(res.status_code, res.content)
 
         return res.json()
 
-    async def async_authz_post(self, request: Any, path: str, body: dict, require_token: bool = False) -> dict:
+    async def async_authz_post(
+        self,
+        request: Any,
+        path: str,
+        body: dict,
+        require_token: bool = False,
+        headers_getter: Callable[[Any], dict[str, str]] | None = None,
+    ) -> dict:
         async with aiohttp.ClientSession() as session:
             async with session.post(
                     self.mk_authz_url(path),
                     json=body,
-                    headers=self._extract_token_and_build_headers(request, require_token),
+                    headers=self._extract_token_and_build_headers(request, require_token, headers_getter),
                     ssl=(None if self._verify_ssl else False)) as res:
 
                 if res.status != 200:  # Invalid authorization service response
                     raise self._gen_exc_non_200_error_from_authz(res.status, await res.content.read())
 
                 return await res.json()
 
@@ -91,23 +113,25 @@
     def check_authz_evaluate(
         self,
         request: Any,
         permissions: frozenset[str],
         resource: dict,
         require_token: bool = True,
         set_authz_flag: bool = False,
+        headers_getter: Callable[[Any], dict[str, str]] | None = None,
     ):
         if not self.enabled:
             return
 
         res = self.authz_post(
             request,
             "/policy/evaluate",
             body={"requested_resource": resource, "required_permissions": list(permissions)},
             require_token=require_token,
+            headers_getter=headers_getter,
         )
 
         if not res.get("result"):
             # We early-return with the flag set - we're returning Forbidden,
             # and we've determined authz, so we can just set the flag.
             raise BentoAuthException("Forbidden", status_code=403)  # Actually forbidden by authz service
 
@@ -117,23 +141,25 @@
     async def async_check_authz_evaluate(
         self,
         request: Any,
         permissions: frozenset[str],
         resource: dict,
         require_token: bool = True,
         set_authz_flag: bool = False,
+        headers_getter: Callable[[Any], dict[str, str]] | None = None,
     ):
         if not self.enabled:
             return
 
         res = await self.async_authz_post(
             request,
             "/policy/evaluate",
             body={"requested_resource": resource, "required_permissions": list(permissions)},
             require_token=require_token,
+            headers_getter=headers_getter,
         )
 
         if not res.get("result"):
             # We early-return with the flag set - we're returning Forbidden,
             # and we've determined authz, so we can just set the flag.
             raise BentoAuthException("Forbidden", status_code=403)  # Actually forbidden by authz service
```

### Comparing `bento_lib-7.0.0a3/bento_lib/auth/middleware/django.py` & `bento_lib-7.0.0a4/bento_lib/auth/middleware/django.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.0.0a4/bento_lib/auth/middleware/fastapi.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/auth/middleware/flask.py` & `bento_lib-7.0.0a4/bento_lib/auth/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/drs/utils.py` & `bento_lib-7.0.0a4/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/events/_event_bus.py` & `bento_lib-7.0.0a4/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/events/notifications.py` & `bento_lib-7.0.0a4/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/events/types.py` & `bento_lib-7.0.0a4/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/responses/errors.py` & `bento_lib-7.0.0a4/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.0.0a4/bento_lib/responses/fastapi_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/responses/flask_errors.py` & `bento_lib-7.0.0a4/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.0.0a4/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.0.0a4/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.0.0a4/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/search/data_structure.py` & `bento_lib-7.0.0a4/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/search/operations.py` & `bento_lib-7.0.0a4/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/search/postgres.py` & `bento_lib-7.0.0a4/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/search/queries.py` & `bento_lib-7.0.0a4/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/types.py` & `bento_lib-7.0.0a4/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib/workflows.py` & `bento_lib-7.0.0a4/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.0.0a4/bento_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 7.0.0a3
+Version: 7.0.0a4
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.0.0a3/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.0.0a4/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.0.0a3/setup.py` & `bento_lib-7.0.0a4/setup.py`

 * *Files identical despite different names*

