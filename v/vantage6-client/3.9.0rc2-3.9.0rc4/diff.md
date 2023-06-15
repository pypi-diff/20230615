# Comparing `tmp/vantage6-client-3.9.0rc2.tar.gz` & `tmp/vantage6-client-3.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-3.9.0rc2.tar", last modified: Tue May  9 13:37:04 2023, max compression
+gzip compressed data, was "vantage6-client-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
```

## Comparing `vantage6-client-3.9.0rc2.tar` & `vantage6-client-3.9.0rc4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:04.810855 vantage6-client-3.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    83897 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/dispatch_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19081 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.073726 vantage6-client-3.9.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.073726 vantage6-client-3.9.0rc4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    83916 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/dispatch_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-3.9.0rc2/PKG-INFO` & `vantage6-client-3.9.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc4 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.9.0rc2/setup.py` & `vantage6-client-3.9.0rc4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'pandas==1.5.3',
         'PyJWT==2.6.0',
         'pyfiglet==0.8.post1',
-        'requests==2.28.2',
+        'requests==2.31.0',
         'SPARQLWrapper==2.0.0',
         'qrcode==7.3.1',
         f'vantage6-common=={version_ns["__version__"]}',
     ],
     tests_require=["pytest"],
     package_data={
         'vantage6.client': [
```

### Comparing `vantage6-client-3.9.0rc2/tests/test_client.py` & `vantage6-client-3.9.0rc4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/tests/test_deserialization.py` & `vantage6-client-3.9.0rc4/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/tests/test_docker_wrapper.py` & `vantage6-client-3.9.0rc4/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/tests/test_serialization.py` & `vantage6-client-3.9.0rc4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/__init__.py` & `vantage6-client-3.9.0rc4/vantage6/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         AssertionError
             Refresh URL not found
         """
         self.log.info("Refreshing token")
         assert self.__refresh_url, \
             "Refresh URL not found, did you authenticate?"
 
-        # if no port is specified explicit, then it should be omnit the
+        # if no port is specified explicit, then it should be omit the
         # colon : in the path. Similar (but different) to the property
         # base_path
         if self.__port:
             url = f"{self.__host}:{self.__port}{self.__refresh_url}"
         else:
             url = f"{self.__host}{self.__refresh_url}"
 
@@ -511,15 +511,15 @@
             "description": description,
             "organizations": organization_json_list,
             'database': database
         })
 
     # TODO BvB 23-01-23 remove this method in v4+ (or make it private?). It is
     # only here for backwards compatibility.
-    def get_results(self, id: int = None, state: str = None,
+    def get_results(self, id_: int = None, state: str = None,
                     include_task: bool = False, task_id: int = None,
                     node_id: int = None, params: dict = {}) -> dict:
         """Get task result(s) from the central server
 
         Depending if a `id` is specified or not, either a single or a
         list of results is returned. The input and result field of the
         result are attempted te be decrypted. This fails if the public
@@ -529,15 +529,15 @@
         Parameters
         ----------
         id : int, optional
             Id of the result, by default None
         state : str, optional
             The state of the task (e.g. `open`), by default None
         include_task : bool, optional
-            Whenever to include the orginating task, by default False
+            Whenever to include the originating task, by default False
         task_id : int, optional
             The id of the originating task, this will return all results
             belonging to this task, by default None
         node_id : int, optional
             The id of the node at which this result has been produced,
             this will return all results from this node, by default None
         params : dict, optional
@@ -545,40 +545,41 @@
 
         Returns
         -------
         dict
             Containing the result(s)
         """
         # Determine endpoint and create dict with query parameters
-        endpoint = 'result' if not id else f'result/{id}'
+        endpoint = 'result' if not id_ else f'result/{id_}'
 
+        extended_params = params.copy()
         if state:
-            params['state'] = state
+            extended_params['state'] = state
         if include_task:
-            params['include'] = 'task'
+            extended_params['include'] = 'task'
         if task_id:
-            params['task_id'] = task_id
+            extended_params['task_id'] = task_id
         if node_id:
-            params['node_id'] = node_id
+            extended_params['node_id'] = node_id
 
         # self.log.debug(f"Retrieving results using query parameters:{params}")
-        results = self.request(endpoint=endpoint, params=params)
+        results = self.request(endpoint=endpoint, params=extended_params)
 
         if isinstance(results, str):
             self.log.warn("Requesting results failed")
             self.log.debug(f"Results message: {results}")
             return {}
 
         # hack: in the case that the pagination metadata is included we
         # need to strip that for decrypting
         if isinstance(results, dict) and 'data' in results:
             wrapper = results
             results = results['data']
 
-        if id:
+        if id_:
             # Single result
             self._decrypt_result(results)
 
         else:
             # Multiple results
             for result in results:
                 self._decrypt_result(result)
@@ -1959,15 +1960,16 @@
             -------
             dict
                 Containing the result data
             """
             self.parent.log.info('--> Attempting to decrypt results!')
 
             # get_results also handles decryption
-            result = self.parent.get_results(id=id_, include_task=include_task)
+            result = self.parent.get_results(id_=id_,
+                                             include_task=include_task)
             result_data = result.get('result')
             if result_data:
                 try:
                     result['result'] = deserialization.load_data(result_data)
                 except Exception as e:
                     self.parent.log.warn('--> Failed to deserialize')
                     self.parent.log.debug(e)
@@ -1977,15 +1979,15 @@
         @post_filtering()
         def list(self, task: int = None, organization: int = None,
                  state: str = None, node: int = None,
                  include_task: bool = False, started: tuple[str, str] = None,
                  assigned: tuple[str, str] = None,
                  finished: tuple[str, str] = None, port: int = None,
                  page: int = None, per_page: int = None,
-                 include_metadata: bool = True) -> list:
+                 include_metadata: bool = True) -> dict | list[dict]:
             """List results
 
             Parameters
             ----------
             task: int, optional
                 Filter by task id
             organization: int, optional
@@ -2066,16 +2068,14 @@
 
             if 'wrapper' in locals():
                 wrapper['data'] = cleaned_results
                 cleaned_results = wrapper
 
             return cleaned_results
 
-        # note: using typing.List instead of `list` to prevent referring
-        # to the list() function in an incorrect manner
         def from_task(
             self, task_id: int, include_task: bool = False
         ) -> typing.List[dict]:
             """
             Get all results from a specific task
 
             Parameters
```

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/_version.py` & `vantage6-client-3.9.0rc4/vantage6/client/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/algorithm_client.py` & `vantage6-client-3.9.0rc4/vantage6/client/algorithm_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/deserialization.py` & `vantage6-client-3.9.0rc4/vantage6/client/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/filter.py` & `vantage6-client-3.9.0rc4/vantage6/client/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,46 +227,46 @@
         The filtered list of dicts.
     """
     if filters:
         return filter_dicts_on_values(dicts, filters)
     return dicts
 
 
-def filter_dicts_keys(dicts: list[dict], keys: list[Any]) -> list[dict]:
+def filter_dicts_keys(dicts: list[dict], keys: list[str]) -> list[dict]:
     """
     Filter a list of dicts on the specified keys. If no keys are given, the
     original list of dicts is returned.
 
     Parameters
     ----------
     dicts : list[dict]
         The list of dicts to filter.
-    keys : list[Any]
+    keys : list[str]
         A list of keys to keep in the dictionaries
 
     Returns
     -------
     list[dict]
         The filtered list of dicts.
     """
     if keys:
         return [filter_dict_keys(adict, keys) for adict in dicts]
     return dicts
 
 
-def filter_dict_keys(dict_: dict, keys: list[Any]) -> dict:
+def filter_dict_keys(dict_: dict, keys: list[str]) -> dict:
     """
     Filter a dict on the specified keys. If no keys are given, the original
     dict is returned.
 
     Parameters
     ----------
     dict_ : dict
         The dict to filter.
-    keys : list[Any]
+    keys : list[str]
         A list of keys to keep in the dictionary
 
     Returns
     -------
     dict
         The filtered dict.
     """
```

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/serialization.py` & `vantage6-client-3.9.0rc4/vantage6/client/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/client/utils.py` & `vantage6-client-3.9.0rc4/vantage6/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/deserialization.py` & `vantage6-client-3.9.0rc4/vantage6/tools/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/dispatch_rpc.py` & `vantage6-client-3.9.0rc4/vantage6/tools/dispatch_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import os
 import importlib
 import jwt
+import traceback
 
-from types import ModuleType
 from typing import Any
 
 from vantage6.client import ContainerClient
 from vantage6.client.algorithm_client import AlgorithmClient
 from vantage6.tools.util import info, warn, error
 
 
-def dispatch_rpc(data: Any, input_data: dict, module: ModuleType, token: str,
-                 use_new_client: bool = False) -> Any:
+def dispatch_rpc(data: Any, input_data: dict, module: str, token: str,
+                 use_new_client: bool = False, log_traceback=False) -> Any:
     """
     Load the algorithm module and call the correct method to run an algorithm.
 
     Parameters
     ----------
     data : Any
         The data that is passed to the algorithm.
     input_data : dict
         The input data that is passed to the algorithm. This should at least
         contain the key 'method' which is the name of the method that should be
         called. Another often used key is 'master' which indicates that this
         container is a master container. Other keys depend on the algorithm.
-    module : ModuleType
-        The module that contains the algorithm.
+    module : str
+        The name of the module that contains the algorithm.
     token : str
         The JWT token that is used to authenticate from the algorithm container
         to the server.
     use_new_client : bool, optional
         Whether to use the new client or the old client, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
 
     Returns
     -------
     Any
         The result of the algorithm.
     """
     # import algorithm module
@@ -93,11 +98,13 @@
     kwargs = input_data.get("kwargs", {})
 
     # try to run the method
     try:
         result = method(client, data, *args, **kwargs) if master else \
                  method(data, *args, **kwargs)
     except Exception as e:
-        warn(f"Error encountered while calling {method_name}: {e}")
+        error(f"Error encountered while calling {method_name}: {e}")
+        if log_traceback:
+            error(traceback.print_exc())
         exit(1)
 
     return result
```

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/mock_client.py` & `vantage6-client-3.9.0rc4/vantage6/tools/mock_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import pandas
 import pickle
 
-from types import ModuleType
 from importlib import import_module
 
 
 class ClientMockProtocol:
     """
     The ClientMockProtocol is used to test your algorithm locally. It
     mimics the behaviour of the client and its communication with the server.
 
     Parameters
     ----------
     datasets : list[str]
         A list of paths to the datasets that are used in the algorithm.
-    module : ModuleType
-        The module that contains the algorithm.
+    module : str
+        The name of the module that contains the algorithm.
     """
-    def __init__(self, datasets: list[str], module: ModuleType) -> None:
+    def __init__(self, datasets: list[str], module: str) -> None:
         self.n = len(datasets)
         self.datasets = []
         for dataset in datasets:
             self.datasets.append(
                 pandas.read_csv(dataset)
             )
 
         self.lib = import_module(module)
         self.tasks = []
 
     # TODO in v4+, don't provide a default value for list? There is no use
     # in calling this function with 0 organizations as the task will never
     # be executed in that case.
     def create_new_task(self, input_: dict,
-                        organization_ids: list[int] = []) -> int:
+                        organization_ids: list[int] = None) -> int:
         """
         Create a new task with the MockProtocol and return the task id.
 
         Parameters
         ----------
         input_ : dict
             The input data that is passed to the algorithm. This should at
@@ -48,14 +47,16 @@
             A list of organization ids that should run the algorithm.
 
         Returns
         -------
         int
             The id of the task.
         """
+        if organization_ids is None:
+            organization_ids = []
 
         # extract method from lib and input
         master = input_.get("master")
 
         method_name = input_.get("method")
         if master:
             method = getattr(self.lib, method_name)
@@ -124,15 +125,15 @@
         for result in task.get("results"):
             print(result)
             res = pickle.loads(result.get("result"))
             results.append(res)
 
         return results
 
-    def get_organizations_in_my_collaboration(self):
+    def get_organizations_in_my_collaboration(self) -> list[dict]:
         """
         Get mocked organizations.
 
         Returns
         -------
         list[dict]
             A list of mocked organizations.
```

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/serialization.py` & `vantage6-client-3.9.0rc4/vantage6/tools/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/util.py` & `vantage6-client-3.9.0rc4/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc2/vantage6/tools/wrapper.py` & `vantage6-client-3.9.0rc4/vantage6/tools/wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,28 +43,34 @@
 _DATA_FORMAT_SEPARATOR = '.'
 _MAX_FORMAT_STRING_LENGTH = 10
 
 _SPARQL_RETURN_FORMAT = CSV
 
 
 def auto_wrapper(module: str, load_data: bool = True,
-                 use_new_client: bool = False) -> None:
+                 use_new_client: bool = False,
+                 log_traceback: bool = False) -> None:
     """
     Wrap an algorithm module to provide input and output handling for the
     vantage6 infrastructure. This function will automatically select the
     correct wrapper based on the database type.
 
     Parameters
     ----------
     module : str
         Python module name of the algorithm to wrap.
     load_data : bool, optional
         Wether to load the data or not, by default True
     use_new_client : bool, optional
         Wether to use the new client or not, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
     """
 
     # Get the database label from the environment variable, this variable is
     # set by the client/user/researcher.
     try:
         label = os.environ["USER_REQUESTED_DATABASE_LABEL"]
     except KeyError:
