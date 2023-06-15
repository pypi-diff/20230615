# Comparing `tmp/edubot-0.7.0.tar.gz` & `tmp/edubot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.7.0.tar", max compression
+gzip compressed data, was "edubot-0.7.1.tar", max compression
```

## Comparing `edubot-0.7.0.tar` & `edubot-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-11-24 18:21:26.784597 edubot-0.7.0/LICENSE
--rw-r--r--   0        0        0     1400 2023-03-29 15:28:01.248879 edubot-0.7.0/README.md
--rw-r--r--   0        0        0      894 2023-05-19 11:19:02.481354 edubot-0.7.0/edubot/__init__.py
--rw-r--r--   0        0        0    22396 2023-06-02 18:11:58.660024 edubot-0.7.0/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-23 10:32:46.665675 edubot-0.7.0/edubot/sql.py
--rw-r--r--   0        0        0      636 2023-06-02 16:51:19.347235 edubot-0.7.0/edubot/types.py
--rw-r--r--   0        0        0      624 2023-06-02 18:11:37.951095 edubot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-24 18:21:26.784597 edubot-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1400 2023-03-29 15:28:01.248879 edubot-0.7.1/README.md
+-rw-r--r--   0        0        0      894 2023-05-19 11:19:02.481354 edubot-0.7.1/edubot/__init__.py
+-rw-r--r--   0        0        0    23354 2023-06-15 11:42:24.690978 edubot-0.7.1/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-23 10:32:46.665675 edubot-0.7.1/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-06-02 16:51:19.347235 edubot-0.7.1/edubot/types.py
+-rw-r--r--   0        0        0      624 2023-06-15 11:42:10.518028 edubot-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.7.1/PKG-INFO
```

### Comparing `edubot-0.7.0/LICENSE` & `edubot-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.7.0/README.md` & `edubot-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.7.0/edubot/__init__.py` & `edubot-0.7.1/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.0/edubot/bot.py` & `edubot-0.7.1/edubot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,26 +68,29 @@
 
 
 class EduBot:
     """
     An AI chatbot which continually improves itself using user feedback.
     """
 
-    def __init__(self, username: str, platform: str, personality: str = ""):
+    def __init__(self, username: str, platform: str, personality: str | list[str] = []):
         """
         Initialise EduBot with personalised information about the bot.
 
         :param username: A unique name to identify this bot from others on the same platform.
         :param platform: The platform the bot is running on E.g. 'telegram' 'matrix' 'mastodon'
-        :param personality: Some example conversation to influence the bots personality and mission.
-            Must be in "username: message\n ..." format.
+        :param personality: Instructions/information for the bot to follow when generating responses.
         """
         self.username = username
         self.platform = platform
-        self.personality = personality
+
+        if type(personality) is str:
+            self.personality = [personality]
+        else:
+            self.personality = personality
 
         self.__add_bot_to_db()
 
         # The primary key of the bot in the database
         self.__bot_pk = self.__get_bot(username).id
 
         openai.api_key = OPENAI_KEY
@@ -194,17 +197,19 @@
     ) -> list[dict]:
         """
         Formats chat context to the format expected by GPT.
 
         :param context: A list of MessageInfo.
         :return: The context as a list of dicts in GPT format.
         """
-        personality = self.personality
         if personality_override:
-            personality = personality_override
+            # We need to shallow copy 'self.personality' to avoid modifying the original list
+            personality = self.personality.copy().append(personality_override)
+        else:
+            personality = self.personality
 
         gpt_context: list[dict] = []
 
         token_count = 0
 
         for msg in context:
             if msg["username"] == self.username:
@@ -217,16 +222,25 @@
 
             token_count += estimate_tokens(content)
 
         while token_count > MAX_PROMPT_TOKENS:
             token_count -= estimate_tokens(gpt_context.pop(0)["content"])
 
         system_messages = [
-            {"role": "system", "content": "You are a chatbot named " + self.username},
-            {"role": "system", "content": f"Your personality is: {personality}"},
+            {
+                "role": "system",
+                "content": f"You are a chatbot named '{self.username}' which is controlled by an open source python"
+                f" program called EduBot that is running on a server owned by the Open EdTech"
+                f" organisation. On the backend, the edubot program connects to the API of an"
+                f" LLM ({GPT_SETTINGS['model']}) which processes prompts and returns responses. "
+                f"On the frontend, the Edubot program connects via API to the {self.platform}"
+                f" platform to write posts and read the posts of others. "
+                f"You, EduBot, are not able to change yourself - all requests to modify your"
+                f" code should be directed to Github: https://github.com/openedtech/edubot.",
+            },
             {
                 "role": "system",
                 "content": "You should pretend you can view images. "
                 "Descriptions of images posted to the chat will be saved to the database. "
                 "These descriptions are in the form: '*A picture of ____'. "
                 "When you spot these descriptions you should pretend you can see the image, using the description. "
                 "Do not mention that you cannot see the image, or that you are instead viewing a description of"
@@ -238,14 +252,17 @@
             },
             {
                 "role": "system",
                 "content": f"You use the language model {GPT_SETTINGS['model']}",
             },
         ]
 
+        for i in personality:
+            system_messages.append({"role": "system", "content": i})
+
         return system_messages + gpt_context
 
     @staticmethod
     def __describe_image(image: Image.Image) -> str:
         """
         Gets an AI generated description of an image.
         """
```

### Comparing `edubot-0.7.0/edubot/sql.py` & `edubot-0.7.1/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.0/edubot/types.py` & `edubot-0.7.1/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.7.0/pyproject.toml` & `edubot-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edubot"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `edubot-0.7.0/PKG-INFO` & `edubot-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

