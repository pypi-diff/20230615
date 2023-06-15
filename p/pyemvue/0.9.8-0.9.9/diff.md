# Comparing `tmp/pyemvue-0.9.8.tar.gz` & `tmp/pyemvue-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyemvue-0.9.8.tar", last modified: Mon Jun 22 02:32:58 2020, max compression
+gzip compressed data, was "dist\pyemvue-0.9.9.tar", last modified: Fri Jul 10 02:06:02 2020, max compression
```

## Comparing `pyemvue-0.9.8.tar` & `pyemvue-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-06-22 02:32:58.704212 pyemvue-0.9.8/
--rw-rw-rw-   0        0        0     8104 2020-06-22 02:32:58.700210 pyemvue-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-06-22 02:32:58.674240 pyemvue-0.9.8/pyemvue/
--rw-rw-rw-   0        0        0       37 2020-03-12 23:12:19.000000 pyemvue-0.9.8/pyemvue/__init__.py
--rw-rw-rw-   0        0        0     3159 2020-06-21 23:25:28.000000 pyemvue-0.9.8/pyemvue/__main__.py
--rw-rw-rw-   0        0        0      789 2020-03-12 21:54:16.000000 pyemvue-0.9.8/pyemvue/customer.py
--rw-rw-rw-   0        0        0     4257 2020-06-05 00:00:08.000000 pyemvue-0.9.8/pyemvue/device.py
--rw-rw-rw-   0        0        0      558 2020-03-12 21:47:57.000000 pyemvue-0.9.8/pyemvue/enums.py
--rw-rw-rw-   0        0        0     8108 2020-06-21 23:22:28.000000 pyemvue-0.9.8/pyemvue/pyemvue.py
-drwxrwxrwx   0        0        0        0 2020-06-22 02:32:58.699208 pyemvue-0.9.8/pyemvue.egg-info/
--rw-rw-rw-   0        0        0     8104 2020-06-22 02:32:58.000000 pyemvue-0.9.8/pyemvue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2020-06-22 02:32:58.000000 pyemvue-0.9.8/pyemvue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-22 02:32:58.000000 pyemvue-0.9.8/pyemvue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2020-06-22 02:32:58.000000 pyemvue-0.9.8/pyemvue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-06-22 02:32:58.000000 pyemvue-0.9.8/pyemvue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-22 02:32:58.704212 pyemvue-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      786 2020-06-21 22:49:40.000000 pyemvue-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-10 02:06:02.581041 pyemvue-0.9.9/
+-rw-rw-rw-   0        0        0     8115 2020-07-10 02:06:02.579041 pyemvue-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2020-07-10 02:06:02.546041 pyemvue-0.9.9/pyemvue/
+-rw-rw-rw-   0        0        0       37 2020-03-12 23:12:19.000000 pyemvue-0.9.9/pyemvue/__init__.py
+-rw-rw-rw-   0        0        0     3465 2020-07-10 02:02:38.000000 pyemvue-0.9.9/pyemvue/__main__.py
+-rw-rw-rw-   0        0        0      789 2020-03-12 21:54:16.000000 pyemvue-0.9.9/pyemvue/customer.py
+-rw-rw-rw-   0        0        0     4257 2020-06-05 00:00:08.000000 pyemvue-0.9.9/pyemvue/device.py
+-rw-rw-rw-   0        0        0      558 2020-03-12 21:47:57.000000 pyemvue-0.9.9/pyemvue/enums.py
+-rw-rw-rw-   0        0        0     8056 2020-07-10 02:00:19.000000 pyemvue-0.9.9/pyemvue/pyemvue.py
+drwxrwxrwx   0        0        0        0 2020-07-10 02:06:02.578040 pyemvue-0.9.9/pyemvue.egg-info/
+-rw-rw-rw-   0        0        0     8115 2020-07-10 02:06:02.000000 pyemvue-0.9.9/pyemvue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2020-07-10 02:06:02.000000 pyemvue-0.9.9/pyemvue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-10 02:06:02.000000 pyemvue-0.9.9/pyemvue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2020-07-10 02:06:02.000000 pyemvue-0.9.9/pyemvue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2020-07-10 02:06:02.000000 pyemvue-0.9.9/pyemvue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-07-10 02:06:02.581041 pyemvue-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      816 2020-07-10 02:04:41.000000 pyemvue-0.9.9/setup.py
```

### Comparing `pyemvue-0.9.8/PKG-INFO` & `pyemvue-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyemvue
-Version: 0.9.8
-Summary: Library for interacting with the Emporia Vue energy monitor.
+Version: 0.9.9
+Summary: Unofficial library for interacting with the Emporia Vue energy monitor.
 Home-page: https://github.com/magico13/PyEmVue
 Author: magico13
 License: UNKNOWN
 Description: # PyEmVue
         
         A Python Library for reading data from the Emporia Vue energy monitoring system.
```

### Comparing `pyemvue-0.9.8/pyemvue/__main__.py` & `pyemvue-0.9.9/pyemvue/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import datetime
 import json
+import dateutil
 
 # Our files
 from pyemvue.enums import Scale, Unit, TotalTimeFrame, TotalUnit
 from pyemvue.customer import Customer
 from pyemvue.device import VueDevice, VueDeviceChannel, VuewDeviceChannelUsage
 from pyemvue.pyemvue import PyEmVue
 
