# Comparing `tmp/mythic-0.1.2.tar.gz` & `tmp/mythic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.2.tar", last modified: Tue May 23 19:10:52 2023, max compression
+gzip compressed data, was "mythic-0.1.3.tar", last modified: Thu Jun 15 15:55:58 2023, max compression
```

## Comparing `mythic-0.1.2.tar` & `mythic-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.999088 mythic-0.1.2/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-23 19:10:51.998706 mythic-0.1.2/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1707 2023-05-10 02:44:23.000000 mythic-0.1.2/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.996771 mythic-0.1.2/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.2/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.2/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    99712 2023-05-17 20:24:46.000000 mythic-0.1.2/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3373 2023-05-23 19:10:45.000000 mythic-0.1.2/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.2/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7731 2023-05-23 19:09:57.000000 mythic-0.1.2/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.998289 mythic-0.1.2/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-23 19:10:51.999186 mythic-0.1.2/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      818 2023-05-23 19:10:30.000000 mythic-0.1.2/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-06-15 15:55:58.843225 mythic-0.1.3/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-06-15 15:55:58.842979 mythic-0.1.3/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1707 2023-05-10 02:44:23.000000 mythic-0.1.3/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-06-15 15:55:58.840784 mythic-0.1.3/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.3/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.3/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)   102657 2023-06-15 15:37:47.000000 mythic-0.1.3/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3373 2023-06-15 15:55:34.000000 mythic-0.1.3/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.3/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7731 2023-05-23 19:09:57.000000 mythic-0.1.3/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-06-15 15:55:58.842513 mythic-0.1.3/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-06-15 15:55:58.000000 mythic-0.1.3/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-06-15 15:55:58.000000 mythic-0.1.3/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-06-15 15:55:58.000000 mythic-0.1.3/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-06-15 15:55:58.000000 mythic-0.1.3/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-06-15 15:55:58.000000 mythic-0.1.3/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-06-15 15:55:58.843323 mythic-0.1.3/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      818 2023-06-15 15:55:27.000000 mythic-0.1.3/setup.py
```

### Comparing `mythic-0.1.2/PKG-INFO` & `mythic-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.2/README.md` & `mythic-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.2/mythic/graphql_queries.py` & `mythic-0.1.3/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.2/mythic/mythic.py` & `mythic-0.1.3/mythic/mythic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1151,17 +1151,59 @@
     ):
         aggregated_output = result["task_stream"][0]["responses"]
         if "error" in result["task_stream"][0]["status"] or result["task_stream"][0]["completed"]:
             break
     final_output = b""
     for output in aggregated_output:
         final_output += base64.b64decode(output["response_text"])
+    subtaskIds = await get_all_subtask_ids(mythic=mythic, task_display_id=task_display_id, fetch_display_id_instead=True)
+    for subtask in subtaskIds:
+        subtaskOutput = await get_all_task_output_by_id(mythic=mythic, task_display_id=subtask)
+        for r in subtaskOutput:
+            final_output += base64.b64decode(r["response_text"])
     return final_output
 
 
+async def get_all_subtask_ids(mythic: mythic_classes.Mythic, task_display_id: int,
+                              fetch_display_id_instead: bool) -> List[int]:
+    subtaskIds = []
+    idQuery = f"""
+    query taskIdFromDisplayID($task_display_id: Int!){{
+        task(where: {{display_id: {{_eq: $task_display_id}}}}){{
+            id
+        }}
+    }}
+    """
+    subtaskQuery = """
+    query subtaskList($task_id: Int!){
+        task(where: {parent_task_id: {_eq: $task_id}}){
+            id
+            display_id
+        }
+    }
+    """
+    initial = await mythic_utilities.graphql_post(
+        mythic=mythic, query=idQuery, variables={"task_display_id": task_display_id}
+    )
+    if initial["task"]:
+        taskIdsToCheck = [initial["task"][0]["id"]]
+        while len(taskIdsToCheck) > 0:
+            currentTaskId = taskIdsToCheck.pop()
+            subtasks = await mythic_utilities.graphql_post(
+                mythic=mythic, query=subtaskQuery, variables={"task_id": currentTaskId}
+            )
+            for t in subtasks["task"]:
+                taskIdsToCheck.append(t["id"])
+                if fetch_display_id_instead:
+                    subtaskIds.append(t["display_id"])
+                else:
+                    subtaskIds.append(t["id"])
+    return subtaskIds
+
+
 async def get_all_task_output(
         mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10
 ) -> AsyncGenerator:
     """
     Execute a query to get all current responses.
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_output_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
@@ -1593,14 +1635,37 @@
         if len(output["filemeta"]) > 0:
             yield output["filemeta"]
             offset += len(output["filemeta"])
         else:
             break
 
 
+async def get_latest_uploaded_file_by_name(
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None, filename: str = None,
+) -> dict:
+    """
+    Execute a query to get metadata about the uploaded file by name.
+    To download the contents of a file, use the `download_file` function with the agent_file_id.
+    The default set of attributes returned in the dictionary can be found at graphql_queries.file_data_fragment.
+    If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
+    """
+    file_query = f"""
+    query uploaded_file_by_name($filename: String!){{
+        filemeta(where: {{is_screenshot: {{_eq: false}}, is_download_from_agent: {{_eq: false}}, is_payload: {{_eq: false}}, deleted: {{_eq: false}}, filename_utf8: {{_eq: $filename}}}}, order_by: {{id: desc}}, limit: 1){{
+            {custom_return_attributes if custom_return_attributes is not None else '...file_data_fragment'}
+        }}
+    }}
+    {graphql_queries.file_data_fragment if custom_return_attributes is None else ''}
+    """
+    output = await mythic_utilities.graphql_post(
+        mythic=mythic, query=file_query,
+    )
+    return output["filemeta"][0] if output["filemeta"] else {}
+
+
 async def update_file_comment(
         mythic: mythic_classes.Mythic, file_uuid: str, comment: str
 ) -> dict:
     """
     Update a file's comment within Mythic
     """
     update_comment_mutation = """
@@ -2229,15 +2294,16 @@
       create_c2_instance(c2_instance: $c2_instance, instance_name: $instance_name, c2profile_id: $c2profile_id){
         status
         error
       }
     }
     """
     resp = await mythic_utilities.graphql_post(mythic=mythic, query=mutation, variables={
-        "instance_name": instance_name, "c2profile_id": resp["c2profile"][0]["id"], "c2_instance": json.dumps(c2_parameters)
+        "instance_name": instance_name, "c2profile_id": resp["c2profile"][0]["id"],
+        "c2_instance": json.dumps(c2_parameters)
     })
     return resp["create_c2_instance"]
 
 
 # ####### Tag Functions ############
```

### Comparing `mythic-0.1.2/mythic/mythic_classes.py` & `mythic-0.1.3/mythic/mythic_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.2"
+        self.scripting_version = "0.1.3"
         self.current_operation_id = 0
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
```

### Comparing `mythic-0.1.2/mythic/mythic_utilities.py` & `mythic-0.1.3/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.2/mythic.egg-info/PKG-INFO` & `mythic-0.1.3/mythic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.2/setup.py` & `mythic-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.2",
+    version="0.1.3",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

