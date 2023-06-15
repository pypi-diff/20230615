# Comparing `tmp/aifunc-0.4.1.tar.gz` & `tmp/aifunc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.4.1.tar", max compression
+gzip compressed data, was "aifunc-0.4.2.tar", max compression
```

## Comparing `aifunc-0.4.1.tar` & `aifunc-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.1/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.1/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.1/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.1/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.1/aifunc/generate_question.py
--rw-r--r--   0        0        0     7159 2023-06-15 04:34:18.362562 aifunc-0.4.1/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-15 04:34:49.497671 aifunc-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.2/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.2/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.2/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.2/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.2/aifunc/generate_question.py
+-rw-r--r--   0        0        0     6766 2023-06-15 04:36:19.130622 aifunc-0.4.2/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-15 04:36:23.459054 aifunc-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.2/PKG-INFO
```

### Comparing `aifunc-0.4.1/aifunc/add_ai_function.py` & `aifunc-0.4.2/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.4.1/aifunc/utility.py` & `aifunc-0.4.2/aifunc/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,68 +58,70 @@
           raise e  # re-raise the last exception
 
   ai_function.__name__ = function_name  # Set the function name
   return ai_function
 
 
 def create_ai_function_from_yaml(yaml_file):
-    import requests
-    import yaml
-    url = 'https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/fixed_format/' + yaml_file
-    response = requests.get(url)
-    if response.status_code == 200:
-        yaml_data = response.text
-        data = yaml.safe_load(yaml_data)
-    else:
-        print("Failed to load YAML file.")
-        exit(0)
-    instruction = data["instruction"]
-    example_pairs = data["example_pairs"]
-    properties = data["properties"]
-    
+  import requests
+  import yaml
+  url = 'https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/fixed_format/' + yaml_file
+  response = requests.get(url)
+  if response.status_code == 200:
+    yaml_data = response.text
+    data = yaml.safe_load(yaml_data)
+  else:
+    print("Failed to load YAML file.")
+    exit(0)
+  instruction = data["instruction"]
+  example_pairs = data["example_pairs"]
+  properties = data["properties"]
+
+  for example in example_pairs:
+    user_content = example["user_content"]
+    assistant_content = example["assistant_content"]
+    example["user_content"] = str(user_content)
+    example["assistant_content"] = str(assistant_content)
+
+  def fixed_format_ai_wrapper(prompt):
+    message = [{"role": "system", "content": instruction}]
     for example in example_pairs:
-        user_content = example["user_content"]
-        assistant_content = example["assistant_content"]
-        example["user_content"] = str(user_content)
-        example["assistant_content"] = str(assistant_content)
-    def fixed_format_ai_wrapper(prompt):
-        message = [{"role": "system", "content": instruction}]
-        for example in example_pairs:
-            user_content = example["user_content"]
-            assistant_content = example["assistant_content"]
-            message.append({"role": "user", "content": user_content})
-            message.append({"role": "assistant", "content": assistant_content})
-        message.append({"role": "user", "content": prompt})
-        function_name = "print_"
-        for prop in properties:
-            function_name += prop + "_"
-        function_name = function_name[:-1]
-        function_description = "print"
-        for prop in properties:
-            function_description += " " + prop + ","
-        function_description = function_description[:-1]
-        response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo-0613",
-            messages=message,
-            functions=[{
-                "name": function_name,
-                "description": function_description,
-                "parameters": {
-                    "type": "object",
-                    "properties": properties,
-                },
-            }],
-            function_call="auto",
-        )
-        message = response["choices"][0]["message"]
-        if message.get("function_call"):
-            arguments = eval(message["function_call"]["arguments"])
-            return arguments
-    
-    return fixed_format_ai_wrapper
+      user_content = example["user_content"]
+      assistant_content = example["assistant_content"]
+      message.append({"role": "user", "content": user_content})
+      message.append({"role": "assistant", "content": assistant_content})
+    message.append({"role": "user", "content": prompt})
+    function_name = "print_"
+    for prop in properties:
+      function_name += prop + "_"
+    function_name = function_name[:-1]
+    function_description = "print"
+    for prop in properties:
+      function_description += " " + prop + ","
+    function_description = function_description[:-1]
+    response = openai.ChatCompletion.create(
+      model="gpt-3.5-turbo-0613",
+      messages=message,
+      functions=[{
+        "name": function_name,
+        "description": function_description,
+        "parameters": {
+          "type": "object",
+          "properties": properties,
+        },
+      }],
+      function_call="auto",
+    )
+    message = response["choices"][0]["message"]
+    if message.get("function_call"):
+      arguments = eval(message["function_call"]["arguments"])
+      return arguments
+
+  return fixed_format_ai_wrapper
+
 
 def create_fixed_format_ai_function(yaml_file):
   url = 'https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/fixed_format/' + yaml_file
   response = requests.get(url)
 
   if response.status_code == 200:
     yaml_data = response.text
