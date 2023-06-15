# Comparing `tmp/deltafi-1.0.0rc3.tar.gz` & `tmp/deltafi-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-1.0.0rc3.tar", max compression
+gzip compressed data, was "deltafi-1.0.0rc5.tar", max compression
```

## Comparing `deltafi-1.0.0rc3.tar` & `deltafi-1.0.0rc5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/deltafi/__init__.py
--rw-r--r--   0        0        0     7326 2023-06-01 15:10:46.434796 deltafi-1.0.0rc3/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc3/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc3/deltafi/actiontype.py
--rw-r--r--   0        0        0    11019 2023-06-01 15:10:46.435796 deltafi-1.0.0rc3/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc3/deltafi/exception.py
--rw-r--r--   0        0        0     6284 2023-06-01 15:10:46.435796 deltafi-1.0.0rc3/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc3/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc3/deltafi/metric.py
--rw-r--r--   0        0        0     8553 2023-05-08 15:00:28.699314 deltafi-1.0.0rc3/deltafi/plugin.py
--rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.0rc3/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc3/deltafi/storage.py
--rw-r--r--   0        0        0     1281 2023-06-02 22:02:57.540036 deltafi-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-1.0.0rc5/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-1.0.0rc5/deltafi/__init__.py
+-rw-r--r--   0        0        0     7330 2023-06-09 15:16:11.399155 deltafi-1.0.0rc5/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-1.0.0rc5/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-1.0.0rc5/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11025 2023-06-09 15:16:11.400155 deltafi-1.0.0rc5/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-1.0.0rc5/deltafi/exception.py
+-rw-r--r--   0        0        0     6290 2023-06-09 15:16:11.401155 deltafi-1.0.0rc5/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-1.0.0rc5/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-1.0.0rc5/deltafi/metric.py
+-rw-r--r--   0        0        0    11666 2023-06-06 18:39:40.022585 deltafi-1.0.0rc5/deltafi/plugin.py
+-rw-r--r--   0        0        0    10706 2023-05-22 14:40:08.186270 deltafi-1.0.0rc5/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-1.0.0rc5/deltafi/storage.py
+-rw-r--r--   0        0        0     1281 2023-06-12 16:39:15.976733 deltafi-1.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc5/PKG-INFO
```

### Comparing `deltafi-1.0.0rc3/deltafi/__init__.py` & `deltafi-1.0.0rc5/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/action.py` & `deltafi-1.0.0rc5/deltafi/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     def __init__(self, description: str, requires_domains: List[str], requires_enrichments: List[str]):
         super().__init__(ActionType.ENRICH, description, requires_domains, requires_enrichments)
 
     def execute(self, event):
         enrich_input = EnrichInput(content=event.delta_file_messages[0].content_list,
                                    metadata=event.delta_file_messages[0].metadata,
                                    domains={domain.name: domain for domain in event.delta_file_messages[0].domains},
-                                   enrichment={domain.name: domain for domain in event.delta_file_messages[0].enrichment})
+                                   enrichments={domain.name: domain for domain in event.delta_file_messages[0].enrichments})
         result = self.enrich(event.context, self.param_class().parse_obj(event.params), enrich_input)
         self.validate_type(result, (EnrichResult, ErrorResult))
         return result
 
     @abstractmethod
     def enrich(self, context: Context, params: BaseModel, enrich_input: EnrichInput):
         pass
@@ -102,15 +102,15 @@
     def __init__(self, description: str, requires_domains: List[str], requires_enrichments: List[str]):
         super().__init__(ActionType.FORMAT, description, requires_domains, requires_enrichments)
 
     def execute(self, event):
         format_input = FormatInput(content=event.delta_file_messages[0].content_list,
                                    metadata=event.delta_file_messages[0].metadata,
                                    domains={domain.name: domain for domain in event.delta_file_messages[0].domains},
-                                   enrichment={domain.name: domain for domain in event.delta_file_messages[0].enrichment})
+                                   enrichments={domain.name: domain for domain in event.delta_file_messages[0].enrichments})
         result = self.format(event.context, self.param_class().parse_obj(event.params), format_input)
         self.validate_type(result, (FormatResult, FormatManyResult, ErrorResult, FilterResult))
         return result
 
     @abstractmethod
     def format(self, context: Context, params: BaseModel, format_input: FormatInput):
         pass
