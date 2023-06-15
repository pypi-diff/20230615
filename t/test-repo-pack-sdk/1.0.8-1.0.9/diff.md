# Comparing `tmp/test-repo-pack-sdk-1.0.8.tar.gz` & `tmp/test-repo-pack-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-repo-pack-sdk-1.0.8.tar", last modified: Thu Jun 15 13:48:56 2023, max compression
+gzip compressed data, was "test-repo-pack-sdk-1.0.9.tar", last modified: Thu Jun 15 13:52:35 2023, max compression
```

## Comparing `test-repo-pack-sdk-1.0.8.tar` & `test-repo-pack-sdk-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.558477 test-repo-pack-sdk-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5472 2023-06-15 13:48:56.559477 test-repo-pack-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5281 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      625 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-15 13:48:56.560478 test-repo-pack-sdk-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.524475 test-repo-pack-sdk-1.0.8/swaggerpetstore/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.529476 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    10595 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.534476 test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/o_auth_provider_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.538476 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.553477 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/category.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/o_auth_provider_error_enum.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/o_auth_scope_enum.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/o_auth_token.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/order.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/pet.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/status_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/swaggerpetstore_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.555477 test-repo-pack-sdk-1.0.8/swaggerpetstore/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-15 13:48:30.000000 test-repo-pack-sdk-1.0.8/swaggerpetstore/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:48:56.558477 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5472 2023-06-15 13:48:56.000000 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-15 13:48:56.000000 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:48:56.000000 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-15 13:48:56.000000 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 13:48:56.000000 test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.530882 test-repo-pack-sdk-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-06-15 13:52:35.530882 test-repo-pack-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      625 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-15 13:52:35.532882 test-repo-pack-sdk-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.494882 test-repo-pack-sdk-1.0.9/swaggerpetstore/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.498882 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.501882 test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/o_auth_provider_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.509882 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.520882 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/o_auth_provider_error_enum.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/o_auth_scope_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/o_auth_token.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/status_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/swaggerpetstore_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.521882 test-repo-pack-sdk-1.0.9/swaggerpetstore/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-15 13:52:05.000000 test-repo-pack-sdk-1.0.9/swaggerpetstore/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:52:35.530882 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-06-15 13:52:35.000000 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-15 13:52:35.000000 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:52:35.000000 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-15 13:52:35.000000 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 13:52:35.000000 test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/top_level.txt
```

### Comparing `test-repo-pack-sdk-1.0.8/LICENSE` & `test-repo-pack-sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/PKG-INFO` & `test-repo-pack-sdk-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-repo-pack-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: this is testing
 Author-email: subtain <subtain@gmail.com>
 Project-URL: Documentation, https://tester.io
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
 License-File: LICENSE
@@ -20,23 +20,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install test-repo-pack-sdk==1.0.8
+pip install test-repo-pack-sdk==1.0.9
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/test-repo-pack-sdk/1.0.8
+https://pypi.python.org/pypi/test-repo-pack-sdk/1.0.9
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -102,17 +102,17 @@
 | Scope Name | Description |
 |  --- | --- |
 | `READPETS` | read your pets |
 | `WRITEPETS` | modify pets in your account |
 
 ## List of APIs
 
