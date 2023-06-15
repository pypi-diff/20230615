# Comparing `tmp/repo-test-sdk-1.0.0.tar.gz` & `tmp/repo-test-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-test-sdk-1.0.0.tar", last modified: Thu Jun 15 11:04:39 2023, max compression
+gzip compressed data, was "repo-test-sdk-2.0.0.tar", last modified: Thu Jun 15 11:13:22 2023, max compression
```

## Comparing `repo-test-sdk-1.0.0.tar` & `repo-test-sdk-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:39.007023 repo-test-sdk-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-15 11:04:39.007023 repo-test-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3092 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.975023 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3367 2023-06-15 11:04:38.000000 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1389 2023-06-15 11:04:38.000000 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:04:38.000000 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-15 11:04:38.000000 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 11:04:38.000000 repo-test-sdk-1.0.0/repo_test_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-15 11:04:39.008023 repo-test-sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.980023 repo-test-sdk-1.0.0/swaggerpetstore/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4322 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.987023 repo-test-sdk-1.0.0/swaggerpetstore/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12585 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    10595 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.989023 repo-test-sdk-1.0.0/swaggerpetstore/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.990023 repo-test-sdk-1.0.0/swaggerpetstore/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:38.991023 repo-test-sdk-1.0.0/swaggerpetstore/http/auth/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/auth/custom_authentication.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:39.004023 repo-test-sdk-1.0.0/swaggerpetstore/models/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/category.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/order.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/pet.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/status_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/swaggerpetstore_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:04:39.007023 repo-test-sdk-1.0.0/swaggerpetstore/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-15 11:04:03.000000 repo-test-sdk-1.0.0/swaggerpetstore/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.935971 repo-test-sdk-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-06-15 11:13:22.935971 repo-test-sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3092 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.910971 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-06-15 11:13:22.000000 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-06-15 11:13:22.000000 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:13:22.000000 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-15 11:13:22.000000 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 11:13:22.000000 repo-test-sdk-2.0.0/repo_test_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-15 11:13:22.937970 repo-test-sdk-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.913971 repo-test-sdk-2.0.0/swaggerpetstore/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.916971 repo-test-sdk-2.0.0/swaggerpetstore/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.917971 repo-test-sdk-2.0.0/swaggerpetstore/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.924970 repo-test-sdk-2.0.0/swaggerpetstore/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.925971 repo-test-sdk-2.0.0/swaggerpetstore/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/auth/custom_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.930971 repo-test-sdk-2.0.0/swaggerpetstore/models/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/status_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/swaggerpetstore_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:13:22.933971 repo-test-sdk-2.0.0/swaggerpetstore/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-15 11:12:53.000000 repo-test-sdk-2.0.0/swaggerpetstore/utilities/file_wrapper.py
```

### Comparing `repo-test-sdk-1.0.0/LICENSE` & `repo-test-sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/PKG-INFO` & `repo-test-sdk-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-test-sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: this porfile is made to test New repositories 
 Author-email: SUbtain <Subtain@gmail.com>
 Project-URL: Documentation, https://tester.com
 Keywords: git,repo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install repo-test-sdk==1.0.0
+pip install repo-test-sdk==2.0.0
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/repo-test-sdk/1.0.0
+https://pypi.python.org/pypi/repo-test-sdk/2.0.0
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -63,17 +63,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/pet.md)
-* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/store.md)
-* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/user.md)
+* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/pet.md)
+* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/store.md)
+* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-response.md)
-* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-request.md)
+* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-response.md)
+* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-request.md)
```

### Comparing `repo-test-sdk-1.0.0/README.md` & `repo-test-sdk-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install repo-test-sdk==1.0.0
+pip install repo-test-sdk==2.0.0
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/repo-test-sdk/1.0.0
+https://pypi.python.org/pypi/repo-test-sdk/2.0.0
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -51,17 +51,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/pet.md)
-* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/store.md)
-* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/user.md)
+* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/pet.md)
+* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/store.md)
+* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-response.md)
-* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-request.md)
+* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-response.md)
+* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-request.md)
```

### Comparing `repo-test-sdk-1.0.0/pyproject.toml` & `repo-test-sdk-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "repo-test-sdk"
 description = "this porfile is made to test New repositories "
-version = "1.0.0"
+version = "2.0.0"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["git", "repo"]
 authors = [{name = "SUbtain", email = "Subtain@gmail.com"}]
 urls = {Documentation = "https://tester.com"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10", "deprecation~=2.1"]
 classifiers = []
```

### Comparing `repo-test-sdk-1.0.0/repo_test_sdk.egg-info/PKG-INFO` & `repo-test-sdk-2.0.0/repo_test_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo-test-sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: this porfile is made to test New repositories 
 Author-email: SUbtain <Subtain@gmail.com>
 Project-URL: Documentation, https://tester.com
 Keywords: git,repo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install repo-test-sdk==1.0.0
+pip install repo-test-sdk==2.0.0
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/repo-test-sdk/1.0.0
+https://pypi.python.org/pypi/repo-test-sdk/2.0.0
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -63,17 +63,17 @@
 
 ## Authorization
 
 This API uses `Custom Authentication`.
 
 ## List of APIs
 
-* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/pet.md)
-* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/store.md)
-* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/controllers/user.md)
+* [Pet](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/pet.md)
+* [Store](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/store.md)
+* [User](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-response.md)
-* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/1.0.0/doc/http-request.md)
+* [Utility Classes](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-response.md)
+* [HttpRequest](https://www.github.com/apimatic/repo-test-python-sdk/tree/2.0.0/doc/http-request.md)
```

### Comparing `repo-test-sdk-1.0.0/repo_test_sdk.egg-info/SOURCES.txt` & `repo-test-sdk-2.0.0/repo_test_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/api_helper.py` & `repo-test-sdk-2.0.0/swaggerpetstore/api_helper.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/configuration.py` & `repo-test-sdk-2.0.0/swaggerpetstore/configuration.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/controllers/base_controller.py` & `repo-test-sdk-2.0.0/swaggerpetstore/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/controllers/pet_controller.py` & `repo-test-sdk-2.0.0/swaggerpetstore/controllers/pet_controller.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/controllers/store_controller.py` & `repo-test-sdk-2.0.0/swaggerpetstore/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/controllers/user_controller.py` & `repo-test-sdk-2.0.0/swaggerpetstore/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/exceptions/api_exception.py` & `repo-test-sdk-2.0.0/swaggerpetstore/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/http/auth/custom_authentication.py` & `repo-test-sdk-2.0.0/swaggerpetstore/http/auth/custom_authentication.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/http/http_request.py` & `repo-test-sdk-2.0.0/swaggerpetstore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/http/http_response.py` & `repo-test-sdk-2.0.0/swaggerpetstore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/api_response.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/api_response.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/category.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/category.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/order.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/order.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/pet.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/pet.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/status_2_enum.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/tag.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/tag.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/models/user.py` & `repo-test-sdk-2.0.0/swaggerpetstore/models/user.py`

 * *Files identical despite different names*

### Comparing `repo-test-sdk-1.0.0/swaggerpetstore/swaggerpetstore_client.py` & `repo-test-sdk-2.0.0/swaggerpetstore/swaggerpetstore_client.py`

 * *Files identical despite different names*

