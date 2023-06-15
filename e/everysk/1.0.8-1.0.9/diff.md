# Comparing `tmp/everysk-1.0.8.tar.gz` & `tmp/everysk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\everysk-1.0.8.tar", last modified: Tue Sep 28 13:19:26 2021, max compression
+gzip compressed data, was "dist\everysk-1.0.9.tar", last modified: Tue Oct 19 20:36:17 2021, max compression
```

## Comparing `everysk-1.0.8.tar` & `everysk-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-09-28 13:19:26.000000 everysk-1.0.8/
-drwxrwxrwx   0        0        0        0 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk/
--rw-rw-rw-   0        0        0     3127 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_requestor.py
-drwxrwxrwx   0        0        0        0 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk/api_resources/
--rw-rw-rw-   0        0        0     4375 2021-09-23 21:24:14.000000 everysk-1.0.8/everysk/api_resources/api_resource.py
--rw-rw-rw-   0        0        0     2572 2021-08-13 21:08:10.000000 everysk-1.0.8/everysk/api_resources/calculation.py
--rw-rw-rw-   0        0        0      850 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/custom_index.py
--rw-rw-rw-   0        0        0      845 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/datastore.py
--rw-rw-rw-   0        0        0      835 2021-09-08 19:30:14.000000 everysk-1.0.8/everysk/api_resources/file.py
--rw-rw-rw-   0        0        0     1490 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/market_data.py
--rw-rw-rw-   0        0        0      994 2021-07-26 14:15:25.000000 everysk-1.0.8/everysk/api_resources/parser.py
--rw-rw-rw-   0        0        0      847 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/portfolio.py
--rw-rw-rw-   0        0        0     2388 2021-09-28 13:09:24.000000 everysk-1.0.8/everysk/api_resources/report.py
--rw-rw-rw-   0        0        0      692 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/report_template.py
--rw-rw-rw-   0        0        0     1230 2021-09-28 13:09:24.000000 everysk-1.0.8/everysk/api_resources/workflow.py
--rw-rw-rw-   0        0        0      752 2021-09-28 13:09:42.000000 everysk-1.0.8/everysk/api_resources/workflow_execution.py
--rw-rw-rw-   0        0        0      887 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/api_resources/workspace.py
--rw-rw-rw-   0        0        0     1100 2021-09-28 13:09:24.000000 everysk-1.0.8/everysk/api_resources/__init__.py
--rw-rw-rw-   0        0        0   212549 2021-05-04 15:03:52.000000 everysk-1.0.8/everysk/ca-certificates.crt
--rw-rw-rw-   0        0        0     4603 2021-05-04 17:42:37.000000 everysk-1.0.8/everysk/http_client.py
--rw-rw-rw-   0        0        0    31779 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/six.py
--rw-rw-rw-   0        0        0     5082 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/utils.py
--rw-rw-rw-   0        0        0     1421 2021-04-29 14:13:07.000000 everysk-1.0.8/everysk/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/
--rw-rw-rw-   0        0        0        1 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3415 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       20 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/requires.txt
--rw-rw-rw-   0        0        0      842 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2021-09-28 13:19:26.000000 everysk-1.0.8/everysk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3415 2021-09-28 13:19:26.000000 everysk-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2786 2021-04-29 14:57:32.000000 everysk-1.0.8/README.md
--rw-rw-rw-   0        0        0      340 2021-09-28 13:19:26.000000 everysk-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      494 2021-09-28 13:19:10.000000 everysk-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-19 20:36:17.000000 everysk-1.0.9/
+drwxrwxrwx   0        0        0        0 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk/
+-rw-rw-rw-   0        0        0     3127 2021-04-29 14:13:07.000000 everysk-1.0.9/everysk/api_requestor.py
+drwxrwxrwx   0        0        0        0 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk/api_resources/
+-rw-rw-rw-   0        0        0     4674 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/api_resource.py
+-rw-rw-rw-   0        0        0     2559 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/calculation.py
+-rw-rw-rw-   0        0        0      850 2021-04-29 14:13:07.000000 everysk-1.0.9/everysk/api_resources/custom_index.py
+-rw-rw-rw-   0        0        0     1157 2021-10-19 20:32:06.000000 everysk-1.0.9/everysk/api_resources/datastore.py
+-rw-rw-rw-   0        0        0      835 2021-09-08 19:30:14.000000 everysk-1.0.9/everysk/api_resources/file.py
+-rw-rw-rw-   0        0        0     1477 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/market_data.py
+-rw-rw-rw-   0        0        0      994 2021-07-26 14:15:25.000000 everysk-1.0.9/everysk/api_resources/parser.py
+-rw-rw-rw-   0        0        0      903 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/portfolio.py
+-rw-rw-rw-   0        0        0     1213 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/report.py
+-rw-rw-rw-   0        0        0      692 2021-04-29 14:13:07.000000 everysk-1.0.9/everysk/api_resources/report_template.py
+-rw-rw-rw-   0        0        0     1217 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/workflow.py
+-rw-rw-rw-   0        0        0      752 2021-09-28 13:09:42.000000 everysk-1.0.9/everysk/api_resources/workflow_execution.py
+-rw-rw-rw-   0        0        0      874 2021-10-19 19:40:35.000000 everysk-1.0.9/everysk/api_resources/workspace.py
+-rw-rw-rw-   0        0        0     1098 2021-10-19 18:35:31.000000 everysk-1.0.9/everysk/api_resources/__init__.py
+-rw-rw-rw-   0        0        0   212549 2021-05-04 15:03:52.000000 everysk-1.0.9/everysk/ca-certificates.crt
+-rw-rw-rw-   0        0        0     4603 2021-05-04 17:42:37.000000 everysk-1.0.9/everysk/http_client.py
+-rw-rw-rw-   0        0        0    31779 2021-04-29 14:13:07.000000 everysk-1.0.9/everysk/six.py
+-rw-rw-rw-   0        0        0     5092 2021-10-19 18:32:35.000000 everysk-1.0.9/everysk/utils.py
+-rw-rw-rw-   0        0        0     1421 2021-04-29 14:13:07.000000 everysk-1.0.9/everysk/__init__.py
+drwxrwxrwx   0        0        0        0 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3415 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      842 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2021-10-19 20:36:17.000000 everysk-1.0.9/everysk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3415 2021-10-19 20:36:17.000000 everysk-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2786 2021-04-29 14:57:32.000000 everysk-1.0.9/README.md
+-rw-rw-rw-   0        0        0      340 2021-10-19 20:36:17.000000 everysk-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      494 2021-10-19 16:10:31.000000 everysk-1.0.9/setup.py
```

### Comparing `everysk-1.0.8/everysk/api_requestor.py` & `everysk-1.0.9/everysk/api_requestor.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/api_resource.py` & `everysk-1.0.9/everysk/api_resources/api_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,7 +123,16 @@
         #response = api_req.put(url, self)
         unsaved_values = self.get_unsaved_values()
         response = api_req.put(url, unsaved_values)
         data = response[self.class_name()]
         self.update(data)
         self.clear_unsaved_values()
         return self
