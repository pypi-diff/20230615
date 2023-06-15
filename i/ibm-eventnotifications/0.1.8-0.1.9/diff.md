# Comparing `tmp/ibm-eventnotifications-0.1.8.tar.gz` & `tmp/ibm-eventnotifications-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-eventnotifications-0.1.8.tar", last modified: Wed Feb  1 08:57:51 2023, max compression
+gzip compressed data, was "dist/ibm-eventnotifications-0.1.9.tar", last modified: Wed Mar  1 06:47:03 2023, max compression
```

## Comparing `ibm-eventnotifications-0.1.8.tar` & `ibm-eventnotifications-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    24631 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    23594 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications/
--rw-rw-r--   0 travis    (2000) travis    (2000)      892 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2446 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   340379 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications/event_notifications_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24631 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-02-01 08:57:02.000000 ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-02-01 08:57:51.000000 ibm-eventnotifications-0.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2678 2023-02-01 08:56:38.000000 ibm-eventnotifications-0.1.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24608 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23571 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      892 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2446 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   341471 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications/event_notifications_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24608 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-03-01 06:46:16.000000 ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      153 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-03-01 06:47:03.000000 ibm-eventnotifications-0.1.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2678 2023-03-01 06:45:52.000000 ibm-eventnotifications-0.1.9/setup.py
```

### Comparing `ibm-eventnotifications-0.1.8/LICENSE` & `ibm-eventnotifications-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.1.8/PKG-INFO` & `ibm-eventnotifications-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-eventnotifications
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python server SDK for IBM Cloud Event Notifications service
 Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
 Author: IBM
 Author-email: Notifications-prod@ibm.com
 License: Apache 2.0
 Keywords: ibm_eventnotifications
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IBM Cloud Event Notifications Python Admin SDK 0.1.8
+# IBM Cloud Event Notifications Python Admin SDK 0.1.9
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.1.8"
+pip install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.1.8"
+easy_install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -541,44 +541,52 @@
 ```
 
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
-            'fcm_devices': ['<fcm-device-ids>'],
-            'apns_devices': ['<apns-device-ids>'],
-            'user_ids': ['<user-ids>'],
-            'tags': ['<tag-names>'],
-            'platforms': ['<device-platforms>'],
-          }
+  'fcm_devices': ['<fcm-device-ids>'],
+  'apns_devices': ['<apns-device-ids>'],
+  'user_ids': ['<user-ids>'],
+  'tags': ['<tag-names>'],
+  'platforms': ['<device-platforms>'],
+}
 
 notification_apns_body_model = {
-                "aps": {
-                    "alert": "<notification-message>",
-                    "badge": 5,
-                },
-            }
+    "aps": {
+        "alert": "<notification-message>",
+        "badge": 5,
+    },
+}
 notification_fcm_body_model = {
-                "notification": {
-                    "title": "<notification-title>",
-                    "body": "<notification-message>",
-                },
-            }
+    'message': {
+        'android': {
+            'notification': {
+                'title': '<notification-title>', 
+                'body': '<notification-message>',
+            },
+            'data': {
+                'name': 'Robert',
+                'description': 'notification for the Poker',
+            },
+        },
+    },
+}
 
 message_apns_headers = {
-                "apns-collapse-id": "<apns-apns-collapse-id-value>",
-            }
+    "apns-collapse-id": "<apns-apns-collapse-id-value>",
+}
 
 notificationSafariBodymodel = {
-            'saf': {
-                'alert': 'Game Request',
-                'badge': 5,
-            },
-        }
+    'saf': {
+        'alert': 'Game Request',
+        'badge': 5,
+    },
+}
 
 notification_id := "<notification-id>"
 notification_severity := "<notification-severity>"
 type_value := "<notification-type>"
 notifications_source := "<notification-source>"
 
 notification_create_model = {
```

### Comparing `ibm-eventnotifications-0.1.8/README.md` & `ibm-eventnotifications-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# IBM Cloud Event Notifications Python Admin SDK 0.1.8
+# IBM Cloud Event Notifications Python Admin SDK 0.1.9
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -37,19 +37,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.1.8"
+pip install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.1.8"
+easy_install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -516,44 +516,52 @@
 ```
 
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
-            'fcm_devices': ['<fcm-device-ids>'],
-            'apns_devices': ['<apns-device-ids>'],
-            'user_ids': ['<user-ids>'],
-            'tags': ['<tag-names>'],
-            'platforms': ['<device-platforms>'],
-          }
+  'fcm_devices': ['<fcm-device-ids>'],
+  'apns_devices': ['<apns-device-ids>'],
+  'user_ids': ['<user-ids>'],
+  'tags': ['<tag-names>'],
+  'platforms': ['<device-platforms>'],
+}
 
 notification_apns_body_model = {
-                "aps": {
-                    "alert": "<notification-message>",
-                    "badge": 5,
-                },
-            }
+    "aps": {
+        "alert": "<notification-message>",
+        "badge": 5,
+    },
+}
 notification_fcm_body_model = {
-                "notification": {
-                    "title": "<notification-title>",
-                    "body": "<notification-message>",
-                },
-            }
+    'message': {
+        'android': {
+            'notification': {
+                'title': '<notification-title>', 
+                'body': '<notification-message>',
+            },
+            'data': {
+                'name': 'Robert',
+                'description': 'notification for the Poker',
+            },
+        },
+    },
+}
 
 message_apns_headers = {
-                "apns-collapse-id": "<apns-apns-collapse-id-value>",
-            }
+    "apns-collapse-id": "<apns-apns-collapse-id-value>",
+}
 
 notificationSafariBodymodel = {
-            'saf': {
-                'alert': 'Game Request',
-                'badge': 5,
-            },
-        }
+    'saf': {
+        'alert': 'Game Request',
+        'badge': 5,
+    },
+}
 
 notification_id := "<notification-id>"
 notification_severity := "<notification-severity>"
 type_value := "<notification-type>"
 notifications_source := "<notification-source>"
 
 notification_create_model = {
```

