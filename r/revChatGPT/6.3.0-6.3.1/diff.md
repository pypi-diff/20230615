# Comparing `tmp/revChatGPT-6.3.0.tar.gz` & `tmp/revChatGPT-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.3.0.tar", last modified: Thu Jun 15 05:39:03 2023, max compression
+gzip compressed data, was "revChatGPT-6.3.1.tar", last modified: Thu Jun 15 07:24:31 2023, max compression
```

## Comparing `revChatGPT-6.3.0.tar` & `revChatGPT-6.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 05:39:03.006659 revChatGPT-6.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:02.994659 revChatGPT-6.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58554 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23440 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 05:39:02.000000 revChatGPT-6.3.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:39:03.002659 revChatGPT-6.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-15 05:38:31.000000 revChatGPT-6.3.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.977736 revChatGPT-6.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.977736 revChatGPT-6.3.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58784 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23440 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 07:24:31.000000 revChatGPT-6.3.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:24:31.981736 revChatGPT-6.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-15 07:24:04.000000 revChatGPT-6.3.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.3.0/LICENSE` & `revChatGPT-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/PKG-INFO` & `revChatGPT-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.0
+Version: 6.3.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -95,15 +95,15 @@
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>", // Only if you have a plus account and use GPT-4
-  "unverfied_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
+  "unverified_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-6.3.0/README.md` & `revChatGPT-6.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>", // Only if you have a plus account and use GPT-4
-  "unverfied_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
+  "unverified_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-6.3.0/setup.py` & `revChatGPT-6.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.3.0",
+    version="6.3.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.3.0/src/revChatGPT/V1.py` & `revChatGPT-6.3.1/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,20 @@
 
         if self.config.get("PUID"):
             self.session.cookies.set("_puid", self.config["PUID"])
 
         if self.config.get("plugin_ids", []):
             for plugin in self.config.get("plugin_ids"):
                 self.install_plugin(plugin)
-        if self.config.get("unverfied_plugin_domains", []):
-            for domain in self.config.get("unverfied_plugin_domains"):
-                self.get_unverified_plugin(domain,install=True)
+        if self.config.get("unverified_plugin_domains", []):
+            for domain in self.config.get("unverified_plugin_domains"):
+                if self.config.get("plugin_ids"):
+                    self.config["plugin_ids"].append(self.get_unverified_plugin(domain,install=True).get("id"))
+                else:
+                    self.config["plugin_ids"] = [self.get_unverified_plugin(domain,install=True).get("id")]
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
```

### Comparing `revChatGPT-6.3.0/src/revChatGPT/V3.py` & `revChatGPT-6.3.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT/__init__.py` & `revChatGPT-6.3.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT/__main__.py` & `revChatGPT-6.3.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.3.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT/typings.py` & `revChatGPT-6.3.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT/utils.py` & `revChatGPT-6.3.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.3.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.0
+Version: 6.3.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -95,15 +95,15 @@
   "conversation_id": "UUID...",
   "parent_id": "UUID...",
   "proxy": "...",
   "model": "gpt-4", // gpt-4-browsing, text-davinci-002-render-sha, gpt-4, gpt-4-plugins
   "plugin_ids": ["plugin-d1d6eb04-3375-40aa-940a-c2fc57ce0f51"], // Wolfram Alpha example
   "disable_history": true,
   "PUID": "<_puid cookie for plus accounts>", // Only if you have a plus account and use GPT-4
-  "unverfied_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
+  "unverified_plugin_domains":["showme.redstarplugin.com"] // Unverfied plugins to install
 }
 ```
 
 1. Save this as `$HOME/.config/revChatGPT/config.json`
 2. If you are using Windows, you will need to create an environment variable named `HOME` and set it to your home profile for the script to be able to locate the config.json file.
 
 Plugin IDs can be found [here](./plugins.json). Remember to set model to `gpt-4-plugins` if plugins are enabled. Plugins may or may not work if you haven't installed them from the web interface. You can call `chatbot.install_plugin(plugin_id=plugin_id)` to install any one of them from code. Call `chatbot.get_plugins()` to get a list of all plugins available.
```

### Comparing `revChatGPT-6.3.0/tests/test_recipient.py` & `revChatGPT-6.3.1/tests/test_recipient.py`

 * *Files identical despite different names*

