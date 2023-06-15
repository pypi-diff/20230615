# Comparing `tmp/uagents-0.4.1.tar.gz` & `tmp/uagents-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents-0.4.1.tar", max compression
+gzip compressed data, was "uagents-0.5.0.tar", max compression
```

## Comparing `uagents-0.4.1.tar` & `uagents-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.4.1/LICENSE
--rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.4.1/README.md
--rw-r--r--   0        0        0      916 2023-05-04 14:30:04.770060 uagents-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.4.1/src/uagents/__init__.py
--rw-r--r--   0        0        0    16441 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/agent.py
--rw-r--r--   0        0        0     5651 2023-05-02 11:10:48.559062 uagents-0.4.1/src/uagents/asgi.py
--rw-r--r--   0        0        0     2363 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/config.py
--rw-r--r--   0        0        0     4979 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/context.py
--rw-r--r--   0        0        0        0 2023-03-02 16:19:41.886178 uagents-0.4.1/src/uagents/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-02 16:20:26.910313 uagents-0.4.1/src/uagents/contrib/protocols/__init__.py
--rw-r--r--   0        0        0     1312 2023-03-07 14:38:10.652721 uagents-0.4.1/src/uagents/contrib/protocols/protocol_query.py
--rw-r--r--   0        0        0     4148 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/crypto/__init__.py
--rw-r--r--   0        0        0     1038 2023-02-24 13:37:53.457125 uagents-0.4.1/src/uagents/dispatch.py
--rw-r--r--   0        0        0     1423 2023-02-24 13:37:53.457125 uagents-0.4.1/src/uagents/envelope.py
--rw-r--r--   0        0        0     6796 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/mailbox.py
--rw-r--r--   0        0        0      464 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/models.py
--rw-r--r--   0        0        0     1737 2023-05-04 13:36:54.712472 uagents-0.4.1/src/uagents/network.py
--rw-r--r--   0        0        0     6661 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/protocol.py
--rw-r--r--   0        0        0     2113 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/query.py
--rw-r--r--   0        0        0     1339 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/resolver.py
--rw-r--r--   0        0        0     1153 2023-03-24 09:42:09.546004 uagents-0.4.1/src/uagents/setup.py
--rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.4.1/src/uagents/storage/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 uagents-0.4.1/setup.py
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 uagents-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-24 13:37:53.437125 uagents-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1397 2023-02-24 13:37:53.441125 uagents-0.5.0/README.md
+-rw-r--r--   0        0        0      944 2023-06-15 09:54:04.795393 uagents-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-03-03 10:39:04.080443 uagents-0.5.0/src/uagents/__init__.py
+-rw-r--r--   0        0        0    16619 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/agent.py
+-rw-r--r--   0        0        0     5669 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/asgi.py
+-rw-r--r--   0        0        0     2363 2023-06-02 09:42:02.550506 uagents-0.5.0/src/uagents/config.py
+-rw-r--r--   0        0        0     5880 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/context.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:44:04.646091 uagents-0.5.0/src/uagents/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/contrib/protocols/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/contrib/protocols/protocol_query.py
+-rw-r--r--   0        0        0     4148 2023-05-22 12:26:05.307659 uagents-0.5.0/src/uagents/crypto/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-15 09:54:04.795393 uagents-0.5.0/src/uagents/dispatch.py
+-rw-r--r--   0        0        0     1697 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/envelope.py
+-rw-r--r--   0        0        0     6826 2023-06-15 09:54:04.799393 uagents-0.5.0/src/uagents/mailbox.py
+-rw-r--r--   0        0        0      464 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/models.py
+-rw-r--r--   0        0        0     1737 2023-06-02 09:42:02.554506 uagents-0.5.0/src/uagents/network.py
+-rw-r--r--   0        0        0     6661 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/protocol.py
+-rw-r--r--   0        0        0     2123 2023-06-14 08:44:04.650092 uagents-0.5.0/src/uagents/query.py
+-rw-r--r--   0        0        0     1339 2023-06-02 09:42:02.558506 uagents-0.5.0/src/uagents/resolver.py
+-rw-r--r--   0        0        0     1153 2023-05-06 15:29:54.115441 uagents-0.5.0/src/uagents/setup.py
+-rw-r--r--   0        0        0     2256 2023-02-24 13:37:53.461125 uagents-0.5.0/src/uagents/storage/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 uagents-0.5.0/setup.py
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 uagents-0.5.0/PKG-INFO
```

### Comparing `uagents-0.4.1/LICENSE` & `uagents-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/README.md` & `uagents-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/pyproject.toml` & `uagents-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "uagents"
-version = "0.4.1"
+version = "0.5.0"
 description = "Lightweight framework for rapid agent-based development"
 authors = ["Ed FitzGerald <edward.fitzgerald@fetch.ai>", "James Riehl <james.riehl@fetch.ai>", "Alejandro Morales <alejandro.madrigal@fetch.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 pydantic = "^1.10.2"
 msgpack = "^1.0.4"
 bech32 = "^1.2.0"
 ecdsa = "^0.18.0"
 apispec = "^6.0.2"
 uvicorn = "^0.19.0"
 aiohttp = "^3.8.3"
-cosmpy = "^0.7.0"
+cosmpy = "^0.8.0"
 websockets = "^10.4"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 pytest = "^7.1.3"
 pylint = "^2.15.3"
 mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.13"
 
 [tool.poetry.group.orm.dependencies]
 tortoise-orm = "^0.19.2"
 
 [tool.poetry.group.geo.dependencies]
 geopy = "^2.3.0"
```

### Comparing `uagents-0.4.1/src/uagents/agent.py` & `uagents-0.5.0/src/uagents/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import functools
 from typing import Dict, List, Optional, Set, Union, Type, Tuple, Any
+import uuid
 
 from cosmpy.aerial.wallet import LocalWallet, PrivateKey
 from cosmpy.crypto.address import Address
 
 from uagents.asgi import ASGIServer
 from uagents.context import (
     Context,
@@ -107,38 +108,40 @@
         self._interval_handlers: List[Tuple[IntervalCallback, float]] = []
         self._interval_messages: Set[str] = set()
         self._signed_message_handlers: Dict[str, MessageCallback] = {}
         self._unsigned_message_handlers: Dict[str, MessageCallback] = {}
         self._models: Dict[str, Type[Model]] = {}
         self._replies: Dict[str, Set[Type[Model]]] = {}
         self._queries: Dict[str, asyncio.Future] = {}
+        self._dispatcher = dispatcher
+        self._message_queue = asyncio.Queue()
+        self._on_startup = []
+        self._on_shutdown = []
+        self._version = version or "0.1.0"
+
+        # initialize the internal agent protocol
+        self._protocol = Protocol(name=self._name, version=self._version)
+
+        # keep track of supported protocols
+        self.protocols: Dict[str, Protocol] = {}
+
         self._ctx = Context(
             self._identity.address,
             self._name,
             self._storage,
             self._resolver,
             self._identity,
             self._wallet,
             self._ledger,
             self._queries,
             replies=self._replies,
             interval_messages=self._interval_messages,
+            protocols=self.protocols,
             logger=self._logger,
         )
-        self._dispatcher = dispatcher
-        self._message_queue = asyncio.Queue()
-        self._on_startup = []
-        self._on_shutdown = []
-        self._version = version or "0.1.0"
-
-        # initialize the internal agent protocol
-        self._protocol = Protocol(name=self._name, version=self._version)
-
-        # keep track of supported protocols
-        self.protocols: Dict[str, Protocol] = {}
 
         # register with the dispatcher
         self._dispatcher.register(self.address, self)
 
         if not self._use_mailbox:
             self._server = ASGIServer(
                 self._port, self._loop, self._queries, logger=self._logger
@@ -320,16 +323,18 @@
 
             if schema_digest in protocol.replies:
                 self._replies[schema_digest] = protocol.replies[schema_digest]
 
         if protocol.digest is not None:
             self.protocols[protocol.digest] = protocol
 
-    async def handle_message(self, sender, schema_digest: str, message: JsonStr):
-        await self._message_queue.put((schema_digest, sender, message))
+    async def handle_message(
+        self, sender, schema_digest: str, message: JsonStr, session: uuid.UUID
+    ):
+        await self._message_queue.put((schema_digest, sender, message, session))
 
     async def _startup(self):
         for handler in self._on_startup:
             await handler(self._ctx)
 
     async def _shutdown(self):
         for handler in self._on_shutdown:
@@ -373,15 +378,15 @@
                 self._loop.run_until_complete(self._server.serve())
         finally:
             self._loop.run_until_complete(self._shutdown())
 
     async def _process_message_queue(self):
         while True:
             # get an element from the queue
-            schema_digest, sender, message = await self._message_queue.get()
+            schema_digest, sender, message, session = await self._message_queue.get()
 
             # lookup the model definition
             model_class: Model = self._models.get(schema_digest)
             if model_class is None:
                 continue
 
             # parse the received message
@@ -392,19 +397,21 @@
                 self._name,
                 self._storage,
                 self._resolver,
                 self._identity,
                 self._wallet,
                 self._ledger,
                 self._queries,
+                session=session,
                 replies=self._replies,
                 interval_messages=self._interval_messages,
                 message_received=MsgDigest(
                     message=message, schema_digest=schema_digest
                 ),
+                protocols=self.protocols,
                 logger=self._logger,
             )
 
             # attempt to find the handler
             handler: MessageCallback = self._unsigned_message_handlers.get(
                 schema_digest
             )
```

### Comparing `uagents-0.4.1/src/uagents/asgi.py` & `uagents-0.5.0/src/uagents/asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                     "type": "http.response.body",
                     "body": b'{"error": "unable to route envelope"}',
                 }
             )
             return
 
         await dispatcher.dispatch(
-            env.sender, env.target, env.protocol, env.decode_payload()
+            env.sender, env.target, env.schema_digest, env.decode_payload(), env.session
         )
 
         # wait for any queries to be resolved
         if expects_response:
             response_msg: Model = await self._queries[env.sender]
             if env.expires is not None:
                 if datetime.now() > datetime.fromtimestamp(env.expires):
