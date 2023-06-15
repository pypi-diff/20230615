# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.914.tar", last modified: Wed Jun 14 00:29:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.915.tar", last modified: Thu Jun 15 00:28:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.914.tar` & `tencentcloud-sdk-python-lighthouse-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    26133 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    92541 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240373 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:29:18.000000 tencentcloud-sdk-python-lighthouse-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    26133 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    92544 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240532 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:28:36.000000 tencentcloud-sdk-python-lighthouse-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ApplyInstanceSnapshot(self, request):
         """本接口（ApplyInstanceSnapshot）用于回滚指定实例的系统盘快照。
         <li>仅支持回滚到原系统盘。</li>
-        <li>用于回滚的快照必须处于 NORMAL 状态。快照状态可以通 DescribeSnapshots 接口查询，见输出参数中 SnapshotState 字段解释。</li>
+        <li>用于回滚的快照必须处于 NORMAL 状态。快照状态可以通过 DescribeSnapshots 接口查询，见输出参数中 SnapshotState 字段解释。</li>
         <li>回滚快照时，实例的状态必须为 STOPPED 或 RUNNING，可通过 DescribeInstances 接口查询实例状态。处于 RUNNING 状态的实例会强制关机，然后回滚快照。</li>
 
         :param request: Request instance for ApplyInstanceSnapshot.
         :type request: :class:`tencentcloud.lighthouse.v20200324.models.ApplyInstanceSnapshotRequest`
         :rtype: :class:`tencentcloud.lighthouse.v20200324.models.ApplyInstanceSnapshotResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 class AutoMountConfiguration(AbstractModel):
     """自动挂载并初始化该数据盘。
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 待挂载的实例ID。指定的实例必须处于“运行中”状态。
+        :param InstanceId: 待挂载的实例ID。指定的实例必须与指定的数据盘处于同一可用区，实例状态必须处于“运行中”状态，且实例必须支持[自动化助手](https://cloud.tencent.com/document/product/1340/50752)。
         :type InstanceId: str
         :param MountPoint: 实例内的挂载点。仅Linux操作系统的实例可传入该参数, 不传则默认挂载在“/data/disk”路径下。
         :type MountPoint: str
         :param FileSystemType: 文件系统类型。取值: “ext4”、“xfs”。仅Linux操作系统的实例可传入该参数, 不传则默认为“ext4”。
         :type FileSystemType: str
         """
         self.InstanceId = None
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.915/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.915/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.914/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.915/setup.py`

 * *Files identical despite different names*