-* [Pet](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/store.md)
-* [User](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/http-request.md)
```

### Comparing `test-repo-pack-sdk-1.0.8/README.md` & `test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,118 @@
-
-# Getting Started with Swagger Petstore
-
-## Introduction
-
-This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.
-
-Find out more about Swagger: [http://swagger.io](http://swagger.io)
-
-## Install the Package
-
+Metadata-Version: 2.1
+Name: test-repo-pack-sdk
+Version: 1.0.9
+Summary: this is testing
+Author-email: subtain <subtain@gmail.com>
+Project-URL: Documentation, https://tester.io
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testutils
+License-File: LICENSE
+
+
+# Getting Started with Swagger Petstore
+
+## Introduction
+
+This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.
+
+Find out more about Swagger: [http://swagger.io](http://swagger.io)
+
+## Install the Package
+
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
-Install the package from PyPi using the following pip command:
-
-```python
-pip install test-repo-pack-sdk==1.0.8
-```
-
+Install the package from PyPi using the following pip command:
+
+```python
+pip install test-repo-pack-sdk==1.0.9
+```
+
 You can also view the package at:
-https://pypi.python.org/pypi/test-repo-pack-sdk/1.0.8
-
-## Initialize the API Client
-
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/client.md)
-
-The following parameters are configurable for the API Client:
-
-| Parameter | Type | Description |
-|  --- | --- | --- |
-| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
-| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
-| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
-| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
-| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
-| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
-| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
-| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
-| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `o_auth_client_id` | `string` | OAuth 2 Client ID |
-| `o_auth_redirect_uri` | `string` | OAuth 2 Redirection endpoint or Callback Uri |
-| `o_auth_token` | `OAuthToken` | Object for storing information about the OAuth token |
-| `o_auth_scopes` | `OAuthScopeEnum` |  |
-
-The API client can be initialized as follows:
-
-```python
-from swaggerpetstore.swaggerpetstore_client import SwaggerpetstoreClient
+https://pypi.python.org/pypi/test-repo-pack-sdk/1.0.9
+
+## Initialize the API Client
+
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/client.md)
+
+The following parameters are configurable for the API Client:
+
+| Parameter | Type | Description |
+|  --- | --- | --- |
+| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
+| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
+| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
+| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
+| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
+| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
+| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
+| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
+| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
+| `o_auth_client_id` | `string` | OAuth 2 Client ID |
+| `o_auth_redirect_uri` | `string` | OAuth 2 Redirection endpoint or Callback Uri |
+| `o_auth_token` | `OAuthToken` | Object for storing information about the OAuth token |
+| `o_auth_scopes` | `OAuthScopeEnum` |  |
+
+The API client can be initialized as follows:
+
+```python
+from swaggerpetstore.swaggerpetstore_client import SwaggerpetstoreClient
 from swaggerpetstore.configuration import Environment
-
+
 client = SwaggerpetstoreClient(
     o_auth_client_id='OAuthClientId',
     o_auth_redirect_uri='OAuthRedirectUri',
     o_auth_scopes=[OAuthScopeEnum.READPETS, OAuthScopeEnum.WRITEPETS]
-)
-```
-
-## Authorization
-
-This API uses `OAuth 2 Implicit Grant`.
-
-## Implicit Grant
-
-Your application must obtain user authorization before it can execute an endpoint call incase this SDK chooses to use *OAuth 2.0 Implicit Grant* to obtain a user's consent to perform an API request on user's behalf. This authorization includes the following steps
-
-This process requires the presence of a client-side JavaScript code on the redirect URI page to receive the *access token* after the consent step is completed.
-
-### 1\. Obtain user consent
-
-To obtain user's consent, you must redirect the user to the authorization page. The `get_authorization_url()` method creates the URL to the authorization page. You must have initialized the client with scopes for which you need permission to access.
-
-```python
-auth_url = client.auth_managers['global'].get_authorization_url()
-```
-
-### 2\. Handle the OAuth server response
-
-Once the user responds to the consent request, the OAuth 2.0 server responds to your application's access request by redirecting the user to the redirect URI specified set in `Configuration`.
-
-The redirect URI will receive the *access token* as the `token` argument in the URL fragment.
-
-```
-https://example.com/oauth/callback#token=XXXXXXXXXXXXXXXXXXXXXXXXX
-```
-
-The access token must be extracted by the client-side JavaScript code. The access token can be used to authorize any further endpoint calls by the JavaScript code.
-
-### Scopes
-
-Scopes enable your application to only request access to the resources it needs while enabling users to control the amount of access they grant to your application. Available scopes are defined in the `OAuthScopeEnum` enumeration.
-
-| Scope Name | Description |
-|  --- | --- |
-| `READPETS` | read your pets |
-| `WRITEPETS` | modify pets in your account |
-
-## List of APIs
-
-* [Pet](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/store.md)
-* [User](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/controllers/user.md)
-
-## Classes Documentation
-
-* [Utility Classes](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/sdks-io/test-repo-pack-python-sdk/tree/1.0.8/doc/http-request.md)
-
+)
+```
+
+## Authorization
+
+This API uses `OAuth 2 Implicit Grant`.
+
+## Implicit Grant
+
+Your application must obtain user authorization before it can execute an endpoint call incase this SDK chooses to use *OAuth 2.0 Implicit Grant* to obtain a user's consent to perform an API request on user's behalf. This authorization includes the following steps
+
+This process requires the presence of a client-side JavaScript code on the redirect URI page to receive the *access token* after the consent step is completed.
+
+### 1\. Obtain user consent
+
+To obtain user's consent, you must redirect the user to the authorization page. The `get_authorization_url()` method creates the URL to the authorization page. You must have initialized the client with scopes for which you need permission to access.
+
+```python
+auth_url = client.auth_managers['global'].get_authorization_url()
+```
+
+### 2\. Handle the OAuth server response
+
+Once the user responds to the consent request, the OAuth 2.0 server responds to your application's access request by redirecting the user to the redirect URI specified set in `Configuration`.
+
+The redirect URI will receive the *access token* as the `token` argument in the URL fragment.
+
+```
+https://example.com/oauth/callback#token=XXXXXXXXXXXXXXXXXXXXXXXXX
+```
+
+The access token must be extracted by the client-side JavaScript code. The access token can be used to authorize any further endpoint calls by the JavaScript code.
+
+### Scopes
+
+Scopes enable your application to only request access to the resources it needs while enabling users to control the amount of access they grant to your application. Available scopes are defined in the `OAuthScopeEnum` enumeration.
+
+| Scope Name | Description |
+|  --- | --- |
+| `READPETS` | read your pets |
+| `WRITEPETS` | modify pets in your account |
+
+## List of APIs
+
+* [Pet](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/controllers/user.md)
+
+## Classes Documentation
+
+* [Utility Classes](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/New repo-two/tree/1.0.9/doc/http-request.md)
+
```

### Comparing `test-repo-pack-sdk-1.0.8/pyproject.toml` & `test-repo-pack-sdk-1.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "test-repo-pack-sdk"
 description = "this is testing"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "subtain", email = "subtain@gmail.com"}]
 urls = {Documentation = "https://tester.io"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10", "deprecation~=2.1"]
 classifiers = []
```

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/api_helper.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/api_helper.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/configuration.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/configuration.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/base_controller.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/pet_controller.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/pet_controller.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/store_controller.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/controllers/user_controller.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/api_exception.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/exceptions/o_auth_provider_exception.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/exceptions/o_auth_provider_exception.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_request.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/http/http_response.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/api_response.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/api_response.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/category.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/category.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/o_auth_provider_error_enum.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/o_auth_provider_error_enum.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/o_auth_token.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/o_auth_token.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/order.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/order.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/pet.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/pet.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/status_2_enum.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/tag.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/tag.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/models/user.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/models/user.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/swaggerpetstore/swaggerpetstore_client.py` & `test-repo-pack-sdk-1.0.9/swaggerpetstore/swaggerpetstore_client.py`

 * *Files identical despite different names*

### Comparing `test-repo-pack-sdk-1.0.8/test_repo_pack_sdk.egg-info/SOURCES.txt` & `test-repo-pack-sdk-1.0.9/test_repo_pack_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