```

### Comparing `uagents-0.4.1/src/uagents/config.py` & `uagents-0.5.0/src/uagents/config.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/context.py` & `uagents-0.5.0/src/uagents/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+from __future__ import annotations
 import asyncio
 import logging
 import uuid
 from dataclasses import dataclass
 from time import time
-from typing import Dict, Set, Optional, Callable, Any, Awaitable, Type
+from typing import Dict, Set, Optional, Callable, Any, Awaitable, Type, TYPE_CHECKING
 
 import aiohttp
 from cosmpy.aerial.client import LedgerClient
 from cosmpy.aerial.wallet import LocalWallet
 
 from uagents.config import DEFAULT_ENVELOPE_TIMEOUT_SECONDS
 from uagents.crypto import Identity
 from uagents.dispatch import dispatcher
 from uagents.envelope import Envelope
 from uagents.models import Model, ErrorMessage
 from uagents.resolver import Resolver
 from uagents.storage import KeyValueStore
 
+if TYPE_CHECKING:
+    from uagents.protocol import Protocol
+
 IntervalCallback = Callable[["Context"], Awaitable[None]]
 MessageCallback = Callable[["Context", str, Any], Awaitable[None]]
 EventCallback = Callable[["Context"], Awaitable[None]]
 
 
 @dataclass
 class MsgDigest:
