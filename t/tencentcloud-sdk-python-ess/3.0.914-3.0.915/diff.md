# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.914.tar", last modified: Wed Jun 14 00:26:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.915.tar", last modified: Thu Jun 15 00:25:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.914.tar` & `tencentcloud-sdk-python-ess-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    57665 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   246979 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    57650 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   247333 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:25:27.000000 tencentcloud-sdk-python-ess-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.914/README.rst` & `tencentcloud-sdk-python-ess-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateIntegrationEmployees(self, request):
-        """创建员工,如需在此接口提醒员工实名，入参Employees的OpenId不传
+        """创建员工,此接口会发送提醒员工实名的短信
 
         :param request: Request instance for CreateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesResponse`
 
         """
         try:
@@ -1209,15 +1209,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateIntegrationEmployees(self, request):
-        """更新员工信息(姓名，手机号，邮件)，用户实名后无法更改姓名与手机号
+        """更新员工信息(姓名，手机号，邮件、部门)，用户实名后无法更改姓名与手机号
 
         :param request: Request instance for UpdateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.915/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,14 +727,15 @@
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
 参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
         :type ComponentExtra: str
         :param IsFormType: 是否是表单域类型，默认不false-不是
+注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
@@ -814,16 +815,18 @@
 KEYWORD 关键字，使用ComponentId指定关键字
         :type GenerateMode: str
         :param ComponentDateFontSize: 日期签署控件的字号，默认为 12
         :type ComponentDateFontSize: int
         :param ChannelComponentId: 第三方应用集成平台模板控件 id 标识
         :type ChannelComponentId: str
         :param OffsetX: 指定关键字时横坐标偏移量，单位pt
+注意：此字段可能返回 null，表示取不到有效值。
         :type OffsetX: float
         :param OffsetY: 指定关键字时纵坐标偏移量，单位pt
+注意：此字段可能返回 null，表示取不到有效值。
         :type OffsetY: float
         :param ChannelComponentSource: 第三方应用集成中子客企业控件来源。0-平台指定；1-用户自定义
         :type ChannelComponentSource: int
         :param KeywordOrder: 指定关键字排序规则，Positive-正序，Reverse-倒序。传入Positive时会根据关键字在PDF文件内的顺序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的第一个关键字。
 传入Reverse时会根据关键字在PDF文件内的反序进行排列。在指定KeywordIndexes时，0代表在PDF内查找内容时，查找到的最后一个关键字。
         :type KeywordOrder: str
         :param KeywordPage: 指定关键字页码，可选参数，指定页码后，将只在指定的页码内查找关键字，非该页码的关键字将不会查询出来
@@ -1852,15 +1855,16 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Employees: 待创建员工的信息，Mobile和DisplayName必填,OpenId和Email选填，其他字段暂不支持
+        :param Employees: 待创建员工的信息，不超过20个。
+Mobile和DisplayName必填,OpenId、Email和Department.DepartmentId选填，其他字段暂不支持。
         :type Employees: list of Staff
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.Employees = None
         self.Agent = None
@@ -3611,15 +3615,15 @@
 class DescribeIntegrationRolesRequest(AbstractModel):
     """DescribeIntegrationRoles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Limit: 返回最大数量，最大为200
         :type Limit: int
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Filters: 查询的关键字段:
 Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
@@ -6322,15 +6326,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Employees: 员工信息，OpenId和UserId必填一个,Email、DisplayName和Email选填，其他字段暂不支持
+        :param Employees: 员工信息，不超过100个。
+根据UserId或OpenId更新员工，必填一个，优先UserId。
+可更新Mobile、DisplayName、Email和Department.DepartmentId字段，其他字段暂不支持
         :type Employees: list of Staff
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.Employees = None
         self.Agent = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.915/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.915/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.914/setup.py` & `tencentcloud-sdk-python-ess-3.0.915/setup.py`

 * *Files identical despite different names*

