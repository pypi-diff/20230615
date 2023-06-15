# Comparing `tmp/mercury-sync-0.1.2.tar.gz` & `tmp/mercury-sync-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.2.tar", last modified: Thu Jun 15 05:50:31 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.3.tar", last modified: Thu Jun 15 15:12:48 2023, max compression
```

## Comparing `mercury-sync-0.1.2.tar` & `mercury-sync-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:50:31.000000 mercury-sync-0.1.2/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-15 05:50:31.000000 mercury-sync-0.1.2/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:50:31.000000 mercury-sync-0.1.2/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 05:50:31.000000 mercury-sync-0.1.2/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:50:31.836101 mercury-sync-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 05:50:28.000000 mercury-sync-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/setup.py
```

### Comparing `mercury-sync-0.1.2/LICENSE` & `mercury-sync-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/PKG-INFO` & `mercury-sync-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.2/README.md` & `mercury-sync-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 import asyncio
 import pickle
+import time
 import zlib
 from collections import deque, defaultdict
-from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
+from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
 from mercury_sync.models.message import Message
+from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import Tuple, Deque, Any, Dict, Coroutine, AsyncIterable
-from mercury_sync.connection.tcp.protocols import (
-    MercurySyncTCPClientProtocol,
-    MercurySyncTCPServerProtocol
-)
 
 
-class MercurySyncTCPConnection:
+class MercurySyncUDPConnection:
 
     def __init__(
         self,
         host: str,
         port: int,
         instance_id: int
     ) -> None:
@@ -27,75 +25,53 @@
         self.port = port
 
         self.events: Dict[
             str,
             Coroutine
         ] = {}
 
-        self._client_transports: Dict[str, asyncio.Transport] = {}
-        self._server: asyncio.Server = None
+        self._transport: asyncio.DatagramTransport = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
+        self._pending_requests = deque()
         self._pending_responses = deque()
-        self._sent_values = deque()
-    
+
     def connect(self):
-        server = self._loop.create_server(
-            lambda: MercurySyncTCPServerProtocol(
+        server = self._loop.create_datagram_endpoint(
+            lambda: MercurySyncUDPProtocol(
                 self.read
             ),
-            host=self.host,
-            port=self.port
+            local_addr=(
+                self.host,
+                self.port
+            )
         )
-
         
-        self._server = self._loop.run_until_complete(server)
-
-    async def connect_client(
-        self,
-        address: Tuple[str, int]
-    ):
-
-        host, port = address
-
-        client_transport, _ = await self._loop.create_connection(
-            lambda: MercurySyncTCPClientProtocol(
-                self.read
-            ),
-            host=host,
-            port=port
-        )
-
-        self._client_transports[address] = client_transport
-
-        return client_transport
 
+        transport, _ = self._loop.run_until_complete(server)
+        self._transport = transport
 
     async def send(
         self, 
-        event_name: bytes,
-        data: bytes, 
-        address: Tuple[str, int]
-    ) -> str:
-        
-        client_transport = self._client_transports.get(address)
+        event_name: str,
+        data: Any, 
+        addr: Tuple[str, int]
+    ) -> Tuple[int, Any]:
 
         item = pickle.dumps((
             'request',
             next(self.id_generator),
             event_name,
-            data,
-            self.host,
-            self.port
+            data
         ))
 
         compressed = zlib.compress(item)
-
-        client_transport.write(compressed)
+        
+        self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
 
         (
@@ -107,35 +83,32 @@
             _
         ) = self.queue[event_name].pop()
 
         return (
             shard_id,
             response_data
         )
-    
+
     async def stream(
         self, 
         event_name: str,
         data: Any, 
-        address: Tuple[str, int]
+        addr: Tuple[str, int]
     ): 
-        client_transport = self._client_transports.get(address)
 
         item = pickle.dumps((
             'stream',
             next(self.id_generator),
             event_name,
-            data,
-            self.host,
-            self.port
+            data
         ))
 
         compressed = zlib.compress(item)
-
-        client_transport.write(compressed)
+        
+        self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
 
         for item in self.queue[event_name]:
@@ -143,139 +116,118 @@
                 _,
                 shard_id,
                 _,
                 response_data,
                 _, 
                 _
             ) = item
-         
+
             yield(
                 shard_id,
                 response_data
             )
 
         self.queue.clear()
 
     def read(
         self,
-        data: bytes,
-        transport: asyncio.Transport
+        data: bytes, 
+        addr: Tuple[str, int]
     ):
-    
-        result: Tuple[
-            str, 
-            int, 
-            float, 
-            Any, 
-            str, 
-            int
-        ] = pickle.loads(
-            zlib.decompress(data)
-        )
-
+        result: Tuple[str, int, float, Any] = pickle.loads(zlib.decompress(data))
         (
             message_type, 
             shard_id, 
-            event_name,
-            payload, 
-            incoming_host, 
-            incoming_port
+            event_name, 
+            payload
         ) = result
 
+        incoming_host, incoming_port = addr
+
+
         if message_type == 'request':
             self._pending_responses.append(
                 asyncio.create_task(
                     self._read(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
                             payload
                         ),
-                        transport
+                        addr
                     )
                 )
             )
-
+            
         elif message_type == 'stream':
-
             self._pending_responses.append(
                 asyncio.create_task(
                     self._read_iterator(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
                             payload
                         ),
-                        transport
+                        addr
                     )
                 )
             )
 
         else:
-            print(result)
+
             self.queue[event_name].append((
                 message_type, 
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
             ))
 
-                
             event_waiter = self._waiters[event_name]
 