### Comparing `ibm-eventnotifications-0.1.8/ibm_eventnotifications/__init__.py` & `ibm-eventnotifications-0.1.9/ibm_eventnotifications/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.1.8/ibm_eventnotifications/common.py` & `ibm-eventnotifications-0.1.9/ibm_eventnotifications/common.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.1.8/ibm_eventnotifications/event_notifications_v1.py` & `ibm-eventnotifications-0.1.9/ibm_eventnotifications/event_notifications_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1119,17 +1119,17 @@
         instance_id: str,
         id: str,
         device_id: str,
         tag_name: str,
         **kwargs
     ) -> DetailedResponse:
         """
-        Create a new Tag subscription.
+        Create a new tag subscription.
 
-        Create a new Tag subscription.
+        Create a new tag subscription.
 
         :param str instance_id: Unique identifier for IBM Cloud Event Notifications
                instance.
         :param str id: Unique identifier for Destination.
         :param str device_id: Unique identifier of the device.
         :param str tag_name: The name of the tag its subscribed.
         :param dict headers: A `dict` containing the request headers
@@ -1186,17 +1186,17 @@
         tag_name: str = None,
         limit: int = None,
         offset: int = None,
         search: str = None,
         **kwargs
     ) -> DetailedResponse:
         """
-        List all Tag Subscriptions.
+        List all tag subscriptions.
 
-        List all Tag Subscriptions.
+        List all tag subscriptions.
 
         :param str instance_id: Unique identifier for IBM Cloud Event Notifications
                instance.
         :param str id: Unique identifier for Destination.
         :param str device_id: (optional) Device ID of the destination
                tagsubscription.
         :param str user_id: (optional) UserID of the destination.
@@ -1251,17 +1251,17 @@
         id: str,
         *,
         device_id: str = None,
         tag_name: str = None,
         **kwargs
     ) -> DetailedResponse:
         """
-        Delete a Tag subcription.
+        Delete a tag subscription.
 
-        Delete a Tag subcription.
+        Delete a tag subscription.
 
         :param str instance_id: Unique identifier for IBM Cloud Event Notifications
                instance.
         :param str id: Unique identifier for Destination.
         :param str device_id: (optional) Device ID of the destination
                tagsubscription.
         :param str tag_name: (optional) TagName of the subscription.
@@ -5740,52 +5740,67 @@
 
     def __ne__(self, other: 'DestinationConfigOneOfChromeDestinationConfig') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 class DestinationConfigOneOfFCMDestinationConfig(DestinationConfigOneOf):
     """
-    Payload describing an FCM destination configuration.
+    Payload describing an FCM destination configuration. project_id, private_key and
+    client_email for FCM HTTP v1 APIs.
 
-    :attr str server_key: FCM server_key.
-    :attr str sender_id: FCM sender_id.
+    :attr str server_key: (optional) FCM server_key.
+    :attr str sender_id: (optional) FCM sender_id.
     :attr bool pre_prod: (optional) If pre prod enabled.
+    :attr str project_id: (optional) FCM project_id.
+    :attr str private_key: (optional) FCM private_key.
+    :attr str client_email: (optional) FCM client_email.
     """
 
     def __init__(self,
-                 server_key: str,
-                 sender_id: str,
                  *,
-                 pre_prod: bool = None) -> None:
+                 server_key: str = None,
+                 sender_id: str = None,
+                 pre_prod: bool = None,
+                 project_id: str = None,
+                 private_key: str = None,
+                 client_email: str = None) -> None:
         """
         Initialize a DestinationConfigOneOfFCMDestinationConfig object.
 
-        :param str server_key: FCM server_key.
-        :param str sender_id: FCM sender_id.
+        :param str server_key: (optional) FCM server_key.
+        :param str sender_id: (optional) FCM sender_id.
         :param bool pre_prod: (optional) If pre prod enabled.
