# Comparing `tmp/sharktopoda-client-0.1.3.tar.gz` & `tmp/sharktopoda-client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharktopoda-client-0.1.3.tar", max compression
+gzip compressed data, was "sharktopoda-client-0.1.4.tar", max compression
```

## Comparing `sharktopoda-client-0.1.3.tar` & `sharktopoda-client-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1070 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/LICENSE
--rw-r--r--   0        0        0      411 2022-04-27 20:02:30.261641 sharktopoda-client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5499 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/ClientController.py
--rw-r--r--   0        0        0      450 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/IOBus.py
--rw-r--r--   0        0        0      487 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/JavaTypes.py
--rw-r--r--   0        0        0      339 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/Log.py
--rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/__init__.py
--rw-r--r--   0        0        0       37 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/decorators/LocalizationDecorator.py
--rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/decorators/__init__.py
--rw-r--r--   0        0        0     4232 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/localization/IO.py
--rw-r--r--   0        0        0     1867 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.3/sharktopoda_client/localization/Localization.py
--rw-r--r--   0        0        0     6373 2022-04-27 20:02:00.901532 sharktopoda-client-0.1.3/sharktopoda_client/localization/LocalizationController.py
--rw-r--r--   0        0        0      716 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/localization/Message.py
--rw-r--r--   0        0        0      128 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/localization/Preconditions.py
--rw-r--r--   0        0        0     1889 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/localization/SelectionController.py
--rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/localization/__init__.py
--rw-r--r--   0        0        0      408 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/model/ConnectCommand.py
--rw-r--r--   0        0        0      345 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/model/FrameCapture.py
--rw-r--r--   0        0        0      699 2022-03-09 18:34:36.225656 sharktopoda-client-0.1.3/sharktopoda_client/model/GenericCommand.py
--rw-r--r--   0        0        0     1543 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/model/GenericResponse.py
--rw-r--r--   0        0        0      580 2022-01-14 18:05:23.528699 sharktopoda-client-0.1.3/sharktopoda_client/model/Video.py
--rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.3/sharktopoda_client/model/__init__.py
--rw-r--r--   0        0        0     5269 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/udp/CommandService.py
--rw-r--r--   0        0        0      432 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/udp/FramecaptureUdpIO.py
--rw-r--r--   0        0        0      511 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/udp/IO.py
--rw-r--r--   0        0        0     2507 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.3/sharktopoda_client/udp/UdpIO.py
--rw-r--r--   0        0        0        0 2022-01-14 16:59:47.797072 sharktopoda-client-0.1.3/sharktopoda_client/udp/__init__.py
--rw-r--r--   0        0        0      826 2022-04-27 20:03:06.892957 sharktopoda-client-0.1.3/setup.py
--rw-r--r--   0        0        0      582 2022-04-27 20:03:06.893163 sharktopoda-client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/LICENSE
+-rw-r--r--   0        0        0      411 2022-05-10 21:12:04.464331 sharktopoda-client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5499 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/ClientController.py
+-rw-r--r--   0        0        0      450 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/IOBus.py
+-rw-r--r--   0        0        0      487 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/JavaTypes.py
+-rw-r--r--   0        0        0      339 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/Log.py
+-rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/__init__.py
+-rw-r--r--   0        0        0       37 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/decorators/LocalizationDecorator.py
+-rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/decorators/__init__.py
+-rw-r--r--   0        0        0     4232 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/localization/IO.py
+-rw-r--r--   0        0        0     1867 2022-03-10 22:42:32.640693 sharktopoda-client-0.1.4/sharktopoda_client/localization/Localization.py
+-rw-r--r--   0        0        0     5984 2022-05-10 21:11:30.336579 sharktopoda-client-0.1.4/sharktopoda_client/localization/LocalizationController.py
+-rw-r--r--   0        0        0      716 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/localization/Message.py
+-rw-r--r--   0        0        0      128 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/localization/Preconditions.py
+-rw-r--r--   0        0        0     1889 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/localization/SelectionController.py
+-rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/localization/__init__.py
+-rw-r--r--   0        0        0      408 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/model/ConnectCommand.py
+-rw-r--r--   0        0        0      345 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/model/FrameCapture.py
+-rw-r--r--   0        0        0      699 2022-03-09 18:34:36.225656 sharktopoda-client-0.1.4/sharktopoda_client/model/GenericCommand.py
+-rw-r--r--   0        0        0     1543 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/model/GenericResponse.py
+-rw-r--r--   0        0        0      580 2022-01-14 18:05:23.528699 sharktopoda-client-0.1.4/sharktopoda_client/model/Video.py
+-rw-r--r--   0        0        0        0 2022-01-14 16:59:47.793072 sharktopoda-client-0.1.4/sharktopoda_client/model/__init__.py
+-rw-r--r--   0        0        0     5269 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/udp/CommandService.py
+-rw-r--r--   0        0        0      432 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/udp/FramecaptureUdpIO.py
+-rw-r--r--   0        0        0      511 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/udp/IO.py
+-rw-r--r--   0        0        0     2507 2022-03-10 22:42:32.644693 sharktopoda-client-0.1.4/sharktopoda_client/udp/UdpIO.py
+-rw-r--r--   0        0        0        0 2022-01-14 16:59:47.797072 sharktopoda-client-0.1.4/sharktopoda_client/udp/__init__.py
+-rw-r--r--   0        0        0      826 2022-05-10 21:12:33.643319 sharktopoda-client-0.1.4/setup.py
+-rw-r--r--   0        0        0      582 2022-05-10 21:12:33.643481 sharktopoda-client-0.1.4/PKG-INFO
```

### Comparing `sharktopoda-client-0.1.3/LICENSE` & `sharktopoda-client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/ClientController.py` & `sharktopoda-client-0.1.4/sharktopoda_client/ClientController.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/localization/IO.py` & `sharktopoda-client-0.1.4/sharktopoda_client/localization/IO.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/localization/Localization.py` & `sharktopoda-client-0.1.4/sharktopoda_client/localization/Localization.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/localization/LocalizationController.py` & `sharktopoda-client-0.1.4/sharktopoda_client/localization/LocalizationController.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,18 @@
         else:
             self.log.error('Unknown message action: ' + message.action)
     
     def _on_error(self, e):
         self.log.warn('An error occurred on the incoming localization bus', e)
     
     def _add_or_replace_localizations_internal(self, localizations: List[Localization]):
