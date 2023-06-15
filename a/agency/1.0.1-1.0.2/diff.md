# Comparing `tmp/agency-1.0.1.tar.gz` & `tmp/agency-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.0.1.tar", max compression
+gzip compressed data, was "agency-1.0.2.tar", max compression
```

## Comparing `agency-1.0.1.tar` & `agency-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 agency-1.0.1/LICENSE
--rw-r--r--   0        0        0    25810 2023-06-14 13:13:25.936547 agency-1.0.1/README.md
--rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 agency-1.0.1/agency/__init__.py
--rw-r--r--   0        0        0    10785 2023-06-14 13:13:25.936902 agency-1.0.1/agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 agency-1.0.1/agency/agents/__init__.py
--rw-r--r--   0        0        0     2791 2023-06-12 21:57:53.079991 agency-1.0.1/agency/agents/chattyai.py
--rw-r--r--   0        0        0     2202 2023-06-12 20:36:46.457242 agency-1.0.1/agency/agents/host.py
--rw-r--r--   0        0        0     2729 2023-06-14 13:13:25.937150 agency-1.0.1/agency/agents/openai_completion_agent.py
--rw-r--r--   0        0        0     7797 2023-06-14 13:13:25.937407 agency-1.0.1/agency/agents/openai_function_agent.py
--rw-r--r--   0        0        0     1519 2023-06-12 20:36:46.457203 agency-1.0.1/agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 agency-1.0.1/agency/schema.py
--rwxr-xr-x   0        0        0     3261 2023-06-14 13:13:25.937665 agency-1.0.1/agency/space.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 agency-1.0.1/agency/spaces/__init__.py
--rw-r--r--   0        0        0     6646 2023-06-14 13:13:25.937925 agency-1.0.1/agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4027 2023-06-14 13:13:25.938200 agency-1.0.1/agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 agency-1.0.1/agency/util.py
--rw-r--r--   0        0        0      557 2023-06-14 13:17:07.822930 agency-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    26649 1970-01-01 00:00:00.000000 agency-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 agency-1.0.2/LICENSE
+-rw-r--r--   0        0        0    25690 2023-06-15 19:41:44.309956 agency-1.0.2/README.md
+-rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 agency-1.0.2/agency/__init__.py
+-rw-r--r--   0        0        0    10347 2023-06-15 19:59:59.343889 agency-1.0.2/agency/agent.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 agency-1.0.2/agency/agents/__init__.py
+-rw-r--r--   0        0        0     2791 2023-06-12 21:57:53.079991 agency-1.0.2/agency/agents/chattyai.py
+-rw-r--r--   0        0        0     2202 2023-06-12 20:36:46.457242 agency-1.0.2/agency/agents/host.py
+-rw-r--r--   0        0        0     2729 2023-06-14 13:13:25.937150 agency-1.0.2/agency/agents/openai_completion_agent.py
+-rw-r--r--   0        0        0     7797 2023-06-14 13:13:25.937407 agency-1.0.2/agency/agents/openai_function_agent.py
+-rw-r--r--   0        0        0     1519 2023-06-12 20:36:46.457203 agency-1.0.2/agency/agents/prompt_methods.py
+-rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 agency-1.0.2/agency/schema.py
+-rwxr-xr-x   0        0        0     3261 2023-06-14 13:13:25.937665 agency-1.0.2/agency/space.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 agency-1.0.2/agency/spaces/__init__.py
+-rw-r--r--   0        0        0     6646 2023-06-14 13:13:25.937925 agency-1.0.2/agency/spaces/templates/index.html
+-rw-r--r--   0        0        0     4027 2023-06-14 13:13:25.938200 agency-1.0.2/agency/spaces/web_app.py
+-rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 agency-1.0.2/agency/util.py
+-rw-r--r--   0        0        0      557 2023-06-15 20:21:51.900010 agency-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    26529 1970-01-01 00:00:00.000000 agency-1.0.2/PKG-INFO
```

### Comparing `agency-1.0.1/LICENSE` & `agency-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/README.md` & `agency-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -731,24 +731,22 @@
   Currently the limitations of python multi-threading are a bottleneck.
 - **Access Control and Safety**:
   An effective access control solution for agent-integrated systems is
   fundamental to ensure safety. I believe I've included a sane first step at
   such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
