# Comparing `tmp/tencentcloud-sdk-python-yunjing-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-yunjing-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.913.tar", last modified: Tue Jun 13 02:29:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yunjing-3.0.914.tar", last modified: Wed Jun 14 00:39:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yunjing-3.0.913.tar` & `tencentcloud-sdk-python-yunjing-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3960 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240956 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)    93972 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/yunjing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:29:52.000000 tencentcloud-sdk-python-yunjing-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240956 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)    93972 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/yunjing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-14 00:39:25.000000 tencentcloud-sdk-python-yunjing-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:39:26.000000 tencentcloud-sdk-python-yunjing-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/README.rst` & `tencentcloud-sdk-python-yunjing-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.913'
+__version__ = '3.0.914'
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/errorcodes.py` & `tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/models.py` & `tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud/yunjing/v20180228/yunjing_client.py` & `tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud/yunjing/v20180228/yunjing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.914/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yunjing-3.0.914/tencentcloud_sdk_python_yunjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunjing
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Yunjing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunjing-3.0.913/setup.py` & `tencentcloud-sdk-python-yunjing-3.0.914/setup.py`

 * *Files identical despite different names*