```

### Comparing `deltafi-1.0.0rc3/deltafi/actioneventqueue.py` & `deltafi-1.0.0rc5/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/actiontype.py` & `deltafi-1.0.0rc5/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/domain.py` & `deltafi-1.0.0rc5/deltafi/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,27 +277,27 @@
                       media_type=media_type)
 
 
 class DeltaFileMessage(NamedTuple):
     metadata: Dict[str, str]
     content_list: List[Content]
     domains: List[Domain]
-    enrichment: List[Domain]
+    enrichments: List[Domain]
 
     @classmethod
     def from_dict(cls, delta_file_message: dict, content_service: ContentService):
         metadata = delta_file_message['metadata']
         content_list = [Content.from_dict(content, content_service) for content in delta_file_message['contentList']]
         domains = [Domain.from_dict(domain) for domain in delta_file_message['domains']] if 'domains' in delta_file_message else []
-        enrichment = [Domain.from_dict(domain) for domain in delta_file_message['enrichment']] if 'enrichment' in delta_file_message else []
+        enrichments = [Domain.from_dict(domain) for domain in delta_file_message['enrichments']] if 'enrichments' in delta_file_message else []
 
         return DeltaFileMessage(metadata=metadata,
                                 content_list=content_list,
                                 domains=domains,
-                                enrichment=enrichment)
+                                enrichments=enrichments)
 
 
 class Event(NamedTuple):
     delta_file_messages: List[DeltaFileMessage]
     context: Context
     params: dict
     queue_name: str
```

### Comparing `deltafi-1.0.0rc3/deltafi/exception.py` & `deltafi-1.0.0rc5/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/input.py` & `deltafi-1.0.0rc5/deltafi/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     metadata: dict
 
 
 class EnrichInput(NamedTuple):
     content: List[Content]
     metadata: dict
     domains: Dict[str, Domain]
-    enrichment: Dict[str, Domain]
+    enrichments: Dict[str, Domain]
 
     def has_content(self) -> bool:
         return len(self.content) > 0
 
     def content_at(self, index: int) -> Content:
         if len(self.content) < index + 1:
             raise ExpectedContentException(index, len(self.content))
@@ -97,27 +97,27 @@
 
     def domain(self, name: str) -> Domain:
         if not self.has_domain(name):
             raise MissingDomainException(name)
         return self.domains[name]
 
     def has_enrichment(self, name: str) -> bool:
-        return name in self.enrichment
+        return name in self.enrichments
 
     def enrichment(self, name: str) -> Domain:
         if not self.has_enrichment(name):
             raise MissingEnrichmentException(name)
-        return self.enrichment[name]
+        return self.enrichments[name]
 
 
 class FormatInput(NamedTuple):
     content: List[Content]
     metadata: dict
     domains: Dict[str, Domain]
-    enrichment: Dict[str, Domain]
+    enrichments: Dict[str, Domain]
 
     def has_content(self) -> bool:
         return len(self.content) > 0
 
     def content_at(self, index: int) -> Content:
         if len(self.content) < index + 1:
             raise ExpectedContentException(index, len(self.content))
@@ -143,20 +143,20 @@
 
     def domain(self, name: str) -> Domain:
         if not self.has_domain(name):
             raise MissingDomainException(name)
         return self.domains[name]
 
     def has_enrichment(self, name: str) -> bool:
-        return name in self.enrichment
+        return name in self.enrichments
 
     def enrichment(self, name: str) -> Domain:
         if not self.has_enrichment(name):
             raise MissingEnrichmentException(name)
-        return self.enrichment[name]
+        return self.enrichments[name]
 
 
 class LoadInput(NamedTuple):
     content: List[Content]
     metadata: dict
 
     def has_content(self) -> bool:
```

### Comparing `deltafi-1.0.0rc3/deltafi/logger.py` & `deltafi-1.0.0rc5/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/metric.py` & `deltafi-1.0.0rc5/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/plugin.py` & `deltafi-1.0.0rc5/deltafi/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,32 +21,32 @@
 import sys
 import threading
 import time
 import traceback
 from os.path import isdir, isfile, join
 from pathlib import Path
 from typing import List
+import importlib
+import inspect
+import pkgutil
 
