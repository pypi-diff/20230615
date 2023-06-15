# Comparing `tmp/elevenlabslib-0.9.2.tar.gz` & `tmp/elevenlabslib-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.9.2.tar", last modified: Sat Jun 10 20:52:53 2023, max compression
+gzip compressed data, was "elevenlabslib-0.9.3.tar", last modified: Thu Jun 15 21:32:39 2023, max compression
```

## Comparing `elevenlabslib-0.9.2.tar` & `elevenlabslib-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     3379 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.834947 elevenlabslib-0.9.2/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    40835 2023-06-10 20:51:36.000000 elevenlabslib-0.9.2/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.2/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     8403 2023-05-31 21:35:21.000000 elevenlabslib-0.9.2/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-10 20:52:53.839950 elevenlabslib-0.9.2/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     3379 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 20:52:53.000000 elevenlabslib-0.9.2/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-10 20:52:35.000000 elevenlabslib-0.9.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 20:52:53.840947 elevenlabslib-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     3379 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.775509 elevenlabslib-0.9.3/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    42069 2023-06-15 21:32:11.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.3/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-06-15 21:13:31.000000 elevenlabslib-0.9.3/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.779508 elevenlabslib-0.9.3/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3379 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-15 21:19:01.000000 elevenlabslib-0.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/setup.cfg
```

### Comparing `elevenlabslib-0.9.2/LICENSE` & `elevenlabslib-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/PKG-INFO` & `elevenlabslib-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.2
+Version: 0.9.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.2 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.3 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.2/README.md` & `elevenlabslib-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsVoice.py`

 * *Files 3% similar despite different names*

```diff
@@ -454,24 +454,53 @@
 
         Args:
             sharingEnabled (bool): Whether to enable or disable sharing.
 
         Returns:
             str|None: The share URL for the voice, if you enabled sharing, or None if you disabled it.
         """
-        sharingEnabledString = str(sharingEnabled).lower()
+        warn("This is currently broken, as ElevenLabs have disabled accessing the sharing endpoints via the API key.")
+
+        payload = {
+            "enable":sharingEnabled,
+            "emails":[]
+        }
         sharingInfo = self.get_info()["sharing"]
         if sharingInfo is not None and sharingInfo["status"] == "copied":
             raise RuntimeError("Cannot change sharing status of copied voices!")
 
-        response = _api_multipart("/voices/" + self._voiceID + "/share", self._linkedUser.headers, data=sharingEnabledString)
+        response = _api_json("/voices/" + self._voiceID + "/share", self._linkedUser.headers, jsonData=payload)
         if sharingEnabled:
             return self.get_share_link()
         else:
             return None
+
+    def set_library_sharing(self, sharingEnabled:bool) -> None:
+        """
+        Edits the library sharing status, assuming it is not a copied voice.
+
+        Note:
+            If you try to enable library sharing but don't have normal sharing enabled, it will be enabled automatically.
+
+            The same does NOT apply in reverse - if you disable library sharing, normal sharing will remain enabled.
+
+        Args:
+            sharingEnabled (bool): Whether to enable or disable public library sharing.
+
+        """
+        sharingEnabledString = str(sharingEnabled).lower()
+        sharingInfo = self.get_info()["sharing"]
+        if sharingInfo is not None and sharingInfo["status"] == "copied":
+            raise RuntimeError("Cannot change library sharing status of copied voices!")
+
+        if sharingInfo is None or sharingInfo["status"] != "enabled" and sharingEnabled:
+            self.set_sharing(sharingEnabled)
+
+        response = _api_multipart("/voices/" + self._voiceID + "/share-library", self._linkedUser.headers, data=sharingEnabledString)
+
     def get_share_link(self) -> str:
         """
         Returns the share link for the voice.
 
         Warning:
             If sharing is disabled, raises a RuntimeError.
```

### Comparing `elevenlabslib-0.9.2/elevenlabslib/__init__.py` & `elevenlabslib-0.9.3/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.2/elevenlabslib/helpers.py` & `elevenlabslib-0.9.3/elevenlabslib/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,27 @@
         '-----------START-----------',
         req.method + ' ' + req.url,
         '\r\n'.join('{}: {}'.format(k, v) for k, v in req.headers.items()),
         req.body,
     ))
 
 
+def run_ai_speech_classifier(audioBytes:bytes):
+    """
+    Runs Elevenlabs' AI speech classifier on the provided audio data.
+    Parameters:
+        audioBytes: The bytes of the audio file (mp3, wav, most formats should work) you want to analzye
 
+    Returns:
+        Dict containing all the information returned by the tool (usually just the probability of it being AI generated)
+    """
+    data = io.BytesIO(audioBytes)
+    files = {'file': ('audioSample.mp3', data, 'audio/mpeg')}
+    response = _api_multipart("/moderation/ai-speech-classification", headers=None, data=None, filesData=files)
+    return response.json()
 
 def play_audio_bytes(audioData:bytes, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                      onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None) -> sd.OutputStream:
     """
     Plays the given audio and calls the given functions.
     
     Parameters:
```

### Comparing `elevenlabslib-0.9.2/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.9.3/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.2
+Version: 0.9.3
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.2 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.3 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.2/pyproject.toml` & `elevenlabslib-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

