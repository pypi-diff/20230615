# Comparing `tmp/starmoth-0.4.1.tar.gz` & `tmp/starmoth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.4.1.tar", last modified: Mon Jun 12 18:46:53 2023, max compression
+gzip compressed data, was "starmoth-0.5.0.tar", last modified: Thu Jun 15 20:18:41 2023, max compression
```

## Comparing `starmoth-0.4.1.tar` & `starmoth-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.632138 starmoth-0.4.1/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-12 18:46:53.632138 starmoth-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1288 2023-06-12 18:02:40.000000 starmoth-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.624137 starmoth-0.4.1/moth/
--rw-rw-rw-   0 root         (0) root         (0)     4276 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.624137 starmoth-0.4.1/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.4.1/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.4.1/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     7186 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.4.1/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.628137 starmoth-0.4.1/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     5763 2023-06-12 18:02:40.000000 starmoth-0.4.1/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:46:53.632138 starmoth-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:46:53.632138 starmoth-0.4.1/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-12 18:46:53.000000 starmoth-0.4.1/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-06-15 20:18:41.716005 starmoth-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2023-06-15 20:13:10.000000 starmoth-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4428 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.5.0/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.5.0/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.5.0/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-06-15 20:13:10.000000 starmoth-0.5.0/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 20:18:41.716005 starmoth-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:18:41.716005 starmoth-0.5.0/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 20:18:41.000000 starmoth-0.5.0/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.4.1/moth/__init__.py` & `starmoth-0.5.0/moth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import zmq
 import time
 import queue
 import threading
