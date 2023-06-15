# Comparing `tmp/zcbot-crawl-sdk-0.0.8.tar.gz` & `tmp/zcbot-crawl-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-crawl-sdk-0.0.8.tar", last modified: Fri Mar 31 08:02:00 2023, max compression
+gzip compressed data, was "dist\zcbot-crawl-sdk-0.0.9.tar", last modified: Fri Mar 31 09:03:30 2023, max compression
```

## Comparing `zcbot-crawl-sdk-0.0.8.tar` & `zcbot-crawl-sdk-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.553859 zcbot-crawl-sdk-0.0.8/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-crawl-sdk-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      375 2023-03-31 08:02:00.553859 zcbot-crawl-sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-03-29 06:37:01.000000 zcbot-crawl-sdk-0.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-31 08:02:00.554858 zcbot-crawl-sdk-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-03-31 08:01:48.000000 zcbot-crawl-sdk-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.522859 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.537860 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/
--rw-rw-rw-   0        0        0        0 2022-03-23 07:19:36.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     5011 2023-03-29 06:40:27.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/api.py
--rw-rw-rw-   0        0        0      327 2022-03-23 00:45:58.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/auth.py
--rw-rw-rw-   0        0        0     1245 2022-03-23 07:09:21.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/exceptions.py
--rw-rw-rw-   0        0        0     2128 2023-03-29 06:41:13.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/http_client.py
--rw-rw-rw-   0        0        0     2802 2023-03-29 06:40:15.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/model.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.547858 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/
--rw-rw-rw-   0        0        0        0 2022-03-23 07:22:16.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/__init__.py
--rw-rw-rw-   0        0        0      317 2022-03-23 08:05:10.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/exceptions.py
--rw-rw-rw-   0        0        0     1039 2023-03-30 11:47:15.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/model.py
--rw-rw-rw-   0        0        0     3557 2023-03-30 12:39:24.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/processor.py
--rw-rw-rw-   0        0        0     1051 2023-03-30 14:41:55.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/rabbit_keys.py
--rw-rw-rw-   0        0        0     9473 2023-03-31 07:59:43.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/receiver.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.551859 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/util/
--rw-rw-rw-   0        0        0        0 2022-05-27 06:44:19.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/util/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/util/decator.py
--rw-rw-rw-   0        0        0     3908 2023-02-28 01:05:14.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/util/time.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:02:00.528859 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/
--rw-rw-rw-   0        0        0      375 2023-03-31 08:02:00.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-03-31 08:02:00.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:02:00.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-31 08:02:00.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-31 08:02:00.000000 zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.632575 zcbot-crawl-sdk-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-crawl-sdk-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      375 2023-03-31 09:03:30.631575 zcbot-crawl-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2023-03-29 06:37:01.000000 zcbot-crawl-sdk-0.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-03-31 09:03:30.632575 zcbot-crawl-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-03-31 09:03:22.000000 zcbot-crawl-sdk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.605576 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.618575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/
+-rw-rw-rw-   0        0        0        0 2022-03-23 07:19:36.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     5011 2023-03-29 06:40:27.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/api.py
+-rw-rw-rw-   0        0        0      327 2022-03-23 00:45:58.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/auth.py
+-rw-rw-rw-   0        0        0     1245 2022-03-23 07:09:21.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/exceptions.py
+-rw-rw-rw-   0        0        0     2128 2023-03-29 06:41:13.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/http_client.py
+-rw-rw-rw-   0        0        0     2802 2023-03-29 06:40:15.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/model.py
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.626576 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/
+-rw-rw-rw-   0        0        0        0 2022-03-23 07:22:16.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/__init__.py
+-rw-rw-rw-   0        0        0      317 2022-03-23 08:05:10.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/exceptions.py
+-rw-rw-rw-   0        0        0     1039 2023-03-30 11:47:15.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/model.py
+-rw-rw-rw-   0        0        0     3557 2023-03-30 12:39:24.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/processor.py
+-rw-rw-rw-   0        0        0     1051 2023-03-30 14:41:55.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/rabbit_keys.py
+-rw-rw-rw-   0        0        0     9249 2023-03-31 09:02:18.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/receiver.py
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.629575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/
+-rw-rw-rw-   0        0        0        0 2022-05-27 06:44:19.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/decator.py
+-rw-rw-rw-   0        0        0     3908 2023-02-28 01:05:14.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/time.py
+drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.611575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-crawl-sdk-0.0.8/setup.py` & `zcbot-crawl-sdk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-crawl-sdk',
-      version='0.0.8',
+      version='0.0.9',
       description='zcbot celery sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['pika', 'demjson', 'requests'],
       python_requires='>=3.7',
