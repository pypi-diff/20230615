# Comparing `tmp/data_collect-0.8.7.tar.gz` & `tmp/data_collect-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.7.tar", last modified: Wed Jun 14 19:46:33 2023, max compression
+gzip compressed data, was "data_collect-0.8.8.tar", last modified: Thu Jun 15 02:32:29 2023, max compression
```

## Comparing `data_collect-0.8.7.tar` & `data_collect-0.8.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.517897 data_collect-0.8.7/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:46:33.517991 data_collect-0.8.7/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.515792 data_collect-0.8.7/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12648 2023-06-14 19:46:12.000000 data_collect-0.8.7/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.517606 data_collect-0.8.7/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:41:14.000000 data_collect-0.8.7/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.7/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.7/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.7/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.7/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.7/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.7/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.7/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-14 19:46:33.516601 data_collect-0.8.7/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-14 19:46:33.000000 data_collect-0.8.7/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-14 19:46:33.518445 data_collect-0.8.7/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-14 19:46:32.000000 data_collect-0.8.7/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.185801 data_collect-0.8.8/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-15 02:32:29.185896 data_collect-0.8.8/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.183364 data_collect-0.8.8/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12756 2023-06-15 02:29:17.000000 data_collect-0.8.8/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.185309 data_collect-0.8.8/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:41:14.000000 data_collect-0.8.8/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.8/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.8/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.8/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.8/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.8/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.8/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.184363 data_collect-0.8.8/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-15 02:32:29.186327 data_collect-0.8.8/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-15 02:32:28.000000 data_collect-0.8.8/setup.py
```

### Comparing `data_collect-0.8.7/PKG-INFO` & `data_collect-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.7
+Version: 0.8.8
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.7/data_collect/client.py` & `data_collect-0.8.8/data_collect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,27 +137,28 @@
 
     def log(self,
             correlation_id: str,
             logline: Dict[str, Any] = None,
             designation: str = '',
             text: Sequence = None,
             time_series: Sequence = None,
-            file_paths: Union[Dict, List, str] = None,
+            blob_paths: Union[Dict, List, str] = None,
             image: WindmillImage = None,
             blob: Union[WindmillText, WindmillBlob] = None,
             prediction: Union[Dict, List, str] = None,
             ground_truth: Union[Dict, List] = None,
             config: DataCollectConfig = None,
             ):
         """
         data capture main log function
         :param correlation_id: 请求id，用于关联请求和响应
         :param logline: 日志行，字典类型，key为字符串，value为字符串、数字、列表、字典
         :param designation: 用于区分不同的数据类型，如input、prediction、ground_truth
         :param blob: 二进制文件 类型定义在data_types/blob.py
+        :blob_paths: 二进制文件路径，用于记录二进制文件路径，类型为dict、list、str
         :param image: 图片 data_types/image.py
         :param text: 文本，本期未支持，预留记录nlp模型的输出
         :param time_series: 时间序列，本期未支持
         :param prediction: 模型预测结果
         :param ground_truth: ground truth 本期未支持
         :param config: DataCollectConfig 支持在log时重新执行DataCollectConfig
         :return:
@@ -197,16 +198,16 @@
                                                                                                     cls=NpEncoder)
         if image is not None and self.input_enable:
             self._log_image(correlation_id, image, designation)
 
         if blob is not None and self._is_data_capture_enable():
             self._log_blob(correlation_id, blob, designation)
         
-        if file_paths is not None and self._is_data_capture_enable():
-            message['file_paths'] = file_paths
+        if blob_paths is not None and self._is_data_capture_enable():
+            message['blob_paths'] = blob_paths
             
         if self._is_data_capture_enable() and message is not None:
             self._logger.log(message)
 
     def _load_env_setting_and_config(self, config: DataCollectConfig):
         """
         load env setting and config
```

### Comparing `data_collect-0.8.7/data_collect/constants.py` & `data_collect-0.8.8/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/data_types/blob.py` & `data_collect-0.8.8/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/data_types/image.py` & `data_collect-0.8.8/data_collect/data_types/image.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/logger.py` & `data_collect-0.8.8/data_collect/logger.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/queue.py` & `data_collect-0.8.8/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/thread.py` & `data_collect-0.8.8/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect/utils.py` & `data_collect-0.8.8/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.8/data_collect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.7
+Version: 0.8.8
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.7/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.8/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.7/setup.cfg` & `data_collect-0.8.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.7
+version = 0.8.8
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

