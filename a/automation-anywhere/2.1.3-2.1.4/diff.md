# Comparing `tmp/automation_anywhere-2.1.3.tar.gz` & `tmp/automation_anywhere-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.1.3.tar", last modified: Wed May 31 14:30:47 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.4.tar", last modified: Thu Jun 15 15:05:28 2023, max compression
```

## Comparing `automation_anywhere-2.1.3.tar` & `automation_anywhere-2.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/LICENSE
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.3/README.md
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/automation_anywhere/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.3/automation_anywhere/base.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/automation_anywhere/errors.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10423 2023-05-31 14:29:22.000000 automation_anywhere-2.1.3/automation_anywhere/executor.py
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/automation_anywhere.egg-info/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/SOURCES.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/dependency_links.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/top_level.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-31 14:29:48.000000 automation_anywhere-2.1.3/pyproject.toml
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3470 2023-06-15 15:04:13.000000 automation_anywhere-2.1.4/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.4/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.4/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    11716 2023-06-15 14:56:44.000000 automation_anywhere-2.1.4/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-06-15 15:05:28.000000 automation_anywhere-2.1.4/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-06-15 15:01:54.000000 automation_anywhere-2.1.4/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-06-15 15:05:28.992704 automation_anywhere-2.1.4/setup.cfg
```

### Comparing `automation_anywhere-2.1.3/LICENSE` & `automation_anywhere-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.3/PKG-INFO` & `automation_anywhere-2.1.4/automation_anywhere.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: automation_anywhere
-Version: 2.1.3
+Name: automation-anywhere
+Version: 2.1.4
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,28 +34,28 @@
 
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     aa_executor = Executor(base_url, username, password)
-    devices, _, error = aa_executor.list_devices()
+    devices, _, error = aa_executor.list_devices(hostname='host', run_as_user='user_to_run_as')
     if error is not None:
       # handle the error
       pass
     automations, _, error = aa_executor.list_automations(name='Test')
     if error is not None:
       # handle the error
       pass
-    # Get the device id to execute, we'll just get the first one
-    device_id = int(devices[0]['id'])
+    # Get the run as user id to execute, we'll just get the first one
+    users_ids = int(devices[0]['defaultUsers'][0]['id'])
     # Get the automation id to execute, we'll just get the first one
     automation_id = int(automations[0]['id'])
     # Deploy
-    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [device_id])
+    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [users_ids])
     if success:
       # handle the error
       pass
     else:
       print(f'Deployed on id {deployment_id} with name {deployment_name}')
     aa_executor.logout()
     
@@ -67,22 +67,22 @@
 I found an endpoint where you can get the job execution status, by filtering it via deployment id or deployment name. Here's a sample usage:
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     deploy_id = '377b04a5-fa8b-4e4a-8db5-8d769fd6639b'
-    deploy_name = 'Test.2023.05.19.17.28.51.minterciso@deloitte.com'
+    deploy_name = 'Test.2023.05.19.17.28.51.test@test.com'
     aa_executor = Executor(base_url, username, password)
     success, error, data = aa_executor.status(deploy_id=deploy_id)
 
 And the dictionary output:
 
     [{'automationId': '',
-    'automationName': 'Test.2023.05.19.17.28.51.minterciso@deloitte.com',
+    'automationName': 'Test.2023.05.19.17.28.51.test@test.com',
     'automationPriority': 'PRIORITY_MEDIUM',
     'botLabel': '',
     'callbackInfo': '',
     'canManage': True,
     'command': 'logToFile',
     'createdBy': '41',
     'createdOn': '2023-05-19T17:28:51.949121Z',
@@ -105,11 +105,11 @@
     'runElevated': False,
     'startDateTime': '2023-05-19T17:29:21.602952600Z',
     'status': 'COMPLETED',
     'tenantUuid': '0a662aeb-8728-11a9-8187-bed41445010e',
     'totalLines': 1,
     'type': 'RUN_NOW',
     'userId': '41',
-    'userName': 'minterciso@deloitte.com',
+    'userName': 'test@test.com',
     'usingRdp': False}]
 
 Basically it's a list with all executions found with the filter, and all their status.
```

### Comparing `automation_anywhere-2.1.3/README.md` & `automation_anywhere-2.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     aa_executor = Executor(base_url, username, password)
-    devices, _, error = aa_executor.list_devices()
+    devices, _, error = aa_executor.list_devices(hostname='host', run_as_user='user_to_run_as')
     if error is not None:
       # handle the error
       pass
     automations, _, error = aa_executor.list_automations(name='Test')
     if error is not None:
       # handle the error
       pass