@@ -38,30 +42,34 @@
         name: Optional[str],
         storage: KeyValueStore,
         resolve: Resolver,
         identity: Identity,
         wallet: LocalWallet,
         ledger: LedgerClient,
         queries: Dict[str, asyncio.Future],
+        session: Optional[uuid.UUID] = None,
         replies: Optional[Dict[str, Set[Type[Model]]]] = None,
         interval_messages: Optional[Set[str]] = None,
         message_received: Optional[MsgDigest] = None,
+        protocols: Optional[Dict[str, Protocol]] = None,
         logger: Optional[logging.Logger] = None,
     ):
         self.storage = storage
         self.wallet = wallet
         self.ledger = ledger
         self._name = name
         self._address = str(address)
         self._resolver = resolve
         self._identity = identity
         self._queries = queries
+        self._session = session or uuid.uuid4()
         self._replies = replies
         self._interval_messages = interval_messages
         self._message_received = message_received
+        self._protocols = protocols or {}
         self._logger = logger
 
     @property
     def name(self) -> str:
         if self._name is not None:
             return self._name
         return self._address[:10]
@@ -70,14 +78,29 @@
     def address(self) -> str:
         return self._address
 
     @property
     def logger(self) -> logging.Logger:
         return self._logger
 
+    @property
+    def protocols(self) -> Optional[Dict[str, Protocol]]:
+        return self._protocols
+
+    @property
+    def session(self) -> uuid.UUID:
+        return self._session
+
+    def get_message_protocol(self, message_schema_digest) -> Optional[str]:
+        for protocol_digest, protocol in self._protocols.items():
+            for reply_models in protocol.replies.values():
+                if message_schema_digest in reply_models:
+                    return protocol_digest
+        return None
+
     async def send(
         self,
         destination: str,
         message: Model,
         timeout: Optional[int] = DEFAULT_ENVELOPE_TIMEOUT_SECONDS,
     ):
         # convert the message into object form
