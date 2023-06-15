# Comparing `tmp/mercury-sync-0.1.3.tar.gz` & `tmp/mercury-sync-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.3.tar", last modified: Thu Jun 15 15:12:48 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.4.tar", last modified: Thu Jun 15 18:31:29 2023, max compression
```

## Comparing `mercury-sync-0.1.3.tar` & `mercury-sync-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 15:12:48.000000 mercury-sync-0.1.3/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:12:48.890246 mercury-sync-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 15:12:41.000000 mercury-sync-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:31:29.300128 mercury-sync-0.1.4/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 18:31:29.000000 mercury-sync-0.1.4/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:31:29.304129 mercury-sync-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 18:31:23.000000 mercury-sync-0.1.4/setup.py
```

### Comparing `mercury-sync-0.1.3/LICENSE` & `mercury-sync-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/PKG-INFO` & `mercury-sync-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.3/README.md` & `mercury-sync-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.4/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 
 import asyncio
 import pickle
 import socket
+import ssl
 import zlib
 from collections import deque, defaultdict
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from mercury_sync.models.message import Message
-from typing import Tuple, Deque, Any, Dict, Coroutine, AsyncIterable
+from typing import (
+    Tuple, 
+    Deque, 
+    Any, 
+    Dict, 
+    Coroutine, 
+    AsyncIterable,
+    Union,
+    Optional
+)
 from mercury_sync.connection.tcp.protocols import (
     MercurySyncTCPClientProtocol,
     MercurySyncTCPServerProtocol
 )
 
 
 class MercurySyncTCPConnection:
@@ -32,67 +42,143 @@
             Coroutine
         ] = {}
 
         self._client_transports: Dict[str, asyncio.Transport] = {}
         self._server: asyncio.Server = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
+        self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_responses: Dict[str, Deque[asyncio.Task]] = defaultdict(deque)
+
         self._sent_values = deque()
         self.connected = False
         self._server_socket = None
         self._stream = False
+        
+        self._client_key_path: Union[str, None] = None
+        self._client_cert_path: Union[str, None] = None
+
+        self._server_key_path: Union[str, None] = None
+        self._server_cert_path: Union[str, None] = None 
+        
+        self._client_ssl_context: Union[ssl.SSLContext, None] = None
+        self._server_ssl_context: Union[ssl.SSLContext, None] = None
     
-    def connect(self):
+    def connect(
+        self,
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ):
+        if cert_path and key_path:
+            self._server_ssl_context = self._create_server_ssl_context(
+                cert_path=cert_path,
+                key_path=key_path
+            ) 
 
         if self.connected is False:
 
             self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             self._server_socket.bind((self.host, self.port))
 
             self._server_socket.setblocking(False)
 
             server = self._loop.create_server(
                 lambda: MercurySyncTCPServerProtocol(
                     self.read
                 ),
-                sock= self._server_socket
+                sock=self._server_socket,
+                ssl=self._server_ssl_context
             )
 
-            
             self._server = self._loop.run_until_complete(server)
 
             self.connected = True
 
+    def _create_server_ssl_context(
+        self, 
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ) -> ssl.SSLContext:
+        
+        if self._server_cert_path is None:
+            self._server_cert_path = cert_path
+
+        if self._server_key_path is None:
+            self._server_key_path = key_path
+
+        ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+        ssl_ctx.options |= ssl.OP_NO_TLSv1
+        ssl_ctx.options |= ssl.OP_NO_TLSv1_1
+        ssl_ctx.options |= ssl.OP_SINGLE_DH_USE
+        ssl_ctx.options |= ssl.OP_SINGLE_ECDH_USE
+        ssl_ctx.load_cert_chain(cert_path, keyfile=key_path)
+        ssl_ctx.load_verify_locations(cafile=cert_path)
+        ssl_ctx.check_hostname = False
+        ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
+        ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
+
+        return ssl_ctx
+
     async def connect_client(
         self,
-        address: Tuple[str, int]
+        address: Tuple[str, int],
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
     ):
+        
+        if cert_path and key_path:
+            self._client_ssl_context = self._create_client_ssl_context(
+                cert_path=cert_path,
+                key_path=key_path
+            ) 
 
         host, port = address
         tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         tcp_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         await self._loop.run_in_executor(None, tcp_socket.connect, address)
 
         tcp_socket.setblocking(False)
 
         client_transport, _ = await self._loop.create_connection(
             lambda: MercurySyncTCPClientProtocol(
                 self.read
             ),
             host=host,
-            port=port
+            port=port,
+            ssl=self._client_ssl_context
         )
 
         self._client_transports[address] = client_transport
 
         return client_transport
+    
+    def _create_client_ssl_context(
+        self, 
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ) -> ssl.SSLContext:
+        
+        if self._client_cert_path is None:
+            self._client_cert_path = cert_path
+
+        if self._client_key_path is None:
+            self._client_key_path = key_path
+
+        ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+        ssl_ctx.options |= ssl.OP_NO_TLSv1
+        ssl_ctx.options |= ssl.OP_NO_TLSv1_1
+        ssl_ctx.load_cert_chain(cert_path, keyfile=key_path)
+        ssl_ctx.load_verify_locations(cafile=cert_path)
+        ssl_ctx.check_hostname = False
+        ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
+        ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
 
+        return ssl_ctx
 
     async def send(
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
     ) -> str:
@@ -245,15 +331,15 @@
         if message_type == 'request':
             self._pending_responses[event_name].append(
                 asyncio.create_task(
                     self._read(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
-                            payload
+                            self.parsers[event_name](**payload)
                         ),
                         transport
                     )
                 )
             )
 
         elif message_type == "stream_connect":
@@ -295,15 +381,15 @@
 
             self._pending_responses[event_name].append(
                 asyncio.create_task(
                     self._read_iterator(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
-                            payload
+                            self.parsers[event_name](**payload)
                         ),
                         transport
                     )
                 )
             )
 
             event_waiter = self._waiters[event_name]
```

### Comparing `mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.4/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.4/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 
 import asyncio
 import pickle
-import time
+import socket
+import ssl
 import zlib
 from collections import deque, defaultdict
+from dtls import do_patch
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
-from typing import Tuple, Deque, Any, Dict, Coroutine, AsyncIterable
+from typing import (
+    Tuple, 
+    Deque, 
+    Any, 
+    Dict, 
+    Coroutine, 
+    AsyncIterable,
+    Optional,
+    Union
+)
+
+do_patch()
 
 
 class MercurySyncUDPConnection:
 
     def __init__(
         self,
         host: str,
@@ -28,33 +41,82 @@
             str,
             Coroutine
         ] = {}
 
         self._transport: asyncio.DatagramTransport = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
+        self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_requests = deque()
         self._pending_responses = deque()
 
-    def connect(self):
+        self._udp_cert_path: Union[str, None] = None
+        self._udp_key_path: Union[str, None] = None
+        self._udp_ssl_context: Union[ssl.SSLContext, None] = None
+
+    def connect(
+        self, 
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ):
+
+        udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+        udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+
+        if cert_path and key_path:
+            self._udp_ssl_context = self._create_udp_ssl_context(
+                cert_path=cert_path,
+                key_path=key_path,
+            )
+
+            udp_socket = self._udp_ssl_context.wrap_socket(udp_socket)
+
+        udp_socket.bind((
+            self.host,
+            self.port
+        ))
+
+        udp_socket.setblocking(False)
+
         server = self._loop.create_datagram_endpoint(
             lambda: MercurySyncUDPProtocol(
                 self.read
             ),
-            local_addr=(
-                self.host,
-                self.port
-            )
+            sock=udp_socket
         )
-        
 
         transport, _ = self._loop.run_until_complete(server)
         self._transport = transport
 
+    def _create_udp_ssl_context(
+        self,
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None
+    ) -> ssl.SSLContext: 
+        
+        if self._udp_cert_path is None:
+            self._udp_cert_path = cert_path
+
+        if self._udp_key_path is None:
+            self._udp_key_path = key_path
+
+        ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
+        ssl_ctx.options |= ssl.OP_NO_TLSv1
+        ssl_ctx.options |= ssl.OP_NO_TLSv1_1
+        ssl_ctx.options |= ssl.OP_SINGLE_DH_USE
+        ssl_ctx.options |= ssl.OP_SINGLE_ECDH_USE
+        ssl_ctx.load_cert_chain(cert_path, keyfile=key_path)
+        ssl_ctx.load_verify_locations(cafile=cert_path)
+        ssl_ctx.check_hostname = False
+        ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
+        ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
+        
+        return ssl_ctx
+    
     async def send(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
     ) -> Tuple[int, Any]:
 
@@ -147,29 +209,29 @@
         if message_type == 'request':
             self._pending_responses.append(
                 asyncio.create_task(
                     self._read(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
-                            payload
+                            self.parsers[event_name](**payload)
                         ),
                         addr
                     )
                 )
             )
             
         elif message_type == 'stream':
             self._pending_responses.append(
                 asyncio.create_task(
                     self._read_iterator(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
-                            payload
+                            self.parsers[event_name](**payload)
                         ),
                         addr
                     )
                 )
             )
 
         else:
```

### Comparing `mercury-sync-0.1.3/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.4/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.4/mercury_sync/hooks/client_hook.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     call_name: str, 
     as_tcp: bool=False
 ):
 
     def wraps(func):
 
         func.client_only = True
+        func.target = call_name
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
             connection: Service = args[0]
```

### Comparing `mercury-sync-0.1.3/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.4/mercury_sync/hooks/stream_hook.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     call_name: str, 
     as_tcp: bool=False
 ):
 
     def wraps(func):
 
         func.client_only = True
+        func.target = call_name
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
             connection: Service = args[0]
```

### Comparing `mercury-sync-0.1.3/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.4/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.4/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.3/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.4/mercury_sync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.3/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.4/mercury_sync.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 mercury_sync/__init__.py
 mercury_sync.egg-info/PKG-INFO
 mercury_sync.egg-info/SOURCES.txt
 mercury_sync.egg-info/dependency_links.txt
+mercury_sync.egg-info/requires.txt
 mercury_sync.egg-info/top_level.txt
 mercury_sync/connection/__init__.py
 mercury_sync/connection/tcp/__init__.py
 mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
 mercury_sync/connection/tcp/protocols/__init__.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
```

### Comparing `mercury-sync-0.1.3/setup.py` & `mercury-sync-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,9 +35,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
+    install_requires=[
+        'pydantic',
+        'python3-dtls'
+    ],
     python_requires='>=3.10'
 )
```

