# Comparing `tmp/tencentcloud-sdk-python-live-3.0.914.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.914.tar", last modified: Wed Jun 14 00:29:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.915.tar", last modified: Thu Jun 15 00:28:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.914.tar` & `tencentcloud-sdk-python-live-3.0.915.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   138415 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   435096 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:29:24.000000 tencentcloud-sdk-python-live-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   153149 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    19977 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   480059 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-15 00:28:42.000000 tencentcloud-sdk-python-live-3.0.915/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.915/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/README.rst` & `tencentcloud-sdk-python-live-3.0.915/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/live_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateLivePadRule(self, request):
+        """创建直播垫片规则。
+
+        :param request: Request instance for CreateLivePadRule.
+        :type request: :class:`tencentcloud.live.v20180801.models.CreateLivePadRuleRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.CreateLivePadRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateLivePadRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateLivePadRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateLivePadTemplate(self, request):
+        """创建直播垫片模板。
+
+        :param request: Request instance for CreateLivePadTemplate.
+        :type request: :class:`tencentcloud.live.v20180801.models.CreateLivePadTemplateRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.CreateLivePadTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateLivePadTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateLivePadTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateLivePullStreamTask(self, request):
         """创建直播拉流任务。支持将外部已有的点播文件，或者直播源拉取过来转推到指定的目标地址。
         注意：
         1. 默认支持任务数上限200个，如有特殊需求，可通过提单到售后进行评估增加上限。
         2. 源流视频编码目前只支持: H264, H265。其他编码格式建议先进行转码处理。
         3. 源流音频编码目前只支持: AAC。其他编码格式建议先进行转码处理。
         4. 可在控制台开启过期自动清理，避免过期任务占用任务数额度。
@@ -378,14 +424,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateLiveStreamMonitor(self, request):
+        """该接口用来创建直播流监播任务。
+
+        :param request: Request instance for CreateLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.CreateLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.CreateLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateLiveTimeShiftRule(self, request):
         """创建直播时移规则，需要先调用[CreateLiveTimeShiftTemplate](/document/product/267/86169)接口创建直播时移模板，将返回的模板id绑定到流使用。
         <br>直播时移相关文档：[直播时移](/document/product/267/86134)。
 
         :param request: Request instance for CreateLiveTimeShiftRule.
         :type request: :class:`tencentcloud.live.v20180801.models.CreateLiveTimeShiftRuleRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.CreateLiveTimeShiftRuleResponse`
@@ -654,14 +723,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteLivePadRule(self, request):
+        """删除直播垫片规则。
+
+        :param request: Request instance for DeleteLivePadRule.
+        :type request: :class:`tencentcloud.live.v20180801.models.DeleteLivePadRuleRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DeleteLivePadRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteLivePadRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteLivePadRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteLivePadTemplate(self, request):
+        """删除直播垫片模板。
+
+        :param request: Request instance for DeleteLivePadTemplate.
+        :type request: :class:`tencentcloud.live.v20180801.models.DeleteLivePadTemplateRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DeleteLivePadTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteLivePadTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteLivePadTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteLivePullStreamTask(self, request):
         """删除接口 CreateLivePullStreamTask 创建的拉流任务。
         注意：
         1. 入参中的 TaskId 为 CreateLivePullStreamTask 接口创建时返回的TaskId。
         2. 也可通过 DescribeLivePullStreamTasks 进行查询创建的任务。
 
         :param request: Request instance for DeleteLivePullStreamTask.
@@ -795,14 +910,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteLiveStreamMonitor(self, request):
+        """该接口用来删除直播流监播任务。
+
+        :param request: Request instance for DeleteLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DeleteLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteLiveTimeShiftRule(self, request):
         """删除直播时移规则。
 
         :param request: Request instance for DeleteLiveTimeShiftRule.
         :type request: :class:`tencentcloud.live.v20180801.models.DeleteLiveTimeShiftRuleRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DeleteLiveTimeShiftRuleResponse`
 
@@ -1513,14 +1651,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLivePadRules(self, request):
+        """获取直播垫片规则列表。
+
+        :param request: Request instance for DescribeLivePadRules.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadRulesRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePadRulesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLivePadRules", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLivePadRulesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLivePadTemplate(self, request):
+        """获取单个直播垫片模板
+
+        :param request: Request instance for DescribeLivePadTemplate.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplateRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLivePadTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLivePadTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLivePadTemplates(self, request):
+        """获取直播垫片模板。
+
+        :param request: Request instance for DescribeLivePadTemplates.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplatesRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePadTemplatesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLivePadTemplates", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLivePadTemplatesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLivePlayAuthKey(self, request):
         """查询播放鉴权key。
 
         :param request: Request instance for DescribeLivePlayAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePlayAuthKeyRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePlayAuthKeyResponse`
 
@@ -1748,14 +1955,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLiveStreamMonitor(self, request):
+        """该接口用来查询某个特定监播任务的配置。
+
+        :param request: Request instance for DescribeLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeLiveStreamMonitorList(self, request):
+        """该接口用来查询直播流监播任务配置的列表信息。
+
+        :param request: Request instance for DescribeLiveStreamMonitorList.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorListRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamMonitorListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLiveStreamMonitorList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLiveStreamMonitorListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLiveStreamOnlineList(self, request):
         """返回正在直播中的流列表。适用于推流成功后查询在线流信息。
 
         注意：
         1. 该接口仅提供辅助查询在线流列表功能，业务重要场景不可强依赖该接口。
         2. 该接口仅适用于流数少于2万路的情况，对于流数较大用户请联系售后。
 
@@ -2156,14 +2409,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeMonitorReport(self, request):
+        """用来查询监播场次7天内的智能识别、断流、低帧率等信息的汇总报告。
+
+        :param request: Request instance for DescribeMonitorReport.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeMonitorReportRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeMonitorReportResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeMonitorReport", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeMonitorReportResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribePlayErrorCodeDetailInfoList(self, request):
         """查询下行播放错误码信息，某段时间内1分钟粒度的各http错误码出现的次数，包括4xx，5xx。
 
 
         :param request: Request instance for DescribePlayErrorCodeDetailInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeDetailInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeDetailInfoListResponse`
