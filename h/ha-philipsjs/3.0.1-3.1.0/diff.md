# Comparing `tmp/ha-philipsjs-3.0.1.tar.gz` & `tmp/ha-philipsjs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-philipsjs-3.0.1.tar", last modified: Fri Feb 17 18:45:11 2023, max compression
+gzip compressed data, was "ha-philipsjs-3.1.0.tar", last modified: Wed Jun 14 22:06:05 2023, max compression
```

## Comparing `ha-philipsjs-3.0.1.tar` & `ha-philipsjs-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-02-17 18:45:11.001122 ha-philipsjs-3.0.1/
--rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.0.1/LICENSE
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-02-17 18:45:11.001230 ha-philipsjs-3.0.1/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)     1479 2021-05-14 12:35:57.000000 ha-philipsjs-3.0.1/README.md
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-02-17 18:45:10.997859 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/
--rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-02-17 18:45:10.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/PKG-INFO
--rw-r--r--   0 joakim     (501) staff       (20)      469 2023-02-17 18:45:10.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/SOURCES.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2023-02-17 18:45:10.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/dependency_links.txt
--rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/not-zip-safe
--rw-r--r--   0 joakim     (501) staff       (20)      123 2023-02-17 18:45:10.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/requires.txt
--rw-r--r--   0 joakim     (501) staff       (20)       12 2023-02-17 18:45:10.000000 ha-philipsjs-3.0.1/ha_philipsjs.egg-info/top_level.txt
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-02-17 18:45:10.998689 ha-philipsjs-3.0.1/haphilipsjs/
--rw-r--r--   0 joakim     (501) staff       (20)    50886 2023-02-17 18:44:47.000000 ha-philipsjs-3.0.1/haphilipsjs/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)    11393 2023-01-23 23:00:50.000000 ha-philipsjs-3.0.1/haphilipsjs/__main__.py
--rw-r--r--   0 joakim     (501) staff       (20)     7379 2022-10-15 15:42:29.000000 ha-philipsjs-3.0.1/haphilipsjs/auth.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-02-17 18:45:10.999404 ha-philipsjs-3.0.1/haphilipsjs/data/
--rw-r--r--   0 joakim     (501) staff       (20)       20 2021-04-15 20:10:56.000000 ha-philipsjs-3.0.1/haphilipsjs/data/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     6598 2022-03-03 14:18:45.000000 ha-philipsjs-3.0.1/haphilipsjs/data/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)   422994 2023-01-23 23:00:50.000000 ha-philipsjs-3.0.1/haphilipsjs/data/v6.py
-drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-02-17 18:45:11.000930 ha-philipsjs-3.0.1/haphilipsjs/dummy/
--rw-r--r--   0 joakim     (501) staff       (20)       18 2021-04-15 20:10:56.000000 ha-philipsjs-3.0.1/haphilipsjs/dummy/__init__.py
--rw-r--r--   0 joakim     (501) staff       (20)     1588 2021-04-15 20:10:56.000000 ha-philipsjs-3.0.1/haphilipsjs/dummy/v1.py
--rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-02-17 18:44:47.000000 ha-philipsjs-3.0.1/haphilipsjs/typing.py
--rw-r--r--   0 joakim     (501) staff       (20)      132 2023-02-17 18:45:11.001572 ha-philipsjs-3.0.1/setup.cfg
--rw-r--r--   0 joakim     (501) staff       (20)     1550 2023-02-17 18:44:47.000000 ha-philipsjs-3.0.1/setup.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.402359 ha-philipsjs-3.1.0/
+-rw-r--r--   0 joakim     (501) staff       (20)     1069 2018-09-06 12:45:31.000000 ha-philipsjs-3.1.0/LICENSE
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-06-14 22:06:05.402493 ha-philipsjs-3.1.0/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)     1479 2021-05-14 12:35:57.000000 ha-philipsjs-3.1.0/README.md
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.399322 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/
+-rw-r--r--   0 joakim     (501) staff       (20)     2124 2023-06-14 22:06:05.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/PKG-INFO
+-rw-r--r--   0 joakim     (501) staff       (20)      503 2023-06-14 22:06:05.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/SOURCES.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2023-06-14 22:06:05.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/dependency_links.txt
+-rw-r--r--   0 joakim     (501) staff       (20)        1 2018-09-06 12:45:43.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/not-zip-safe
+-rw-r--r--   0 joakim     (501) staff       (20)      123 2023-06-14 22:06:05.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/requires.txt
+-rw-r--r--   0 joakim     (501) staff       (20)       12 2023-06-14 22:06:05.000000 ha-philipsjs-3.1.0/ha_philipsjs.egg-info/top_level.txt
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.400234 ha-philipsjs-3.1.0/haphilipsjs/
+-rw-r--r--   0 joakim     (501) staff       (20)    51418 2023-06-14 22:05:19.000000 ha-philipsjs-3.1.0/haphilipsjs/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)    11393 2023-01-23 23:00:50.000000 ha-philipsjs-3.1.0/haphilipsjs/__main__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     7379 2022-10-15 15:42:29.000000 ha-philipsjs-3.1.0/haphilipsjs/auth.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.400841 ha-philipsjs-3.1.0/haphilipsjs/data/
+-rw-r--r--   0 joakim     (501) staff       (20)       20 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.0/haphilipsjs/data/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     6598 2022-03-03 14:18:45.000000 ha-philipsjs-3.1.0/haphilipsjs/data/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)   428050 2023-06-14 22:05:19.000000 ha-philipsjs-3.1.0/haphilipsjs/data/v6.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.401724 ha-philipsjs-3.1.0/haphilipsjs/dummy/
+-rw-r--r--   0 joakim     (501) staff       (20)       18 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.0/haphilipsjs/dummy/__init__.py
+-rw-r--r--   0 joakim     (501) staff       (20)     1588 2021-04-15 20:10:56.000000 ha-philipsjs-3.1.0/haphilipsjs/dummy/v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)     9389 2023-02-17 18:44:47.000000 ha-philipsjs-3.1.0/haphilipsjs/typing.py
+-rw-r--r--   0 joakim     (501) staff       (20)      132 2023-06-14 22:06:05.402758 ha-philipsjs-3.1.0/setup.cfg
+-rw-r--r--   0 joakim     (501) staff       (20)     1550 2023-06-14 22:05:19.000000 ha-philipsjs-3.1.0/setup.py
+drwxr-xr-x   0 joakim     (501) staff       (20)        0 2023-06-14 22:06:05.402206 ha-philipsjs-3.1.0/tests/
+-rw-r--r--   0 joakim     (501) staff       (20)    10142 2023-01-23 23:01:01.000000 ha-philipsjs-3.1.0/tests/test_v1.py
+-rw-r--r--   0 joakim     (501) staff       (20)    20459 2023-06-14 22:05:19.000000 ha-philipsjs-3.1.0/tests/test_v6.py
```

### Comparing `ha-philipsjs-3.0.1/LICENSE` & `ha-philipsjs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/PKG-INFO` & `ha-philipsjs-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.0.1
+Version: 3.1.0
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.0.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.1.0
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.0.1/README.md` & `ha-philipsjs-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/ha_philipsjs.egg-info/PKG-INFO` & `ha-philipsjs-3.1.0/ha_philipsjs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ha-philipsjs
-Version: 3.0.1
+Version: 3.1.0
 Summary: jointSPACE API for Home-Assistant
 Home-page: https://github.com/danielperna84/ha-philipsjs
-Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.0.1
+Download-URL: https://github.com/danielperna84/ha-philipsjs/tarball/3.1.0
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
 Keywords: jointSPACE
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/__init__.py` & `ha-philipsjs-3.1.0/haphilipsjs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,25 +552,24 @@
     async def aclose(self) -> None:
         await self.session.aclose()
 
     def _url(self, path, protocol = None):
         if protocol is None:
             protocol = self.protocol
 
-        if self.protocol == "https":
+        if protocol == "https":
             port = HTTPS_PORT
         else:
             port = HTTP_PORT
 
         return f"{protocol}://{self._host}:{port}/{self.api_version}/{path}"
 
-    async def getReq(self, path) -> Optional[Dict]:
-
+    async def getReq(self, path, protocol = None) -> Optional[Dict]:
         try:
-            resp = await self.session.get(self._url(path))
+            resp = await self.session.get(self._url(path, protocol = protocol))
             if resp.status_code == 401:
                 raise AutenticationFailure("Authenticaion failed to device")
 
             if resp.status_code != 200:
                 LOG.debug("Get failed: %s -> %d %s", path, resp.status_code, resp.text)
                 return None
 
@@ -725,14 +724,15 @@
             await self.getApplication()
             await self.getContext()
             await self.getScreenState()
             await self.getAmbilightMode()
             await self.getAmbilightPower()
             await self.getAmbilightCurrentConfiguration()
             await self.getHueLampPower()
+            await self.getRecordings()
             self.on = True
             return True
         except ConnectionFailure as err:
             LOG.debug("TV not available: %s", repr(err))
             self.on = False
             return False
 
@@ -742,21 +742,29 @@
             if key.endswith("_encrypted"):
                 result[key[:-10]] = cbc_decode(self.auth_shared_key, value)
             else:
                 result[key] = value
         return cast(SystemType, result)
 
     async def getSystem(self):
