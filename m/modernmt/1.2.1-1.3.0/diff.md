# Comparing `tmp/modernmt-1.2.1.tar.gz` & `tmp/modernmt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernmt-1.2.1.tar", last modified: Thu May 11 09:26:43 2023, max compression
+gzip compressed data, was "modernmt-1.3.0.tar", last modified: Thu Jun 15 09:18:59 2023, max compression
```

## Comparing `modernmt-1.2.1.tar` & `modernmt-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.846063 modernmt-1.2.1/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.2.1/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-11 09:26:43.846063 modernmt-1.2.1/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.2.1/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.2.1/pyproject.toml
--rw-rw-r--   0 davide    (1000) davide    (1000)      648 2023-05-11 09:26:43.846063 modernmt-1.2.1/setup.cfg
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.842063 modernmt-1.2.1/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.842063 modernmt-1.2.1/src/modernmt/
--rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.2.1/src/modernmt/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    10989 2023-05-11 09:26:35.000000 modernmt-1.2.1/src/modernmt/modernmt.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-05-11 09:26:43.846063 modernmt-1.2.1/src/modernmt.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-05-11 09:26:43.000000 modernmt-1.2.1/src/modernmt.egg-info/top_level.txt
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.652890 modernmt-1.3.0/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.3.0/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-06-15 09:18:59.652890 modernmt-1.3.0/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.3.0/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.3.0/pyproject.toml
+-rw-rw-r--   0 davide    (1000) davide    (1000)      655 2023-06-15 09:18:59.652890 modernmt-1.3.0/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.648890 modernmt-1.3.0/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.648890 modernmt-1.3.0/src/modernmt/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.3.0/src/modernmt/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12266 2023-06-15 09:18:35.000000 modernmt-1.3.0/src/modernmt/modernmt.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.652890 modernmt-1.3.0/src/modernmt.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       15 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/top_level.txt
```

### Comparing `modernmt-1.2.1/LICENSE` & `modernmt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modernmt-1.2.1/PKG-INFO` & `modernmt-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.2.1
+Version: 1.3.0
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modernmt-1.2.1/setup.cfg` & `modernmt-1.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modernmt
-version = 1.2.1
+version = 1.3.0
 author = ModernMT
 author_email = info@modernmt.com
 description = ModernMT API wrapper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/modernmt/modernmt-python
 project_urls = 
@@ -17,14 +17,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3
 install_requires = 
 	requests
+	pyjwt
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `modernmt-1.2.1/src/modernmt/modernmt.py` & `modernmt-1.3.0/src/modernmt/modernmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.message = message
 
         if metadata is not None:
             self.metadata = metadata
 
 
 class ModernMT(object):
-    def __init__(self, api_key, platform="modernmt-python", platform_version="1.2.1", api_client=None) -> None:
+    def __init__(self, api_key, platform="modernmt-python", platform_version="1.3.0", api_client=None) -> None:
         self.__batch_public_key = None
         self.__batch_public_key_timestamp_sec = 0
 
         self.__base_url = "https://api.modernmt.com"
         self.__headers = {
             "MMT-ApiKey": api_key,
             "MMT-Platform": platform,
@@ -41,15 +41,15 @@
     def detect_language(self, q, format=None):
         data = {"q": q}
         if format is not None:
             data["format"] = format
 
         res = self.__send("get", "/translate/detect", data=data)
 
-        if not isinstance(q, list):
+        if not isinstance(res, list):
             return DetectedLanguage(res)
 
         languages = []
         for el in res:
             languages.append(DetectedLanguage(el))
 
         return languages
@@ -77,15 +77,15 @@
             if "format" in options:
                 data["format"] = options["format"]
             if "alt_translations" in options:
                 data["alt_translations"] = options["alt_translations"]
 
         res = self.__send("get", "/translate", data=data)
 
-        if not isinstance(q, list):
+        if not isinstance(res, list):
             return Translation(res)
 
         translations = []
         for el in res:
             translations.append(Translation(el))
 
         return translations
@@ -206,14 +206,30 @@
             return res["vectors"]
         else:
             if targets in res["vectors"]:
                 return res["vectors"][targets]
             else:
                 return None
 
+    def me(self):
+        return self.__send("get", "/users/me", cls=User)
+
+    def qe(self, source, target, sentence, translation):
+        data = {"source": source, "target": target, "sentence": sentence, "translation": translation}
+        res = self.__send("get", "/qe", data=data)
+
+        if not isinstance(res, list):
+            return QualityEstimation(res)
+
+        qes = []
+        for el in res:
+            qes.append(QualityEstimation(el))
+
+        return qes
+
     def __send(self, method, endpoint, data=None, files=None, cls=None, headers=None):
         url = self.__base_url + endpoint
 
         _headers = self.__headers
         _headers["X-HTTP-Method-Override"] = method
 
         if headers is not None:
@@ -336,7 +352,43 @@
     def __init__(self, data) -> None:
         super().__init__(data, ["id", "memory", "size", "progress"])
 
 
 class DetectedLanguage(_Model):
     def __init__(self, data) -> None:
         super().__init__(data, ["billedCharacters", "detectedLanguage"])
+
+
+class User(_Model):
+    def __init__(self, data) -> None:
+        super().__init__(data, [
+            "id",
+            "name",
+            "email",
+            "registrationDate",
+            "country",
+            "isBusiness",
+            "status"
+        ])
+        self.billingPeriod = BillingPeriod(data["billingPeriod"])
+
+
+class BillingPeriod(_Model):
+    def __init__(self, data) -> None:
+        super().__init__(data, [
+            "begin",
+            "end",
+            "chars",
+            "plan",
+            "planDescription",
+            "planForCatTool",
+            "amount",
+            "currency",
+            "currencySymbol"
+        ])
+
+
+class QualityEstimation(_Model):
+    def __init__(self, data) -> None:
+        super().__init__(data, [
+            "score"
+        ])
```

### Comparing `modernmt-1.2.1/src/modernmt.egg-info/PKG-INFO` & `modernmt-1.3.0/src/modernmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.2.1
+Version: 1.3.0
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

