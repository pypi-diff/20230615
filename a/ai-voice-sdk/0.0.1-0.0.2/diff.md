# Comparing `tmp/ai-voice-sdk-0.0.1.tar.gz` & `tmp/ai-voice-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ai-voice-sdk-0.0.1.tar", last modified: Tue May 30 03:56:10 2023, max compression
+gzip compressed data, was "dist\ai-voice-sdk-0.0.2.tar", last modified: Thu Jun 15 08:41:54 2023, max compression
```

## Comparing `ai-voice-sdk-0.0.1.tar` & `ai-voice-sdk-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/
--rw-rw-rw-   0        0        0     1065 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1497 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/
--rw-rw-rw-   0        0        0      117 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/__init__.py
--rw-rw-rw-   0        0        0     1697 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/config.py
--rw-rw-rw-   0        0        0    16204 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/converter.py
--rw-rw-rw-   0        0        0      629 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/enums.py
--rw-rw-rw-   0        0        0    12262 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/textedit.py
--rw-rw-rw-   0        0        0     1053 2023-05-30 03:54:26.000000 ai-voice-sdk-0.0.1/ai_voice_sdk/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/
--rw-rw-rw-   0        0        0     1497 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:56:10.000000 ai-voice-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-05-30 03:54:27.000000 ai-voice-sdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/
+-rw-rw-rw-   0        0        0     1079 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1673 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1214 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/
+-rw-rw-rw-   0        0        0      117 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/config.py
+-rw-rw-rw-   0        0        0    11970 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/converter.py
+-rw-rw-rw-   0        0        0      629 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/enums.py
+-rw-rw-rw-   0        0        0    23776 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/textedit.py
+-rw-rw-rw-   0        0        0     6340 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/ai_voice_sdk/units.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1673 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:41:54.000000 ai-voice-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-06-15 08:41:39.000000 ai-voice-sdk-0.0.2/setup.py
```

### Comparing `ai-voice-sdk-0.0.1/LICENSE` & `ai-voice-sdk-0.0.2/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 ATEN
+Copyright (c) 2023 ATEN-International
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ai-voice-sdk-0.0.1/PKG-INFO` & `ai-voice-sdk-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: ai-voice-sdk
-Version: 0.0.1
-Summary: This is aten ai voice sdk
-Author: yimin
-Author-email: no@example.com
+Version: 0.0.2
+Summary: Aten AI Voice SDK
+Home-page: https://github.com/ATEN-International/ai-voice-sdk-python
+Author: ATEN-International
+Author-email: rdmaten@aten.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,14 +16,17 @@
 
 <br>
 
 ## 目錄
  - [簡介](#簡介)
  - [需求](#需求)
  - [開始使用](#開始使用)
+    - [安裝](#安裝)
+    - [教學課程](#教學課程-tutorial)
+
 <br><br>
 
 ## 簡介
 AI Voice是宏正自動科技的語音合成服務優聲學，使用本SDK是必須租用優聲學服務。租用服務請至`https://www.aivoice.com.tw`上留下聯絡資料。<br>
 宏正優聲學，推出限量企業體驗版之語音合成服務，提供六個優質美聲，大量語音合成，歡迎企業用戶填寫表格連繫, 了解更多企業體驗版方案細節!
 <br><br>
 
@@ -40,24 +44,22 @@
 
 <br><br>
 
 ## 開始使用
 ### 安裝
  - 透過`pip`安裝SDK
 ```shell
-pip install ai_voice_sdk
+pip install ai-voice-sdk
 ```
 
  - 手動安裝SDK
 ```shell
 git clone https://github.com/ATEN-International/ai-voice-sdk-python.git
 cd ai-voice-sdk-python
+python -m pip install wheel
 python setup.py sdist bdist_wheel # 建立SDK安裝檔
-pip install dist/ai_voice_sdk-0.0.1-py3-none-any.whl # 安裝SDK
+pip install dist/ai_voice_sdk-x.x.x-py3-none-any.whl # 安裝SDK，其中 'x.x.x' 填入現在的版本號
 ```
 <br><br>
 
-### 教學課程 [tutorial](./tutorial.ipynb)
-<br><br>
-
-### 更多範例 [example code](./examples)
+### 教學課程 [tutorial](./examples/tutorial.ipynb)
 <br><br>
```

### Comparing `ai-voice-sdk-0.0.1/README.md` & `ai-voice-sdk-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 <br>
 
 ## 目錄
  - [簡介](#簡介)
  - [需求](#需求)
  - [開始使用](#開始使用)
+    - [安裝](#安裝)
+    - [教學課程](#教學課程-tutorial)
+
 <br><br>
 
 ## 簡介
 AI Voice是宏正自動科技的語音合成服務優聲學，使用本SDK是必須租用優聲學服務。租用服務請至`https://www.aivoice.com.tw`上留下聯絡資料。<br>
 宏正優聲學，推出限量企業體驗版之語音合成服務，提供六個優質美聲，大量語音合成，歡迎企業用戶填寫表格連繫, 了解更多企業體驗版方案細節!
 <br><br>
 
@@ -27,24 +30,22 @@
 
 <br><br>
 
 ## 開始使用
 ### 安裝
  - 透過`pip`安裝SDK
 ```shell
-pip install ai_voice_sdk
+pip install ai-voice-sdk
 ```
 
  - 手動安裝SDK
 ```shell
 git clone https://github.com/ATEN-International/ai-voice-sdk-python.git
 cd ai-voice-sdk-python
+python -m pip install wheel
 python setup.py sdist bdist_wheel # 建立SDK安裝檔
-pip install dist/ai_voice_sdk-0.0.1-py3-none-any.whl # 安裝SDK
+pip install dist/ai_voice_sdk-x.x.x-py3-none-any.whl # 安裝SDK，其中 'x.x.x' 填入現在的版本號
 ```
 <br><br>
 
-### 教學課程 [tutorial](./tutorial.ipynb)
+### 教學課程 [tutorial](./examples/tutorial.ipynb)
 <br><br>
-
-### 更多範例 [example code](./examples)
-<br><br>
```

### Comparing `ai-voice-sdk-0.0.1/ai_voice_sdk/config.py` & `ai-voice-sdk-0.0.2/ai_voice_sdk/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 from .enums import Voice
 
 class Settings(object):
     text_limit = 1500
-
-    # _support_file_type = [".txt", ".ssml"] # 暫不支援ssml
-    support_file_type = [".txt"]
-
-    task_each_text_limit = text_limit + 200
-    # server_support_json_status_code = [200, 400, 500, 503] # 401 server回傳會少帶code參數，所以暫時移除
-
+    elastic_value = 200
+    support_file_type = [".txt", ".ssml", ".xml"]
+    each_task_text_limit = text_limit + elastic_value
     print_log = False
 
 class ConverterConfig(object):
     _token:str
     _server_url:str
 
-    voice = Voice.NOETIC
-    _ssml_version = ""
-    _ssml_lang = ""
+    voice = None # 聲音預設值為None
+    _ssml_version = "1.0.demo"
+    _ssml_lang = "zh-TW"
 
     def __init__(self, token = "", server_url = "https://www.aivoice.com.tw") -> None:
-        if type(token) != str:
-            raise TypeError("Parameter 'token(str)' type error.")
-
-        self._token = token
+        self.set_token(token)
         self.set_server(server_url)
 
 
     def set_token(self, token = "") -> None:
         if type(token) != str:
             raise TypeError("Parameter 'token(str)' type error.")
 
@@ -48,16 +41,24 @@
             raise ValueError("Please check url, it should be with 'http' or 'https'.")
 
 
     def get_server(self) -> str:
         return self._server_url
 
 
-    def set_voice(self, voice = Voice.NOETIC) -> None:
+    def set_voice(self, voice:Voice) -> None:
         if type(voice) != Voice:
             raise TypeError("Parameter 'voice(Voice)' type error.")
 
         self.voice = voice
 
 
     def get_voice(self) -> str:
-        return self.voice
+        return self.voice
+
+
+    def get_ssml_version(self) -> str:
+        return self._ssml_version
+
+
+    def get_ssml_lang(self) -> str:
+        return self._ssml_lang
```

### Comparing `ai-voice-sdk-0.0.1/ai_voice_sdk/enums.py` & `ai-voice-sdk-0.0.2/ai_voice_sdk/enums.py`

 * *Files identical despite different names*

### Comparing `ai-voice-sdk-0.0.1/ai_voice_sdk.egg-info/PKG-INFO` & `ai-voice-sdk-0.0.2/ai_voice_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: ai-voice-sdk
-Version: 0.0.1
-Summary: This is aten ai voice sdk
-Author: yimin
-Author-email: no@example.com
+Version: 0.0.2
+Summary: Aten AI Voice SDK
+Home-page: https://github.com/ATEN-International/ai-voice-sdk-python
+Author: ATEN-International
+Author-email: rdmaten@aten.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,14 +16,17 @@
 
 <br>
 
 ## 目錄
  - [簡介](#簡介)
  - [需求](#需求)
  - [開始使用](#開始使用)
+    - [安裝](#安裝)
+    - [教學課程](#教學課程-tutorial)
+
 <br><br>
 
 ## 簡介
 AI Voice是宏正自動科技的語音合成服務優聲學，使用本SDK是必須租用優聲學服務。租用服務請至`https://www.aivoice.com.tw`上留下聯絡資料。<br>
 宏正優聲學，推出限量企業體驗版之語音合成服務，提供六個優質美聲，大量語音合成，歡迎企業用戶填寫表格連繫, 了解更多企業體驗版方案細節!
 <br><br>
 
@@ -40,24 +44,22 @@
 
 <br><br>
 
 ## 開始使用
 ### 安裝
  - 透過`pip`安裝SDK
 ```shell
-pip install ai_voice_sdk
+pip install ai-voice-sdk
 ```
 
  - 手動安裝SDK
 ```shell
 git clone https://github.com/ATEN-International/ai-voice-sdk-python.git
 cd ai-voice-sdk-python
+python -m pip install wheel
 python setup.py sdist bdist_wheel # 建立SDK安裝檔
-pip install dist/ai_voice_sdk-0.0.1-py3-none-any.whl # 安裝SDK
+pip install dist/ai_voice_sdk-x.x.x-py3-none-any.whl # 安裝SDK，其中 'x.x.x' 填入現在的版本號
 ```
 <br><br>
 
-### 教學課程 [tutorial](./tutorial.ipynb)
-<br><br>
-
-### 更多範例 [example code](./examples)
+### 教學課程 [tutorial](./examples/tutorial.ipynb)
 <br><br>
```

### Comparing `ai-voice-sdk-0.0.1/setup.py` & `ai-voice-sdk-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ai-voice-sdk",
-    version="0.0.1",
-    author="yimin",
-    author_email="no@example.com",
-    description="This is aten ai voice sdk",
+    version="0.0.2",
+    author="ATEN-International",
+    author_email="rdmaten@aten.com.tw",
+    url="https://github.com/ATEN-International/ai-voice-sdk-python",
+    description="Aten AI Voice SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires=[
         'requests',
-        # 'python-magic-bin==0.4.14',
     ],
 )
```