@@ -76,103 +82,128 @@
     database_type = os.environ.get(f"{label.upper()}_DATABASE_TYPE", "csv")\
         .lower()
 
     # Create the correct wrapper based on the database type, note that the
     # multi database wrapper is not available.
     if database_type == "csv":
         wrapper = CSVWrapper()
-    if database_type == "excel":
+    elif database_type == "excel":
         wrapper = ExcelWrapper()
     elif database_type == "sparql":
         wrapper = SparqlDockerWrapper()
     elif database_type == "parquet":
         wrapper = ParquetWrapper()
     elif database_type == "sql":
         wrapper = SQLWrapper()
     elif database_type == "omop":
         wrapper = OMOPWrapper()
     else:
         error(f"Unknown database type: {database_type}")
         return
 
     # Execute the algorithm with the correct data wrapper
-    wrapper.wrap_algorithm(module, load_data, use_new_client)
+    wrapper.wrap_algorithm(module, load_data, use_new_client, log_traceback)
 
 
 def docker_wrapper(module: str, load_data: bool = True,
-                   use_new_client: bool = False) -> None:
+                   use_new_client: bool = False,
+                   log_traceback: bool = False) -> None:
     """
     Specific wrapper for CSV only data sources. Use the ``auto_wrapper``
     to automatically select the correct wrapper based on the database type.
 
     Parameters
     ----------
     module : str
         Module name of the algorithm package.
     load_data : bool, optional
         Whether to load the data into a pandas DataFrame or not, by default
         True
     use_new_client : bool, optional
         Whether to use the new or old client, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
     """
     wrapper = DockerWrapper()