+
+class FilterableAPIResource(APIResource):
+
+    @classmethod
+    def filter(cls,**kwargs):
+        api_req = utils.create_api_requestor(kwargs)
+        url = '/%s/filter' % cls.class_name_list()
+        response = api_req.post(url, kwargs)
+        return utils.to_list(cls, kwargs, response)
```

### Comparing `everysk-1.0.8/everysk/api_resources/calculation.py` & `everysk-1.0.9/everysk/api_resources/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # (C) Copyright 2020 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-import time
 from everysk.api_resources.api_resource import APIResource
 from everysk import utils
 
 class Calculation(APIResource):
 
     def refresh(self):
         return self
```

### Comparing `everysk-1.0.8/everysk/api_resources/custom_index.py` & `everysk-1.0.9/everysk/api_resources/custom_index.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/datastore.py` & `everysk-1.0.9/everysk/api_resources/workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 ###############################################################################
 #
-# (C) Copyright 2018 EVERYSK TECHNOLOGIES
+# (C) Copyright 2020 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
 from everysk.api_resources.api_resource import (
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
     UpdateableAPIResource
 )
+from everysk import utils
 
-class Datastore(
+class Workspace(
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
     UpdateableAPIResource
 ):
+
     @classmethod
     def class_name(cls):
-        return 'datastore'
+        return 'workspace'
```

### Comparing `everysk-1.0.8/everysk/api_resources/file.py` & `everysk-1.0.9/everysk/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/market_data.py` & `everysk-1.0.9/everysk/api_resources/market_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # (C) Copyright 2020 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-import time
 from everysk.api_resources.api_resource import APIResource
 from everysk import utils
 
 class MarketData(APIResource):
 
     def refresh(self):
         return selfs
```

### Comparing `everysk-1.0.8/everysk/api_resources/parser.py` & `everysk-1.0.9/everysk/api_resources/parser.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/portfolio.py` & `everysk-1.0.9/everysk/api_resources/portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 #
 ###############################################################################
 from everysk.api_resources.api_resource import (
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
-    UpdateableAPIResource
+    UpdateableAPIResource,
+    FilterableAPIResource
 )
 
 class Portfolio(
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
-    UpdateableAPIResource
+    UpdateableAPIResource,
+    FilterableAPIResource
 ):
     @classmethod
     def class_name(cls):
         return 'portfolio'
```

### Comparing `everysk-1.0.8/everysk/api_resources/report.py` & `everysk-1.0.9/everysk/api_resources/datastore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,37 @@
 ###############################################################################
 #
-# (C) Copyright 2020 EVERYSK TECHNOLOGIES
+# (C) Copyright 2018 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-import time
 from everysk.api_resources.api_resource import (
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
-    UpdateableAPIResource
+    UpdateableAPIResource,
+    FilterableAPIResource
 )
-from everysk.api_resources.workflow_execution import WorkflowExecution
-
 from everysk import utils
 
-class Report(
+class Datastore(
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
-    UpdateableAPIResource
+    UpdateableAPIResource,
+    FilterableAPIResource
 ):
     @classmethod
     def class_name(cls):
-        return 'report'
+        return 'datastore'
 
     @classmethod
-    def create(cls, debug_callback=None, **kwargs):
-        debug_callback = (lambda x, y: None) if (debug_callback is None) else debug_callback
-        api_req = utils.create_api_requestor(kwargs)
-        url = cls.class_url()
-        response = api_req.post(url, kwargs)
-        kwargs = {}
-        proc = utils.to_object(WorkflowExecution, kwargs, response)
-        debug_callback(0, proc)
-
-        loop_sleep = 1
-        loop_max = 700
-        loop_count = 0
-        done = ('completed', 'failed', 'timeout')
-        while proc.status not in done:
-            time.sleep(loop_sleep)
-            proc.refresh()
-            loop_count += 1
-            debug_callback(loop_count, proc)
-            if loop_count > loop_max:
-                raise Exception('max run loop achieved')
-        time.sleep(loop_sleep)
-        result = None
-        if proc.status in done:
-            result_ = proc.result
-            if result_['status'] == 'ok':
-                result = utils.to_object(Report, kwargs, {'report': result_['data']})
-        return result        
-
-    def share(self, **kwargs):
+    def explore(cls, **kwargs):
         api_req = utils.create_api_requestor(kwargs)
-        url = '%s/%s/share' % (self.class_url(), self.get('id'))
+        url = '/%s/explore' % cls.class_name_list()
         response = api_req.post(url, kwargs)
-        data = response[self.class_name()]
-        self.update(data)
-        self.clear_unsaved_values()
-        return self
+        return response
```

### Comparing `everysk-1.0.8/everysk/api_resources/report_template.py` & `everysk-1.0.9/everysk/api_resources/report_template.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/workflow.py` & `everysk-1.0.9/everysk/api_resources/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # (C) Copyright 2020 EVERYSK TECHNOLOGIES
 #
 # This is an unpublished work containing confidential and proprietary
 # information of EVERYSK TECHNOLOGIES. Disclosure, use, or reproduction
 # without authorization of EVERYSK TECHNOLOGIES is prohibited.
 #
 ###############################################################################
-import time
 from everysk.api_resources.api_resource import (
     RetrievableAPIResource,
     ListableAPIResource,
     DeletableAPIResource,
     CreateableAPIResource,
     UpdateableAPIResource
 )
```

### Comparing `everysk-1.0.8/everysk/api_resources/workflow_execution.py` & `everysk-1.0.9/everysk/api_resources/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/api_resources/__init__.py` & `everysk-1.0.9/everysk/api_resources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 from everysk.api_resources.report_template import ReportTemplate
 from everysk.api_resources.datastore import Datastore
 from everysk.api_resources.file import File
 from everysk.api_resources.custom_index import CustomIndex
 from everysk.api_resources.calculation import Calculation
 from everysk.api_resources.market_data import MarketData
 from everysk.api_resources.parser import Parser
-
```

### Comparing `everysk-1.0.8/everysk/ca-certificates.crt` & `everysk-1.0.9/everysk/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/http_client.py` & `everysk-1.0.9/everysk/http_client.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/six.py` & `everysk-1.0.9/everysk/six.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk/utils.py` & `everysk-1.0.9/everysk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         #     self._unsaved_values.remove(k)
 
 
 class EveryskList(list):
     def __init__(self, retrieve_params, response, key, cls):
         super(EveryskList, self).__init__()
         self.__page_size = retrieve_params.get('page_size', 10)
-        self.__next_page_token = response['next_page_token']
+        self.__next_page_token = response.get('next_page_token', None)
         self.extend([cls({}, params) for params in response[key]])
         return
 
     def page_size(self):
         return self.__page_size
 
     def next_page_token(self):
```

### Comparing `everysk-1.0.8/everysk/__init__.py` & `everysk-1.0.9/everysk/__init__.py`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/everysk.egg-info/PKG-INFO` & `everysk-1.0.9/everysk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everysk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for Everysk API
 Home-page: https://github.com/Everysk/Everysk-API-Python
 Author: Everysk Technologies
 Author-email: contact@everysk.com
 License: MIT
 Description: <p align="center"><img src="https://www.everysk.com/images/everysk_logo.svg" width="400"></p>
```

### Comparing `everysk-1.0.8/everysk.egg-info/SOURCES.txt` & `everysk-1.0.9/everysk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `everysk-1.0.8/PKG-INFO` & `everysk-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everysk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python client for Everysk API
 Home-page: https://github.com/Everysk/Everysk-API-Python
 Author: Everysk Technologies
 Author-email: contact@everysk.com
 License: MIT
 Description: <p align="center"><img src="https://www.everysk.com/images/everysk_logo.svg" width="400"></p>
```

### Comparing `everysk-1.0.8/README.md` & `everysk-1.0.9/README.md`

 * *Files identical despite different names*