+from typing import Optional, List
 
 from moth.message import (
     HandshakeMsg,
     HandshakeResponseMsg,
     HeartbeatMsg,
     ImagePromptMsg,
     parse_message,
@@ -21,30 +22,32 @@
     HEARTBEAT_INTERVAL = 1
 
     def __init__(
         self,
         name: str,
         token: str = "",
         task_type: HandshakeTaskTypes = HandshakeTaskTypes.CLASSIFICATION,
+        output_classes: Optional[List[str]] = None,
     ):
         self.name = name
         self._token = token
         self.stop = False
         self.task_type = task_type
+        self.output_classes = output_classes
 
     def run(self, url="tcp://localhost:7171"):
         self.stop = False
         context = zmq.Context()
         socket = context.socket(zmq.DEALER)
         socket.setsockopt_string(zmq.IDENTITY, self.name)
 
         try:
             socket.connect(url)
             # This is a handshake call to prove our identity
-            handshake = HandshakeMsg(self.name, self._token, "v0.0.0", self.task_type)
+            handshake = HandshakeMsg(self.name, self._token, "v0.0.0", self.task_type, self.output_classes)
             socket.send(handshake.serialize_envelope())
             self._req_loop(socket)
         except KeyboardInterrupt:
             print("\nExit...")
             self.stop = True
 
     def prompt(self, func):
```

### Comparing `starmoth-0.4.1/moth/cli/__init__.py` & `starmoth-0.5.0/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.1/moth/driver/__init__.py` & `starmoth-0.5.0/moth/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.4.1/moth/message/__init__.py` & `starmoth-0.5.0/moth/message/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import abc
-from ast import Dict
+from typing import Dict
 from enum import Enum
 import io
 import time
 from dataclasses import dataclass
 from typing import List, Optional, Type
 import uuid
 import msgpack
@@ -214,32 +214,36 @@
 
 @dataclass
 class HandshakeMsg(Msg):
     name: str
     handshake_token: str
     version: str = "v0"
     task_type: HandshakeTaskTypes = HandshakeTaskTypes.CLASSIFICATION
+    output_classes: Optional[List[str]] = None
+
 
     def serialize(self) -> bytes:
         obj = {
             "name": self.name,
             "token": self.handshake_token,
             "version": self.version,
             "taskType": self.task_type,
+            "outputClasses": self.output_classes,
         }
         return msgpack.packb(obj)
 
     @staticmethod
     def deserialize(data: bytes) -> HandshakeMsg:
         obj = msgpack.unpackb(data)
         return HandshakeMsg(
             name=obj["name"],
             handshake_token=obj["token"],
             version=obj["version"],
             task_type=obj.get("taskType", HandshakeTaskTypes.CLASSIFICATION), # Ensure backwards compatibility
+            output_classes=obj.get("outputClasses", None), # Ensure backwards compatibility
         )
 
 @dataclass
 class HandshakeResponseMsg(Msg):
     def serialize(self) -> bytes:
         return msgpack.packb({})
```

### Comparing `starmoth-0.4.1/moth/server/__init__.py` & `starmoth-0.5.0/moth/server/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,64 @@
+""" Server module for the Moth project. """
+
 from typing import Callable, Dict, List, Optional
-import zmq
+from dataclasses import dataclass
 import time
+import zmq
 from moth.driver import ModelDriver
 from moth.message import (
     HandshakeMsg,
     ClassificationResultMsg,
     HandshakeResponseMsg,
     HeartbeatMsg,
     Msg,
     ObjectDetectionResultMsg,
     parse_message,
 )
 from moth.message.exceptions import MothMessageError
 
 
-class IdentityPool:
-    def __init__(self):
-        self._ids = []
-
-    def add_identity(self, name: str, token: str):
-        self._ids.append((name, token))
-
-    def validate_handshake(self, identity: str, msg: HandshakeMsg) -> bool:
-        if identity != msg.name:
-            return False
-
-        id_ = [i for i in self._ids if i[1] == msg.handshake_token]
-        if len(id_) != 1:
-            return False
-
-        if id_[0][0] == identity and id_[0][1] == msg.handshake_token:
-            return True
-
-
-class MessageHandler:
-    def onMessage(self, msg: Msg):
-        pass
+@dataclass
+class Model:
+    """Holds information about a model that is connected to the server."""
+
+    id: str
+    task_type: str
+    output_classes: Optional[List[str]] = None
+
+    def serialize(self):
+        return {
+            "id": self.id,
+            "taskType": self.task_type,
+            "outputClasses": self.output_classes,
+        }
+
+    @staticmethod
+    def deserialize(json) -> "Model":
+        return Model(
+            id=json["id"],
+            task_type=json["taskType"],
+            output_classes=json["outputClasses"],
+        )
 
 
 class Server:
+    """Server class that accepts connections from models."""
+
     HEARTBEAT_TIMEOUT = 5
     HEARTBEAT_INTERVAL = 1
 
-    def __init__(self, port=7171):
+    def __init__(self, port: int = 7171):
         self.port = port
         self._stop = False
-        self._driver_factory = None
-        self._drivers: Dict[str, ModelDriver] = {}
-        self._models: Dict[str, Dict[str, str]] = {}
-        self._on_model_change_handler: Optional[
-            Callable[[List[Dict[str, str]]], None]
-        ] = None
-        self._heartbeats: Dict[str, float] = {}
+        self._driver_factory: Optional[Callable[[HandshakeMsg], ModelDriver]] = None
+        self._drivers: Dict[bytes, ModelDriver] = {}
+        self._models: Dict[bytes, Model] = {}
+        self._on_model_change_handler: Optional[Callable[[List[Model]], None]] = None
+        self._heartbeats: Dict[bytes, float] = {}
 
     def driver_factory(self, func: Callable[[HandshakeMsg], ModelDriver]):
         """
         Annotation to provide driver factory function.
         For every incoming model connection, this factory is called to get a driver for
         that model.
         """
@@ -67,15 +70,15 @@
         socket = context.socket(zmq.ROUTER)
         socket.bind(f"tcp://*:{self.port}")
         self._recv_loop(socket)
 
     def stop(self):
         self._stop = True
 
-    def _recv_loop(self, socket):
+    def _recv_loop(self, socket: zmq.Socket):
         poll = zmq.Poller()
         poll.register(socket, zmq.POLLIN)
         last_heartbeat = time.time()
         print("Server listening...")
         while not self._stop:
             # handle input
             events = dict(poll.poll(1000))
@@ -84,18 +87,19 @@
                 msg_bytes = socket.recv()
 
                 try:
                     message = parse_message(msg_bytes)
                     if isinstance(message, HandshakeMsg) and self._driver_factory:
                         driver = self._driver_factory(message)
                         identity_str = identity.decode("utf-8")
-                        model = {
-                            "id": identity_str,
-                            "taskType": message.task_type,
-                        }
+                        model = Model(
+                            id=identity_str,
+                            task_type=message.task_type,
+                            output_classes=message.output_classes,
+                        )
                         self._drivers[identity] = driver
                         self._models[identity] = model
                         self._heartbeats[identity] = time.time()
                         if self._on_model_change_handler:
                             self._on_model_change_handler(
                                 list(self._models.values())
                             )  # Pass the list of current drivers
@@ -131,28 +135,31 @@
             for identity in self._drivers:
                 next_prompt = self._drivers[identity].next_model_prompt()
                 if next_prompt is not None:
                     socket.send(identity, zmq.SNDMORE)
                     socket.send(next_prompt.serialize_envelope())
                 # Check heartbeat status
                 if identity in self._heartbeats:
-                    if self._heartbeats[identity] + Server.HEARTBEAT_TIMEOUT < time.time():
+                    if (
+                        self._heartbeats[identity] + Server.HEARTBEAT_TIMEOUT
+                        < time.time()
+                    ):
                         # Mark as diconnected
                         disconnected.append(identity)
 
             # Remove disconnected models
             for identity in disconnected:
                 self._drivers.pop(identity)
                 self._models.pop(identity)
                 self._heartbeats.pop(identity)
                 if self._on_model_change_handler:
                     self._on_model_change_handler(list(self._models.values()))
                 print(f"MUT disconnected: {identity.decode('utf-8')}")
 
         socket.close()
 
-    def on_model_change(self, func: Callable[[List[Dict[str, str]]], None]):
+    def on_model_change(self, func: Callable[[List[Model]], None]):
         """
         Annotation to provide a function that is called when the list of connected models changes.
         """
         self._on_model_change_handler = func
         return func
```

### Comparing `starmoth-0.4.1/setup.py` & `starmoth-0.5.0/setup.py`

 * *Files identical despite different names*