-    # Get the device id to execute, we'll just get the first one
-    device_id = int(devices[0]['id'])
+    # Get the run as user id to execute, we'll just get the first one
+    users_ids = int(devices[0]['defaultUsers'][0]['id'])
     # Get the automation id to execute, we'll just get the first one
     automation_id = int(automations[0]['id'])
     # Deploy
-    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [device_id])
+    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [users_ids])
     if success:
       # handle the error
       pass
     else:
       print(f'Deployed on id {deployment_id} with name {deployment_name}')
     aa_executor.logout()
     
@@ -53,22 +53,22 @@
 I found an endpoint where you can get the job execution status, by filtering it via deployment id or deployment name. Here's a sample usage:
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     deploy_id = '377b04a5-fa8b-4e4a-8db5-8d769fd6639b'
-    deploy_name = 'Test.2023.05.19.17.28.51.minterciso@deloitte.com'
+    deploy_name = 'Test.2023.05.19.17.28.51.test@test.com'
     aa_executor = Executor(base_url, username, password)
     success, error, data = aa_executor.status(deploy_id=deploy_id)
 
 And the dictionary output:
 
     [{'automationId': '',
-    'automationName': 'Test.2023.05.19.17.28.51.minterciso@deloitte.com',
+    'automationName': 'Test.2023.05.19.17.28.51.test@test.com',
     'automationPriority': 'PRIORITY_MEDIUM',
     'botLabel': '',
     'callbackInfo': '',
     'canManage': True,
     'command': 'logToFile',
     'createdBy': '41',
     'createdOn': '2023-05-19T17:28:51.949121Z',
@@ -91,11 +91,11 @@
     'runElevated': False,
     'startDateTime': '2023-05-19T17:29:21.602952600Z',
     'status': 'COMPLETED',
     'tenantUuid': '0a662aeb-8728-11a9-8187-bed41445010e',
     'totalLines': 1,
     'type': 'RUN_NOW',
     'userId': '41',
-    'userName': 'minterciso@deloitte.com',
+    'userName': 'test@test.com',
     'usingRdp': False}]
 
 Basically it's a list with all executions found with the filter, and all their status.
```

### Comparing `automation_anywhere-2.1.3/automation_anywhere/base.py` & `automation_anywhere-2.1.4/automation_anywhere/base.py`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.3/automation_anywhere/executor.py` & `automation_anywhere-2.1.4/automation_anywhere/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,41 +17,60 @@
         :param multiple_logins: If the user can and should have multiple logins, set to True, defaults to False
         :param ignore_ssl: If set to False, it'll ignore the SSL on the requests, defaults to True
         :type ignore_ssl: bool, optional
         :type multiple_logins: bool, optional
         :raises AuthenticationError: If there was an issue authenticating, it'll raise an AuthenticationError Exception
         """
         super().__init__(base_url=base_url, verify_ssl=verify_ssl)
-        success, error = self.authenticate(
-            username=username, password=password, multiple_login=multiple_logins)
+        success, error = self.authenticate(username=username, password=password, multiple_login=multiple_logins)
         if success is False:
             raise AuthenticationError(error)
 
-    def list_devices(self, sort: list = None, page: dict = None) -> tuple[list, dict, str]:
+    def list_devices(self, sort: list = None, page: dict = None, run_as_user: str = None, hostname: str = None, custom_filter: dict = None,) -> tuple[list, dict, str]:
         """List all devices that can execute something. You need the user id of the device in order to execute something.
 
         :param sort: If set, it's a list that executes the sorting, defaults to None
         :type sort: list, optional
         :param page: If set, a dictionary with page parameters to add on the payload, defaults to None
         :type page: dict, optional
+        :param run_as_user: If configured, it'll search for the exact username on the "defaultUsers" list, in order to filter it, defaults to None
+        :type run_as_user: str, optional
+        :param hostname: If configured, it'll search for the hostname (as a substring) on all the devices the user has permission to see, defaults to None
+        :type hostname: str, optional
+        :param custom_filter: If sent, it'll add to the other filters on the query, defaults to None
+        :type custom_filter: dict, optional
         :return: A tuple with a list of devices, a list of page data and a string to show errors
         :rtype: tuple[list, dict, str]
         """
         devices = None
         page_data = None
         error = None
-        endpoint = f'{self._base_url}v1/devices/runasusers/list'
+        endpoint = f'{self._base_url}v2/devices/list'
         payload = dict()
         payload['page'] = page
-        payload['sort'] = sort if sort is not None else [
-            {'field': 'username', 'direction': 'asc'}]
+        payload['sort'] = sort if sort is not None else [{'field': 'id', 'direction': 'asc'}]
+        local_filter = {'operator': 'and', 'operands': []}
+        if hostname:
+            local_filter['operands'].append({'operator': 'substring', 'field': 'hostName', 'value': hostname})
+        if custom_filter:
+            local_filter['operands'].append(custom_filter)
         response = post(url=endpoint, headers=self.headers, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             page_data = response.json()['page']
             devices = response.json()['list']
+            if run_as_user:
+                found_devices = list()
+                for device in devices:
+                    found_users = next((x for x in device['defaultUsers'] if x['username'] == run_as_user), None)
+                    if found_users:
+                        found_devices.append(device.copy())
+                        found_devices[-1]['defaultUsers'] = [found_users]
+            del devices
+            devices = found_devices.copy()
+
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
             error = f'Authentication Error - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 500:
             error = f'Server Error - {response.json()["code"]}: {response.json()["message"]}'
         else:
```

