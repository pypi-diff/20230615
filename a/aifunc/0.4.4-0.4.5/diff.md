# Comparing `tmp/aifunc-0.4.4.tar.gz` & `tmp/aifunc-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.4.4.tar", max compression
+gzip compressed data, was "aifunc-0.4.5.tar", max compression
```

## Comparing `aifunc-0.4.4.tar` & `aifunc-0.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.4/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.4/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.4/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.4/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.4/aifunc/generate_question.py
--rw-r--r--   0        0        0     6753 2023-06-15 04:39:58.236501 aifunc-0.4.4/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-15 04:40:15.046180 aifunc-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.5/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.5/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.5/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.5/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.5/aifunc/generate_question.py
+-rw-r--r--   0        0        0     6690 2023-06-15 05:02:10.949575 aifunc-0.4.5/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-15 05:06:50.997504 aifunc-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.5/PKG-INFO
```

### Comparing `aifunc-0.4.4/aifunc/add_ai_function.py` & `aifunc-0.4.5/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.4.4/aifunc/utility.py` & `aifunc-0.4.5/aifunc/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,15 @@
     message = [{"role": "system", "content": instruction}]
     for example in example_pairs:
       user_content = example["user_content"]
       assistant_content = example["assistant_content"]
       message.append({"role": "user", "content": user_content})
       message.append({"role": "assistant", "content": assistant_content})
     message.append({"role": "user", "content": prompt})
-    function_name = "print_"
-    for prop in properties:
-      function_name += prop + "_"
-    function_name = function_name[:-1]
+    function_name = "print_parametes"
     function_description = "print"
     for prop in properties:
       function_description += " " + prop + ","
     function_description = function_description[:-1]
     for i in range(5):
       try:
         response = openai.ChatCompletion.create(
@@ -166,21 +163,23 @@
             "parameters": {
               "type": "object",
               "properties": properties,
             },
           }],
           function_call="auto",
         )
-        message = response["choices"][0]["message"]
-        if message.get("function_call"):
-          arguments = eval(message["function_call"]["arguments"])
+        response = response["choices"][0]["message"]
+        if response.get("function_call"):
+          arguments = eval(response["function_call"]["arguments"])
           return arguments
+        else:
+          raise
       except Exception as e:
         if i < 4:  # if it's not the last attempt
-          print(f"Attempt {i + 2} failed, retrying in 5 seconds...")
+          print(f"Attempt {i} failed, retrying in 5 seconds...")
           time.sleep(5)  # wait for 5 seconds before next attempt
         else:  # if it's the last attempt
           print("All attempts failed.")
           raise e  # re-raise the last exception
     raise Exception(
       "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
```

