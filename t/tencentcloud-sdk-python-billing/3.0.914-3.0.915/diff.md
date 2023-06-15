# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.914.tar", last modified: Wed Jun 14 00:19:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.915.tar", last modified: Thu Jun 15 00:18:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.914.tar` & `tencentcloud-sdk-python-billing-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   166860 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    21124 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:19:14.000000 tencentcloud-sdk-python-billing-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   167054 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:18:29.000000 tencentcloud-sdk-python-billing-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.914/README.rst` & `tencentcloud-sdk-python-billing-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1630,15 +1630,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param OrderId: 订单号
         :type OrderId: str
-        :param Status: 订单状态
+        :param Status: 订单的状态 1：未支付 2：已支付3：发货中 4：已发货 5：发货失败 6：已退款 7：已关单 8：订单过期 9：订单已失效 10：产品已失效 11：代付拒绝 12：支付中
         :type Status: int
         :param Payer: 支付者
         :type Payer: str
         :param CreateTime: 创建时间
         :type CreateTime: str
         :param Creator: 创建人
         :type Creator: str
```

### Comparing `tencentcloud-sdk-python-billing-3.0.914/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.915/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.914/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.915/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.915/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.914/setup.py` & `tencentcloud-sdk-python-billing-3.0.915/setup.py`

 * *Files identical despite different names*