@@ -49,26 +50,31 @@
     vue.login(email, passw, idToken, accessToken, refreshToken, token_storage_file='keys.json')
     print('Logged in. Authtoken follows:')
     print(vue.cognito.id_token)
     print()
     devices = vue.get_devices()
     for device in devices:
         print(device.device_gid, device.manufacturer_id, device.model, device.firmware)
+        vue.populate_device_properties(device)
         for chan in device.channels:
             print('\t', chan.device_gid, chan.name, chan.channel_num, chan.channel_multiplier)
     print(vue.get_total_usage(devices[0].channels[0], TotalTimeFrame.MONTH.value) / 1000, 'kwh used month to date')
     print(vue.get_total_usage(devices[0].channels[0], TotalTimeFrame.ALL.value) / 1000, 'kwh used total')
     now = datetime.datetime.utcnow()
+    yesterday = datetime.datetime.now(dateutil.tz.gettz(devices[0].time_zone))
+    yesterday = yesterday.replace(hour=23, minute=59, second=59) - datetime.timedelta(days=1)
+    yesterday = yesterday.astimezone(dateutil.tz.UTC).replace(tzinfo=None)
+    print(yesterday.isoformat())
     minAgo = now - datetime.timedelta(minutes=1)
     print('Total usage for today in kwh: ')
     use = vue.get_recent_usage(Scale.DAY.value)
     for chan in use:
         print(f'{chan.device_gid} ({chan.channel_num}): {chan.usage/1000} kwh')
     print('Total usage for yesterday in kwh: ')
-    use, realStart, realEnd = vue.get_usage_for_time_scale(datetime.datetime.utcnow()-datetime.timedelta(days=1), Scale.DAY.value)
+    use, realStart, realEnd = vue.get_usage_for_time_scale(yesterday, Scale.DAY.value)
     print(f'Time range: {realStart} to {realEnd}')
     for chan in use:
         print(f'{chan.device_gid} ({chan.channel_num}): {chan.usage/1000} kwh')
     print('Average usage over the last minute in watts: ')
     use = vue.get_recent_usage(Scale.MINUTE.value)
     for chan in use:
         print(f'{chan.device_gid} ({chan.channel_num}): {chan.usage} W')
```

### Comparing `pyemvue-0.9.8/pyemvue/customer.py` & `pyemvue-0.9.9/pyemvue/customer.py`

 * *Files identical despite different names*

### Comparing `pyemvue-0.9.8/pyemvue/device.py` & `pyemvue-0.9.9/pyemvue/device.py`

 * *Files identical despite different names*

### Comparing `pyemvue-0.9.8/pyemvue/enums.py` & `pyemvue-0.9.9/pyemvue/enums.py`

 * *Files identical despite different names*

### Comparing `pyemvue-0.9.8/pyemvue/pyemvue.py` & `pyemvue-0.9.9/pyemvue/pyemvue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import datetime
 import json
+from dateutil.parser import parse
 
 # These provide AWS cognito authentication support
 import boto3
 import botocore
 from warrant import Cognito
 
 # Our files
@@ -103,17 +104,17 @@
         response.raise_for_status()
         channels = []
         realStart = None
         realEnd = None
         if response.text:
             j = response.json()
             if 'start' in j: 
-                realStart = datetime.datetime.strptime(j['start'], '%Y-%m-%dT%H:%M:%SZ')
+                realStart = parse(j['start'])
             if 'end' in j: 
-                realEnd = datetime.datetime.strptime(j['end'], '%Y-%m-%dT%H:%M:%SZ')
+                realEnd = parse(j['end'])
             if 'channels' in j:
                 for channel in j['channels']:
                     channels.append(VuewDeviceChannelUsage().from_json_dictionary(channel))
         return channels, realStart, realEnd
 
 
     def login(self, username=None, password=None, id_token=None, access_token=None, refresh_token=None, token_storage_file=None):
```

### Comparing `pyemvue-0.9.8/pyemvue.egg-info/PKG-INFO` & `pyemvue-0.9.9/pyemvue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyemvue
-Version: 0.9.8
-Summary: Library for interacting with the Emporia Vue energy monitor.
+Version: 0.9.9
+Summary: Unofficial library for interacting with the Emporia Vue energy monitor.
 Home-page: https://github.com/magico13/PyEmVue
 Author: magico13
 License: UNKNOWN
 Description: # PyEmVue
         
         A Python Library for reading data from the Emporia Vue energy monitoring system.
```

### Comparing `pyemvue-0.9.8/setup.py` & `pyemvue-0.9.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except:
     long_description = ""
     
 setuptools.setup(
     name="pyemvue",
-    version="0.9.8",
+    version="0.9.9",
     author="magico13",
-    description="Library for interacting with the Emporia Vue energy monitor.",
+    description="Unofficial library for interacting with the Emporia Vue energy monitor.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/magico13/PyEmVue",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
 
     ],
     python_requires='>=2.7',
-    install_requires=['warrant', 'requests'],
+    install_requires=['warrant', 'requests', 'python-dateutil'],
 )
```

