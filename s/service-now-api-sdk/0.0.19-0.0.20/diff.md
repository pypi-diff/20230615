# Comparing `tmp/service_now_api_sdk-0.0.19.tar.gz` & `tmp/service_now_api_sdk-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_now_api_sdk-0.0.19.tar", max compression
+gzip compressed data, was "service_now_api_sdk-0.0.20.tar", max compression
```

## Comparing `service_now_api_sdk-0.0.19.tar` & `service_now_api_sdk-0.0.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/LICENSE
--rw-r--r--   0        0        0     6564 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/README.md
--rw-r--r--   0        0        0      565 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/__init__.py
--rw-r--r--   0        0        0       43 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/exceptions.py
--rw-r--r--   0        0        0      140 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/client.py
--rw-r--r--   0        0        0      227 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
--rw-r--r--   0        0        0     2874 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/client.py
--rw-r--r--   0        0        0    10869 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
--rw-r--r--   0        0        0        0 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/__init__.py
--rw-r--r--   0        0        0    15486 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/client.py
--rw-r--r--   0        0        0      818 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/exceptions.py
--rw-r--r--   0        0        0      255 2023-04-19 17:55:15.602561 service_now_api_sdk-0.0.19/service_now_api_sdk/settings.py
--rw-r--r--   0        0        0     6906 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/LICENSE
+-rw-r--r--   0        0        0     6564 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/README.md
+-rw-r--r--   0        0        0      708 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/exceptions.py
+-rw-r--r--   0        0        0      140 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
+-rw-r--r--   0        0        0     7114 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/client.py
+-rw-r--r--   0        0        0      227 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/client.py
+-rw-r--r--   0        0        0    10869 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/__init__.py
+-rw-r--r--   0        0        0    15486 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/client.py
+-rw-r--r--   0        0        0      818 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/exceptions.py
+-rw-r--r--   0        0        0      255 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/settings.py
+-rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.20/PKG-INFO
```

### Comparing `service_now_api_sdk-0.0.19/LICENSE` & `service_now_api_sdk-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/README.md` & `service_now_api_sdk-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/pyproject.toml` & `service_now_api_sdk-0.0.20/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "service_now_api_sdk"
-version = "0.0.19"
+version = "0.0.20"
 description = "Service Now API SDK is used to facilitate integrations, automations and also code reuse"
-authors = [
-    "Guilherme Laercio da Silva <guilhermelaerciodasilva@gmail.com>",
-    "Stone People Analytic <systems-techpeople@stone.com.br>"
+authors = ["stone_people_analytics <systems-techpeople@stone.com.br>"]
+maintainers = [
+    "guilherme_lsilva <manager.guilherme.silva@gmail.com>",
+    "diogo56 <diogo.amorim2001@gmail.com>",
 ]
 readme = "README.md"
+license = "MIT"
+repository = "https://github.com/people-analytics-tech/ service-now-api-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.27.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.17.0"
```

### Comparing `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/attachments/client.py` & `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/client.py` & `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py` & `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/client.py` & `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/service_now_api_sdk/sdk/servicenow/table/exceptions.py` & `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.19/PKG-INFO` & `service_now_api_sdk-0.0.20/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: service-now-api-sdk
-Version: 0.0.19
+Version: 0.0.20
 Summary: Service Now API SDK is used to facilitate integrations, automations and also code reuse
-Author: Guilherme Laercio da Silva
-Author-email: guilhermelaerciodasilva@gmail.com
+Home-page: https://github.com/people-analytics-tech/ service-now-api-sdk
+License: MIT
+Author: stone_people_analytics
+Author-email: systems-techpeople@stone.com.br
+Maintainer: guilherme_lsilva
+Maintainer-email: manager.guilherme.silva@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Repository, https://github.com/people-analytics-tech/ service-now-api-sdk
 Description-Content-Type: text/markdown
 
 # ServiceNow API SDK
 [![PyPI Latest Release](https://img.shields.io/pypi/v/service-now-api-sdk.svg)](https://pypi.org/project/service-now-api-sdk/)
 
 Check out our [GitHub Repository](https://github.com/guilhermelaercio/service_now_api_sdk)!
```