-    wrapper.wrap_algorithm(module, load_data, use_new_client)
+    wrapper.wrap_algorithm(module, load_data, use_new_client, log_traceback)
 
 
-def sparql_wrapper(module: str, use_new_client: bool = False) -> None:
+def sparql_wrapper(module: str, use_new_client: bool = False,
+                   log_traceback: bool = False) -> None:
     """
     Specific wrapper for SPARQL only data sources. Use the ``auto_wrapper``
     to automatically select the correct wrapper based on the database type.
 
     Parameters
     ----------
     module : str
         Module name of the algorithm package.
     use_new_client : bool, optional
         Whether to use the new or old client, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
     """
     wrapper = SparqlDockerWrapper()
-    wrapper.wrap_algorithm(module, use_new_client)
+    wrapper.wrap_algorithm(module, use_new_client, log_traceback)
 
 
-def parquet_wrapper(module: str, use_new_client: bool = False) -> None:
+def parquet_wrapper(module: str, use_new_client: bool = False,
+                    log_traceback: bool = False) -> None:
     """
     Specific wrapper for Parquet only data sources. Use the ``auto_wrapper``
     to automatically select the correct wrapper based on the database type.
 
     Parameters
     ----------
     module : str
         Module name of the algorithm package.
     use_new_client : bool, optional
         Whether to use the new or old client, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
     """
     wrapper = ParquetWrapper()
