# Comparing `tmp/cq23-1.8.0.tar.gz` & `tmp/cq23-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.8.0.tar", last modified: Wed Jun 14 13:53:09 2023, max compression
+gzip compressed data, was "cq23-1.9.0.tar", last modified: Thu Jun 15 15:18:11 2023, max compression
```

## Comparing `cq23-1.8.0.tar` & `cq23-1.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 13:53:09.150584 cq23-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 13:53:00.000000 cq23-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 13:53:00.000000 cq23-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-14 13:53:09.150584 cq23-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 13:53:00.000000 cq23-1.8.0/src/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-14 13:53:00.000000 cq23-1.8.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-14 13:53:00.000000 cq23-1.8.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 13:53:09.000000 cq23-1.8.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 13:53:00.000000 cq23-1.8.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-14 13:53:00.000000 cq23-1.8.0/src/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.146584 cq23-1.8.0/src/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-14 13:53:00.000000 cq23-1.8.0/src/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-14 13:53:00.000000 cq23-1.8.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/web_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-14 13:53:00.000000 cq23-1.8.0/src/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:09.150584 cq23-1.8.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:00.000000 cq23-1.8.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-14 13:53:00.000000 cq23-1.8.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-15 15:18:11.984197 cq23-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 15:18:03.000000 cq23-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 15:18:03.000000 cq23-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 15:18:11.988198 cq23-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.976197 cq23-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 15:18:03.000000 cq23-1.9.0/src/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-15 15:18:03.000000 cq23-1.9.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 15:18:03.000000 cq23-1.9.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.980197 cq23-1.9.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 15:18:11.000000 cq23-1.9.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 15:18:03.000000 cq23-1.9.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-15 15:18:03.000000 cq23-1.9.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-15 15:18:03.000000 cq23-1.9.0/src/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-15 15:18:03.000000 cq23-1.9.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/web_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-15 15:18:03.000000 cq23-1.9.0/src/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:11.984197 cq23-1.9.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:18:03.000000 cq23-1.9.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-15 15:18:03.000000 cq23-1.9.0/src/zip/command.py
```

### Comparing `cq23-1.8.0/PKG-INFO` & `cq23-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.8.0/setup.cfg` & `cq23-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.8.0
+version = 1.9.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.8.0/src/admin/aws.py` & `cq23-1.9.0/src/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/admin/builder.py` & `cq23-1.9.0/src/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/admin/worker.py` & `cq23-1.9.0/src/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/check/command.py` & `cq23-1.9.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/cleanup/command.py` & `cq23-1.9.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.9.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-1.8.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.9.0/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/main/command.py` & `cq23-1.9.0/src/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/main/utils.py` & `cq23-1.9.0/src/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/new_client/command.py` & `cq23-1.9.0/src/new_client/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     if not args:
         print("You must specify the language for the client: cq23 new python my_bot")
         return
 
     language_map = {
         "raw": "https://github.com/CALED-Team/codequest23-raw-submission.git",
         "python": "https://github.com/CALED-Team/codequest23-python-submission.git",
+        "cpp": "https://github.com/CALED-Team/codequest23-cpp-submission.git",
     }
     language = args[0]
 
     if language not in language_map.keys():
         return print(
             "Invalid language selected for the new bot. Language should be one of:",
             "[" + " - ".join(language_map.keys()) + "]",
```

### Comparing `cq23-1.8.0/src/replay/command.py` & `cq23-1.9.0/src/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/run_game/command.py` & `cq23-1.9.0/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/run_game/docker_tools.py` & `cq23-1.9.0/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/run_game/gcs.py` & `cq23-1.9.0/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/web_server/flask_api.py` & `cq23-1.9.0/src/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-1.8.0/src/zip/command.py` & `cq23-1.9.0/src/zip/command.py`

 * *Files identical despite different names*