@@ -107,15 +130,15 @@
                     f"Outgoing message {type(message)} is not a valid interval message"
                 )
                 return
 
         # handle local dispatch of messages
         if dispatcher.contains(destination):
             await dispatcher.dispatch(
-                self.address, destination, schema_digest, json_message
+                self.address, destination, schema_digest, json_message, self._session
             )
             return
 
         # handle queries waiting for a response
         if destination in self._queries:
             self._queries[destination].set_result(message)
             del self._queries[destination]
@@ -133,16 +156,17 @@
         expires = int(time()) + timeout
 
         # handle external dispatch of messages
         env = Envelope(
             version=1,
             sender=self.address,
             target=destination,
-            session=uuid.uuid4(),
-            protocol=schema_digest,
+            session=self._session,
+            schema_digest=schema_digest,
+            protocol_digest=self.get_message_protocol(schema_digest),
             expires=expires,
         )
         env.encode_payload(json_message)
         env.sign(self._identity)
 
         async with aiohttp.ClientSession() as session:
             async with session.post(
```

### Comparing `uagents-0.4.1/src/uagents/crypto/__init__.py` & `uagents-0.5.0/src/uagents/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/dispatch.py` & `uagents-0.5.0/src/uagents/dispatch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Set
+import uuid
 
 JsonStr = str
 
 
 class Sink(ABC):
     @abstractmethod
-    async def handle_message(self, sender: str, schema_digest: str, message: JsonStr):
+    async def handle_message(
+        self, sender: str, schema_digest: str, message: JsonStr, session: uuid.UUID
+    ):
         pass
 
 
 class Dispatcher:
     def __init__(self):
         self._sinks: Dict[str, Set[Sink]] = {}
 
@@ -24,14 +27,19 @@
         destinations.discard(sink)
         self._sinks[address] = destinations
 
     def contains(self, address: str) -> bool:
         return address in self._sinks
 
     async def dispatch(
-        self, sender: str, destination: str, schema_digest: str, message: JsonStr
+        self,
+        sender: str,
+        destination: str,
+        schema_digest: str,
+        message: JsonStr,
+        session: uuid.UUID,
     ):
         for handler in self._sinks.get(destination, set()):
-            await handler.handle_message(sender, schema_digest, message)
+            await handler.handle_message(sender, schema_digest, message, session)
 
 
 dispatcher = Dispatcher()
```

### Comparing `uagents-0.4.1/src/uagents/envelope.py` & `uagents-0.5.0/src/uagents/envelope.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import base64
 import hashlib
 import struct
 from typing import Optional, Any
 
-from pydantic import BaseModel, UUID4
+from pydantic import BaseModel, Field, UUID4
 
 from uagents.crypto import Identity
 from uagents.dispatch import JsonStr
 
 
 class Envelope(BaseModel):
     version: int
     sender: str
     target: str
     session: UUID4
-    protocol: str
+    schema_digest: str = Field(alias="protocol")
+    protocol_digest: Optional[str] = None
     payload: Optional[str] = None
     expires: Optional[int] = None
+    nonce: Optional[int] = None
     signature: Optional[str] = None
 
+    class Config:
+        allow_population_by_field_name = True
+
     def encode_payload(self, value: JsonStr):
         self.payload = base64.b64encode(value.encode()).decode()
 
     def decode_payload(self) -> Optional[Any]:
         if self.payload is None:
             return None
 
@@ -38,13 +43,15 @@
         return Identity.verify_digest(self.sender, self._digest(), self.signature)
 
     def _digest(self) -> bytes:
         hasher = hashlib.sha256()
         hasher.update(self.sender.encode())
         hasher.update(self.target.encode())
         hasher.update(str(self.session).encode())
-        hasher.update(self.protocol.encode())
+        hasher.update(self.schema_digest.encode())
         if self.payload is not None:
             hasher.update(self.payload.encode())
         if self.expires is not None:
             hasher.update(struct.pack(">Q", self.expires))
+        if self.nonce is not None:
+            hasher.update(struct.pack(">Q", self.nonce))
         return hasher.digest()
```

### Comparing `uagents-0.4.1/src/uagents/mailbox.py` & `uagents-0.5.0/src/uagents/mailbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,17 @@
         if not dispatcher.contains(env.target):
             self._logger.warning("Received envelope for unrecognized address")
             return
 
         await dispatcher.dispatch(
             env.sender,
             env.target,
-            env.protocol,
+            env.schema_digest,
             env.decode_payload(),
+            env.session,
         )
 
         # queue envelope for deletion from server
         await self._envelopes_to_delete.put(payload)
 
     async def process_deletion_queue(self):
         async with aiohttp.ClientSession() as session:
```

### Comparing `uagents-0.4.1/src/uagents/network.py` & `uagents-0.5.0/src/uagents/network.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/protocol.py` & `uagents-0.5.0/src/uagents/protocol.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/query.py` & `uagents-0.5.0/src/uagents/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     # handle external dispatch of messages
     env = Envelope(
         version=1,
         sender=generate_user_address(),
         target=destination,
         session=uuid.uuid4(),
-        protocol=schema_digest,
+        schema_digest=schema_digest,
         expires=expires,
     )
     env.encode_payload(json_message)
 
     async with aiohttp.ClientSession() as session:
         async with session.post(
             endpoint,
@@ -69,11 +69,11 @@
 
 def enclose_response(message: Model, sender: str, session: str) -> str:
     response_env = Envelope(
         version=1,
         sender=sender,
         target="",
         session=session,
-        protocol=Model.build_schema_digest(message),
+        schema_digest=Model.build_schema_digest(message),
     )
     response_env.encode_payload(message.json())
     return response_env.json()
```

### Comparing `uagents-0.4.1/src/uagents/resolver.py` & `uagents-0.5.0/src/uagents/resolver.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/setup.py` & `uagents-0.5.0/src/uagents/setup.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/src/uagents/storage/__init__.py` & `uagents-0.5.0/src/uagents/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.4.1/setup.py` & `uagents-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0',
  'apispec>=6.0.2,<7.0.0',
  'bech32>=1.2.0,<2.0.0',
- 'cosmpy>=0.7.0,<0.8.0',
+ 'cosmpy>=0.8.0,<0.9.0',
  'ecdsa>=0.18.0,<0.19.0',
  'msgpack>=1.0.4,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'uvicorn>=0.19.0,<0.20.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'uagents',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Lightweight framework for rapid agent-based development',
     'long_description': 'The **μAgents** (micro-Agents) project is a fast and lightweight framework that makes it easy to build agents for all kinds of decentralised use cases.\n\n## Installation\n\nInstall μAgents for Python 3.8, 3.9, or 3.10:\n\n```bash\npoetry install\npoetry shell\n```\n\n## Documentation\n\nBuild and run the docs locally with:\n\n```bash\nmkdocs serve\n```\n\nOr go to the official docs site: https://docs.fetch.ai/uAgents.\n\n## Examples\n\nThe [`examples`](https://github.com/fetchai/uAgents/tree/main/examples) folder contains several examples of how to create and run various types of agents.\n\n## Contributing\n\nAll contributions are welcome! Remember, contribution includes not only code, but any help with docs or issues raised by other developers. See our [contribution guidelines](https://github.com/fetchai/uAgents/blob/main/CONTRIBUTING.md) for more details.\n\n### Development Guidelines\n\nRead our [development guidelines](https://github.com/fetchai/uAgents/blob/main/DEVELOPING.md) to learn some useful tips related to development.\n\n### Issues, Questions and Discussions\n\nWe use [GitHub Issues](https://github.com/fetchai/uAgents/issues) for tracking requests and bugs, and [GitHub Discussions](https://github.com/fetchai/uAgents/discussions) for general questions and discussion.\n\n## License\n\nThe μAgents project is licensed under [Apache License 2.0](https://github.com/fetchai/uAgents/blob/main/LICENSE).\n\n',
     'author': 'Ed FitzGerald',
     'author_email': 'edward.fitzgerald@fetch.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `uagents-0.4.1/PKG-INFO` & `uagents-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: uagents
-Version: 0.4.1
+Version: 0.5.0
 Summary: Lightweight framework for rapid agent-based development
 License: Apache 2.0
 Author: Ed FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: apispec (>=6.0.2,<7.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
-Requires-Dist: cosmpy (>=0.7.0,<0.8.0)
+Requires-Dist: cosmpy (>=0.8.0,<0.9.0)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Description-Content-Type: text/markdown
```

