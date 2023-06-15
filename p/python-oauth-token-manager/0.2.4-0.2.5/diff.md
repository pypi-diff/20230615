# Comparing `tmp/python-oauth-token-manager-0.2.4.tar.gz` & `tmp/python-oauth-token-manager-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.2.4.tar", last modified: Thu Jun 15 15:22:16 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.5.tar", last modified: Thu Jun 15 15:28:29 2023, max compression
```

## Comparing `python-oauth-token-manager-0.2.4.tar` & `python-oauth-token-manager-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:22:16.026661 python-oauth-token-manager-0.2.4/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.4/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:22:16.026661 python-oauth-token-manager-0.2.4/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.4/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:22:16.022661 python-oauth-token-manager-0.2.4/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      749 2023-05-18 18:01:29.000000 python-oauth-token-manager-0.2.4/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.4/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5774 2023-05-16 15:53:57.000000 python-oauth-token-manager-0.2.4/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.4/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.4/auth/credentials_helpers_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:22:16.026661 python-oauth-token-manager-0.2.4/auth/datastore/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.4/auth/datastore/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5922 2023-06-15 15:21:02.000000 python-oauth-token-manager-0.2.4/auth/datastore/cloud_storage.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.4/auth/datastore/cloud_storage_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4687 2023-05-18 14:47:50.000000 python-oauth-token-manager-0.2.4/auth/datastore/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5048 2023-05-18 14:51:31.000000 python-oauth-token-manager-0.2.4/auth/datastore/local_file.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.4/auth/datastore/local_file_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5986 2023-05-18 14:49:59.000000 python-oauth-token-manager-0.2.4/auth/datastore/secret_manager.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.4/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.4/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.4/auth/exceptions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-15 15:18:55.000000 python-oauth-token-manager-0.2.4/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:22:16.026661 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:22:16.000000 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-15 15:22:16.000000 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-15 15:22:16.000000 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-15 15:22:16.000000 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-15 15:22:16.000000 python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-15 15:22:16.026661 python-oauth-token-manager-0.2.4/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.5/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.5/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.233966 python-oauth-token-manager-0.2.5/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.2.5/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.5/auth/abstract_datastore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5760 2023-06-15 15:27:55.000000 python-oauth-token-manager-0.2.5/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.5/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.5/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.5/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.2.5/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.2.5/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.5/auth/datastore/local_file_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6001 2023-06-15 15:27:21.000000 python-oauth-token-manager-0.2.5/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.5/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.5/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.5/auth/exceptions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-15 15:28:16.000000 python-oauth-token-manager-0.2.5/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/setup.cfg
```

### Comparing `python-oauth-token-manager-0.2.4/LICENSE` & `python-oauth-token-manager-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/PKG-INFO` & `python-oauth-token-manager-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.4
+Version: 0.2.5
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.4/README.md` & `python-oauth-token-manager-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.5/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/credentials.py` & `python-oauth-token-manager-0.2.5/auth/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Any, Dict, Type, TypeVar
 
 import pytz
 from dateutil.relativedelta import relativedelta
 from google.auth.transport import requests
 from google.oauth2 import credentials as oauth
 
-from auth import decorators
-from auth.credentials_helpers import encode_key
+import decorators
+from .credentials_helpers import encode_key
 
 from .abstract_datastore import AbstractDatastore
 from .exceptions import CredentialsError
 
 
 @dataclass
 class ProjectCredentials(object):
```

### Comparing `python-oauth-token-manager-0.2.4/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.5/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.5/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/__init__.py` & `python-oauth-token-manager-0.2.5/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/cloud_storage.py` & `python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import json
 from typing import Any, Callable, Dict, List, Mapping, Optional
 
-import decorators
 import gcsfs
-from abstract_datastore import AbstractDatastore
+from auth import decorators
+from auth.abstract_datastore import AbstractDatastore
 
 
 def persist(f: Callable) -> Any:
   """Persists the datastore after internal manipulations.
 
   This is used to decorate functions that modify the internal json object
   containing the authentication credentials and ensures that any changes
```

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/cloud_storage_test.py` & `python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/firestore.py` & `python-oauth-token-manager-0.2.5/auth/datastore/firestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
-import decorators
-from abstract_datastore import AbstractDatastore
+from auth import decorators
+from auth.abstract_datastore import AbstractDatastore
 
 from google.cloud import firestore
 
 
 class Firestore(AbstractDatastore):
   @decorators.lazy_property
   def client(self) -> Any:
```

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/local_file.py` & `python-oauth-token-manager-0.2.5/auth/datastore/local_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import json
 from typing import Any, Callable, Dict, List, Mapping, Optional
 
-import decorators
-from abstract_datastore import AbstractDatastore
+from auth import decorators
+from auth.abstract_datastore import AbstractDatastore
 
 
 def persist(f: Callable) -> Any:
   def f_persist(*args: Mapping[str, Any], **kw: Mapping[str, Any]) -> Any:
     datastore = args[0]
     try:
       return f(*args, **kw)
```

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/local_file_test.py` & `python-oauth-token-manager-0.2.5/auth/datastore/local_file_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/datastore/secret_manager.py` & `python-oauth-token-manager-0.2.5/auth/datastore/secret_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import json
 from typing import Any, List, Mapping, Optional, Type
 
 from google.cloud import secretmanager, secretmanager_v1
 from google.cloud.secretmanager_v1.types import resources
 from google.cloud.secretmanager_v1.services.secret_manager_service import pagers
 
-import decorators
-from abstract_datastore import AbstractDatastore
+from auth import decorators
+from auth.abstract_datastore import AbstractDatastore
 
 
 class SecretManager(AbstractDatastore):
 
   def __init__(self, email: str = None,
                project: str = None) -> AbstractDatastore:
     self._project = project
```

### Comparing `python-oauth-token-manager-0.2.4/auth/decorators.py` & `python-oauth-token-manager-0.2.5/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/decorators_test.py` & `python-oauth-token-manager-0.2.5/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/auth/exceptions.py` & `python-oauth-token-manager-0.2.5/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.4/pyproject.toml` & `python-oauth-token-manager-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-oauth-token-manager"
-version = "0.2.4"
+version = "0.2.5"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "API for managing stored OAuth credentials."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
```

### Comparing `python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/PKG-INFO` & `python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.4
+Version: 0.2.5
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.4/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