### Comparing `automation_anywhere-2.1.3/automation_anywhere.egg-info/PKG-INFO` & `automation_anywhere-2.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: automation-anywhere
-Version: 2.1.3
+Name: automation_anywhere
+Version: 2.1.4
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,28 +34,28 @@
 
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     aa_executor = Executor(base_url, username, password)
-    devices, _, error = aa_executor.list_devices()
+    devices, _, error = aa_executor.list_devices(hostname='host', run_as_user='user_to_run_as')
     if error is not None:
       # handle the error
       pass
     automations, _, error = aa_executor.list_automations(name='Test')
     if error is not None:
       # handle the error
       pass
-    # Get the device id to execute, we'll just get the first one
-    device_id = int(devices[0]['id'])
+    # Get the run as user id to execute, we'll just get the first one
+    users_ids = int(devices[0]['defaultUsers'][0]['id'])
     # Get the automation id to execute, we'll just get the first one
     automation_id = int(automations[0]['id'])
     # Deploy
-    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [device_id])
+    success, error, deployment_id, deployment_name = aa_executor.deploy(automation_id, [users_ids])
     if success:
       # handle the error
       pass
     else:
       print(f'Deployed on id {deployment_id} with name {deployment_name}')
     aa_executor.logout()
     
@@ -67,22 +67,22 @@
 I found an endpoint where you can get the job execution status, by filtering it via deployment id or deployment name. Here's a sample usage:
 
     from automation_anywhere.executor import Executor
     base_url = 'https://your-automation-controlroom-url/'
     username = 'your-username'
     password = 'your-password'
     deploy_id = '377b04a5-fa8b-4e4a-8db5-8d769fd6639b'
-    deploy_name = 'Test.2023.05.19.17.28.51.minterciso@deloitte.com'
+    deploy_name = 'Test.2023.05.19.17.28.51.test@test.com'
     aa_executor = Executor(base_url, username, password)
     success, error, data = aa_executor.status(deploy_id=deploy_id)
 
 And the dictionary output:
 
     [{'automationId': '',
-    'automationName': 'Test.2023.05.19.17.28.51.minterciso@deloitte.com',
+    'automationName': 'Test.2023.05.19.17.28.51.test@test.com',
     'automationPriority': 'PRIORITY_MEDIUM',
     'botLabel': '',
     'callbackInfo': '',
     'canManage': True,
     'command': 'logToFile',
     'createdBy': '41',
     'createdOn': '2023-05-19T17:28:51.949121Z',
@@ -105,11 +105,11 @@
     'runElevated': False,
     'startDateTime': '2023-05-19T17:29:21.602952600Z',
     'status': 'COMPLETED',
     'tenantUuid': '0a662aeb-8728-11a9-8187-bed41445010e',
     'totalLines': 1,
     'type': 'RUN_NOW',
     'userId': '41',
-    'userName': 'minterciso@deloitte.com',
+    'userName': 'test@test.com',
     'usingRdp': False}]
 
 Basically it's a list with all executions found with the filter, and all their status.
```

### Comparing `automation_anywhere-2.1.3/pyproject.toml` & `automation_anywhere-2.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="automation_anywhere"
-version="2.1.3"
+version="2.1.4"
 authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
 description="A Python Package to deploy tasks on Automation Anywhere 360"
 readme="README.md"
 requires-python=">=3.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