+        :param str project_id: (optional) FCM project_id.
+        :param str private_key: (optional) FCM private_key.
+        :param str client_email: (optional) FCM client_email.
         """
         # pylint: disable=super-init-not-called
         self.server_key = server_key
         self.sender_id = sender_id
         self.pre_prod = pre_prod
+        self.project_id = project_id
+        self.private_key = private_key
+        self.client_email = client_email
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'DestinationConfigOneOfFCMDestinationConfig':
         """Initialize a DestinationConfigOneOfFCMDestinationConfig object from a json dictionary."""
         args = {}
         if 'server_key' in _dict:
             args['server_key'] = _dict.get('server_key')
-        else:
-            raise ValueError('Required property \'server_key\' not present in DestinationConfigOneOfFCMDestinationConfig JSON')
         if 'sender_id' in _dict:
             args['sender_id'] = _dict.get('sender_id')
-        else:
-            raise ValueError('Required property \'sender_id\' not present in DestinationConfigOneOfFCMDestinationConfig JSON')
         if 'pre_prod' in _dict:
             args['pre_prod'] = _dict.get('pre_prod')
+        if 'project_id' in _dict:
+            args['project_id'] = _dict.get('project_id')
+        if 'private_key' in _dict:
+            args['private_key'] = _dict.get('private_key')
+        if 'client_email' in _dict:
+            args['client_email'] = _dict.get('client_email')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a DestinationConfigOneOfFCMDestinationConfig object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5794,14 +5809,20 @@
         _dict = {}
         if hasattr(self, 'server_key') and self.server_key is not None:
             _dict['server_key'] = self.server_key
         if hasattr(self, 'sender_id') and self.sender_id is not None:
             _dict['sender_id'] = self.sender_id
         if hasattr(self, 'pre_prod') and self.pre_prod is not None:
             _dict['pre_prod'] = self.pre_prod
+        if hasattr(self, 'project_id') and self.project_id is not None:
+            _dict['project_id'] = self.project_id
+        if hasattr(self, 'private_key') and self.private_key is not None:
+            _dict['private_key'] = self.private_key
+        if hasattr(self, 'client_email') and self.client_email is not None:
+            _dict['client_email'] = self.client_email
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
```

### Comparing `ibm-eventnotifications-0.1.8/ibm_eventnotifications/version.py` & `ibm-eventnotifications-0.1.9/ibm_eventnotifications/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_eventnotifications
 """
-__version__ = '0.1.8'
+__version__ = '0.1.9'
```

### Comparing `ibm-eventnotifications-0.1.8/ibm_eventnotifications.egg-info/PKG-INFO` & `ibm-eventnotifications-0.1.9/ibm_eventnotifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-eventnotifications
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python server SDK for IBM Cloud Event Notifications service
 Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
 Author: IBM
 Author-email: Notifications-prod@ibm.com
 License: Apache 2.0
 Keywords: ibm_eventnotifications
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IBM Cloud Event Notifications Python Admin SDK 0.1.8
+# IBM Cloud Event Notifications Python Admin SDK 0.1.9
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.1.8"
+pip install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.1.8"
+easy_install --upgrade "ibm_eventnotifications>=0.1.9"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -541,44 +541,52 @@
 ```
 
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
-            'fcm_devices': ['<fcm-device-ids>'],
-            'apns_devices': ['<apns-device-ids>'],
-            'user_ids': ['<user-ids>'],
-            'tags': ['<tag-names>'],
-            'platforms': ['<device-platforms>'],
-          }
+  'fcm_devices': ['<fcm-device-ids>'],
+  'apns_devices': ['<apns-device-ids>'],
+  'user_ids': ['<user-ids>'],
+  'tags': ['<tag-names>'],
+  'platforms': ['<device-platforms>'],
+}
 
 notification_apns_body_model = {
-                "aps": {
-                    "alert": "<notification-message>",
-                    "badge": 5,
-                },
-            }
+    "aps": {
+        "alert": "<notification-message>",
+        "badge": 5,
+    },
+}
 notification_fcm_body_model = {
-                "notification": {
-                    "title": "<notification-title>",
-                    "body": "<notification-message>",
-                },
-            }
+    'message': {
+        'android': {
+            'notification': {
+                'title': '<notification-title>', 
+                'body': '<notification-message>',
+            },
+            'data': {
+                'name': 'Robert',
+                'description': 'notification for the Poker',
+            },
+        },
+    },
+}
 
 message_apns_headers = {
-                "apns-collapse-id": "<apns-apns-collapse-id-value>",
-            }
+    "apns-collapse-id": "<apns-apns-collapse-id-value>",
+}
 
 notificationSafariBodymodel = {
-            'saf': {
-                'alert': 'Game Request',
-                'badge': 5,
-            },
-        }
+    'saf': {
+        'alert': 'Game Request',
+        'badge': 5,
+    },
+}
 
 notification_id := "<notification-id>"
 notification_severity := "<notification-severity>"
 type_value := "<notification-type>"
 notifications_source := "<notification-source>"
 
 notification_create_model = {
```

### Comparing `ibm-eventnotifications-0.1.8/setup.py` & `ibm-eventnotifications-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 PACKAGE_NAME = 'ibm_eventnotifications'
 PACKAGE_DESC = 'Python server SDK for IBM Cloud Event Notifications service'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