-import pkg_resources
+from importlib import metadata
 import requests
 from deltafi.actioneventqueue import ActionEventQueue
 from deltafi.domain import Event
 from deltafi.exception import ExpectedContentException, MissingDomainException, MissingEnrichmentException, \
     MissingMetadataException
 from deltafi.logger import get_logger
 from deltafi.result import ErrorResult
 from deltafi.storage import ContentService
+from deltafi.action import Action
 
 
 def _coordinates():
-    return {
-        'groupId': os.getenv('PROJECT_GROUP'),
-        'artifactId': os.getenv('PROJECT_NAME'),
-        'version': os.getenv('PROJECT_VERSION')
-    }
+    return PluginCoordinates(os.getenv('PROJECT_GROUP'), os.getenv('PROJECT_NAME'), os.getenv('PROJECT_VERSION'))
 
 
 def _setup_queue(max_connections):
     redis_url = os.getenv('REDIS_URL', 'http://deltafi-redis-master:6379')
     password = os.getenv('REDIS_PASSWORD')
     return ActionEventQueue(redis_url, max_connections, password)
 
@@ -54,51 +54,123 @@
 def _setup_content_service():
     minio_url = os.getenv('MINIO_URL', 'http://deltafi-minio:9000')
     return ContentService(minio_url,
                           os.getenv('MINIO_ACCESSKEY'),
                           os.getenv('MINIO_SECRETKEY'))
 
 
-class Plugin(object):
-    def __init__(self, actions: List, description: str):
-        self.actions = [action() for action in actions]
-        self.description = description
-        self.coordinates = _coordinates()
+class PluginCoordinates(object):
+    def __init__(self, group_id: str, artifact_id: str, version: str):
+        self.group_id = group_id
+        self.artifact_id = artifact_id
+        self.version = version
 
+    def __json__(self):
+        return {
+            "groupId": self.group_id,
+            "artifactId": self.artifact_id,
+            "version": self.version
+        }
+
+
+class Plugin(object):
+    def __init__(self, description: str, plugin_name: str = None, plugin_coordinates: PluginCoordinates = None,
+                 actions: List = None, action_package: str = None):
+        """
+        Initialize the plugin object
+        :param plugin_name: Name of the plugin project
+        :param description: Description of the plugin
+        :param plugin_coordinates: plugin coordinates of the plugin, if None the coordinates must be defined
+        in environment variables
+        :param actions: list of action classes to run
+        :param action_package: name of the package containing the actions to run
+        """
+        self.content_service = None
+        self.queue = None
+        self.actions = []
         self.core_url = os.getenv('CORE_URL')
-        self.queue = _setup_queue(len(self.actions) + 1)
-        self.content_service = _setup_content_service()
+        action_classes = []
+        if actions is not None and len(actions):
+            action_classes.extend(actions)
+
+        if action_package is not None:
+            found_actions = Plugin.find_actions(action_package)
+            if len(found_actions):
+                action_classes.extend(found_actions)
+
+        unique_actions = dict.fromkeys(action_classes)
+        self.actions = [action() for action in unique_actions]
+
+        self.description = description
+        self.display_name = os.getenv('PROJECT_NAME') if plugin_name is None else plugin_name
+        self.coordinates = _coordinates() if plugin_coordinates is None else plugin_coordinates
 
         if os.getenv('ACTIONS_HOSTNAME'):
             self.hostname = os.getenv('ACTIONS_HOSTNAME')
         elif os.getenv('HOSTNAME'):
             self.hostname = os.getenv('HOSTNAME')
         elif os.getenv('COMPUTERNAME'):
             self.hostname = os.getenv('COMPUTERNAME')
         else:
             self.hostname = 'UNKNOWN'
 
         self.logger = get_logger()
 
