# Comparing `tmp/sync-pack-sdk-7.3.8.tar.gz` & `tmp/sync-pack-sdk-7.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync-pack-sdk-7.3.8.tar", last modified: Mon Jun 12 08:20:36 2023, max compression
+gzip compressed data, was "sync-pack-sdk-7.7.7.tar", last modified: Tue Jun 13 10:29:18 2023, max compression
```

## Comparing `sync-pack-sdk-7.3.8.tar` & `sync-pack-sdk-7.7.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.799030 sync-pack-sdk-7.3.8/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 08:20:36.799030 sync-pack-sdk-7.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3120 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/README.md
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-12 08:20:36.800030 sync-pack-sdk-7.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.775029 sync-pack-sdk-7.3.8/swaggerpetstore/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4322 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.779029 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12585 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    10595 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.780029 sync-pack-sdk-7.3.8/swaggerpetstore/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.783029 sync-pack-sdk-7.3.8/swaggerpetstore/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.784029 sync-pack-sdk-7.3.8/swaggerpetstore/http/auth/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/auth/custom_authentication.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.792030 sync-pack-sdk-7.3.8/swaggerpetstore/models/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/category.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/order.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/pet.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/status_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/swaggerpetstore_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.793030 sync-pack-sdk-7.3.8/swaggerpetstore/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-12 08:20:06.000000 sync-pack-sdk-7.3.8/swaggerpetstore/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:20:36.799030 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 08:20:36.000000 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1389 2023-06-12 08:20:36.000000 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:20:36.000000 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-12 08:20:36.000000 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 08:20:36.000000 sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.342529 sync-pack-sdk-7.7.7/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-13 10:29:18.342529 sync-pack-sdk-7.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-13 10:29:18.343529 sync-pack-sdk-7.7.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.316528 sync-pack-sdk-7.7.7/swaggerpetstore/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.320529 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.321529 sync-pack-sdk-7.7.7/swaggerpetstore/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.325529 sync-pack-sdk-7.7.7/swaggerpetstore/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.327529 sync-pack-sdk-7.7.7/swaggerpetstore/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/auth/custom_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.335529 sync-pack-sdk-7.7.7/swaggerpetstore/models/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/status_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/swaggerpetstore_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.335529 sync-pack-sdk-7.7.7/swaggerpetstore/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-13 10:28:49.000000 sync-pack-sdk-7.7.7/swaggerpetstore/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:29:18.342529 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-13 10:29:18.000000 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-06-13 10:29:18.000000 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:29:18.000000 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-13 10:29:18.000000 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-13 10:29:18.000000 sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/top_level.txt
```

### Comparing `sync-pack-sdk-7.3.8/LICENSE` & `sync-pack-sdk-7.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/PKG-INFO` & `sync-pack-sdk-7.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-pack-sdk
-Version: 7.3.8
+Version: 7.7.7
 Summary: this is a testing description
 Author-email: subtain <subtain@gmail.com>
 Project-URL: Documentation, https://whats.com
 Keywords: this,testing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install sync-pack-sdk==7.3.8
+pip install sync-pack-sdk==7.7.7
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/sync-pack-sdk/7.3.8
+https://pypi.python.org/pypi/sync-pack-sdk/7.7.7
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -63,17 +63,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/store.md)
-* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-request.md)
```

### Comparing `sync-pack-sdk-7.3.8/README.md` & `sync-pack-sdk-7.7.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install sync-pack-sdk==7.3.8
+pip install sync-pack-sdk==7.7.7
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/sync-pack-sdk/7.3.8
+https://pypi.python.org/pypi/sync-pack-sdk/7.7.7
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -51,17 +51,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/store.md)
-* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-request.md)
```

### Comparing `sync-pack-sdk-7.3.8/pyproject.toml` & `sync-pack-sdk-7.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "sync-pack-sdk"
 description = "this is a testing description"
-version = "7.3.8"
+version = "7.7.7"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["this", "testing"]
 authors = [{name = "subtain", email = "subtain@gmail.com"}]
 urls = {Documentation = "https://whats.com"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10", "deprecation~=2.1"]
 classifiers = []
```

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/api_helper.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/api_helper.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/configuration.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/configuration.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/controllers/base_controller.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/controllers/pet_controller.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/controllers/pet_controller.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/controllers/store_controller.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/controllers/user_controller.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/exceptions/api_exception.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/http/auth/custom_authentication.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/http/auth/custom_authentication.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/http/http_request.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/http/http_response.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/api_response.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/api_response.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/category.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/category.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/order.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/order.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/pet.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/pet.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/status_2_enum.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/tag.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/tag.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/models/user.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/models/user.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/swaggerpetstore/swaggerpetstore_client.py` & `sync-pack-sdk-7.7.7/swaggerpetstore/swaggerpetstore_client.py`

 * *Files identical despite different names*

### Comparing `sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/PKG-INFO` & `sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-pack-sdk
-Version: 7.3.8
+Version: 7.7.7
 Summary: this is a testing description
 Author-email: subtain <subtain@gmail.com>
 Project-URL: Documentation, https://whats.com
 Keywords: this,testing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install sync-pack-sdk==7.3.8
+pip install sync-pack-sdk==7.7.7
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/sync-pack-sdk/7.3.8
+https://pypi.python.org/pypi/sync-pack-sdk/7.7.7
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -63,17 +63,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/store.md)
-* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.3.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/7.7.7/doc/http-request.md)
```

### Comparing `sync-pack-sdk-7.3.8/sync_pack_sdk.egg-info/SOURCES.txt` & `sync-pack-sdk-7.7.7/sync_pack_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