@@ -133,52 +135,53 @@
   properties = data["properties"]
   for example in example_pairs:
     user_content = example["user_content"]
     assistant_content = example["assistant_content"]
     example["user_content"] = str(user_content)
     example["assistant_content"] = str(assistant_content)
 
- def fixed_format_ai_wrapper(prompt):
+  def fixed_format_ai_wrapper(prompt):
     message = [{"role": "system", "content": instruction}]
     for example in example_pairs:
-        user_content = example["user_content"]
-        assistant_content = example["assistant_content"]
-        message.append({"role": "user", "content": user_content})
-        message.append({"role": "assistant", "content": assistant_content})
+      user_content = example["user_content"]
+      assistant_content = example["assistant_content"]
+      message.append({"role": "user", "content": user_content})
+      message.append({"role": "assistant", "content": assistant_content})
     message.append({"role": "user", "content": prompt})
     function_name = "print_"
     for prop in properties:
-        function_name += prop + "_"
+      function_name += prop + "_"
     function_name = function_name[:-1]
     function_description = "print"
     for prop in properties:
-        function_description += " " + prop + ","
+      function_description += " " + prop + ","
     function_description = function_description[:-1]
     for i in range(5):
-        try:
-            response = openai.ChatCompletion.create(
-                model="gpt-3.5-turbo-0613",
-                messages=message,
-                functions=[{
-                    "name": function_name,
-                    "description": function_description,
-                    "parameters": {
-                        "type": "object",
-                        "properties": properties,
-                    },
-                }],
-                function_call="auto",
-            )
-            message = response["choices"][0]["message"]
-            if message.get("function_call"):
-                arguments = eval(message["function_call"]["arguments"])
-                return arguments
-        except Exception as e:
-            if i < 4:  # if it's not the last attempt
-                print(f"Attempt {i + 2} failed, retrying in 5 seconds...")
-                time.sleep(5)  # wait for 5 seconds before next attempt
-            else:  # if it's the last attempt
-                print("All attempts failed.")
-                raise e  # re-raise the last exception
-    raise Exception("Unable to execute fixed_format_ai_wrapper after 5 attempts.")
+      try:
+        response = openai.ChatCompletion.create(
+          model="gpt-3.5-turbo-0613",
+          messages=message,
+          functions=[{
+            "name": function_name,
+            "description": function_description,
+            "parameters": {
+              "type": "object",
+              "properties": properties,
+            },
+          }],
+          function_call="auto",
+        )
+        message = response["choices"][0]["message"]
+        if message.get("function_call"):
+          arguments = eval(message["function_call"]["arguments"])
+          return arguments
+      except Exception as e:
+        if i < 4:  # if it's not the last attempt
+          print(f"Attempt {i + 2} failed, retrying in 5 seconds...")
+          time.sleep(5)  # wait for 5 seconds before next attempt
+        else:  # if it's the last attempt
+          print("All attempts failed.")
+          raise e  # re-raise the last exception
+    raise Exception(
+      "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
-  return fixed_format_ai_wrapper
+  return fixed_format_ai_wrapper
```

