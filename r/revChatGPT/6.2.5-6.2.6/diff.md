# Comparing `tmp/revChatGPT-6.2.5.tar.gz` & `tmp/revChatGPT-6.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.2.5.tar", last modified: Wed Jun 14 15:37:44 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.6.tar", last modified: Wed Jun 14 15:43:57 2023, max compression
```

## Comparing `revChatGPT-6.2.5.tar` & `revChatGPT-6.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 15:37:44.820719 revChatGPT-6.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 15:37:44.820719 revChatGPT-6.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.812719 revChatGPT-6.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 15:43:57.965862 revChatGPT-6.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23440 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 15:43:57.000000 revChatGPT-6.2.6/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:43:57.961862 revChatGPT-6.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-14 15:43:29.000000 revChatGPT-6.2.6/tests/test_recipient.py
```

### Comparing `revChatGPT-6.2.5/LICENSE` & `revChatGPT-6.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/PKG-INFO` & `revChatGPT-6.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.5
+Version: 6.2.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) - [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
@@ -52,35 +52,38 @@
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
 
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
+
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -89,15 +92,15 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
@@ -180,45 +183,29 @@
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
 
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
-  $ python3 -m revChatGPT.V3 --help
+  $ python3 -m revChatGPT.V3
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
+    Version: 6.2
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
-             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
-             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
+             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
+             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
+             [--submit_key SUBMIT_KEY]
+             [--model {gpt-3.5-turbo,gpt-3.5-turbo-16k,gpt-3.5-turbo-0301,gpt-3.5-turbo-0613,gpt-4,gpt-4-0314,gpt-4-32k,gpt-4-32k-0314,gpt-4-0613}]
              [--truncate_limit TRUNCATE_LIMIT]
-
-options:
-  -h, --help            show this help message and exit
-  --api_key API_KEY     OpenAI API key
-  --temperature TEMPERATURE
-                        Temperature for response
-  --no_stream           Disable streaming
-  --base_prompt BASE_PROMPT
-                        Base prompt for chatbot
-  --proxy PROXY         Proxy address
-  --top_p TOP_P         Top p for response
-  --reply_count REPLY_COUNT
-                        Number of replies for each prompt
-  --enable_internet     Allow ChatGPT to search the internet
-  --config CONFIG       Path to V3 config json file
-  --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see README
-  --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
-  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
 
 ```python
```

### Comparing `revChatGPT-6.2.5/README.md` & `revChatGPT-6.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) - [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
@@ -30,35 +30,38 @@
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
 
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
+
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -67,15 +70,15 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
@@ -158,45 +161,29 @@
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
 
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
-  $ python3 -m revChatGPT.V3 --help
+  $ python3 -m revChatGPT.V3
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
+    Version: 6.2
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
-             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
-             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
+             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
+             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
+             [--submit_key SUBMIT_KEY]
+             [--model {gpt-3.5-turbo,gpt-3.5-turbo-16k,gpt-3.5-turbo-0301,gpt-3.5-turbo-0613,gpt-4,gpt-4-0314,gpt-4-32k,gpt-4-32k-0314,gpt-4-0613}]
              [--truncate_limit TRUNCATE_LIMIT]
-
-options:
-  -h, --help            show this help message and exit
-  --api_key API_KEY     OpenAI API key
-  --temperature TEMPERATURE
-                        Temperature for response
-  --no_stream           Disable streaming
-  --base_prompt BASE_PROMPT
-                        Base prompt for chatbot
-  --proxy PROXY         Proxy address
-  --top_p TOP_P         Top p for response
-  --reply_count REPLY_COUNT
-                        Number of replies for each prompt
-  --enable_internet     Allow ChatGPT to search the internet
-  --config CONFIG       Path to V3 config json file
-  --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see README
-  --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
-  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
 
 ```python
```

### Comparing `revChatGPT-6.2.5/setup.py` & `revChatGPT-6.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.2.5",
+    version="6.2.6",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.2.5/src/revChatGPT/V1.py` & `revChatGPT-6.2.6/src/revChatGPT/V1.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT/V3.py` & `revChatGPT-6.2.6/src/revChatGPT/V3.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from .utils import get_filtered_keys_from_object
 from .utils import get_input
 
 ENGINES = [
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-16k",
     "gpt-3.5-turbo-0301",
-    "gpt-3.5-turbo-0613" "gpt-4",
+    "gpt-3.5-turbo-0613",
+    "gpt-4",
     "gpt-4-0314",
     "gpt-4-32k",
     "gpt-4-32k-0314",
     "gpt-4-0613",
 ]
```

### Comparing `revChatGPT-6.2.5/src/revChatGPT/__init__.py` & `revChatGPT-6.2.6/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT/__main__.py` & `revChatGPT-6.2.6/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.6/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT/typings.py` & `revChatGPT-6.2.6/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT/utils.py` & `revChatGPT-6.2.6/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.5/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.6/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.5
+Version: 6.2.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) - [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
@@ -52,35 +52,38 @@
 V1 uses a cloudflare bypass proxy to make life convenient for everyone. The proxy is open source: https://github.com/acheong08/ChatGPT-Proxy-V4
 
 To set your own deployed proxy, set the environment variable `CHATGPT_BASE_URL` to `https://yourproxy.com/api/`
 
 </summary>
 
 ## Rate limits
+
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > Not supported for Google/Microsoft accounts.
+
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -89,15 +92,15 @@
 
 ```json
 {
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
-  "plugin_ids" : ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
+  "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>" // Only if you have a plus account and use GPT-4
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
@@ -180,45 +183,29 @@
 Get API key from https://platform.openai.com/account/api-keys
 
 ## Command line
 
 `python3 -m revChatGPT.V3 --api_key <api_key>`
 
 ```
-  $ python3 -m revChatGPT.V3 --help
+  $ python3 -m revChatGPT.V3
 
     ChatGPT - Official ChatGPT API
     Repo: github.com/acheong08/ChatGPT
+    Version: 6.2
 
 Type '!help' to show a full list of commands
 Press Esc followed by Enter or Alt+Enter to send a message.
 
-usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream] [--base_prompt BASE_PROMPT]
-             [--proxy PROXY] [--top_p TOP_P] [--reply_count REPLY_COUNT] [--enable_internet]
-             [--config CONFIG] [--submit_key SUBMIT_KEY] [--model {gpt-3.5-turbo,gpt-4,gpt-4-32k}]
+usage: V3.py [-h] --api_key API_KEY [--temperature TEMPERATURE] [--no_stream]
+             [--base_prompt BASE_PROMPT] [--proxy PROXY] [--top_p TOP_P]
+             [--reply_count REPLY_COUNT] [--enable_internet] [--config CONFIG]
+             [--submit_key SUBMIT_KEY]
+             [--model {gpt-3.5-turbo,gpt-3.5-turbo-16k,gpt-3.5-turbo-0301,gpt-3.5-turbo-0613,gpt-4,gpt-4-0314,gpt-4-32k,gpt-4-32k-0314,gpt-4-0613}]
              [--truncate_limit TRUNCATE_LIMIT]
-
-options:
-  -h, --help            show this help message and exit
-  --api_key API_KEY     OpenAI API key
-  --temperature TEMPERATURE
-                        Temperature for response
-  --no_stream           Disable streaming
-  --base_prompt BASE_PROMPT
-                        Base prompt for chatbot
-  --proxy PROXY         Proxy address
-  --top_p TOP_P         Top p for response
-  --reply_count REPLY_COUNT
-                        Number of replies for each prompt
-  --enable_internet     Allow ChatGPT to search the internet
-  --config CONFIG       Path to V3 config json file
-  --submit_key SUBMIT_KEY
-                        Custom submit key for chatbot. For more information on keys, see README
-  --model {gpt-3.5-turbo,gpt-4,gpt-4-32k}
-  --truncate_limit TRUNCATE_LIMIT
 ```
 
 ## Developer API
 
 ### Basic example
 
 ```python
```

### Comparing `revChatGPT-6.2.5/tests/test_recipient.py` & `revChatGPT-6.2.6/tests/test_recipient.py`

 * *Files identical despite different names*

