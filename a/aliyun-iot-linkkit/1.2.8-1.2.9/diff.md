# Comparing `tmp/aliyun-iot-linkkit-1.2.8.tar.gz` & `tmp/aliyun-iot-linkkit-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-iot-linkkit-1.2.8.tar", last modified: Mon Apr 17 02:01:22 2023, max compression
+gzip compressed data, was "dist/aliyun-iot-linkkit-1.2.9.tar", last modified: Thu May 18 09:31:14 2023, max compression
```

## Comparing `aliyun-iot-linkkit-1.2.8.tar` & `aliyun-iot-linkkit-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     1561 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/PKG-INFO
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linkkit/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)   124142 2023-04-07 06:44:24.000000 aliyun-iot-linkkit-1.2.8/linkkit/linkkit.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       16 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linkkit/__init__.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)    19761 2020-10-30 09:09:42.000000 aliyun-iot-linkkit-1.2.8/linkkit/h2client.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linksdktest/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/__init__.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      361 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/__init__.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     3558 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/var.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/method.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     1561 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/PKG-INFO
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      396 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/SOURCES.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       17 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/requires.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       20 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/top_level.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        1 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/dependency_links.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      840 2023-04-03 12:41:56.000000 aliyun-iot-linkkit-1.2.8/README.md
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      695 2023-04-07 06:41:26.000000 aliyun-iot-linkkit-1.2.8/setup.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       38 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/setup.cfg
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     1692 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/PKG-INFO
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/linkkit/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)   124328 2023-05-16 07:42:58.000000 aliyun-iot-linkkit-1.2.9/linkkit/linkkit.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       16 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.9/linkkit/__init__.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)    19761 2020-10-30 09:09:42.000000 aliyun-iot-linkkit-1.2.9/linkkit/h2client.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/linksdktest/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.9/linksdktest/__init__.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/linksdktest/common/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      361 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.9/linksdktest/common/__init__.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     3558 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.9/linksdktest/common/var.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.9/linksdktest/common/method.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     1692 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/PKG-INFO
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      396 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/SOURCES.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       17 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/requires.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       20 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/top_level.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        1 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/dependency_links.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      947 2023-05-16 07:42:58.000000 aliyun-iot-linkkit-1.2.9/README.md
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      695 2023-05-16 07:42:58.000000 aliyun-iot-linkkit-1.2.9/setup.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       38 2023-05-18 09:31:14.000000 aliyun-iot-linkkit-1.2.9/setup.cfg
```

### Comparing `aliyun-iot-linkkit-1.2.8/PKG-INFO` & `aliyun-iot-linkkit-1.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliyun-iot-linkkit
-Version: 1.2.8
+Version: 1.2.9
 Summary: Aliyun IoT Linkkit SDK for Python
 Home-page: UNKNOWN
 Author: Aliyun IoT Linkkit Python SDK
 Author-email: xicai.cxc@alibaba-inc.com
 License: UNKNOWN
 Description: #Python SDK for Aliyun IoT device
         
@@ -37,12 +37,15 @@
         
         ### 1.2.7
         * [UPDATE] add ota feature
         
         ### 1.2.8
         * [UPDATE] add mqtt dynamic-register with pre-registration feature
         
+        ### 1.2.9
+        * [UPDATE] add api to enable users to re-connect to iot platform manually in case of exceptions
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aliyun-iot-linkkit-1.2.8/linkkit/linkkit.py` & `aliyun-iot-linkkit-1.2.9/linkkit/linkkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
         self.__device_interface_info = ""
         self.__device_mac = None
         self.__cellular_IMEI = None
         self.__cellular_ICCID = None
         self.__cellular_IMSI = None
         self.__cellular_MSISDN = None
         self.__mqtt_client = None
-        self.__sdk_version = "1.2.8"
+        self.__sdk_version = "1.2.9"
         self.__sdk_program_language = "Python"
         self.__endpoint = None
         self.__instance_id = instance_id
 
         self.__mqtt_port = 1883
         self.__mqtt_protocol = "MQTTv311"
         self.__mqtt_transport = "TCP"
@@ -2824,14 +2824,19 @@
                 self.__on_unsubscribe_topic(mid, self.__user_data)
             except Exception as err:
                 self.__link_log.error('Caught exception in on_unsubscribe_topic: %s', err)
 
     def dump_user_topics(self):
         return self.__user_topics
 
+    def force_reconnect(self):
+        self.__link_log.error("force reconnecting")
+        self.__linkkit_state = LinkKit.LinkKitState.CONNECTING
+        self.__mqtt_client.reconnect()
+
     @staticmethod
     def to_user_topic(topic):
         topic_section = topic.split('/', 3)
         user_topic = topic_section[3]
         return user_topic
 
     def to_full_topic(self, topic):
```

### Comparing `aliyun-iot-linkkit-1.2.8/linkkit/h2client.py` & `aliyun-iot-linkkit-1.2.9/linkkit/h2client.py`

 * *Files identical despite different names*

### Comparing `aliyun-iot-linkkit-1.2.8/linksdktest/common/var.py` & `aliyun-iot-linkkit-1.2.9/linksdktest/common/var.py`

 * *Files identical despite different names*

### Comparing `aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/PKG-INFO` & `aliyun-iot-linkkit-1.2.9/aliyun_iot_linkkit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliyun-iot-linkkit
-Version: 1.2.8
+Version: 1.2.9
 Summary: Aliyun IoT Linkkit SDK for Python
 Home-page: UNKNOWN
 Author: Aliyun IoT Linkkit Python SDK
 Author-email: xicai.cxc@alibaba-inc.com
 License: UNKNOWN
 Description: #Python SDK for Aliyun IoT device
         
@@ -37,12 +37,15 @@
         
         ### 1.2.7
         * [UPDATE] add ota feature
         
         ### 1.2.8
         * [UPDATE] add mqtt dynamic-register with pre-registration feature
         
+        ### 1.2.9
+        * [UPDATE] add api to enable users to re-connect to iot platform manually in case of exceptions
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aliyun-iot-linkkit-1.2.8/README.md` & `aliyun-iot-linkkit-1.2.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -28,7 +28,10 @@
 * [UPDATE] set Endpoint parameter with default value
 
 ### 1.2.7
 * [UPDATE] add ota feature
 
 ### 1.2.8
 * [UPDATE] add mqtt dynamic-register with pre-registration feature
+
+### 1.2.9
+* [UPDATE] add api to enable users to re-connect to iot platform manually in case of exceptions
```

### Comparing `aliyun-iot-linkkit-1.2.8/setup.py` & `aliyun-iot-linkkit-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", mode='r', encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aliyun-iot-linkkit",
-    version="1.2.8",
+    version="1.2.9",
     author="Aliyun IoT Linkkit Python SDK",
     author_email="xicai.cxc@alibaba-inc.com",
     description="Aliyun IoT Linkkit SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