-        r = cast(Optional[SystemType], await self.getReq("system"))
-        if r:
-            self.system = self._decodeSystem(r)
-            self.name = r.get("name")
-        else:
-            self.system = {}
-            self.name = None
+        # Newest TV software requires https for system-info. Therefore we will try both protocols.
+        protocols = ["http", "https"]
+
+        if protocols[0] != self.protocol:
+            protocols = reversed(protocols)
+        
+        for prot in protocols:
+            r = cast(Optional[SystemType], await self.getReq("system", protocol=prot))
+            if r:
+                self.system = self._decodeSystem(r)
+                self.name = r.get("name")
+                return r
+            else:
+                self.system = {}
+                self.name = None
         return r
 
     async def getAudiodata(self):
         r = await self.getReq("audio/volume")
         if r:
             self.audio_volume = r
         else:
@@ -1282,24 +1290,26 @@
 
             if self.quirk_ambilight_mode_ignored:
                 self.ambilight_mode_set = None
 
             return True
 
     async def getRecordings(self):
-        if self.json_feature_supported("recordings", "List"):
-            r = cast(
-                Optional[RecordingsListed],
-                await self.getReq("recordings/list"),
-            )
-            if r:
-                self.recordings_list = r
-            else:
-                self.recordings_list = None
-            return r
+        #Just known working with API level 6 currently
+        if self.api_version == 6:
+            if self.json_feature_supported("recordings", "List"):
+                r = cast(
+                    Optional[RecordingsListed],
+                    await self.getReq("recordings/list"),
+                )
+                if r:
+                    self.recordings_list = r
+                else:
+                    self.recordings_list = None
+                return r
 
     async def openURL(self, url: str):
         if self.json_feature_supported("activities", "browser"):
             r = await self.postReq("activities/browser", {"url": url})
             return r is not None
 
     async def getStringsCached(self, string_ids: Iterable[str]) -> Union[Dict[str, str], None]:
