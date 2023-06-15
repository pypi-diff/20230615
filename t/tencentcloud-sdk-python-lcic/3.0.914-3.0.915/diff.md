# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.914.tar", last modified: Wed Jun 14 00:29:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.915.tar", last modified: Thu Jun 15 00:28:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.914.tar` & `tencentcloud-sdk-python-lcic-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4414 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142076 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:29:13.000000 tencentcloud-sdk-python-lcic-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142130 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    48649 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:28:32.000000 tencentcloud-sdk-python-lcic-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/README.rst` & `tencentcloud-sdk-python-lcic-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -923,17 +923,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 房间名称。
         :type Name: str
-        :param StartTime: 预定的房间开始时间，unix时间戳。
+        :param StartTime: 预定的房间开始时间，unix时间戳（秒）。
         :type StartTime: int
-        :param EndTime: 预定的房间结束时间，unix时间戳。
+        :param EndTime: 预定的房间结束时间，unix时间戳（秒）。
         :type EndTime: int
         :param SdkAppId: 低代码互动课堂的SdkAppId。
         :type SdkAppId: int
         :param Resolution: 分辨率。可以有如下取值：
 1 标清
 2 高清
 3 全高清
@@ -2171,17 +2171,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 房间名称。
         :type Name: str
-        :param StartTime: 预定的房间开始时间，unix时间戳。
+        :param StartTime: 预定的房间开始时间，unix时间戳（秒）。
         :type StartTime: int
-        :param EndTime: 预定的房间结束时间，unix时间戳。
+        :param EndTime: 预定的房间结束时间，unix时间戳（秒）。
         :type EndTime: int
         :param TeacherId: 老师的UserId。
         :type TeacherId: str
         :param SdkAppId: 低代码互动课堂的SdkAppId。
         :type SdkAppId: int
         :param Resolution: 分辨率。可以有如下取值：
 1 标清
@@ -3569,17 +3569,17 @@
 
     def __init__(self):
         r"""
         :param RoomId: 房间ID。
         :type RoomId: int
         :param SdkAppId: 低代码互动课堂的SdkAppId
         :type SdkAppId: int
-        :param StartTime: 预定的房间开始时间，unix时间戳。直播开始后不允许修改。
+        :param StartTime: 预定的房间开始时间，unix时间戳（秒）。直播开始后不允许修改。
         :type StartTime: int
-        :param EndTime: 预定的房间结束时间，unix时间戳。直播开始后不允许修改。
+        :param EndTime: 预定的房间结束时间，unix时间戳（秒）。直播开始后不允许修改。
         :type EndTime: int
         :param TeacherId: 老师ID。直播开始后不允许修改。
         :type TeacherId: str
         :param Name: 房间名称。
         :type Name: str
         :param Resolution: 分辨率。可以有如下取值：
 1 标清
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.915/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.915/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.914/setup.py` & `tencentcloud-sdk-python-lcic-3.0.915/setup.py`

 * *Files identical despite different names*