@@ -2746,14 +3022,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyLivePadTemplate(self, request):
+        """修改直播垫片模板。
+
+        :param request: Request instance for ModifyLivePadTemplate.
+        :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePadTemplateRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.ModifyLivePadTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyLivePadTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyLivePadTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyLivePlayAuthKey(self, request):
         """修改播放鉴权key
 
         :param request: Request instance for ModifyLivePlayAuthKey.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLivePlayAuthKeyRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.ModifyLivePlayAuthKeyResponse`
 
@@ -2886,14 +3185,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyLiveStreamMonitor(self, request):
+        """该接口用来修改直播流监播任务的配置。
+
+        :param request: Request instance for ModifyLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.ModifyLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyLiveTimeShiftTemplate(self, request):
         """修改直播时移模板。
 
         :param request: Request instance for ModifyLiveTimeShiftTemplate.
         :type request: :class:`tencentcloud.live.v20180801.models.ModifyLiveTimeShiftTemplateRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.ModifyLiveTimeShiftTemplateResponse`
 
@@ -3050,14 +3372,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def StartLiveStreamMonitor(self, request):
+        """该接口用来启动直播流监播任务。
+
+        :param request: Request instance for StartLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.StartLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.StartLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def StopLiveRecord(self, request):
         """说明：录制后的文件存放于点播平台。用户如需使用录制功能，需首先自行开通点播账号并确保账号可用。录制文件存放后，相关费用（含存储以及下行播放流量）按照点播平台计费方式收取，请参考对应文档。
 
         :param request: Request instance for StopLiveRecord.
         :type request: :class:`tencentcloud.live.v20180801.models.StopLiveRecordRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.StopLiveRecordResponse`
 
@@ -3071,14 +3416,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def StopLiveStreamMonitor(self, request):
+        """该接口用来停止直播流监播任务。
+
+        :param request: Request instance for StopLiveStreamMonitor.
+        :type request: :class:`tencentcloud.live.v20180801.models.StopLiveStreamMonitorRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.StopLiveStreamMonitorResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopLiveStreamMonitor", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopLiveStreamMonitorResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def StopRecordTask(self, request):
         """提前结束录制，中止运行中的录制任务并生成录制文件。任务被成功终止后，本次任务将不再启动。
 
         :param request: Request instance for StopRecordTask.
         :type request: :class:`tencentcloud.live.v20180801.models.StopRecordTaskRequest`
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+# CAM签名/鉴权错误。
+AUTHFAILURE = 'AuthFailure'
+
 # DryRun 操作，代表请求将会是成功的，只是多传了 DryRun 参数。
 DRYRUNOPERATION = 'DryRunOperation'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 操作 AI 接口失败。
@@ -58,23 +61,29 @@
 
 # 模版使用中。
 FAILEDOPERATION_CONFINUSED = 'FailedOperation.ConfInUsed'
 
 # 下发CDN平台失败。
 FAILEDOPERATION_CONFIGCDNFAILED = 'FailedOperation.ConfigCDNFailed'
 
+# 任务接口执行冲突。
+FAILEDOPERATION_CONFLICTACTION = 'FailedOperation.ConflictAction'
+
 # Cos bucket 不存在。
 FAILEDOPERATION_COSBUCKETNOTEXIST = 'FailedOperation.CosBucketNotExist'
 
 # 无权限访问 Cos bucket。
 FAILEDOPERATION_COSBUCKETNOTPERMISSION = 'FailedOperation.CosBucketNotPermission'
 
 # Cos 角色不存在，请前往 控制台 -> 功能配置 -> 直播截图&鉴黄 页面进行授权。
 FAILEDOPERATION_COSROLENOTEXISTS = 'FailedOperation.CosRoleNotExists'
 
+# 数据库访问异常。
+FAILEDOPERATION_DATABASENOTACCESSIBLE = 'FailedOperation.DatabaseNotAccessible'
+
 # 2天内有产生流量，域名处于锁定期间，2天内无流量产生才允许删除域名。
 FAILEDOPERATION_DELETEDOMAININLOCKEDTIME = 'FailedOperation.DeleteDomainInLockedTime'
 
 # 域名已添加。
 FAILEDOPERATION_DOMAINADDED = 'FailedOperation.DomainAdded'
 
 # 配置域名规则失败。
@@ -97,14 +106,17 @@
 
 # 无在线流。
 FAILEDOPERATION_HASNOTLIVINGSTREAM = 'FailedOperation.HasNotLivingStream'
 
 # 域名数量超过限制(100个）。
 FAILEDOPERATION_HOSTOUTLIMIT = 'FailedOperation.HostOutLimit'
 
+# 禁止监播c流。
+FAILEDOPERATION_INPUTSTREAMMIXTYPENOTACCESSIBLE = 'FailedOperation.InputStreamMixTypeNotAccessible'
+
 # 证书状态不正确。
 FAILEDOPERATION_INVALIDCERTIFICATESTATUSCODE = 'FailedOperation.InvalidCertificateStatusCode'
 
 # 参数有误。
 FAILEDOPERATION_INVALIDPARAM = 'FailedOperation.InvalidParam'
 
 # 操作 CDN 接口失败。
@@ -112,14 +124,23 @@
 
 # 操作点播接口异常。
 FAILEDOPERATION_INVOKEVIDEOAPIFAIL = 'FailedOperation.InvokeVideoApiFail'
 
 # 计费平台返回余额不足。
 FAILEDOPERATION_JIFEINOENOUGHFUND = 'FailedOperation.JiFeiNoEnoughFund'
 
+# 监播任务处于启动状态。
+FAILEDOPERATION_MONITORISACTIVE = 'FailedOperation.MonitorIsActive'
+
+# 监播任务超出限制。
+FAILEDOPERATION_MONITORLIMITEXCEEDED = 'FailedOperation.MonitorLimitExceeded'
+
+# 监播任务不存在。
+FAILEDOPERATION_MONITORNOTEXIST = 'FailedOperation.MonitorNotExist'
+
 # 当前 CA 机构访问繁忙，请稍后重试。
 FAILEDOPERATION_NETWORKERROR = 'FailedOperation.NetworkError'
 
 # 您没有该项目的操作权限。
 FAILEDOPERATION_NOPROJECTPERMISSION = 'FailedOperation.NoProjectPermission'
 
 # 尚未通过实名认证。
@@ -133,20 +154,32 @@
 
 # 启动混流失败。
 FAILEDOPERATION_PROCESSMIXERROR = 'FailedOperation.ProcessMixError'
 
 # 查询 upload 信息失败。
 FAILEDOPERATION_QUERYUPLOADINFOFAILED = 'FailedOperation.QueryUploadInfoFailed'
 
+# 关联服务无法访问。
+FAILEDOPERATION_RELATESERVERNOTACCESSIBLE = 'FailedOperation.RelateServerNotAccessible'
+
+# 输入关联的运行中的监播任务超出限制。
+FAILEDOPERATION_RELATEDRUNNINGMONITORLIMITEXCEEDED = 'FailedOperation.RelatedRunningMonitorLimitExceeded'
+
 # 规则已经存在。
 FAILEDOPERATION_RULEALREADYEXIST = 'FailedOperation.RuleAlreadyExist'
 
 # 用户没有有效的流量套餐包。
 FAILEDOPERATION_SDKNOPACKAGE = 'FailedOperation.SdkNoPackage'
 
+# 启动监播任务失败。
+FAILEDOPERATION_STARTTASKFAILED = 'FailedOperation.StartTaskFailed'
+
+# 停止监播任务失败。
+FAILEDOPERATION_STOPTASKFAILED = 'FailedOperation.StopTaskFailed'
+
 # 流不存在。
 FAILEDOPERATION_STREAMNOTEXIST = 'FailedOperation.StreamNotExist'
 
 # 子域名已添加。
 FAILEDOPERATION_SUBDOMAINADDED = 'FailedOperation.SubDomainAdded'
 
 # 解绑Tag失败，请尝试手动解绑。
@@ -427,14 +460,17 @@
 
 # 当月不允许添加已删除的小程序域名。
 INVALIDPARAMETER_MPHOSTDELETE = 'InvalidParameter.MpHostDelete'
 
 # 小程序插件没有授权。
 INVALIDPARAMETER_MPPLUGINNOUSE = 'InvalidParameter.MpPluginNoUse'
 
+# 该APPID未开通LVB服务。
+INVALIDPARAMETER_NOTALLOWUSELVB = 'InvalidParameter.NotAllowUseLVB'
+
 # 其他错误。
 INVALIDPARAMETER_OTHERERROR = 'InvalidParameter.OtherError'
 
 # 转码模板已存在。
 INVALIDPARAMETER_PROCESSORALREADYEXIST = 'InvalidParameter.ProcessorAlreadyExist'
 
 # 规则没有找到。
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.915/tencentcloud/live/v20180801/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1317,14 +1317,143 @@
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateLivePadRuleRequest(AbstractModel):
+    """CreateLivePadRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DomainName: 推流域名。
+        :type DomainName: str
+        :param TemplateId: 模板 ID。
+        :type TemplateId: int
+        :param AppName: 推流路径，与推流和播放地址中的AppName保持一致，默认为 live。
+        :type AppName: str
+        :param StreamName: 流名称。
+注：如果本参数设置为非空字符串，规则将只对此推流起作用。
+        :type StreamName: str
+        """
+        self.DomainName = None
+        self.TemplateId = None
+        self.AppName = None
+        self.StreamName = None
+
+
+    def _deserialize(self, params):
+        self.DomainName = params.get("DomainName")
+        self.TemplateId = params.get("TemplateId")
+        self.AppName = params.get("AppName")
+        self.StreamName = params.get("StreamName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateLivePadRuleResponse(AbstractModel):
+    """CreateLivePadRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class CreateLivePadTemplateRequest(AbstractModel):
+    """CreateLivePadTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateName: 模板名称。
+长度上限：255字节。
+仅支持中文、英文、数字、_、-。
+        :type TemplateName: str
+        :param Url: 垫片内容。
+        :type Url: str
+        :param Description: 描述信息。
+长度上限：1024字节。
+仅支持中文、英文、数字、_、-。
+        :type Description: str
+        :param WaitDuration: 断流等待时间。
+取值范围：0-30000。
+单位：ms。
+        :type WaitDuration: int
+        :param MaxDuration: 最大垫片时长。
+取值范围：0 - 正无穷。
+单位：ms。
+        :type MaxDuration: int
+        :param Type: 垫片内容类型：
+1：图片，2：视频。
+默认值：1。
+        :type Type: int
+        """
+        self.TemplateName = None
+        self.Url = None
+        self.Description = None
+        self.WaitDuration = None
+        self.MaxDuration = None
+        self.Type = None
+
+
+    def _deserialize(self, params):
+        self.TemplateName = params.get("TemplateName")
+        self.Url = params.get("Url")
+        self.Description = params.get("Description")
+        self.WaitDuration = params.get("WaitDuration")
+        self.MaxDuration = params.get("MaxDuration")
+        self.Type = params.get("Type")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateLivePadTemplateResponse(AbstractModel):
+    """CreateLivePadTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateId: 模板Id。
+        :type TemplateId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TemplateId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TemplateId = params.get("TemplateId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateLivePullStreamTaskRequest(AbstractModel):
     """CreateLivePullStreamTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1922,14 +2051,114 @@
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateLiveStreamMonitorRequest(AbstractModel):
+    """CreateLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OutputInfo: 监播任务的输出信息。
+        :type OutputInfo: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorOutputInfo`
+        :param InputList: 待监播的输入流信息列表。
+        :type InputList: list of LiveStreamMonitorInputInfo
+        :param MonitorName: 监播任务名称。字段长度小于128字节（一个汉字两个字节）。
+        :type MonitorName: str
+        :param NotifyPolicy: 监播事件通知策略。
+不填默认为没有任何通知。
+        :type NotifyPolicy: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorNotifyPolicy`
+        :param AsrLanguage: 智能语音识别语种设置：
+0 关闭 1 中文 2 英文 3 日文 4 韩文。
+        :type AsrLanguage: int
+        :param OcrLanguage: 智能文字识别语种设置：
+0 关闭 1 中、英文。
+        :type OcrLanguage: int
+        :param AiAsrInputIndexList: 智能语音识别的输入列表，若开启语音识别则必填。
+（第1条输入流index为1）
+        :type AiAsrInputIndexList: list of int non-negative
+        :param AiOcrInputIndexList: 智能文字识别的输入列表，若开启文字识别则必填。
+（第1条输入流index为1）
+        :type AiOcrInputIndexList: list of int non-negative
+        :param CheckStreamBroken: 是否开启断流检测。
+        :type CheckStreamBroken: int
+        :param CheckStreamLowFrameRate: 是否开启低帧率检测。
+        :type CheckStreamLowFrameRate: int
+        :param AllowMonitorReport: 是否存储监播事件到监播报告，以及是否允许查询监播报告。
+        :type AllowMonitorReport: int
+        """
+        self.OutputInfo = None
+        self.InputList = None
+        self.MonitorName = None
+        self.NotifyPolicy = None
+        self.AsrLanguage = None
+        self.OcrLanguage = None
+        self.AiAsrInputIndexList = None
+        self.AiOcrInputIndexList = None
+        self.CheckStreamBroken = None
+        self.CheckStreamLowFrameRate = None
+        self.AllowMonitorReport = None
+
+
+    def _deserialize(self, params):
+        if params.get("OutputInfo") is not None:
+            self.OutputInfo = LiveStreamMonitorOutputInfo()
+            self.OutputInfo._deserialize(params.get("OutputInfo"))
+        if params.get("InputList") is not None:
+            self.InputList = []
+            for item in params.get("InputList"):
+                obj = LiveStreamMonitorInputInfo()
+                obj._deserialize(item)
+                self.InputList.append(obj)
+        self.MonitorName = params.get("MonitorName")
+        if params.get("NotifyPolicy") is not None:
+            self.NotifyPolicy = LiveStreamMonitorNotifyPolicy()
+            self.NotifyPolicy._deserialize(params.get("NotifyPolicy"))
+        self.AsrLanguage = params.get("AsrLanguage")
+        self.OcrLanguage = params.get("OcrLanguage")
+        self.AiAsrInputIndexList = params.get("AiAsrInputIndexList")
+        self.AiOcrInputIndexList = params.get("AiOcrInputIndexList")
+        self.CheckStreamBroken = params.get("CheckStreamBroken")
+        self.CheckStreamLowFrameRate = params.get("CheckStreamLowFrameRate")
+        self.AllowMonitorReport = params.get("AllowMonitorReport")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateLiveStreamMonitorResponse(AbstractModel):
+    """CreateLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MonitorId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.MonitorId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateLiveTimeShiftRuleRequest(AbstractModel):
     """CreateLiveTimeShiftRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2793,14 +3022,111 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteLivePadRuleRequest(AbstractModel):
