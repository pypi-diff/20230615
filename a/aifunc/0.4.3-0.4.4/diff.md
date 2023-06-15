# Comparing `tmp/aifunc-0.4.3.tar.gz` & `tmp/aifunc-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.4.3.tar", max compression
+gzip compressed data, was "aifunc-0.4.4.tar", max compression
```

## Comparing `aifunc-0.4.3.tar` & `aifunc-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.3/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.3/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.3/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.3/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.3/aifunc/generate_question.py
--rw-r--r--   0        0        0     6766 2023-06-15 04:36:19.130622 aifunc-0.4.3/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-15 04:38:42.352924 aifunc-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.4/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.4/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.4/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.4/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.4/aifunc/generate_question.py
+-rw-r--r--   0        0        0     6753 2023-06-15 04:39:58.236501 aifunc-0.4.4/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-15 04:40:15.046180 aifunc-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.4/PKG-INFO
```

### Comparing `aifunc-0.4.3/aifunc/add_ai_function.py` & `aifunc-0.4.4/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.4.3/aifunc/utility.py` & `aifunc-0.4.4/aifunc/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   ai_function.__name__ = function_name  # Set the function name
   return ai_function
 
 
 def create_ai_function_from_yaml(yaml_file):
   import requests
   import yaml
-  url = 'https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/fixed_format/' + yaml_file
+  url = 'https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/' + yaml_file
   response = requests.get(url)
   if response.status_code == 200:
     yaml_data = response.text
     data = yaml.safe_load(yaml_data)
   else:
     print("Failed to load YAML file.")
     exit(0)
```

