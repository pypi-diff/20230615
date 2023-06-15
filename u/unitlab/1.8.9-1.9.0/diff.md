# Comparing `tmp/unitlab-1.8.9.tar.gz` & `tmp/unitlab-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.9.tar", last modified: Wed Jun 14 10:48:11 2023, max compression
+gzip compressed data, was "unitlab-1.9.0.tar", last modified: Thu Jun 15 09:27:33 2023, max compression
```

## Comparing `unitlab-1.8.9.tar` & `unitlab-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.9/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.9/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      685 2023-06-14 10:48:11.913919 unitlab-1.8.9/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.8.9/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-14 10:48:11.913919 unitlab-1.8.9/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-14 10:47:45.000000 unitlab-1.8.9/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.909919 unitlab-1.8.9/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.9/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     2112 2023-06-13 12:01:49.000000 unitlab-1.8.9/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    12257 2023-06-13 12:34:06.000000 unitlab-1.8.9/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.8.9/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-06-13 12:01:36.000000 unitlab-1.8.9/src/unitlab/run.py
--rw-rw-r--   0 me        (1000) me        (1000)     2103 2023-06-14 10:47:11.000000 unitlab-1.8.9/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 10:48:11.913919 unitlab-1.8.9/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      685 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-14 10:48:11.000000 unitlab-1.8.9/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.936770 unitlab-1.9.0/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.9.0/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.9.0/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 09:27:33.936770 unitlab-1.9.0/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.9.0/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-15 09:27:33.936770 unitlab-1.9.0/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-15 09:21:00.000000 unitlab-1.9.0/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.932770 unitlab-1.9.0/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.932770 unitlab-1.9.0/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.9.0/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1631 2023-06-14 17:52:10.000000 unitlab-1.9.0/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11367 2023-06-14 17:52:57.000000 unitlab-1.9.0/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.9.0/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1671 2023-06-15 09:20:10.000000 unitlab-1.9.0/src/unitlab/run.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1933 2023-06-15 07:09:10.000000 unitlab-1.9.0/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.936770 unitlab-1.9.0/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.9/LICENSE.md` & `unitlab-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.9/README.md` & `unitlab-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.9/setup.py` & `unitlab-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.9",
+    version="1.9.0",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.8.9/src/unitlab/cli.py` & `unitlab-1.9.0/src/unitlab/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,36 +56,14 @@
             "headers": get_headers(api_key),
             "endpoint": ENDPOINTS["cli_task_statistics"].format(task_id),
         }
     )
     print(response.json())
 
 
-def ai_models(api_key):
-    response = send_request(
-        {
-            "method": "GET",
-            "headers": get_headers(api_key),
-            "endpoint": ENDPOINTS["cli_ai_models"],
-        }
-    )
-    print(response.json())
-
-
-def ai_model(api_key, pk):
-    response = send_request(
-        {
-            "method": "GET",
-            "headers": get_headers(api_key),
-            "endpoint": ENDPOINTS["cli_ai_model"].format(pk),
-        }
-    )
-    print(response.json())
-
-
 def datasets(api_key):
     response = send_request(
         {
             "method": "GET",
             "headers": get_headers(api_key),
             "endpoint": ENDPOINTS["cli_datasets"],
         }
```

### Comparing `unitlab-1.8.9/src/unitlab/client.py` & `unitlab-1.9.0/src/unitlab/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -300,48 +300,14 @@
                 filename = f"task-data-{task_id}.json"
 
             with open(filename, "wb") as f:
                 for chunk in r.iter_content(chunk_size=1024 * 1024):
                     f.write(chunk)
         return os.path.abspath(filename)
 
-    def ai_models(self):
-        """Get a list of all ai models.
-
-        Returns:
-            A list of all ai models.
-        """
-        response = send_request(
-            {
-                "method": "GET",
-                "endpoint": ENDPOINTS["ai_models"],
-                "headers": self._get_headers(),
-            },
-            session=self.api_session,
-        )
-        return response.json()
-
-    def ai_model(self, ai_model_id):
-        """Get an ai model by id.
-
-        Args:
-            ai_model_id: The id of the ai model.
-        Returns:
-            An ai model.
-        """
-        response = send_request(
-            {
-                "method": "GET",
-                "endpoint": ENDPOINTS["ai_model"].format(ai_model_id),
-                "headers": self._get_headers(),
-            },
-            session=self.api_session,
-        )
-        return response.json()
-
     def datasets(self):
         """Get a list of all datasets.
 
         Returns:
             A list of all datasets.
         """
         response = send_request(
```

### Comparing `unitlab-1.8.9/src/unitlab/exceptions.py` & `unitlab-1.9.0/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.9/src/unitlab/utils.py` & `unitlab-1.9.0/src/unitlab/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 
 import requests
 
 from .exceptions import AuthenticationError
 
 ENDPOINTS = {
     "check": "/api/check/",
-    "ai_models": "/api/sdk/ai-models/",
-    "ai_model": "/api/sdk/ai-model/{}/",
     "tasks": "/api/sdk/tasks/",
     "task": "/api/sdk/tasks/{}/",
     "task_datasources": "/api/sdk/tasks/{}/datasources/",
     "task_workers": "/api/sdk/tasks/{}/workers/",
     "task_statistics": "/api/sdk/tasks/{}/statistics/",
     "upload_data": "/api/sdk/upload-data/",
     "download_data": "/api/sdk/tasks/{}/download-data/",
     "datasets": "/api/sdk/datasets/",
     "dataset": "/api/sdk/datasets/{}/",
-    "cli_ai_models": "/api/cli/ai-models/",
-    "cli_ai_model": "/api/cli/ai-model/{}/",
     "cli_tasks": "/api/cli/tasks/",
     "cli_task": "/api/cli/tasks/{}/",
     "cli_task_datasources": "/api/cli/tasks/{}/datasources/",
     "cli_task_workers": "/api/cli/tasks/{}/workers/",
     "cli_task_statistics": "/api/cli/tasks/{}/statistics/",
     "cli_datasets": "/api/cli/datasets/",
 }
```