-  creating agent systems. I hope to ensure ensure the API is kept small, and
+  creating agent systems. I hope to ensure the API is kept small, and
   compatible with a wide variety of use cases.
 - **Documentation**:
   I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add schema support for [OpenAI Function
-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 - Add web app multimodal i/o examples
   - image
   - audio
   - video
 - Add multimodal model integration example
 - Add message broker/networking support (RabbitMQ)
 - Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
```

### Comparing `agency-1.0.1/agency/agent.py` & `agency-1.0.2/agency/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -252,43 +252,27 @@
         is passed.
         """
         return self._get_help(action_name)
 
     @access_policy(ACCESS_PERMITTED)
     def _action__return(self, original_message: MessageSchema, return_value: str):
         """
-        Overwrite this action to handle returned data from a prior action. By
+        Implement this action to handle returned data from a prior action. By
         default this action simply replaces it with an incoming "say".
         """
-        self._receive({
-          "from": original_message['to'],
-          "to": self.id(),
-          "thoughts": "A value was returned for your action",
-          "action": "say",
-          "args": {
-            "content": return_value.__str__(),
-          },
-        })
+        print("WARNING: Data was returned from an action. Implement _action__return to handle it.")
+        pass
 
     @access_policy(ACCESS_PERMITTED)
     def _action__error(self, original_message: MessageSchema, error: str):
         """
-        Overwrite this action to handle errors from an action. By default this
-        action simply converts it to an incoming "say".
+        Implement this action to handle errors from an action.
         """
-        # TODO: handle errors during errors to stop infinite loops
-        self._receive({
-          "from": original_message['to'],
-          "to": self.id(),
-          "thoughts": "An error occurred",
-          "action": "say",
-          "args": {
-            "content": f"ERROR: {error}",
-          },
-        })
+        print("WARNING: An error occurred in an action. Implement _action__error to handle it.")
+        pass
 
     def _after_action(self, original_message: MessageSchema, return_value: str, error: str):
         """
         Called after every action. Override and use this method for logging or other
         situations where you may want to pass through all actions.
 
         Note that this is only called if the action was actually attempted, meaning
```

### Comparing `agency-1.0.1/agency/agents/chattyai.py` & `agency-1.0.2/agency/agents/chattyai.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/agents/host.py` & `agency-1.0.2/agency/agents/host.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/agents/openai_completion_agent.py` & `agency-1.0.2/agency/agents/openai_completion_agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/agents/openai_function_agent.py` & `agency-1.0.2/agency/agents/openai_function_agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/agents/prompt_methods.py` & `agency-1.0.2/agency/agents/prompt_methods.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/schema.py` & `agency-1.0.2/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/space.py` & `agency-1.0.2/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/spaces/templates/index.html` & `agency-1.0.2/agency/spaces/templates/index.html`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/spaces/web_app.py` & `agency-1.0.2/agency/spaces/web_app.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/agency/util.py` & `agency-1.0.2/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.1/pyproject.toml` & `agency-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agency"
-version = "1.0.1"
+version = "1.0.2"
 description = "A fast and minimal foundation for unifying human, AI, and other computing systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `agency-1.0.1/PKG-INFO` & `agency-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.0.1
+Version: 1.0.2
 Summary: A fast and minimal foundation for unifying human, AI, and other computing systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -753,24 +753,22 @@
   Currently the limitations of python multi-threading are a bottleneck.
 - **Access Control and Safety**:
   An effective access control solution for agent-integrated systems is
   fundamental to ensure safety. I believe I've included a sane first step at
   such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
-  creating agent systems. I hope to ensure ensure the API is kept small, and
+  creating agent systems. I hope to ensure the API is kept small, and
   compatible with a wide variety of use cases.
 - **Documentation**:
   I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add schema support for [OpenAI Function
-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 - Add web app multimodal i/o examples
   - image
   - audio
   - video
 - Add multimodal model integration example
 - Add message broker/networking support (RabbitMQ)
 - Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
```