+        self.log.debug('Adding/replacing ' + str(len(localizations)) + ' localizations')
         localizations = set(localizations)
         self._localizations -= localizations
         self._localizations |= localizations
-        # for localization in localizations:
-        #     self._add_or_replace_localization_internal(localization)
         
     def _add_or_replace_localization_internal(self, a: Localization):
         if a in self._localizations:
             self._localizations.remove(a)
             self.log.debug('Replacing localization (uuid = ' + str(a.localizationUuid) + ')')
         else:
             self.log.debug('Adding localization (uuid = ' + str(a.localizationUuid) + ')')
@@ -92,33 +91,24 @@
         self._incoming.on_next(msg)
         self._outgoing.on_next(msg)
 
     def _validateLocalizationForRemove(self, localization: Localization):
         Preconditions.require(localization.localizationUuid is not None, 'Can not remove a localization without a localizationUuid')
 
     def _remove_localizations_internal(self, localizations: List[Localization]):
-        for localization in localizations:
-            try:
-                self._remove_localization_internal(localization)
-            except Exception as e:
-                self.log.warn('Failed to remove a localization that was missing required values.', e)
+        self.log.debug('Removing ' + str(len(localizations)) + ' localizations')
+        self._localizations -= set(localizations)
     
     def _remove_localization_internal(self, a: Localization):
-        exists = False
-        msg = None
-        for i in range(len(self._localizations)):
-            b = self._localizations[i]
-            if b.localizationUuid == a.localizationUuid:
-                self._localizations.pop(i)
-                exists = True
-                break
-        if not exists:
+        if a not in self._localizations:
             self.log.debug('A localization with UUID of ' + a.localizationUuid + ' was not found. Unable to remove.')
-        if msg is not None:
-            self.log.debug('Removing localization (uuid = ' + a.localizationUuid + ')')
+            return
+        
+        self.log.debug('Removing localization (uuid = ' + a.localizationUuid + ')')
+        self._localizations.remove(a)
     
     def clear(self):
         msg = Message(MessageAction.ACTION_CLEAR)
         self._incoming.on_next(msg)
         self._outgoing.on_next(msg)
     
     def getLocalizations(self) -> List[Localization]:
```

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/localization/Message.py` & `sharktopoda-client-0.1.4/sharktopoda_client/localization/Message.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/localization/SelectionController.py` & `sharktopoda-client-0.1.4/sharktopoda_client/localization/SelectionController.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/model/GenericCommand.py` & `sharktopoda-client-0.1.4/sharktopoda_client/model/GenericCommand.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/model/GenericResponse.py` & `sharktopoda-client-0.1.4/sharktopoda_client/model/GenericResponse.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/model/Video.py` & `sharktopoda-client-0.1.4/sharktopoda_client/model/Video.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/udp/CommandService.py` & `sharktopoda-client-0.1.4/sharktopoda_client/udp/CommandService.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/sharktopoda_client/udp/UdpIO.py` & `sharktopoda-client-0.1.4/sharktopoda_client/udp/UdpIO.py`

 * *Files identical despite different names*

### Comparing `sharktopoda-client-0.1.3/setup.py` & `sharktopoda-client-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Rx>=3.2.0,<4.0.0', 'dataclasses-json>=0.5.4,<0.6.0', 'zmq>=0.0.0,<0.0.1']
 
 setup_kwargs = {
     'name': 'sharktopoda-client',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Sharktopoda client API, translated to Python',
     'long_description': None,
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sharktopoda-client-0.1.3/PKG-INFO` & `sharktopoda-client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharktopoda-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sharktopoda client API, translated to Python
 License: MIT
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