+    """DeleteLivePadRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DomainName: 推流域名。
+域名+AppName+StreamName唯一标识单个转码规则，如需删除需要强匹配，例如AppName为空也需要传空字符串进行强匹配。
+        :type DomainName: str
+        :param AppName: 推流路径，与推流和播放地址中的AppName保持一致，默认为 live。
+域名+AppName+StreamName唯一标识单个转码规则，如需删除需要强匹配，例如AppName为空也需要传空字符串进行强匹配。
+        :type AppName: str
+        :param StreamName: 流名称。
+域名+AppName+StreamName唯一标识单个转码规则，如需删除需要强匹配，例如AppName为空也需要传空字符串进行强匹配。
+        :type StreamName: str
+        :param TemplateId: 直播垫片模板id。
+        :type TemplateId: int
+        """
+        self.DomainName = None
+        self.AppName = None
+        self.StreamName = None
+        self.TemplateId = None
+
+
+    def _deserialize(self, params):
+        self.DomainName = params.get("DomainName")
+        self.AppName = params.get("AppName")
+        self.StreamName = params.get("StreamName")
+        self.TemplateId = params.get("TemplateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteLivePadRuleResponse(AbstractModel):
+    """DeleteLivePadRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class DeleteLivePadTemplateRequest(AbstractModel):
+    """DeleteLivePadTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateId: 模板 ID。
+        :type TemplateId: int
+        """
+        self.TemplateId = None
+
+
+    def _deserialize(self, params):
+        self.TemplateId = params.get("TemplateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteLivePadTemplateResponse(AbstractModel):
+    """DeleteLivePadTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteLivePullStreamTaskRequest(AbstractModel):
     """DeleteLivePullStreamTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3068,14 +3394,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteLiveStreamMonitorRequest(AbstractModel):
+    """DeleteLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID
+        :type MonitorId: str
+        """
+        self.MonitorId = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteLiveStreamMonitorResponse(AbstractModel):
+    """DeleteLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteLiveTimeShiftRuleRequest(AbstractModel):
     """DeleteLiveTimeShiftRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4868,14 +5235,125 @@
         self.TotalNum = params.get("TotalNum")
         self.PageNum = params.get("PageNum")
         self.PageSize = params.get("PageSize")
         self.FluxPackageBillMode = params.get("FluxPackageBillMode")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLivePadRulesRequest(AbstractModel):
+    """DescribeLivePadRules请求参数结构体
+
+    """
+
+
+class DescribeLivePadRulesResponse(AbstractModel):
+    """DescribeLivePadRules返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Rules: 规则信息列表。
+        :type Rules: list of RuleInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Rules = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Rules") is not None:
+            self.Rules = []
+            for item in params.get("Rules"):
+                obj = RuleInfo()
+                obj._deserialize(item)
+                self.Rules.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeLivePadTemplateRequest(AbstractModel):
+    """DescribeLivePadTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateId: 模板id。
+        :type TemplateId: int
+        """
+        self.TemplateId = None
+
+
+    def _deserialize(self, params):
+        self.TemplateId = params.get("TemplateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLivePadTemplateResponse(AbstractModel):
+    """DescribeLivePadTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Template: 直播垫片模板信息。
+        :type Template: :class:`tencentcloud.live.v20180801.models.PadTemplate`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Template = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Template") is not None:
+            self.Template = PadTemplate()
+            self.Template._deserialize(params.get("Template"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeLivePadTemplatesRequest(AbstractModel):
+    """DescribeLivePadTemplates请求参数结构体
+
+    """
+
+
+class DescribeLivePadTemplatesResponse(AbstractModel):
+    """DescribeLivePadTemplates返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Templates: 直播垫片模板信息。
+        :type Templates: list of PadTemplate
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Templates = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Templates") is not None:
+            self.Templates = []
+            for item in params.get("Templates"):
+                obj = PadTemplate()
+                obj._deserialize(item)
+                self.Templates.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLivePlayAuthKeyRequest(AbstractModel):
     """DescribeLivePlayAuthKey请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5406,14 +5884,122 @@
         self.PageNum = params.get("PageNum")
         self.PageSize = params.get("PageSize")
         self.TotalNum = params.get("TotalNum")
         self.TotalPage = params.get("TotalPage")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLiveStreamMonitorListRequest(AbstractModel):
+    """DescribeLiveStreamMonitorList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Index: 查询列表时的起始偏移。
+        :type Index: int
+        :param Count: 本次查询的记录个数。最小值为1。
+        :type Count: int
+        """
+        self.Index = None
+        self.Count = None
+
+
+    def _deserialize(self, params):
+        self.Index = params.get("Index")
+        self.Count = params.get("Count")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLiveStreamMonitorListResponse(AbstractModel):
+    """DescribeLiveStreamMonitorList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalNum: 账号下的直播流监播任务个数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalNum: int
+        :param LiveStreamMonitors: 直播流监播任务列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LiveStreamMonitors: list of LiveStreamMonitorInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalNum = None
+        self.LiveStreamMonitors = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalNum = params.get("TotalNum")
+        if params.get("LiveStreamMonitors") is not None:
+            self.LiveStreamMonitors = []
+            for item in params.get("LiveStreamMonitors"):
+                obj = LiveStreamMonitorInfo()
+                obj._deserialize(item)
+                self.LiveStreamMonitors.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeLiveStreamMonitorRequest(AbstractModel):
+    """DescribeLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID。
+        :type MonitorId: str
+        """
+        self.MonitorId = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLiveStreamMonitorResponse(AbstractModel):
+    """DescribeLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LiveStreamMonitor: 直播监播任务相关信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LiveStreamMonitor: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorInfo`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.LiveStreamMonitor = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("LiveStreamMonitor") is not None:
+            self.LiveStreamMonitor = LiveStreamMonitorInfo()
+            self.LiveStreamMonitor._deserialize(params.get("LiveStreamMonitor"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLiveStreamOnlineListRequest(AbstractModel):
     """DescribeLiveStreamOnlineList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6412,14 +6998,69 @@
                 obj = LogInfo()
                 obj._deserialize(item)
                 self.LogInfoList.append(obj)
         self.TotalNum = params.get("TotalNum")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeMonitorReportRequest(AbstractModel):
+    """DescribeMonitorReport请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID。
+        :type MonitorId: str
+        """
+        self.MonitorId = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeMonitorReportResponse(AbstractModel):
+    """DescribeMonitorReport返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MPSResult: 媒体处理结果信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MPSResult: :class:`tencentcloud.live.v20180801.models.MPSResult`
+        :param DiagnoseResult: 媒体诊断结果信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DiagnoseResult: :class:`tencentcloud.live.v20180801.models.DiagnoseResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.MPSResult = None
+        self.DiagnoseResult = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("MPSResult") is not None:
+            self.MPSResult = MPSResult()
+            self.MPSResult._deserialize(params.get("MPSResult"))
+        if params.get("DiagnoseResult") is not None:
+            self.DiagnoseResult = DiagnoseResult()
+            self.DiagnoseResult._deserialize(params.get("DiagnoseResult"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribePlayErrorCodeDetailInfoListRequest(AbstractModel):
     """DescribePlayErrorCodeDetailInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7929,14 +8570,44 @@
             for item in params.get("DataInfoList"):
                 obj = PlaySumStatInfo()
                 obj._deserialize(item)
                 self.DataInfoList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DiagnoseResult(AbstractModel):
+    """媒体诊断结果，包含断流信息、低帧率信息等
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StreamBrokenResults: 断流信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StreamBrokenResults: list of str
+        :param LowFrameRateResults: 低帧率信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LowFrameRateResults: list of str
+        """
+        self.StreamBrokenResults = None
+        self.LowFrameRateResults = None
+
+
+    def _deserialize(self, params):
+        self.StreamBrokenResults = params.get("StreamBrokenResults")
+        self.LowFrameRateResults = params.get("LowFrameRateResults")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DomainCertInfo(AbstractModel):
     """域名证书信息
 
     """
 
     def __init__(self):
         r"""
@@ -8784,14 +9455,262 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LiveStreamMonitorInfo(AbstractModel):
+    """直播监播任务信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MonitorId: str
+        :param MonitorName: 监播任务名称。128字节以内。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MonitorName: str
+        :param OutputInfo: 监播任务输出信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputInfo: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorOutputInfo`
+        :param InputList: 待监播的输入流信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputList: list of LiveStreamMonitorInputInfo
+        :param Status: 监播任务状态。
+0： 代表空闲
+1： 代表监播中。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param StartTime: 上一次的启动时间，unix时间戳。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: int
+        :param StopTime: 上一次的停止时间，unix时间戳。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StopTime: int
+        :param CreateTime: 监播任务创建时间，unix时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: int
+        :param UpdateTime: 监播任务更新时间，unix时间戳
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: int
+        :param NotifyPolicy: 监播事件通知策略。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NotifyPolicy: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorNotifyPolicy`
+        :param AudibleInputIndexList: 输出音频的输入Index列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AudibleInputIndexList: list of int non-negative
+        :param AiAsrInputIndexList: 开启智能语音识别的输入Index列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiAsrInputIndexList: list of int non-negative
+        :param CheckStreamBroken: 是否开启断流检测
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CheckStreamBroken: int
+        :param CheckStreamLowFrameRate: 是否开启低帧率检测
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CheckStreamLowFrameRate: int
+        :param AsrLanguage: 智能语音识别语种：
+0 关闭 1 中文 2 英文 3日文 4 韩文
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsrLanguage: int
+        :param OcrLanguage: 智能文字识别语种：
+0 关闭 1 中、英文
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OcrLanguage: int
+        :param AiOcrInputIndexList: 开启智能文字识别的输入Index列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiOcrInputIndexList: list of int non-negative
+        :param AllowMonitorReport: 是否存储监播事件到监播报告，以及是否允许查询监播报告
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AllowMonitorReport: int
+        """
+        self.MonitorId = None
+        self.MonitorName = None
+        self.OutputInfo = None
+        self.InputList = None
+        self.Status = None
+        self.StartTime = None
+        self.StopTime = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.NotifyPolicy = None
+        self.AudibleInputIndexList = None
+        self.AiAsrInputIndexList = None
+        self.CheckStreamBroken = None
+        self.CheckStreamLowFrameRate = None
+        self.AsrLanguage = None
+        self.OcrLanguage = None
+        self.AiOcrInputIndexList = None
+        self.AllowMonitorReport = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        self.MonitorName = params.get("MonitorName")
+        if params.get("OutputInfo") is not None:
+            self.OutputInfo = LiveStreamMonitorOutputInfo()
+            self.OutputInfo._deserialize(params.get("OutputInfo"))
+        if params.get("InputList") is not None:
+            self.InputList = []
+            for item in params.get("InputList"):
+                obj = LiveStreamMonitorInputInfo()
+                obj._deserialize(item)
+                self.InputList.append(obj)
+        self.Status = params.get("Status")
+        self.StartTime = params.get("StartTime")
+        self.StopTime = params.get("StopTime")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        if params.get("NotifyPolicy") is not None:
+            self.NotifyPolicy = LiveStreamMonitorNotifyPolicy()
+            self.NotifyPolicy._deserialize(params.get("NotifyPolicy"))
+        self.AudibleInputIndexList = params.get("AudibleInputIndexList")
+        self.AiAsrInputIndexList = params.get("AiAsrInputIndexList")
+        self.CheckStreamBroken = params.get("CheckStreamBroken")
+        self.CheckStreamLowFrameRate = params.get("CheckStreamLowFrameRate")
+        self.AsrLanguage = params.get("AsrLanguage")
+        self.OcrLanguage = params.get("OcrLanguage")
+        self.AiOcrInputIndexList = params.get("AiOcrInputIndexList")
+        self.AllowMonitorReport = params.get("AllowMonitorReport")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveStreamMonitorInputInfo(AbstractModel):
+    """直播监播功能输入流信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InputStreamName: 待监播的输入流名称。256字节以内，只允许包含字母、数字、‘-’，‘_’，'.'字符。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputStreamName: str
+        :param InputDomain: 待监播的输入流推流域名。128字节以内，只允许填处于启用状态的推流域名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputDomain: str
+        :param InputApp: 待监播的输入流推流路径。32字节以内，只允许包含字母、数字、‘-’，‘_’，'.'字符。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputApp: str
+        :param InputUrl: 待监播的输入流推流url。一般场景下，无需该参数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InputUrl: str
+        :param Description: 描述。256字节以内。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        """
+        self.InputStreamName = None
+        self.InputDomain = None
+        self.InputApp = None
+        self.InputUrl = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.InputStreamName = params.get("InputStreamName")
+        self.InputDomain = params.get("InputDomain")
+        self.InputApp = params.get("InputApp")
+        self.InputUrl = params.get("InputUrl")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveStreamMonitorNotifyPolicy(AbstractModel):
+    """直播流监播通知策略
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NotifyPolicyType: 通知策略类型：范围[0,1]
+0:代表不使用任何通知策略
+1:代表使用全局回调策略，所有事件通知到CallbackUrl。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NotifyPolicyType: int
+        :param CallbackUrl: 回调URL：长度[0,512]
+只支持http和https类型的url。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CallbackUrl: str
+        """
+        self.NotifyPolicyType = None
+        self.CallbackUrl = None
+
+
+    def _deserialize(self, params):
+        self.NotifyPolicyType = params.get("NotifyPolicyType")
+        self.CallbackUrl = params.get("CallbackUrl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveStreamMonitorOutputInfo(AbstractModel):
+    """直播流监播输出流信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OutputStreamWidth: 监播任务输出流宽度像素。范围[1,1920]。建议至少大于100像素。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputStreamWidth: int
+        :param OutputStreamHeight: 监播任务输出流长度像素。范围[1,1080]，建议至少大于100像素。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputStreamHeight: int
+        :param OutputStreamName: 监播任务输出流名称。
+不填时，系统会自动生成。
+256字节以内，只允许包含字母、数字、‘-’，‘_’，'.'字符。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputStreamName: str
+        :param OutputDomain: 监播任务播放域名。128字节以内，只允许填处于启用状态的播放域名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputDomain: str
+        :param OutputApp: 监播任务播放路径。32字节以内，只允许包含字母、数字、‘-’，‘_’，'.'字符。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OutputApp: str
+        """
+        self.OutputStreamWidth = None
+        self.OutputStreamHeight = None
+        self.OutputStreamName = None
+        self.OutputDomain = None
+        self.OutputApp = None
+
+
+    def _deserialize(self, params):
+        self.OutputStreamWidth = params.get("OutputStreamWidth")
+        self.OutputStreamHeight = params.get("OutputStreamHeight")
+        self.OutputStreamName = params.get("OutputStreamName")
+        self.OutputDomain = params.get("OutputDomain")
+        self.OutputApp = params.get("OutputApp")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class LogInfo(AbstractModel):
     """日志url信息。
 
     """
 
     def __init__(self):
         r"""
@@ -8821,14 +9740,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class MPSResult(AbstractModel):
+    """媒体处理结果，包含智能语音识别、智能文字识别结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AiAsrResults: 智能语音识别结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiAsrResults: list of str
+        :param AiOcrResults: 智能文字识别结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiOcrResults: list of str
+        """
+        self.AiAsrResults = None
+        self.AiOcrResults = None
+
+
+    def _deserialize(self, params):
+        self.AiAsrResults = params.get("AiAsrResults")
+        self.AiOcrResults = params.get("AiOcrResults")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ModifyLiveCallbackTemplateRequest(AbstractModel):
     """ModifyLiveCallbackTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9040,14 +9989,87 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyLivePadTemplateRequest(AbstractModel):
+    """ModifyLivePadTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateId: 模板id。
+        :type TemplateId: int
+        :param Url: 垫片内容。
+        :type Url: str
+        :param WaitDuration: 断流等待时间。
+取值范围：0-30000。
+单位：ms。
+        :type WaitDuration: int
+        :param MaxDuration: 最大垫片时长。
+取值范围：0 - 正无穷。
+单位：ms。
+        :type MaxDuration: int
+        :param TemplateName: 模板名称。
+长度上限：255字节。
+仅支持中文、英文、数字、_、-。
+        :type TemplateName: str
+        :param Description: 描述信息。
+长度上限：1024字节。
+仅支持中文、英文、数字、_、-。
+        :type Description: str
+        :param Type: 垫片内容类型： 1：图片，2：视频。 默认值：1。
+        :type Type: int
+        """
+        self.TemplateId = None
+        self.Url = None
+        self.WaitDuration = None
+        self.MaxDuration = None
+        self.TemplateName = None
+        self.Description = None
+        self.Type = None
+
+
+    def _deserialize(self, params):
+        self.TemplateId = params.get("TemplateId")
+        self.Url = params.get("Url")
+        self.WaitDuration = params.get("WaitDuration")
+        self.MaxDuration = params.get("MaxDuration")
+        self.TemplateName = params.get("TemplateName")
+        self.Description = params.get("Description")
+        self.Type = params.get("Type")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyLivePadTemplateResponse(AbstractModel):
+    """ModifyLivePadTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyLivePlayAuthKeyRequest(AbstractModel):
     """ModifyLivePlayAuthKey请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9553,14 +10575,110 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyLiveStreamMonitorRequest(AbstractModel):
+    """ModifyLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播任务ID。
+        :type MonitorId: str
+        :param MonitorName: 监播任务的名称。长度128字节以内（一个汉字两个字节）。
+        :type MonitorName: str
+        :param OutputInfo: 监播任务输出信息。
+        :type OutputInfo: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorOutputInfo`
+        :param InputList: 待监播的输入流信息。
+        :type InputList: list of LiveStreamMonitorInputInfo
+        :param NotifyPolicy: 监播事件通知策略。
+        :type NotifyPolicy: :class:`tencentcloud.live.v20180801.models.LiveStreamMonitorNotifyPolicy`
+        :param AsrLanguage: 智能语音识别语种：
+0 关闭 1 中文 2 英文 3 日文 4 韩文。
+        :type AsrLanguage: int
+        :param OcrLanguage: 智能文字识别语种：
+0 关闭 1 中、英文。
+        :type OcrLanguage: int
+        :param AiAsrInputIndexList: 语音识别输入流列表，1代表第一条输入流。
+        :type AiAsrInputIndexList: list of int non-negative
+        :param AiOcrInputIndexList: 文字识别输入流列表，1代表第一条输入流。
+        :type AiOcrInputIndexList: list of int non-negative
+        :param CheckStreamBroken: 是否开启断流检测。
+        :type CheckStreamBroken: int
+        :param CheckStreamLowFrameRate: 是否开启低帧率检测。
+        :type CheckStreamLowFrameRate: int
+        :param AllowMonitorReport: 是否存储监播事件到监播报告，以及是否允许查询监播报告。
+        :type AllowMonitorReport: int
+        """
+        self.MonitorId = None
+        self.MonitorName = None
+        self.OutputInfo = None
+        self.InputList = None
+        self.NotifyPolicy = None
+        self.AsrLanguage = None
+        self.OcrLanguage = None
+        self.AiAsrInputIndexList = None
+        self.AiOcrInputIndexList = None
+        self.CheckStreamBroken = None
+        self.CheckStreamLowFrameRate = None
+        self.AllowMonitorReport = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        self.MonitorName = params.get("MonitorName")
+        if params.get("OutputInfo") is not None:
+            self.OutputInfo = LiveStreamMonitorOutputInfo()
+            self.OutputInfo._deserialize(params.get("OutputInfo"))
+        if params.get("InputList") is not None:
+            self.InputList = []
+            for item in params.get("InputList"):
+                obj = LiveStreamMonitorInputInfo()
+                obj._deserialize(item)
+                self.InputList.append(obj)
+        if params.get("NotifyPolicy") is not None:
+            self.NotifyPolicy = LiveStreamMonitorNotifyPolicy()
+            self.NotifyPolicy._deserialize(params.get("NotifyPolicy"))
+        self.AsrLanguage = params.get("AsrLanguage")
+        self.OcrLanguage = params.get("OcrLanguage")
+        self.AiAsrInputIndexList = params.get("AiAsrInputIndexList")
+        self.AiOcrInputIndexList = params.get("AiOcrInputIndexList")
+        self.CheckStreamBroken = params.get("CheckStreamBroken")
+        self.CheckStreamLowFrameRate = params.get("CheckStreamLowFrameRate")
+        self.AllowMonitorReport = params.get("AllowMonitorReport")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyLiveStreamMonitorResponse(AbstractModel):
+    """ModifyLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyLiveTimeShiftTemplateRequest(AbstractModel):
     """ModifyLiveTimeShiftTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9967,14 +11085,74 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PadTemplate(AbstractModel):
+    """直播垫片模板。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TemplateId: 模板id。
+        :type TemplateId: int
+        :param TemplateName: 模板名称。
+        :type TemplateName: str
+        :param Url: 垫片内容。
+        :type Url: str
+        :param CreateTime: 模板创建时间。
+        :type CreateTime: str
+        :param UpdateTime: 模板修改时间。
+        :type UpdateTime: str
+        :param Description: 模板描述。
+        :type Description: str
+        :param WaitDuration: 断流等待时间。
+取值范围：0-30000。
+单位：ms。
+        :type WaitDuration: int
+        :param MaxDuration: 最大垫片时长。
+取值范围：0 - 正无穷。
+单位：ms。
+        :type MaxDuration: int
+        :param Type: 垫片内容类型： 1：图片，2：视频。 默认值：1。
+        :type Type: int
+        """
+        self.TemplateId = None
+        self.TemplateName = None
+        self.Url = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Description = None
+        self.WaitDuration = None
+        self.MaxDuration = None
+        self.Type = None
+
+
+    def _deserialize(self, params):
+        self.TemplateId = params.get("TemplateId")
+        self.TemplateName = params.get("TemplateName")
+        self.Url = params.get("Url")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Description = params.get("Description")
+        self.WaitDuration = params.get("WaitDuration")
+        self.MaxDuration = params.get("MaxDuration")
+        self.Type = params.get("Type")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PlayAuthKeyInfo(AbstractModel):
     """播放鉴权key信息。
 
     """
 
     def __init__(self):
         r"""
@@ -11408,14 +12586,61 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StartLiveStreamMonitorRequest(AbstractModel):
+    """StartLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播ID。
+        :type MonitorId: str
+        :param AudibleInputIndexList: 监播画面声音InputIndex,支持多个输入声音。
+取值范围 InputIndex必须已经存在。
+不填默认无声音输出。
+        :type AudibleInputIndexList: list of int non-negative
+        """
+        self.MonitorId = None
+        self.AudibleInputIndexList = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        self.AudibleInputIndexList = params.get("AudibleInputIndexList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StartLiveStreamMonitorResponse(AbstractModel):
+    """StartLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class StopLiveRecordRequest(AbstractModel):
     """StopLiveRecord请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11445,14 +12670,55 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class StopLiveStreamMonitorRequest(AbstractModel):
+    """StopLiveStreamMonitor请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MonitorId: 监播ID
+        :type MonitorId: str
+        """
+        self.MonitorId = None
+
+
+    def _deserialize(self, params):
+        self.MonitorId = params.get("MonitorId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StopLiveStreamMonitorResponse(AbstractModel):
+    """StopLiveStreamMonitor返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.915/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.914/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.915/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.914
+Version: 3.0.915
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.914/setup.py` & `tencentcloud-sdk-python-live-3.0.915/setup.py`

 * *Files identical despite different names*