```

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/api.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/api.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/exceptions.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/http_client.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/http_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/api/model.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/model.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/processor.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/processor.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/rabbit_keys.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/rabbit_keys.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/receive/receiver.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,28 +105,30 @@
     2、消息与队列自动创建自动删除
     3、通道按批次区分
     """
 
     def __init__(self, processor: Union[AbstractStreamMessageProcess, Callable], rabbit_uri: str, max_watcher_count: int = None, max_processor_count: int = None):
         self.processor = processor
         self.rabbit_uri = rabbit_uri
+        # 默认值，和zcbot_spider保持一致
+        self.queue_expires = 28800
         _max_watcher_count = max_watcher_count or 4
         _max_processor_count = max_processor_count or 24
         self.watcher_executor = ThreadPoolExecutor(max_workers=_max_watcher_count, thread_name_prefix='stream-watcher')
         self.processor_executor = ThreadPoolExecutor(max_workers=_max_processor_count, thread_name_prefix='stream-processor')
         LOGGER.info(f'[流采结果]监听器初始化 rabbit_uri={self.rabbit_uri}')
 
     def watch(self, exchange_name: str, routing_name: str, queue_name: str):
-        self.watcher_executor.submit(self._receive_message, kwargs={'exchange_name': exchange_name, 'routing_name': routing_name, 'queue_name': queue_name})
+        self.watcher_executor.submit(self._receive_message, exchange_name, routing_name, queue_name)
 
     def _declare(self, exchange_name: str, routing_name: str, queue_name: str):
         # 定义
         connection = pika.BlockingConnection(pika.URLParameters(self.rabbit_uri))
-        channel = self.connection.channel()
-        channel.queue_declare(queue=queue_name)
+        channel = connection.channel()
+        channel.queue_declare(queue=queue_name, arguments={'x-expires': self.queue_expires * 1000})
         channel.exchange_declare(exchange=exchange_name)
         channel.queue_bind(queue=queue_name, exchange=exchange_name, routing_key=routing_name)
         LOGGER.info(f'[流采结果]队列信息 queue={queue_name}, exchange={exchange_name}, routing={routing_name}')
 
         return connection, channel
 
     def _receive_message(self, exchange_name: str, routing_name: str, queue_name: str):
@@ -138,42 +140,35 @@
         _process_func = self.processor
         if isinstance(self.processor, AbstractStreamMessageProcess):
             _process_func = self.processor.process_message
 
         connection, channel = self._declare(exchange_name, routing_name, queue_name)
         try:
             # 接收
-            for method, properties, body in channel.consume(self.queue_name, auto_ack=False):
+            for method, properties, body in channel.consume(queue_name, auto_ack=False):
                 # 保持通道激活状态
-                if not method or not properties:
+                if not method or not properties or not properties.headers:
                     LOGGER.error(f'[流采结果]无效消息 method={method}, properties={properties}, body={body}')
                     continue
-                try:
-                    headers = properties.headers
-                    if not headers:
-                        LOGGER.error(f'[流采结果]消息结构异常 properties={properties}, body={body}')
-                        continue
-                    # 消息解析并发处理
-                    msg_type = headers.get('msg_type', None)
-                    body_json = json.loads(body.decode())
-                    self.process_executor.submit(_process_func, msg_type, body_json)
-                except (StreamLostError, ConnectionAbortedError):
-                    LOGGER.error(f'[流采结果]服务端关闭链接通道')
-                except Exception:
-                    LOGGER.error(f'[流采结果]解析异常 {traceback.format_exc()}')
+                # 消息解析并发处理
+                msg_type = properties.headers.get('msg_type', None)
+                body_json = json.loads(body.decode())
+                self.processor_executor.submit(_process_func, msg_type, body_json)
                 # 消息确认
                 channel.basic_ack(method.delivery_tag)
+        except (StreamLostError, ConnectionAbortedError):
+            LOGGER.error(f'[流采结果]服务端关闭链接通道StreamLostError,ConnectionAbortedError -> 重连 {traceback.format_exc()}')
         except pika.exceptions.ConnectionClosedByBroker:
-            LOGGER.error(f'[流采结果]链接关闭异常ConnectionClosedByBroker -> 重试 {traceback.format_exc()}')
-        except pika.exceptions.AMQPChannelError as err:
-            LOGGER.error(f'[流采结果]通道关闭异常AMQPChannelError -> 重试 {traceback.format_exc()}')
+            LOGGER.error(f'[流采结果]链接关闭异常ConnectionClosedByBroker -> 重连 {traceback.format_exc()}')
+        except pika.exceptions.AMQPChannelError:
+            LOGGER.error(f'[流采结果]通道关闭异常AMQPChannelError -> 重连 {traceback.format_exc()}')
         except pika.exceptions.AMQPConnectionError:
-            LOGGER.error(f'[流采结果]链接关闭异常AMQPConnectionError -> 重试 {traceback.format_exc()}')
+            LOGGER.error(f'[流采结果]链接关闭异常AMQPConnectionError -> 重连 {traceback.format_exc()}')
         except Exception:
-            LOGGER.error(f'[流采结果]接收过程异常 {traceback.format_exc()}')
+            LOGGER.error(f'[流采结果]接收过程异常 -> 重连 {traceback.format_exc()}')
         finally:
             try:
                 # 关闭链接和通道（链接关闭通道自动关闭）
                 channel.close()
                 connection.close()
                 LOGGER.info(f'[流采结果]销毁队列')
             except Exception:
```

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk/util/time.py` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/time.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.8/zcbot_crawl_sdk.egg-info/SOURCES.txt` & `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

