# Comparing `tmp/aifunc-0.3.7.tar.gz` & `tmp/aifunc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.3.7.tar", max compression
+gzip compressed data, was "aifunc-0.4.0.tar", max compression
```

## Comparing `aifunc-0.3.7.tar` & `aifunc-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      176 2023-06-14 15:08:17.823020 aifunc-0.3.7/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.3.7/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.3.7/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.3.7/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.7/aifunc/generate_question.py
--rw-r--r--   0        0        0     3400 2023-06-14 01:42:54.282815 aifunc-0.3.7/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-14 15:08:34.568319 aifunc-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      102 2023-06-15 03:22:13.011275 aifunc-0.4.0/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.4.0/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.4.0/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.4.0/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.4.0/aifunc/generate_question.py
+-rw-r--r--   0        0        0     5373 2023-06-15 03:20:26.008282 aifunc-0.4.0/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-15 03:26:59.200678 aifunc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.4.0/PKG-INFO
```

### Comparing `aifunc-0.3.7/aifunc/add_ai_function.py` & `aifunc-0.4.0/aifunc/add_ai_function.py`

 * *Files identical despite different names*