-        self.logger.info(f"Initialized ActionRunner with actions {actions}")
+        self.logger.debug(f"Initialized ActionRunner with actions {self.actions}")
+
+    @staticmethod
+    def find_actions(package_name) -> List[object]:
+        """
+        Find all concrete classes that extend the base Action class in the given package
+        :param package_name: name of the package to load and scan for actions
+        :return: list of classes that extend the Action class
+        """
+        package = importlib.import_module(package_name)
+        classes = []
+        visited = set()
+
+        # Iterate over all submodules in the package
+        for _, module_name, _ in pkgutil.walk_packages(package.__path__):
+            try:
+                module = importlib.import_module(package.__name__ + '.' + module_name)
+            except ModuleNotFoundError:
+                continue
+
+            # Iterate over all members in the module
+            for name, obj in inspect.getmembers(module):
+                if inspect.isclass(obj) and obj not in visited:
+                    if Plugin.is_action(obj):
+                        classes.append(obj)
+                    visited.add(obj)
+
+        return classes
+
+    @staticmethod
+    def is_action(maybe_action: type) -> bool:
+        """
+        Check if the given object is a non-abstract subclass of the Action class
+        :param maybe_action: object to inspect to see if it is an Action class
+        :return: true if the object is a non-abstract subclass of the Action class
+        """
+        return not inspect.isabstract(maybe_action) and issubclass(maybe_action, Action)
 
     def action_name(self, action):
-        return f"{self.coordinates['groupId']}.{action.__class__.__name__}"
+        return f"{self.coordinates.group_id}.{action.__class__.__name__}"
 
     def _action_json(self, action):
         return {
             'name': self.action_name(action),
             'description': action.description,
             'type': action.action_type.name,
             'requiresDomains': action.requires_domains,
             'requiresEnrichments': action.requires_enrichments,
             'schema': action.param_class().schema()
         }
 
-    def _register(self):
+    def registration_json(self):
         flows_path = str(Path(os.path.dirname(os.path.abspath(sys.argv[0]))) / 'flows')
 
         flow_files = []
         variables = []
         if isdir(flows_path):
             flow_files = [f for f in os.listdir(flows_path) if isfile(join(flows_path, f))]
             if 'variables.json' in flow_files:
@@ -106,51 +178,55 @@
                 variables = json.load(open(join(flows_path, 'variables.json')))
         else:
             self.logger.warning(f"Flows directory ({flows_path}) does not exist. No flows will be installed.")
 
         flows = [json.load(open(join(flows_path, f))) for f in flow_files]
         actions = [self._action_json(action) for action in self.actions]
 
-        url = f"{self.core_url}/plugins"
-        headers = {'Content-type': 'application/json'}
-        registration_json = \
-            {
-                'pluginCoordinates': self.coordinates,
-                'displayName': os.getenv('PROJECT_NAME'),
+        return {
+                'pluginCoordinates': self.coordinates.__json__(),
+                'displayName': self.display_name,
                 'description': self.description,
-                'actionKitVersion': pkg_resources.get_distribution('deltafi').version,
+                'actionKitVersion': metadata.version('deltafi'),
                 'dependencies': [],
                 'actions': actions,
                 'variables': variables,
                 'flowPlans': flows
             }
 
+    def _register(self):
+        url = f"{self.core_url}/plugins"
+        headers = {'Content-type': 'application/json'}
+        registration_json = self.registration_json()
+
         self.logger.info(f"Registering plugin:\n{registration_json}")
 
         response = requests.post(url, headers=headers, json=registration_json)
         if not response.ok:
             self.logger.error(f"Failed to register plugin ({response.status_code}):\n{response.content}")
             exit(1)
 
-        self.logger.info(f"Plugin registered")
+        self.logger.info("Plugin registered")
 
     def run(self):
-        self.logger.info(f"Plugin starting")
+        self.logger.info("Plugin starting")
+        self.queue = _setup_queue(len(self.actions) + 1)
+        self.content_service = _setup_content_service()
         self._register()
         for action in self.actions:
             threading.Thread(target=self._do_action, args=(action,)).start()
 
         threading.Thread(target=self._heartbeat).start()
 
-        self.logger.info(f"All threads running")
+        self.logger.info("All threads running")
 
         f = open("/tmp/running", "w")
         f.close()
 
-        self.logger.info(f"Application initialization complete")
+        self.logger.info("Application initialization complete")
 
     def _heartbeat(self):
         while True:
             try:
                 for action in self.actions:
                     self.queue.heartbeat(self.action_name(action))
             except Exception as e:
```

### Comparing `deltafi-1.0.0rc3/deltafi/result.py` & `deltafi-1.0.0rc5/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/deltafi/storage.py` & `deltafi-1.0.0rc5/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-1.0.0rc3/pyproject.toml` & `deltafi-1.0.0rc5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "1.0.0-RC3"
+version = "1.0.0-RC5"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-1.0.0rc3/PKG-INFO` & `deltafi-1.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 1.0.0rc3
+Version: 1.0.0rc5
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

