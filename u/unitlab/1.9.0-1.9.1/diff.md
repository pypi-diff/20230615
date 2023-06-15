# Comparing `tmp/unitlab-1.9.0.tar.gz` & `tmp/unitlab-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.9.0.tar", last modified: Thu Jun 15 09:27:33 2023, max compression
+gzip compressed data, was "unitlab-1.9.1.tar", last modified: Thu Jun 15 10:30:57 2023, max compression
```

## Comparing `unitlab-1.9.0.tar` & `unitlab-1.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.936770 unitlab-1.9.0/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.9.0/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.9.0/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 09:27:33.936770 unitlab-1.9.0/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.9.0/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-15 09:27:33.936770 unitlab-1.9.0/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-15 09:21:00.000000 unitlab-1.9.0/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.932770 unitlab-1.9.0/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.932770 unitlab-1.9.0/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.9.0/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     1631 2023-06-14 17:52:10.000000 unitlab-1.9.0/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    11367 2023-06-14 17:52:57.000000 unitlab-1.9.0/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.9.0/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1671 2023-06-15 09:20:10.000000 unitlab-1.9.0/src/unitlab/run.py
--rw-rw-r--   0 me        (1000) me        (1000)     1933 2023-06-15 07:09:10.000000 unitlab-1.9.0/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 09:27:33.936770 unitlab-1.9.0/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-15 09:27:33.000000 unitlab-1.9.0/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 10:30:57.554186 unitlab-1.9.1/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.9.1/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.9.1/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 10:30:57.554186 unitlab-1.9.1/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.9.1/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-15 10:30:57.554186 unitlab-1.9.1/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-15 10:20:31.000000 unitlab-1.9.1/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 10:30:57.550186 unitlab-1.9.1/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 10:30:57.550186 unitlab-1.9.1/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.9.1/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1631 2023-06-15 09:37:56.000000 unitlab-1.9.1/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11359 2023-06-15 10:02:07.000000 unitlab-1.9.1/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.9.1/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1671 2023-06-15 09:37:16.000000 unitlab-1.9.1/src/unitlab/run.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1933 2023-06-15 09:38:00.000000 unitlab-1.9.1/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-15 10:30:57.554186 unitlab-1.9.1/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-15 10:30:57.000000 unitlab-1.9.1/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.9.0/LICENSE.md` & `unitlab-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.0/PKG-INFO` & `unitlab-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.9.0
+Version: 1.9.1
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.9.0/README.md` & `unitlab-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.0/setup.py` & `unitlab-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.9.0",
+    version="1.9.1",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.9.0/src/unitlab/cli.py` & `unitlab-1.9.1/src/unitlab/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,20 @@
             "headers": get_headers(api_key),
             "endpoint": ENDPOINTS["cli_task_datasources"].format(task_id),
         }
     )
     print(response.json())
 
 
-def task_workers(api_key, task_id):
+def task_members(api_key, task_id):
     response = send_request(
         {
             "method": "GET",
             "headers": get_headers(api_key),
-            "endpoint": ENDPOINTS["cli_task_workers"].format(task_id),
+            "endpoint": ENDPOINTS["cli_task_members"].format(task_id),
         }
     )
     print(response.json())
 
 
 def task_statistics(api_key, task_id):
     response = send_request(
```

### Comparing `unitlab-1.9.0/src/unitlab/client.py` & `unitlab-1.9.1/src/unitlab/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,26 +141,26 @@
                 "endpoint": ENDPOINTS["task_datasources"].format(task_id),
                 "headers": self._get_headers(),
             },
             session=self.api_session,
         )
         return response.json()
 
-    def task_workers(self, task_id):
-        """Get the workers of a task by id.
+    def task_members(self, task_id):
+        """Get members of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
-            The workers of a task.
+            Members of a task.
         """
         response = send_request(
             {
                 "method": "GET",
-                "endpoint": ENDPOINTS["task_workers"].format(task_id),
+                "endpoint": ENDPOINTS["task_members"].format(task_id),
                 "headers": self._get_headers(),
             },
             session=self.api_session,
         )
         return response.json()
 
     def task_statistics(self, task_id):
```

### Comparing `unitlab-1.9.0/src/unitlab/exceptions.py` & `unitlab-1.9.1/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.0/src/unitlab/run.py` & `unitlab-1.9.1/src/unitlab/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @task_app.command(help="Task datasources")
 def data(pk: UUID, api_key: API_KEY):
     cli.task_data(api_key, pk)
 
 
 @task_app.command(help="Task members")
 def members(pk: UUID, api_key: API_KEY):
-    cli.task_workers(api_key, pk)
+    cli.task_members(api_key, pk)
 
 
 @task_app.command(help="Task statistics")
 def statistics(pk: UUID, api_key: API_KEY):
     cli.task_statistics(api_key, pk)
```

### Comparing `unitlab-1.9.0/src/unitlab/utils.py` & `unitlab-1.9.1/src/unitlab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from .exceptions import AuthenticationError
 
 ENDPOINTS = {
     "check": "/api/check/",
     "tasks": "/api/sdk/tasks/",
     "task": "/api/sdk/tasks/{}/",
     "task_datasources": "/api/sdk/tasks/{}/datasources/",
-    "task_workers": "/api/sdk/tasks/{}/workers/",
+    "task_members": "/api/sdk/tasks/{}/members/",
     "task_statistics": "/api/sdk/tasks/{}/statistics/",
     "upload_data": "/api/sdk/upload-data/",
     "download_data": "/api/sdk/tasks/{}/download-data/",
     "datasets": "/api/sdk/datasets/",
     "dataset": "/api/sdk/datasets/{}/",
     "cli_tasks": "/api/cli/tasks/",
     "cli_task": "/api/cli/tasks/{}/",
     "cli_task_datasources": "/api/cli/tasks/{}/datasources/",
-    "cli_task_workers": "/api/cli/tasks/{}/workers/",
+    "cli_task_members": "/api/cli/tasks/{}/members/",
     "cli_task_statistics": "/api/cli/tasks/{}/statistics/",
     "cli_datasets": "/api/cli/datasets/",
 }
 
 
 def send_request(request, session=None):
     endpoint = request.pop("endpoint")
```

### Comparing `unitlab-1.9.0/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.9.1/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.9.0
+Version: 1.9.1
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

