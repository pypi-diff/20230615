# Comparing `tmp/another_sd_client-1.1.0.tar.gz` & `tmp/another_sd_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.1.0.tar", max compression
+gzip compressed data, was "another_sd_client-1.2.0.tar", max compression
```

## Comparing `another_sd_client-1.1.0.tar` & `another_sd_client-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6296 2023-06-06 11:49:40.431897 another_sd_client-1.1.0/README.md
--rw-r--r--   0        0        0      898 2023-06-06 11:49:41.524998 another_sd_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 11:49:40.478902 another_sd_client-1.1.0/sdclient/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-06 11:49:40.432898 another_sd_client-1.1.0/sdclient/client.py
--rw-r--r--   0        0        0     4905 2023-06-06 11:49:40.433898 another_sd_client-1.1.0/sdclient/requests.py
--rw-r--r--   0        0        0     2697 2023-06-06 11:49:40.433898 another_sd_client-1.1.0/sdclient/responses.py
--rw-r--r--   0        0        0     7229 1970-01-01 00:00:00.000000 another_sd_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-06-15 10:51:25.213720 another_sd_client-1.2.0/README.md
+-rw-r--r--   0        0        0      937 2023-06-15 10:51:26.445838 another_sd_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 10:51:25.261725 another_sd_client-1.2.0/sdclient/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-15 10:51:25.214720 another_sd_client-1.2.0/sdclient/client.py
+-rw-r--r--   0        0        0     4905 2023-06-15 10:51:25.214720 another_sd_client-1.2.0/sdclient/requests.py
+-rw-r--r--   0        0        0     2697 2023-06-15 10:51:25.214720 another_sd_client-1.2.0/sdclient/responses.py
+-rw-r--r--   0        0        0     7049 1970-01-01 00:00:00.000000 another_sd_client-1.2.0/PKG-INFO
```

### Comparing `another_sd_client-1.1.0/README.md` & `another_sd_client-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.1.0/pyproject.toml` & `another_sd_client-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 
 [tool.poetry]
 name = "another-sd-client"
-version = "1.1.0"
+version = "1.2.0"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 structlog = "^22.3.0"
 pydantic = "^1.10.4"
 more-itertools = "^9.0.0"
-pre-commit = "^3.0.0"
-pytest-cov = "^4.0.0"
 click = "^8.1.3"
-pytest-asyncio = "^0.21.0"
-pytest-split = "^0.8.1"
 httpx = "^0.24.0"
-xmltodict = "^0.13.0"
+xmltodict = "^0.12.0"
 lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 
+[tool.poetry.group.test.dependencies]
+pre-commit = "^3.0.0"
+pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.0"
+pytest-split = "^0.8.1"
+
 [tool.pytest.ini_options]
 asyncio_mode="auto"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `another_sd_client-1.1.0/sdclient/client.py` & `another_sd_client-1.2.0/sdclient/client.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.1.0/sdclient/requests.py` & `another_sd_client-1.2.0/sdclient/requests.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.1.0/sdclient/responses.py` & `another_sd_client-1.2.0/sdclient/responses.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.1.0/PKG-INFO` & `another_sd_client-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
-Requires-Dist: pre-commit (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
-Requires-Dist: pytest-split (>=0.8.1,<0.9.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
-Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/another-sd-client
 Description-Content-Type: text/markdown
 
 # Another SD Client
 
 SD client library for communicating with SD Løn
```

