# Comparing `tmp/broadcast_service-2.0.0.tar.gz` & `tmp/broadcast_service-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/broadcast-service/broadcast-service/dist/.tmp-0ofyddo3/broadcast_service-2.0.0.tar", last modified: Wed Jun 14 11:25:45 2023, max compression
+gzip compressed data, was "/home/runner/work/broadcast-service/broadcast-service/dist/.tmp-7o1iltz5/broadcast_service-2.1.0.tar", last modified: Thu Jun 15 13:10:46 2023, max compression
```

## Comparing `broadcast_service-2.0.0.tar` & `broadcast_service-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14258 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/broadcast_service/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/broadcast_service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:25:45.000000 broadcast_service-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-14 11:25:27.000000 broadcast_service-2.0.0/tests/test_publisher_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/broadcast_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/broadcast_service/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/broadcast_service/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/broadcast_service/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/broadcast_service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:10:46.000000 broadcast_service-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-15 13:10:30.000000 broadcast_service-2.1.0/tests/test_publisher_callback.py
```

### Comparing `broadcast_service-2.0.0/LICENSE` & `broadcast_service-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/PKG-INFO` & `broadcast_service-2.1.0/broadcast_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: broadcast_service
-Version: 2.0.0
+Name: broadcast-service
+Version: 2.1.0
 Summary: A lightweight third-party broadcast/pubsub library
 Home-page: https://github.com/Undertone0809/broadcast-service
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: broadcast,broadcast-service,publisher,subscriber,pubsub
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     broadcast-service
 </h1>
 <p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+  <strong>A powerful python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
    <a target="_blank" href=''>
```

### Comparing `broadcast_service-2.0.0/README.md` & `broadcast_service-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <h1 align="center">
     broadcast-service
 </h1>
 <p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+  <strong>A powerful python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
    <a target="_blank" href=''>
```

### Comparing `broadcast_service-2.0.0/broadcast_service/__init__.py` & `broadcast_service-2.1.0/broadcast_service/__init__.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/broadcast_service/_core.py` & `broadcast_service-2.1.0/broadcast_service/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,14 +238,18 @@
     """Used to store the return values of all callback functions for subscribers."""
     callback: Optional[Callable] = None
     """Your publisher will obtain the callback and subscriber parameters after the callback function
     of all subscribers callback is completed."""
     enable_final_return: bool = False
     """This parameter indicates whether you want to call the publisher callback after calling the topic 
     n times, or call the publisher callback after each topic publishing."""
+    split_parameters: Optional[List[Any]] = None
+    """If you initiate multiple calls and want to pass different parameters to the subscriber in each 
+    call, you can use this parameter for parameter passing. Additionally, when you use this parameter, 
+    you do not need to pass any parameters in the broadcast() function."""
 
     @property
     def start_publisher_callback_or_not(self) -> bool:
         if self.status == PUBLISHER_CALLBACK_STATUS["END"]:
             return False
         if not self.enable_final_return:
             return True
@@ -296,42 +300,51 @@
 
     def config(
             self,
             num_of_executions: int = 1,
             callback: Optional[Callable] = None,
             enable_final_return: bool = False,
             interval: float = 0,
+            split_parameters: Optional[List[Any]] = None
     ) -> 'BroadcastService':
         """Provide more complex topic publish mode
 
         Args:
             num_of_executions: default is 1, indicating the number of times the same topic is published at once
             callback: default is None. You can get callback and the parameters of subscriber
                 after all subscribers' callback functions have been completed.
             enable_final_return: default is False, it means you can get callback after you publish
                 n times topic. In this case, finish_callback params is store in *args rather than **kwargs.
             interval: publish interval. Unit seconds.
+            split_parameters: If you initiate multiple calls and want to pass different parameters to the subscriber
+                in each call, you can use this parameter for parameter passing. Additionally, when you use this
+                parameter, you do not need to pass any parameters in the broadcast() function.
         Returns:
             Returns current object, which is used to call broadcast with configuration.
         """
         self.enable_config = True
         self.publish_dispatch_config_manager.create_publisher_callback(
             num_of_executions=num_of_executions,
             callback=callback,
             enable_final_return=enable_final_return,
             interval=interval,
-            status=PUBLISHER_CALLBACK_STATUS['RUNNING']
+            status=PUBLISHER_CALLBACK_STATUS['RUNNING'],
+            split_parameters=split_parameters
         )
         return self
 
     def broadcast(self, topics: str or List[str], *args, **kwargs):
         if self.enable_config:
             self.cur_publisher_dispatch_config = self.publish_dispatch_config_manager.get_latest_publisher_callback()
 
         for i in range(self.cur_publisher_dispatch_config.get_num_of_executions()):
+            if self.cur_publisher_dispatch_config.split_parameters:
+                kwargs.update(
+                    {"split_parameter": self.cur_publisher_dispatch_config.split_parameters[i]}
+                )
             super().broadcast(topics, *args, **kwargs)
             self.cur_publisher_dispatch_config.counter += 1
             time.sleep(self.cur_publisher_dispatch_config.interval)
 
         self.enable_config = False
 
     def _invoke_finish_callback(self):
```

### Comparing `broadcast_service-2.0.0/broadcast_service/logger.py` & `broadcast_service-2.1.0/broadcast_service/logger.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/broadcast_service/singleton.py` & `broadcast_service-2.1.0/broadcast_service/singleton.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/broadcast_service.egg-info/PKG-INFO` & `broadcast_service-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: broadcast-service
-Version: 2.0.0
+Name: broadcast_service
+Version: 2.1.0
 Summary: A lightweight third-party broadcast/pubsub library
 Home-page: https://github.com/Undertone0809/broadcast-service
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: broadcast,broadcast-service,publisher,subscriber,pubsub
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     broadcast-service
 </h1>
 <p align="center">
-  <strong>A lightweight python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
+  <strong>A powerful python broadcast library. You can easily construct a Broadcast pattern/Publish subscriber pattern through this library.</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
    <a target="_blank" href=''>
```

### Comparing `broadcast_service-2.0.0/setup.py` & `broadcast_service-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="broadcast_service",
-    version="2.0.0",
+    version="2.1.0",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A lightweight third-party broadcast/pubsub library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/broadcast-service",
     packages=setuptools.find_packages(),
```

### Comparing `broadcast_service-2.0.0/tests/__init__.py` & `broadcast_service-2.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/tests/test_async.py` & `broadcast_service-2.1.0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/tests/test_base.py` & `broadcast_service-2.1.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `broadcast_service-2.0.0/tests/test_publisher_callback.py` & `broadcast_service-2.1.0/tests/test_publisher_callback.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,7 +78,21 @@
             num_of_executions=5,
             interval=0.2
         ).publish("test_interval")
 
         duration = time.time() - start_time
         self.assertAlmostEqual(1, duration, delta=0.1)
         self.assertEqual(5, self.counter)
+
+    def test_split_parameter(self):
+        self.counter = 1
+
+        @broadcast_service.on_listen("test_split_parameter")
+        def handle_subscriber_callback(**kwargs):
+            self.assertEqual(self.counter, kwargs['split_parameter'])
+            self.counter += 1
+
+        params = [1, 2, 3]
+        broadcast_service.config(
+            num_of_executions=3,
+            split_parameters=params
+        ).publish("test_split_parameter")
```