```

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/__main__.py` & `ha-philipsjs-3.1.0/haphilipsjs/__main__.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/auth.py` & `ha-philipsjs-3.1.0/haphilipsjs/auth.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/data/v1.py` & `ha-philipsjs-3.1.0/haphilipsjs/data/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/data/v6.py` & `ha-philipsjs-3.1.0/haphilipsjs/data/v6.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     FavoriteListType,
     MenuItemsSettingsCurrent,
     MenuItemsSettingsCurrentPost,
     MenuItemsSettingsNode,
     MenuItemsSettingsStructure,
     MenuItemsSettingsUpdate,
     SystemType,
+    RecordingsListed,
 )
 
 
 SYSTEM_ANDROID: SystemType = {
     "notifyChange": "http",
     "menulanguage": "Swedish",
     "name": "65OLED855/12",
@@ -9904,8 +9905,134 @@
 
 MENUITEMS_SETTINGS_CURRENT_POST: MenuItemsSettingsCurrentPost = {
     "nodes": [
         {
             "nodeid": 420
         }
     ]
+}
+
+RECORDINGS_LIST: RecordingsListed = {
+    "version": "253.91",
+    "recordings": [
+        {
+            "RecordingId": 36,
+            "RecordingType": "RECORDING_ONGOING",
+            "IsIpEpgRec": False,
+            "ccid": 2091,
+            "StartTime": 1676833531,
+            "Duration": 569,
+            "MarginStart": 0,
+            "MarginEnd": 0,
+            "EventId": 47369,
+            "EITVersion": 0,
+            "RetentionInfo": 0,
+            "EventInfo": "Eisige Welten II - Planet der Extreme\nDeutschland 2023\nIm Fokus dieser Folge stehen die besonderen Anpassungsstrategien der Bewohner an die Veränderungen in den klimatisch herausfordernden Lebensräumen.\n\nDie Reise beginnt auf dem gefrorenen Kontinent der Antarktis im äußersten Süden, dem lebensfeindlichsten Ort der Erde. Nachdem sie im Winter auf dem Eis aufgewachsen sind, werden die Kaiserpinguinküken im Frühjahr von ihren Eltern verlassen.\nHD-Produktion",
+            "EventExtendedInfo": "",
+            "EventGenre": "8",
+            "RecName": "Terra X",
+            "SeriesID": "None",
+            "SeasonNo": 0,
+            "EpisodeNo": 0,
+            "EpisodeCount": 72300,
+            "ProgramNumber": 11110,
+            "EventRating": 0,
+            "hasDot": True,
+            "isFTARecording": False,
+            "LastPinChangedTime": 0,
+            "Version": 344,
+            "HasCicamPin": False,
+            "HasLicenseFile": False,
+            "Size": 0,
+            "ResumeInfo": 0,
+            "IsPartial": False,
+            "AutoMarginStart": 0,
+            "AutoMarginEnd": 0,
+            "ServerRecordingId": -1,
+            "ActualStartTime": 1676833531,
+            "ProgramDuration": 0,
+            "IsRadio": False,
+            "EITSource": "EIT_SOURCE_PF",
+            "RecError": "REC_ERROR_NONE"
+        },
+        {
+            "RecordingId": 35,
+            "RecordingType": "RECORDING_NEW",
+            "IsIpEpgRec": False,
+            "ccid": 2091,
+            "StartTime": 1676832212,
+            "Duration": 22,
+            "MarginStart": 0,
+            "MarginEnd": 0,
+            "EventId": 47369,
+            "EITVersion": 0,
+            "RetentionInfo": -1,
+            "EventInfo": "Eisige Welten II - Planet der Extreme\nDeutschland 2023\nIm Fokus dieser Folge stehen die besonderen Anpassungsstrategien der Bewohner an die Veränderungen in den klimatisch herausfordernden Lebensräumen.\n\nDie Reise beginnt auf dem gefrorenen Kontinent der Antarktis im äußersten Süden, dem lebensfeindlichsten Ort der Erde. Nachdem sie im Winter auf dem Eis aufgewachsen sind, werden die Kaiserpinguinküken im Frühjahr von ihren Eltern verlassen.\nHD-Produktion",
+            "EventExtendedInfo": "",
+            "EventGenre": "8",
+            "RecName": "Terra X",
+            "SeriesID": "None",
+            "SeasonNo": 0,
+            "EpisodeNo": 0,
+            "EpisodeCount": 70980,
+            "ProgramNumber": 11110,
+            "EventRating": 0,
+            "hasDot": True,
+            "isFTARecording": False,
+            "LastPinChangedTime": 0,
+            "Version": 339,
+            "HasCicamPin": False,
+            "HasLicenseFile": False,
+            "Size": 0,
+            "ResumeInfo": 0,
+            "IsPartial": False,
+            "AutoMarginStart": 0,
+            "AutoMarginEnd": 0,
+            "ServerRecordingId": -1,
+            "ActualStartTime": 1676832212,
+            "ProgramDuration": 0,
+            "IsRadio": False,
+            "EITSource": "EIT_SOURCE_PF",
+            "RecError": "REC_ERROR_NONE"
+        },
+        {
+            "RecordingId": 34,
+            "RecordingType": "RECORDING_PARTIALLY_VIEWED",
+            "IsIpEpgRec": False,
+            "ccid": 2091,
+            "StartTime": 1676677580,
+            "Duration": 484,
+            "MarginStart": 0,
+            "MarginEnd": 0,
+            "EventId": -1,
+            "EITVersion": 0,
+            "RetentionInfo": -1,
+            "EventInfo": "\n\nAlpine Ski-WM: Parallel-Event, Übertragung aus Méribel/Frankreich\n\n14:10: Biathlon-WM (AD): 20 km Einzel Männer, Übertragung aus Oberhof\nHD-Produktion",
+            "EventExtendedInfo": "",
+            "EventGenre": "4",
+            "RecName": "ZDF HD 2023-02-18 00:46",
+            "SeriesID": "None",
+            "SeasonNo": 0,
+            "EpisodeNo": 0,
+            "EpisodeCount": 2760,
+            "ProgramNumber": 11110,
+            "EventRating": 0,
+            "hasDot": True,
+            "isFTARecording": False,
+            "LastPinChangedTime": 0,
+            "Version": 328,
+            "HasCicamPin": False,
+            "HasLicenseFile": False,
+            "Size": 0,
+            "ResumeInfo": 56,
+            "IsPartial": False,
+            "AutoMarginStart": 0,
+            "AutoMarginEnd": 0,
+            "ServerRecordingId": -1,
+            "ActualStartTime": 1676677581,
+            "ProgramDuration": 0,
+            "IsRadio": False,
+            "EITSource": "EIT_SOURCE_PF",
+            "RecError": "REC_ERROR_NONE"
+        }
+      ]
 }
```

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/dummy/v1.py` & `ha-philipsjs-3.1.0/haphilipsjs/dummy/v1.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/haphilipsjs/typing.py` & `ha-philipsjs-3.1.0/haphilipsjs/typing.py`

 * *Files identical despite different names*

### Comparing `ha-philipsjs-3.0.1/setup.py` & `ha-philipsjs-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 PACKAGE_NAME = 'ha-philipsjs'
 HERE = os.path.abspath(os.path.dirname(__file__))
-VERSION = '3.0.1'
+VERSION = '3.1.0'
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*', 'dist', 'ccu', 'build'])
 
 REQUIRES = [
     "cryptography",
     "httpx>=0.22.0",
 ]
```

