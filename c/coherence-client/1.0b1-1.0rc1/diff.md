# Comparing `tmp/coherence_client-1.0b1.tar.gz` & `tmp/coherence_client-1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherence_client-1.0b1.tar", max compression
+gzip compressed data, was "coherence_client-1.0rc1.tar", max compression
```

## Comparing `coherence_client-1.0b1.tar` & `coherence_client-1.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1845 2023-04-25 17:23:31.735653 coherence_client-1.0b1/LICENSE.txt
--rw-r--r--   0        0        0     4565 2023-05-05 17:35:26.370614 coherence_client-1.0b1/README.md
--rw-r--r--   0        0        0     1979 2023-05-05 18:20:32.413037 coherence_client-1.0b1/pyproject.toml
--rw-r--r--   0        0        0      652 2023-05-05 00:00:06.363349 coherence_client-1.0b1/src/coherence/__init__.py
--rw-r--r--   0        0        0    33819 2023-05-04 00:14:21.126853 coherence_client-1.0b1/src/coherence/aggregator.py
--rw-r--r--   0        0        0    60084 2023-05-05 07:05:34.765360 coherence_client-1.0b1/src/coherence/client.py
--rw-r--r--   0        0        0     1060 2023-05-04 17:17:21.901772 coherence_client-1.0b1/src/coherence/comparator.py
--rw-r--r--   0        0        0    31133 2023-05-04 17:17:21.903682 coherence_client-1.0b1/src/coherence/event.py
--rw-r--r--   0        0        0    11175 2023-05-04 17:17:21.904955 coherence_client-1.0b1/src/coherence/extractor.py
--rw-r--r--   0        0        0    32290 2023-04-26 20:41:38.608398 coherence_client-1.0b1/src/coherence/filter.py
--rw-r--r--   0        0        0    11698 2023-04-26 20:41:38.609067 coherence_client-1.0b1/src/coherence/messages_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 20:41:38.609472 coherence_client-1.0b1/src/coherence/messages_pb2_grpc.py
--rw-r--r--   0        0        0    33851 2023-05-04 00:14:21.130957 coherence_client-1.0b1/src/coherence/processor.py
--rw-r--r--   0        0        0     9745 2023-04-26 20:41:38.610630 coherence_client-1.0b1/src/coherence/serialization.py
--rw-r--r--   0        0        0     4040 2023-04-26 20:41:38.611050 coherence_client-1.0b1/src/coherence/services_pb2.py
--rw-r--r--   0        0        0    45397 2023-04-26 20:41:38.611488 coherence_client-1.0b1/src/coherence/services_pb2_grpc.py
--rw-r--r--   0        0        0    11918 2023-05-04 00:14:21.132130 coherence_client-1.0b1/src/coherence/util.py
--rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 coherence_client-1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-06-15 18:35:43.333261 coherence_client-1.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     4548 2023-06-15 18:35:43.434393 coherence_client-1.0rc1/README.md
+-rw-r--r--   0        0        0     1979 2023-06-15 18:38:08.997849 coherence_client-1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      986 2023-06-15 18:38:39.397834 coherence_client-1.0rc1/src/coherence/__init__.py
+-rw-r--r--   0        0        0    33819 2023-06-15 18:35:44.542780 coherence_client-1.0rc1/src/coherence/aggregator.py
+-rw-r--r--   0        0        0    62479 2023-06-15 18:35:44.599870 coherence_client-1.0rc1/src/coherence/client.py
+-rw-r--r--   0        0        0     1060 2023-06-15 18:35:44.649334 coherence_client-1.0rc1/src/coherence/comparator.py
+-rw-r--r--   0        0        0    31397 2023-06-15 18:35:44.692952 coherence_client-1.0rc1/src/coherence/event.py
+-rw-r--r--   0        0        0    11175 2023-06-15 18:35:44.738663 coherence_client-1.0rc1/src/coherence/extractor.py
+-rw-r--r--   0        0        0    36712 2023-06-15 18:35:44.782352 coherence_client-1.0rc1/src/coherence/filter.py
+-rw-r--r--   0        0        0    11698 2023-06-15 18:35:44.838742 coherence_client-1.0rc1/src/coherence/messages_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-15 18:35:44.839539 coherence_client-1.0rc1/src/coherence/messages_pb2_grpc.py
+-rw-r--r--   0        0        0    33851 2023-06-15 18:35:44.939903 coherence_client-1.0rc1/src/coherence/processor.py
+-rw-r--r--   0        0        0     9917 2023-06-15 18:35:45.083192 coherence_client-1.0rc1/src/coherence/serialization.py
+-rw-r--r--   0        0        0     4040 2023-06-15 18:35:45.140812 coherence_client-1.0rc1/src/coherence/services_pb2.py
+-rw-r--r--   0        0        0    45397 2023-06-15 18:35:45.142868 coherence_client-1.0rc1/src/coherence/services_pb2_grpc.py
+-rw-r--r--   0        0        0    11918 2023-06-15 18:35:45.239824 coherence_client-1.0rc1/src/coherence/util.py
+-rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 coherence_client-1.0rc1/PKG-INFO
```

### Comparing `coherence_client-1.0b1/LICENSE.txt` & `coherence_client-1.0rc1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, 2023 Oracle and/or its affiliates.
+Copyright (c) 2023 Oracle and/or its affiliates.
 
 The Universal Permissive License (UPL), Version 1.0
 
 Subject to the condition set forth below, permission is hereby granted to any
 person obtaining a copy of this software, associated documentation and/or data
 (collectively the "Software"), free of charge and under any and all copyright
 rights in the Software, and any and all patent rights owned or freely
