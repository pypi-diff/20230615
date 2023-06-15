# Comparing `tmp/foxglove-data-platform-0.8.0.tar.gz` & `tmp/foxglove-data-platform-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.8.0.tar", last modified: Mon Jun 12 20:23:11 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.8.1.tar", last modified: Thu Jun 15 16:46:42 2023, max compression
```

## Comparing `foxglove-data-platform-0.8.0.tar` & `foxglove-data-platform-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.171754 foxglove-data-platform-0.8.0/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29399 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.171754 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 20:23:11.000000 foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:11.175753 foxglove-data-platform-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 20:22:08.000000 foxglove-data-platform-0.8.0/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.623011 foxglove-data-platform-0.8.1/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.623011 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.8.0/LICENSE` & `foxglove-data-platform-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/PKG-INFO` & `foxglove-data-platform-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.8.0/README.md` & `foxglove-data-platform-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/foxglove_data_platform/client.py` & `foxglove-data-platform-0.8.1/foxglove_data_platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,24 +193,25 @@
         """
         if end is None:
             end = start
         if device_id is None and device_name is None:
             raise RuntimeError(
                 "device_id or device_name must be provided to create_event"
             )
+        params = {
+            "device.id": device_id,
+            "device.name": device_name,
+            "start": start.astimezone().isoformat(),
+            "end": end.astimezone().isoformat(),
+            "metadata": metadata,
+        }
         response = requests.post(
             self.__url__("/v1/events"),
             headers=self.__headers,
-            json={
-                "device.id": device_id,
-                "device.name": device_name,
-                "start": start.astimezone().isoformat(),
-                "end": end.astimezone().isoformat(),
-                "metadata": metadata,
-            },
+            json={k: v for k, v in params.items() if v is not None},
         )
 
         return _event_dict(json_or_raise(response))
 
     def delete_event(
         self,
         *,
@@ -813,22 +814,23 @@
         device_id: Device id of the device from which this data originated.
         device_name: Name id of the device from which this data originated.
         filename: A filename to associate with the data. The data format will be
             inferred from the file extension.
         data: The raw data in .bag or .mcap format.
         callback: An optional callback to report progress on the upload.
         """
+        params = {
+            "device.id": device_id,
+            "device.name": device_name,
+            "filename": filename,
+        }
         link_response = requests.post(
             self.__url__("/v1/data/upload"),
             headers=self.__headers,
-            json={
-                "device.id": device_id,
-                "device.name": device_name,
-                "filename": filename,
-            },
+            json={k: v for k, v in params.items() if v is not None},
         )
 
         json = json_or_raise(link_response)
 
         link = json["link"]
         buffer = ProgressBufferReader(data, callback=callback)
         upload_request = requests.put(
```

### Comparing `foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.8.0
+Version: 0.8.1
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.8.0/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/setup.cfg` & `foxglove-data-platform-0.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.8.0
+version = 0.8.1
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-data-platform-0.8.0/tests/generate.py` & `foxglove-data-platform-0.8.1/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/string_message_pb2.py` & `foxglove-data-platform-0.8.1/tests/string_message_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_attachments.py` & `foxglove-data-platform-0.8.1/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_client.py` & `foxglove-data-platform-0.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_coverage.py` & `foxglove-data-platform-0.8.1/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_data.py` & `foxglove-data-platform-0.8.1/tests/test_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from tempfile import TemporaryFile
 
 import responses
 from faker import Faker
 from foxglove_data_platform.client import Client
+from responses.matchers import json_params_matcher
 
 from .api_url import api_url
 
 fake = Faker()
 
 
 @responses.activate
@@ -53,21 +54,31 @@
     )
     assert upload_response["link"] == upload_link
 
 
 @responses.activate
 def test_upload():
     upload_link = fake.url()
+    device_id = "test_device_id"
+    filename = "test_file.mcap"
     responses.add(
         responses.POST,
         api_url("/v1/data/upload"),
+        match=[
+            json_params_matcher(
+                {
+                    "device.id": device_id,
+                    "filename": filename,
+                },
+            )
+        ],
         json={
             "link": upload_link,
         },
     )
     responses.add(responses.PUT, upload_link)
     client = Client("test")
     data = fake.binary(4096)
     upload_response = client.upload_data(
-        device_id="test_device_id", filename="test_file.mcap", data=data
+        device_id=device_id, filename=filename, data=data
     )
     assert upload_response["link"] == upload_link
```

### Comparing `foxglove-data-platform-0.8.0/tests/test_devices.py` & `foxglove-data-platform-0.8.1/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_events.py` & `foxglove-data-platform-0.8.1/tests/test_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import datetime
 
 import responses
 from faker import Faker
 from foxglove_data_platform.client import Client
+from responses.matchers import json_params_matcher
 
 from .api_url import api_url
 
 fake = Faker()
 
 
 @responses.activate
@@ -17,14 +18,24 @@
     device_name = fake.name()
     start = datetime.datetime.now().astimezone()
     end = start + datetime.timedelta(seconds=10)
     now = datetime.datetime.now().astimezone()
     responses.add(
         responses.POST,
         api_url("/v1/events"),
+        match=[
+            json_params_matcher(
+                {
+                    "device.id": device_id,
+                    "start": start.astimezone().isoformat(),
+                    "end": end.astimezone().isoformat(),
+                    "metadata": {},
+                },
+            )
+        ],
         json={
             "id": id,
             "deviceId": device_id,
             "device": {"id": device_id, "name": device_name},
             "start": start.astimezone().isoformat(),
             "end": end.astimezone().isoformat(),
             "metadata": {"foo": "bar"},
```

### Comparing `foxglove-data-platform-0.8.0/tests/test_imports.py` & `foxglove-data-platform-0.8.1/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.8.1/tests/test_protobuf_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_recordings.py` & `foxglove-data-platform-0.8.1/tests/test_recordings.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_ros1_messages.py` & `foxglove-data-platform-0.8.1/tests/test_ros1_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.0/tests/test_ros2_messages.py` & `foxglove-data-platform-0.8.1/tests/test_ros2_messages.py`

 * *Files identical despite different names*