+
             if len(event_waiter) > 0:
                 waiter = event_waiter.pop()
                 waiter.set_result(None)
 
+
     async def _read(
         self,
         event_name: str,
         coroutine: Coroutine,
-        transport: asyncio.Transport
+        addr: Tuple[str, int]
     ):
         response: Message = await coroutine
 
         item = pickle.dumps(
             (
                 'response', 
                 next(self.id_generator),
                 event_name,
-                response.to_data(), 
-                self.host,
-                self.port
+                response.to_data()
             )
         )
 
         compressed = zlib.compress(item)
-
-        transport.write(compressed)
+        self._transport.sendto(compressed, addr)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
-        transport: asyncio.Transport       
+        addr: Tuple[str, int]    
     ):
-        
         async for response in coroutine:
+
             item = pickle.dumps(
                 (
                     'response', 
                     next(self.id_generator),
                     event_name,
-                    response.to_data(), 
-                    self.host,
-                    self.port
+                    response.to_data()
                 )
             )
 
             compressed = zlib.compress(item)
-            transport.write(compressed)
-            
-
-    async def close(self):
-        for transport in self._client_transports.values():
-            transport.close()
 
-        self._server.close()
+            self._transport.sendto(compressed, addr)
```

### Comparing `mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.3/mercury_sync/hooks/client_hook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import functools
 from mercury_sync.service import Service
 
 
 def client(
     call_name: str, 
-    direct: bool=False
+    as_tcp: bool=False
 ):
 
     def wraps(func):
 
         func.client_only = True
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
             connection: Service = args[0]
 
-            if direct:
-                return await connection.send_direct(
+            if as_tcp:
+                return await connection.send_tcp(
                     call_name,
                     await func(*args, **kwargs)
                 )
 
             else:
                 return await connection.send(
                     call_name,
```

### Comparing `mercury-sync-0.1.2/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.3/mercury_sync/hooks/stream_hook.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 
             
 
 import functools
 from mercury_sync.service import Service
+from mercury_sync.models.message import Message
 
 
 def stream(
     call_name: str, 
-    direct: bool=False
+    as_tcp: bool=False
 ):
 
     def wraps(func):
 
         func.client_only = True
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
             connection: Service = args[0]
 
-            if direct:
+            if as_tcp:
+
                 async for data in func(*args, **kwargs):
-                    async for response in connection.stream_direct(
+                    async for response in connection.stream_tcp(
                         call_name,
                         data
                     ):
                         yield response
 
 
             else:
```

### Comparing `mercury-sync-0.1.2/mercury_sync/service/service.py` & `mercury-sync-0.1.3/mercury_sync/service/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import asyncio
 import random
 import inspect
+import signal
 from mercury_sync.connection.tcp.mercury_sync_tcp_connection import MercurySyncTCPConnection
 from mercury_sync.connection.udp.mercury_sync_udp_connection import MercurySyncUDPConnection
 from mercury_sync.models.message import Message
 from typing import (
     Tuple, 
     Dict, 
     TypeVar, 
@@ -12,14 +14,25 @@
 )
 
 
 T = TypeVar('T', bound=Message)
 R = TypeVar('R', bound=Message)
 
 
+def handle_loop_stop(signame, tcp_connection: MercurySyncTCPConnection):
+        try:
+            tcp_connection.close()
+
+        except BrokenPipeError:
+            pass 
+
+        except RuntimeError:
+            pass
+
+
 class Service(Generic[T, R]):
     
     def __init__(
         self,
         host: str,
         port: int
     ) -> None:
@@ -43,29 +56,42 @@
 
         methods = inspect.getmembers(self, predicate=inspect.ismethod)
 
         reserved_methods = [
             'start',
             'connect',
             'send',
-            'send_direct',
+            'send_tc',
+            'stream',
+            'stream_tcp'
             'close'
         ]
 
         for _, method in methods:
             method_name = method.__name__
 
             not_internal = method_name.startswith('__') is False
             not_reserved = method_name not in reserved_methods
             is_server = hasattr(method, 'server_only')
 
             if not_internal and not_reserved and is_server:
                 self._tcp_connection.events[method.__name__] = method
                 self._udp_connection.events[method.__name__] = method
 
+        self._loop = asyncio.get_event_loop()
+
+        for signame in ('SIGINT', 'SIGTERM'):
+            self._loop.add_signal_handler(
+                getattr(signal, signame),
+                lambda signame=signame: handle_loop_stop(
+                    signame,
+                    self._tcp_connection
+                )
+            )
+
     def start(self):
         self._tcp_connection.connect()
         self._udp_connection.connect()
 
     async def connect(
         self,
         remote: T
@@ -91,15 +117,15 @@
 
         return await self._udp_connection.send(
             event_name,
             message.to_data(),
             address
         )
     
-    async def send_direct(
+    async def send_tcp(
         self,
         event_name: str,
         message: T
     ) -> R:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
@@ -126,15 +152,15 @@
         async for response in self._udp_connection.stream(
             event_name,
             message.to_data(),
             address
         ):
             yield response
 
-    async def stream_direct(
+    async def stream_tcp(
         self,
         event_name: str,
         message: T
     ) -> AsyncIterable[R]:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
@@ -145,8 +171,8 @@
             event_name,
             message.to_data(),
             address
         ):
             yield response
     
     async def close(self):
-        await self._tcp_connection.close()
+        self._tcp_connection.close()
```

### Comparing `mercury-sync-0.1.2/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.3/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.3/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.3/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.2/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.3/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.2/setup.py` & `mercury-sync-0.1.3/setup.py`

 * *Files identical despite different names*

