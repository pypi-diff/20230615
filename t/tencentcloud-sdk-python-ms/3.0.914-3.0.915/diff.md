# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.914.tar", last modified: Wed Jun 14 00:30:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.915.tar", last modified: Thu Jun 15 00:29:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.914.tar` & `tencentcloud-sdk-python-ms-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55731 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:30:43.000000 tencentcloud-sdk-python-ms-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55879 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:29:57.000000 tencentcloud-sdk-python-ms-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ms-3.0.914/README.rst` & `tencentcloud-sdk-python-ms-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/ms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
+# CAM签名/鉴权错误。
+AUTHFAILURE_INVALIDAUTHORIZATION = 'AuthFailure.InvalidAuthorization'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # Apk检测服务端无法响应。
 INTERNALERROR_APKSERVERERROR = 'InternalError.ApkServerError'
 
 # 服务端无法响应。
@@ -91,12 +94,15 @@
 
 # 找不到该资源。
 RESOURCEUNAVAILABLE_NOTFOUND = 'ResourceUnavailable.NotFound'
 
 # 未授权操作。
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
+# 鉴权失败。
+UNAUTHORIZEDOPERATION_AUTHFAILED = 'UnauthorizedOperation.AuthFailed'
+
 # 不是白名单用户。
 UNAUTHORIZEDOPERATION_NOTWHITEUSER = 'UnauthorizedOperation.NotWhiteUser'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
```

### Comparing `tencentcloud-sdk-python-ms-3.0.914/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.915/tencentcloud/ms/v20180408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,37 +334,41 @@
         :type CosId: str
         :param CosKey: 密钥KEY信息
         :type CosKey: str
         :param CosTocken: 密钥TOCKEN信息
         :type CosTocken: str
         :param CosPrefix: 密钥可访问的文件前缀人。例如：CosPrefix=test/123/666，则该密钥只能操作test/123/666为前缀的文件，例如test/123/666/1.txt
         :type CosPrefix: str
+        :param CosToken: 密钥TOCKEN信息
+        :type CosToken: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.CosAppid = None
         self.CosBucket = None
         self.CosRegion = None
         self.ExpireTime = None
         self.CosId = None
         self.CosKey = None
         self.CosTocken = None
         self.CosPrefix = None
+        self.CosToken = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.CosAppid = params.get("CosAppid")
         self.CosBucket = params.get("CosBucket")
         self.CosRegion = params.get("CosRegion")
         self.ExpireTime = params.get("ExpireTime")
         self.CosId = params.get("CosId")
         self.CosKey = params.get("CosKey")
         self.CosTocken = params.get("CosTocken")
         self.CosPrefix = params.get("CosPrefix")
+        self.CosToken = params.get("CosToken")
         self.RequestId = params.get("RequestId")
 
 
 class CreateResourceInstancesRequest(AbstractModel):
     """CreateResourceInstances请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ms-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.914/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.915/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.915/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.914/setup.py` & `tencentcloud-sdk-python-ms-3.0.915/setup.py`

 * *Files identical despite different names*

