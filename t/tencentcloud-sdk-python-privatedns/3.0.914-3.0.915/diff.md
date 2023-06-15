# Comparing `tmp/tencentcloud-sdk-python-privatedns-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-privatedns-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.914.tar", last modified: Wed Jun 14 00:31:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.915.tar", last modified: Thu Jun 15 00:31:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-privatedns-3.0.914.tar` & `tencentcloud-sdk-python-privatedns-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/
--rw-r--r--   0 root         (0) root         (0)     7535 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59039 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)    21077 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/privatedns_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/
+-rw-r--r--   0 root         (0) root         (0)     7535 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59039 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)    21077 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/privatedns_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:31:08.000000 tencentcloud-sdk-python-privatedns-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/README.rst` & `tencentcloud-sdk-python-privatedns-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/errorcodes.py` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/models.py` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/privatedns_client.py` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/privatedns/v20201028/privatedns_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.914'
+__version__ = '3.0.915'
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.915/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.915/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.914/setup.py` & `tencentcloud-sdk-python-privatedns-3.0.915/setup.py`

 * *Files identical despite different names*