```

### Comparing `coherence_client-1.0b1/README.md` & `coherence_client-1.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
 [![License](http://img.shields.io/badge/license-UPL%201.0-blue.svg)](https://oss.oracle.com/licenses/upl/)
 
 <img src=https://oracle.github.io/coherence/assets/images/logo-red.png width="30%"><img>
 
-The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using
-the Google gRPC framework as the network transport.
+The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using gRPC as the network transport.
 
 #### Features
 * Familiar Map-like interface for manipulating cache entries including but not limited to:
     * `put`, `put_if_absent`, `put_all`, `get`, `get_all`, `remove`, `clear`, `get_or_default`, `replace`, `replace_mapping`, `size`, `is_empty`, `contains_key`, `contains_value`
 * Cluster-side querying, aggregation and filtering of map entries
 * Cluster-side manipulation of map entries using EntryProcessors
 * Registration of listeners to be notified of:
     * mutations such as insert, update and delete on Maps
     * map lifecycle events such as truncated, released or destroyed
     * session lifecycle events such as connected, disconnected, reconnected and closed
 * Support for storing Python objects as JSON as well as the ability to serialize to Java objects on the server for access from other Coherence language API's
 
 #### Requirements
-* [Coherence CE](https://github.com/oracle/coherence) 22.06 or later (or equivalent non-open source editions) with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
-* Python 3.10.1
+* [Coherence CE](https://github.com/oracle/coherence) 22.06.4+ or Coherence 14.1.1.2206.4+ Commercial edition with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
+* Python 3.11.x
+
 
 #### Starting a Coherence Cluster
 
 Before testing the Python client, you must ensure a Coherence cluster is available.
 For local development, we recommend using the Coherence CE Docker image; it contains
 everything necessary for the client to operate correctly.
 
@@ -53,15 +53,15 @@
 from coherence import NamedCache, Session
 import asyncio
 
 
 async def run_test():
 
     # create a new Session to the Coherence server
-    session: Session = Session(None)
+    session: Session = await Session.create()
 
     # create a new NamedCache with key of string|int and value of string|int
     cache: NamedCache[str, str|int] = await session.get_cache("test")
 
     # put a new key/value
     k: str = "one"
     v: str = "only-one"
@@ -106,11 +106,11 @@
 
 ## Security
 
 Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
 ## License
 
-Copyright (c) 2022, 2023 Oracle and/or its affiliates.
+Copyright (c) 2023 Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 <https://oss.oracle.com/licenses/upl/>.
```

### Comparing `coherence_client-1.0b1/pyproject.toml` & `coherence_client-1.0rc1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2022, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 [tool.poetry]
 name = "coherence-client"
-version = "1.0b1"
+version = "1.0rc1"
 description = """The Coherence Python Client allows Python applications to act as cache clients to a \
 Coherence Cluster using Google's gRPC framework as the network transport."""
 packages = [
     { include = "coherence", from = "./src"},
 ]
 readme = "README.md"
 authors = ["Oracle <dhiru.pandey@oracle.com>"]
@@ -17,32 +17,32 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Universal Permissive License (UPL)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
-python = "~3.10"
-protobuf = "~4.21"
-grpcio = "~1.51"
-grpcio-tools = "~1.51"
-jsonpickle = "~2.2"
+python = "~3.11"
+protobuf = "~4.23"
+grpcio = "~1.54"
+grpcio-tools = "~1.54"
+jsonpickle = "~3.0"
 pymitter = "~0.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "~7.2"
-pytest-asyncio = "~0.19"
-pytest-cov = "~4.0"
+pytest = "~7.3"
+pytest-asyncio = "~0.21"
+pytest-cov = "~4.1"
 pytest-unordered = "~0.5"
-pre-commit = "~2.20"
+pre-commit = "~3.3"
 Sphinx = "~4.5"
-sphinx-rtd-theme = "~1.1"
+sphinx-rtd-theme = "~1.2"
 sphinxcontrib-napoleon = "~0.7"
 m2r = "~0.3"
-third-party-license-file-generator = "~2022.3"
+third-party-license-file-generator = "~2023.2"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
```

### Comparing `coherence_client-1.0b1/src/coherence/aggregator.py` & `coherence_client-1.0rc1/src/coherence/aggregator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/client.py` & `coherence_client-1.0rc1/src/coherence/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
 import abc
 import asyncio
+import logging
 import os
-from asyncio import Task
+from asyncio import Condition, Task
 from threading import Lock
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     Final,
@@ -41,27 +42,32 @@
 from .util import RequestFactory
 
 K = TypeVar("K")
 V = TypeVar("V")
 R = TypeVar("R")
 T = TypeVar("T")
 
+COH_LOG = logging.getLogger("coherence")
+
 
 @no_type_check
 def _pre_call_cache(func):
     def inner(self, *args, **kwargs):
         if not self.active:
             raise Exception("Cache [] has been " + "released" if self.released else "destroyed")
 
         return func(self, *args, **kwargs)
 
     async def inner_async(self, *args, **kwargs):
         if not self.active:
             raise Exception("Cache [{}] has been {}.".format(self.name, "released" if self.released else "destroyed"))
 
+        # noinspection PyProtectedMember
+        await self._session._wait_for_active()
+
         return await func(self, *args, **kwargs)
 
     if asyncio.iscoroutinefunction(func):
         return inner_async
     return inner
 
 
@@ -334,15 +340,15 @@
         :param value: the value expected to be associated with some key
         :return: resolving to `true` if a mapping exists, or `false` if it does not
         """
 
     @abc.abstractmethod
     async def is_empty(self) -> bool:
         """
-        Returns`true` if this map contains no key-value mappings.
+        Returns `true` if this map contains no key-value mappings.
 
         :return: `true` if this map contains no key-value mappings.
         """
 
     @abc.abstractmethod
     async def size(self) -> int:
         """
@@ -495,14 +501,15 @@
         self._serializer: Serializer = serializer
         self._client_stub: NamedCacheServiceStub = NamedCacheServiceStub(session.channel)
         self._request_factory: RequestFactory = RequestFactory(cache_name, session.scope, serializer)
         self._emitter: EventEmitter = EventEmitter()
         self._internal_emitter: EventEmitter = EventEmitter()
         self._destroyed: bool = False
         self._released: bool = False
+        self._session: Session = session
         from .event import _MapEventsManager
 
         self._setup_event_handlers()
 
         self._events_manager: _MapEventsManager[K, V] = _MapEventsManager(
             self, session, self._client_stub, serializer, self._internal_emitter
         )
@@ -739,24 +746,26 @@
         internal_emitter: EventEmitter = self._internal_emitter
         this: NamedCacheClient[K, V] = self
         cache_name = self._cache_name
 
         # noinspection PyProtectedMember
         def on_destroyed(name: str) -> None:
             if name == cache_name:
-                this._events_manager._close()
-                this._destroyed = True
-                emitter.emit(MapLifecycleEvent.DESTROYED.value, name)
+                if not this.destroyed:
+                    this._events_manager._close()
+                    this._destroyed = True
+                    emitter.emit(MapLifecycleEvent.DESTROYED.value, name)
 
         # noinspection PyProtectedMember
         def on_released(name: str) -> None:
             if name == cache_name:
-                this._events_manager._close()
-                this._released = True
-                emitter.emit(MapLifecycleEvent.RELEASED.value, name)
+                if not this.released:
+                    this._events_manager._close()
+                    this._released = True
+                    emitter.emit(MapLifecycleEvent.RELEASED.value, name)
 
         def on_truncated(name: str) -> None:
             if name == cache_name:
                 emitter.emit(MapLifecycleEvent.TRUNCATED.value, name)
 
         internal_emitter.on(MapLifecycleEvent.DESTROYED.value, on_destroyed)
         internal_emitter.on(MapLifecycleEvent.RELEASED.value, on_released)
@@ -918,15 +927,15 @@
         :param address: Address of the target Coherence cluster.  If not explicitly set, this defaults
           to :func:`coherence.client.Options.DEFAULT_ADDRESS`. See
           also :func:`coherence.client.Options.ENV_SERVER_ADDRESS`
         :param scope: scope name used to link this :func:`coherence.client.Options` to the
           corresponding `ConfigurableCacheFactory` on the server.
         :param request_timeout_seconds: Defines the request timeout, in `seconds`, that will be applied to each
           remote call. If not explicitly set, this defaults to :func:`coherence.client.Options.DEFAULT_REQUEST_TIMEOUT`.
-          See also See also :func:`coherence.client.Options.ENV_REQUEST_TIMEOUT`
+          See also :func:`coherence.client.Options.ENV_REQUEST_TIMEOUT`
         :param ser_format: The serialization format.  Currently, this is always `json`
         :param channel_options: The `gRPC` `ChannelOptions`. See
             https://grpc.github.io/grpc/python/glossary.html#term-channel_arguments and
             https://github.com/grpc/grpc/blob/master/include/grpc/impl/grpc_types.h
         :param tls_options: Optional TLS configuration.
         """
         addr = os.getenv(Options.ENV_SERVER_ADDRESS)
@@ -937,15 +946,16 @@
 
         timeout = os.getenv(Options.ENV_REQUEST_TIMEOUT)
         if timeout is not None:
             time_out: float
             try:
                 time_out = float(timeout)
             except ValueError:
-                print(f"The value of {Options.ENV_REQUEST_TIMEOUT} cannot be converted to a float")
+                COH_LOG.warning("The timeout value of [%s] cannot be converted to a float", Options.ENV_REQUEST_TIMEOUT)
+
             self._request_timeout_seconds = time_out
         else:
             self._request_timeout_seconds = request_timeout_seconds
 
         self._scope = scope
         self._ser_format = ser_format
 
@@ -1076,14 +1086,16 @@
     def __init__(self, session_options: Optional[Options] = None):
         """
         Construct a new `Session` based on the provided :func:`coherence.client.Options`
 
         :param session_options: the provided :func:`coherence.client.Options`
         """
         self._closed: bool = False
+        self._active = False
+        self._active_condition: Condition = Condition()
         self._caches: dict[str, NamedCache[Any, Any]] = dict()
         self._lock: Lock = Lock()
         if session_options is not None:
             self._session_options = session_options
         else:
             self._session_options = Options()
 
@@ -1117,14 +1129,21 @@
                     _InterceptorStreamStream(self),
                 ],
             )
 
         watch_task: Task[None] = asyncio.create_task(watch_channel_state(self))
         self._tasks.add(watch_task)
         self._emitter: EventEmitter = EventEmitter()
+        self._channel.get_state(True)  # trigger connect
+
+    @staticmethod
+    async def create(session_options: Optional[Options] = None) -> Session:
+        session: Session = Session(session_options)
+        await session._set_active(False)
+        return session
 
     # noinspection PyTypeHints
     @_pre_call_session
     def on(
         self,
         event: Literal[MapLifecycleEvent.DESTROYED] | Literal[MapLifecycleEvent.RELEASED] | SessionLifecycleEvent,
         callback: Callable[[str], None] | Callable[[], None],
@@ -1232,26 +1251,54 @@
                 c = NamedCacheClient(name, self, serializer)
                 # initialize the event stream now to ensure lifecycle listeners will work as expected
                 await c._events_manager._ensure_stream()
                 self._setup_event_handlers(c)
                 self._caches.update({name: c})
             return c
 
+    def is_active(self) -> bool:
+        """
+        Returns
+        :return:
+        """
+        return self._active
+
+    async def _set_active(self, active: bool) -> None:
+        self._active = active
+        if self._active:
+            if not self._active_condition.locked():
+                await self._active_condition.acquire()
+            self._active_condition.notify_all()
+            self._active_condition.release()
+        else:
+            await self._active_condition.acquire()
+
+    async def _wait_for_active(self) -> None:
+        if not self.is_active():
+            timeout: float = self._session_options.request_timeout_seconds
+            COH_LOG.debug("Waiting for session to become active; timeout=[%s seconds]", timeout)
+            async with asyncio.timeout(timeout):
+                await self._active_condition.wait()
+
     # noinspection PyUnresolvedReferences
     async def close(self) -> None:
         """
         Close the `Session`
         """
         if not self._closed:
             self._closed = True
             self._emitter.emit(SessionLifecycleEvent.CLOSED.value)
             for task in self._tasks:
                 task.cancel()
             self._tasks.clear()
 
+            caches_copy: dict[str, NamedCache[Any, Any]] = self._caches.copy()
+            for cache in caches_copy.values():
+                await cache.destroy()
+
             await self._channel.close()  # TODO: consider grace period?
 
     def _setup_event_handlers(self, client: NamedCacheClient[K, V]) -> None:
         this: Session = self
 
         def on_destroyed(name: str) -> None:
             if name in this._caches:
@@ -1338,36 +1385,45 @@
 
 
 # noinspection PyProtectedMember
 async def watch_channel_state(session: Session) -> None:
     emitter: EventEmitter = session._emitter
     channel: grpc.aio.Channel = session.channel
     first_connect: bool = True
-    connected: bool = False
+    last_state: grpc.ChannelConnectivity = grpc.ChannelConnectivity.IDLE
 
     try:
         while True:
             state: grpc.ChannelConnectivity = channel.get_state(False)
+            COH_LOG.debug("New Channel State: transitioning from [%s] to [%s]", last_state, state)
             match state:
                 case grpc.ChannelConnectivity.SHUTDOWN:
-                    continue  # nothing to do
+                    COH_LOG.info("Session to [%s] terminated", session.options.address)
+                    await session._set_active(False)
                 case grpc.ChannelConnectivity.READY:
-                    if not first_connect and not connected:
+                    if not first_connect and not session.is_active():
+                        COH_LOG.info("Session re-established to [%s]", session.options.address)
+
                         await emitter.emit_async(SessionLifecycleEvent.RECONNECTED.value)
-                        connected = True
-                    elif first_connect and not connected:
+                        await session._set_active(True)
+                    elif first_connect and not session.is_active():
+                        COH_LOG.info("Session established to [%s]", session.options.address)
+
                         first_connect = False
-                        connected = True
                         await emitter.emit_async(SessionLifecycleEvent.CONNECTED.value)
+                        await session._set_active(True)
                 case _:
-                    if connected:
+                    if session.is_active():
+                        COH_LOG.warning("Session to [%s] disconnected; will attempt reconnect", session.options.address)
+
                         await emitter.emit_async(SessionLifecycleEvent.DISCONNECTED.value)
-                        connected = False
+                        await session._set_active(False)
 
-            await channel.wait_for_state_change(state)
+            COH_LOG.debug("Waiting for state change from [%s]", state)
+            await channel.wait_for_state_change(channel.get_state(True))
     except asyncio.CancelledError:
         return
 
 
 class _Stream(abc.ABC, AsyncIterator[T]):
     """
     A simple AsyncIterator that wraps a Callable that produces iteration
```

### Comparing `coherence_client-1.0b1/src/coherence/comparator.py` & `coherence_client-1.0rc1/src/coherence/comparator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/event.py` & `coherence_client-1.0rc1/src/coherence/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -603,14 +603,15 @@
         :param emitter:     the internal event emitter used to notify registered MapListeners
         """
         self._named_map = named_map
         self._client = client
         self._serializer = serializer
         self._emitter = emitter
         self._map_name = named_map.name
+        self._session = session
 
         self._key_map = {}
         self._filter_map = {}
         self._filter_id_listener_group_map = {}
         self._pending_registrations = {}
 
         self._request_factory = RequestFactory(self._map_name, session.scope, serializer)
@@ -641,33 +642,37 @@
         self._background_tasks.clear()
 
     # noinspection PyProtectedMember
     async def _reconnect(self) -> None:
         group: _ListenerGroup[K, V]
         for group in self._key_map.values():
             await group._subscribe(group._registered_lite)
-            await group._subscribed_waiter.wait()
-            group._subscribed_waiter.clear()
 
         for group in self._filter_map.values():
             await group._subscribe(group._registered_lite)
-            await group._subscribed_waiter.wait()
-            group._subscribed_waiter.clear()
 
     async def _ensure_stream(self) -> grpc.aio.StreamStreamCall:
         """
         Initialize the event stream for MapListener events.
         """
         if self._event_stream is None:
             event_stream: grpc.aio.StreamStreamCall = self._client.events()
             await event_stream.write(self._request_factory.map_event_subscribe())
             self._event_stream = event_stream
             read_task: Task[None] = asyncio.create_task(self._handle_response())
             self._background_tasks.add(read_task)
-            await self._stream_waiter.wait()
+            try:
+                async with asyncio.timeout(self._session.options.request_timeout_seconds):
+                    await self._stream_waiter.wait()
+            except TimeoutError:
+                raise TimeoutError(
+                    "Unable to establish session with [{0}] within [{1}] seconds)".format(
+                        self._session.options.address, str(self._session.options.request_timeout_seconds)
+                    )
+                )
 
         return self._event_stream
 
     async def _register_key_listener(self, listener: MapListener[K, V], key: K, lite: bool = False) -> None:
         """
         Registers the specified listener to listen for events matching the provided key.
         :param listener:  the MapListener to register
```

### Comparing `coherence_client-1.0b1/src/coherence/extractor.py` & `coherence_client-1.0rc1/src/coherence/extractor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/filter.py` & `coherence_client-1.0rc1/src/coherence/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,16 +127,17 @@
 
 @proxy("filter.GreaterFilter")
 class GreaterFilter(ComparisonFilter):
     def __init__(self, extractor: ExtractorExpression[T, E], value: V):
         """
         Construct a `GreaterFilter` for testing `Greater` condition.
 
-        :param extractor: the {@link extractor.ValueExtractor} to use by this :class:`coherence.filter.Filter` or the
-         name of the method to invoke via reflection
+        :param extractor: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
         :param value: the object to compare the result with
         """
         super().__init__(extractor, value)
 
 
 @proxy("filter.GreaterEqualsFilter")
 class GreaterEqualsFilter(ComparisonFilter):
@@ -432,15 +433,15 @@
 
         During pattern matching, regular characters must exactly match the characters in an evaluated string.
         Wildcard character `_` (underscore) can be matched with any single character, and wildcard character `%` can
         be matched with any string fragment of zero or more characters.
 
         Construct a `LikeFilter` for pattern match.
 
-        :param extractor_or_method: the {@link extractor.ValueExtractor} to use by this
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use by this
          :class:`coherence.filter.Filter` or the name of the method to invoke via reflection
         :param pattern: the string pattern to compare the result with
         :param escape_char: the escape character for escaping `%` and `_`
         :param ignore_case: `true` to be case-insensitive
         """
         super().__init__(extractor_or_method, pattern)
         self.escapeChar = escape_char
@@ -712,130 +713,175 @@
         """
 
         return MapEventFilter(mask, filter)
 
     @staticmethod
     def greater(extractor_or_method: ExtractorExpression[T, E], value: Any) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.GreaterFilter` to test
+        `Greater` condition
 
-        :param extractor_or_method:
-        :param value:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param value: the object to compare the result with
+        :return: an instance of :class:`coherence.filter.GreaterFilter`
         """
         return GreaterFilter(extractor_or_method, value)
 
     @staticmethod
     def greater_equals(extractor_or_method: ExtractorExpression[T, E], value: Any) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.GreaterEqualsFilter` to
+        test `Greater or Equal` condition
 
-        :param extractor_or_method:
-        :param value:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param value: the object to compare the result with
+        :return: an instance of :class:`coherence.filter.GreaterEqualsFilter`
         """
         return GreaterEqualsFilter(extractor_or_method, value)
 
     @staticmethod
     def is_in(extractor_or_method: ExtractorExpression[T, E], values: Set[Any]) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.InFilter` to check whether
+         the result of a method invocation belongs to a predefined set of values.
 
-        :param extractor_or_method:
-        :param values:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param values: the Set of values that a Collection or array is tested to contain
+        :return: an instance of :class:`coherence.filter.InFilter`
         """
         return InFilter(extractor_or_method, values)
 
     @staticmethod
     def is_not_none(extractor_or_method: ExtractorExpression[T, E]) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.IsNotNoneFilter` for
+        testing inequality to `None`.
 
-        :param extractor_or_method:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :return: an instance of :class:`coherence.filter.IsNotNoneFilter`
         """
         return IsNotNoneFilter(extractor_or_method)
 
     @staticmethod
     def is_none(extractor_or_method: ExtractorExpression[T, E]) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.IsNoneFilter` for
+        testing equality to `None`.
 
-        :param extractor_or_method:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :return: an instance of :class:`coherence.filter.IsNoneFilter`
         """
         return IsNoneFilter(extractor_or_method)
 
     @staticmethod
     def less(extractor_or_method: ExtractorExpression[T, E], value: Any) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.LessFilter` for testing
+        `Less` condition.
 
-        :param extractor_or_method:
-        :param value:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param value: the object to compare the result with
+        :return: an instance of :class:`coherence.filter.LessFilter`
         """
         return LessFilter(extractor_or_method, value)
 
     @staticmethod
     def less_equals(extractor_or_method: ExtractorExpression[T, E], value: Any) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.LessEqualsFilter` for testing
+        `Less or Equals` condition.
 
-        :param extractor_or_method:
-        :param value:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param value: the object to compare the result with
+        :return: an instance of :class:`coherence.filter.LessEqualsFilter`
         """
         return LessEqualsFilter(extractor_or_method, value)
 
     @staticmethod
     def like(
         extractor_or_method: ExtractorExpression[T, E], pattern: str, escape: str = "0", ignore_case: bool = False
     ) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.LikeFilter` for for pattern match
 
-        :param extractor_or_method:
-        :param pattern:
-        :param escape:
-        :param ignore_case:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use by this
+         :class:`coherence.filter.Filter` or the name of the method to invoke via reflection
+        :param pattern: the string pattern to compare the result with
+        :param escape: the escape character for escaping `%` and `_`
+        :param ignore_case: `true` to be case-insensitive
+        :return: an instance of :class:`coherence.filter.LikeFilter`
         """
         return LikeFilter(extractor_or_method, pattern, escape, ignore_case)
 
     @staticmethod
     def negate(filter: Filter) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.NotFilter` which negates
+         the results of another filter.
 
-        :param filter:
-        :return:
+        :param filter: The Filter whose results are negated by this filter.
+        :return: an instance of :class:`coherence.filter.NotFilter`
         """
         return NotFilter(filter)
 
     @staticmethod
     def never() -> Filter:
         """
+        Returns instance of :class:`coherence.filter.NeverFilter` which always
+        evaluates to `false`.
 
-        :return:
+        :return: an instance of :class:`coherence.filter.NeverFilter`
         """
         return NeverFilter()
 
     @staticmethod
     def not_equals(extractor_or_method: ExtractorExpression[T, E], value: Any) -> Filter:
         """
+        Returns instance of :class:`coherence.filter.NotEqualsFilter` for testing
+         inequality.
 
-        :param extractor_or_method:
-        :param value:
-        :return:
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param value: the object to compare the result with
+        :return: an instance of :class:`coherence.filter.NotEqualsFilter`
         """
         return NotEqualsFilter(extractor_or_method, value)
 
     @staticmethod
     def present() -> Filter:
         """
+        Returns instance of :class:`coherence.filter.PresentFilter` which
+         returns true for entries that currently exist in a map.
 
-        :return:
+        :return: an instance of :class:`coherence.filter.PresentFilter`
         """
         return PresentFilter()
 
     @staticmethod
     def regex(extractor_or_method: ExtractorExpression[T, E], regex: str) -> Filter:
         """
-
-        :param extractor_or_method:
-        :param regex:
-        :return:
+        Returns instance of :class:`coherence.filter.RegexFilter` which uses
+         the regular expression pattern match defined by the Java's
+         `String.matches` contract.
+
+        :param extractor_or_method: the :class:`coherence.extractor.ValueExtractor` to use
+         by this :class:`coherence.filter.Filter` or the name of the method to
+         invoke via reflection
+        :param regex: the regular expression to match the result with
+        :return: an instance of :class:`coherence.filter.RegexFilter`
         """
         return RegexFilter(extractor_or_method, regex)
```

### Comparing `coherence_client-1.0b1/src/coherence/messages_pb2.py` & `coherence_client-1.0rc1/src/coherence/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/processor.py` & `coherence_client-1.0rc1/src/coherence/processor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/serialization.py` & `coherence_client-1.0rc1/src/coherence/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,22 @@
                 return {"@class": "math.BigInt", "value": str(obj)}
 
         if isinstance(obj, set):
             return super()._flatten(list(obj))
 
         return super()._flatten(obj)
 
+    def _getstate(self, obj: Any, data: Any) -> Any:
+        state = self._flatten(obj)
+
+        if state is not None:
+            data.update(state)
+
+        return data
+
     def _flatten_obj(self, obj: Any) -> dict[str, str | dict[str, list[dict[str, Any]]]] | None:
         result = super()._flatten_obj(obj)
         object_type = type(obj)
         alias: Optional[str] = _alias_for(object_type)
         if alias is not None:
             marker = result.get("py/object", None)
             if marker is not None:
```

### Comparing `coherence_client-1.0b1/src/coherence/services_pb2.py` & `coherence_client-1.0rc1/src/coherence/services_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/services_pb2_grpc.py` & `coherence_client-1.0rc1/src/coherence/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/src/coherence/util.py` & `coherence_client-1.0rc1/src/coherence/util.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0b1/PKG-INFO` & `coherence_client-1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: coherence-client
-Version: 1.0b1
+Version: 1.0rc1
 Summary: The Coherence Python Client allows Python applications to act as cache clients to a Coherence Cluster using Google's gRPC framework as the network transport.
 Home-page: https://github.com/oracle/coherenc-py-client
 Author: Oracle
 Author-email: dhiru.pandey@oracle.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: grpcio (>=1.51,<1.52)
-Requires-Dist: grpcio-tools (>=1.51,<1.52)
-Requires-Dist: jsonpickle (>=2.2,<2.3)
-Requires-Dist: protobuf (>=4.21,<4.22)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: grpcio (>=1.54,<1.55)
+Requires-Dist: grpcio-tools (>=1.54,<1.55)
+Requires-Dist: jsonpickle (>=3.0,<3.1)
+Requires-Dist: protobuf (>=4.23,<4.24)
 Requires-Dist: pymitter (>=0.4,<0.5)
 Project-URL: Repository, https://github.com/oracle/coherenc-py-client
 Description-Content-Type: text/markdown
 
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
 [![License](http://img.shields.io/badge/license-UPL%201.0-blue.svg)](https://oss.oracle.com/licenses/upl/)
 
 <img src=https://oracle.github.io/coherence/assets/images/logo-red.png width="30%"><img>
 
-The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using
-the Google gRPC framework as the network transport.
+The Coherence Python Client allows Python applications to act as cache clients to an Oracle Coherence cluster using gRPC as the network transport.
 
 #### Features
 * Familiar Map-like interface for manipulating cache entries including but not limited to:
     * `put`, `put_if_absent`, `put_all`, `get`, `get_all`, `remove`, `clear`, `get_or_default`, `replace`, `replace_mapping`, `size`, `is_empty`, `contains_key`, `contains_value`
 * Cluster-side querying, aggregation and filtering of map entries
 * Cluster-side manipulation of map entries using EntryProcessors
 * Registration of listeners to be notified of:
     * mutations such as insert, update and delete on Maps
     * map lifecycle events such as truncated, released or destroyed
     * session lifecycle events such as connected, disconnected, reconnected and closed
 * Support for storing Python objects as JSON as well as the ability to serialize to Java objects on the server for access from other Coherence language API's
 
 #### Requirements
-* [Coherence CE](https://github.com/oracle/coherence) 22.06 or later (or equivalent non-open source editions) with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
-* Python 3.10.1
+* [Coherence CE](https://github.com/oracle/coherence) 22.06.4+ or Coherence 14.1.1.2206.4+ Commercial edition with a configured [gRPCProxy](https://docs.oracle.com/en/middleware/standalone/coherence/14.1.1.2206/develop-remote-clients/using-coherence-grpc-server.html).
+* Python 3.11.x
+
 
 #### Starting a Coherence Cluster
 
 Before testing the Python client, you must ensure a Coherence cluster is available.
 For local development, we recommend using the Coherence CE Docker image; it contains
 everything necessary for the client to operate correctly.
 
@@ -75,15 +74,15 @@
 from coherence import NamedCache, Session
 import asyncio
 
 
 async def run_test():
 
     # create a new Session to the Coherence server
-    session: Session = Session(None)
+    session: Session = await Session.create()
 
     # create a new NamedCache with key of string|int and value of string|int
     cache: NamedCache[str, str|int] = await session.get_cache("test")
 
     # put a new key/value
     k: str = "one"
     v: str = "only-one"
@@ -128,12 +127,12 @@
 
 ## Security
 
 Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process
 
 ## License
 
-Copyright (c) 2022, 2023 Oracle and/or its affiliates.
+Copyright (c) 2023 Oracle and/or its affiliates.
 
 Released under the Universal Permissive License v1.0 as shown at
 <https://oss.oracle.com/licenses/upl/>.
```