-    wrapper.wrap_algorithm(module, use_new_client)
+    wrapper.wrap_algorithm(module, use_new_client, log_traceback)
 
 
-def multidb_wrapper(module: str, use_new_client: bool = False) -> None:
+def multidb_wrapper(module: str, use_new_client: bool = False,
+                    log_traceback: bool = False) -> None:
     """
     Specific wrapper for multiple data sources.
 
     Parameters
     ----------
     module : str
         Module name of the algorithm package.
     use_new_client : bool, optional
         Whether to use the new or old client, by default False
+    log_traceback: bool, optional
+        Whether to print the full error message from algorithms or not, by
+        default False. Algorithm developers should only use this option if
+        they are sure that the error message does not contain any sensitive
+        information. By default False.
     """
     wrapper = MultiDBWrapper()
-    wrapper.wrap_algorithm(module, use_new_client)
+    wrapper.wrap_algorithm(module, use_new_client, log_traceback)
 
 
 class WrapperBase(ABC):
 
     def wrap_algorithm(self, module: str, load_data: bool = True,
-                       use_new_client: bool = False) -> None:
+                       use_new_client: bool = False,
+                       log_traceback: bool = False) -> None:
         """
         Wrap an algorithm module to provide input and output handling for the
         vantage6 infrastructure.
 
         Data is received in the form of files, whose location should be
         specified in the following environment variables:
 
@@ -208,14 +239,22 @@
         Parameters
         ----------
         module : str
             Python module name of the algorithm to wrap.
         load_data : bool, optional
             Whether to load the data into a pandas DataFrame or not, by default
             True
+        use_new_client: bool
+            Whether to use the new AlgorithmClient or the old ContainerClient,
+            by default False
+        log_traceback: bool
+            Whether to print the full error message from algorithms or not, by
+            default False. Algorithm developers should only use this option if
+            they are sure that the error message does not contain any sensitive
+            information.
         """
         info(f"wrapper for {module}")
 
         # read input from the mounted input file.
         input_file = os.environ["INPUT_FILE"]
         info(f"Reading input file {input_file}")
 
@@ -238,15 +277,16 @@
         if load_data:
             data = self.load_data(database_uri, input_data)
         else:
             data = None
 
         # make the actual call to the method/function
         info("Dispatching ...")
-        output = dispatch_rpc(data, input_data, module, token, use_new_client)
+        output = dispatch_rpc(data, input_data, module, token, use_new_client,
+                              log_traceback)
 
         # write output from the method to mounted output file. Which will be
         # transferred back to the server by the node-instance.
         output_file = os.environ["OUTPUT_FILE"]
         info(f"Writing output to {output_file}")
 
         output_format = input_data.get('output_format', None)
```

### Comparing `vantage6-client-3.9.0rc2/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-3.9.0rc4/vantage6_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc4 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.9.0rc2/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-3.9.0rc4/vantage6_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

