# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.914.tar", last modified: Wed Jun 14 00:18:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.915.tar", last modified: Thu Jun 15 00:18:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.914.tar` & `tencentcloud-sdk-python-autoscaling-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)    60526 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)    19836 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258716 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:18:42.000000 tencentcloud-sdk-python-autoscaling-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)    60526 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)    19836 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258716 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-15 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:18:01.000000 tencentcloud-sdk-python-autoscaling-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.915/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.915/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.914/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.915/setup.py`

 * *Files identical despite different names*

