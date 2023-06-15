# Comparing `tmp/rstream-0.7.0.tar.gz` & `tmp/rstream-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstream-0.7.0.tar", max compression
+gzip compressed data, was "rstream-0.8.0.tar", max compression
```

## Comparing `rstream-0.7.0.tar` & `rstream-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-05-22 09:13:56.508781 rstream-0.7.0/LICENSE
--rw-r--r--   0        0        0     6796 2023-05-22 09:13:56.508781 rstream-0.7.0/README.md
--rw-r--r--   0        0        0      660 2023-05-22 09:13:56.508781 rstream-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      799 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/__init__.py
--rw-r--r--   0        0        0      651 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/amqp.py
--rw-r--r--   0        0        0    17432 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/client.py
--rw-r--r--   0        0        0     4883 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/compression.py
--rw-r--r--   0        0        0     2117 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/connection.py
--rw-r--r--   0        0        0      928 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/constants.py
--rw-r--r--   0        0        0     8080 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/consumer.py
--rw-r--r--   0        0        0     5638 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/encoding.py
--rw-r--r--   0        0        0     1364 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/exceptions.py
--rw-r--r--   0        0        0    15804 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/producer.py
--rw-r--r--   0        0        0    15024 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/schema.py
--rw-r--r--   0        0        0      950 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/utils.py
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 rstream-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-15 14:49:11.010400 rstream-0.8.0/LICENSE
+-rw-r--r--   0        0        0     9865 2023-06-15 14:49:11.010400 rstream-0.8.0/README.md
+-rw-r--r--   0        0        0      734 2023-06-15 14:49:11.010400 rstream-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/__init__.py
+-rw-r--r--   0        0        0      651 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/amqp.py
+-rw-r--r--   0        0        0    18240 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/client.py
+-rw-r--r--   0        0        0     4883 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/compression.py
+-rw-r--r--   0        0        0     2117 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/connection.py
+-rw-r--r--   0        0        0      928 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/constants.py
+-rw-r--r--   0        0        0     8611 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/consumer.py
+-rw-r--r--   0        0        0     5638 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/encoding.py
+-rw-r--r--   0        0        0     1364 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/exceptions.py
+-rw-r--r--   0        0        0    15804 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/producer.py
+-rw-r--r--   0        0        0    16111 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/schema.py
+-rw-r--r--   0        0        0     2434 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream.py
+-rw-r--r--   0        0        0     5637 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream_consumer.py
+-rw-r--r--   0        0        0     4372 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/superstream_producer.py
+-rw-r--r--   0        0        0      950 2023-06-15 14:49:11.010400 rstream-0.8.0/rstream/utils.py
+-rw-r--r--   0        0        0    10575 1970-01-01 00:00:00.000000 rstream-0.8.0/PKG-INFO
```

### Comparing `rstream-0.7.0/LICENSE` & `rstream-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/README.md` & `rstream-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -155,38 +155,132 @@
 With `send_wait` instead will wait until the confirmation from the server is received.
 
 ### Consuming messages:
 
 ```python
 import asyncio
 import signal
-from rstream import Consumer, amqp_decoder, AMQPMessage
+from rstream import Consumer, amqp_decoder, AMQPMessage, MessageContext
 
 async def consume():
     consumer = Consumer(
         host='localhost',
         port=5552,
         vhost='/',
         username='guest',
         password='guest',
     )
 
     loop = asyncio.get_event_loop()
     loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
 
-    def on_message(msg: AMQPMessage):
-        print('Got message: {}'.format(msg.body))
+    def on_message(msg: AMQPMessage, message_context: MessageContext):
+        print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
 
     await consumer.start()
     await consumer.subscribe('mystream', on_message, decoder=amqp_decoder)
     await consumer.run()
 
 asyncio.run(consume())
 ```
 
+### Superstreams
+
+The client is also supporting superstream: https://blog.rabbitmq.com/posts/2022/07/rabbitmq-3-11-feature-preview-super-streams/
+A super stream is a logical stream made of individual, regular streams. It is a way to scale out publishing and consuming with RabbitMQ Streams: a large logical stream is divided into partition streams, splitting up the storage and the traffic on several cluster nodes.
+
+You can use superstream_producer and superstream_consumer classes which internally uses producers and consumers to operate on the componsing streams.
+
+How to create a superstream:
+
+```
+rabbitmq-streams add_super_stream orders  --routing-keys key1, key2,key3
+```
+
+How to send a message to a supersteream
+
+```python
+import asyncio
+import time
+import uamqp
+
+from rstream import Producer, AMQPMessage, ConfirmationStatus, CompressionType, SuperStreamProducer, RouteType
+
+async def routing_extractor(message: AMQPMessage) -> str:
+    return str(message.properties.message_id)
+
+async def publish():
+    global counter
+    counter = 0
+    sent = 0
+    async with SuperStreamProducer('localhost', username='guest', password='guest', super_stream='mixing', routing=RouteType.Hash, routing_extractor=routing_extractor) as producer:
+
+        messages = []
+        for i in range(1000):
+            amqp_message = AMQPMessage(
+                body='a:{}'.format(i),
+                properties=uamqp.message.MessageProperties(message_id=i),
+               
+            )
+           
+            await producer.send(message=amqp_message, on_publish_confirm=_on_publish_confirm_client)
+
+    
+        await asyncio.sleep(1)
+asyncio.run(publish())
+```
+
+How to consume from a superstream:
+
+```python
+import asyncio
+import signal
+from rstream import Consumer, amqp_decoder, AMQPMessage, SuperStreamConsumer, OffsetType, MessageContext
+from typing import Optional
+
+def on_message(msg: AMQPMessage, message_context: Optional[MessageContext]):
+    print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
+        
+async def consume():
+    print("consume")
+    consumer = SuperStreamConsumer(
+        host='localhost',
+        port=5552,
+        vhost='/',
+        username='guest',
+        password='guest',
+        super_stream='mixing'
+    )
+
+    loop = asyncio.get_event_loop()
+    loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
+
+    await consumer.start()
+    await consumer.subscribe(callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.FIRST)
+    await consumer.run()
+
+# main coroutine
+async def main():
+    print("starting")
+    # schedule the task
+    task = asyncio.create_task(consume())
+    # suspend a moment
+      # wait a moment
+    await asyncio.sleep(3)
+    # cancel the task
+    was_cancelled = task.cancel()
+   
+    # report a message
+    print('Main done')
+ 
+# run the asyncio program
+asyncio.run(main())
+```
+
+
 ### Connecting with SSL:
 
 ```python
 import ssl
 
 ssl_context = ssl.SSLContext()
 ssl_context.load_cert_chain('/path/to/certificate.pem', '/path/to/key.pem')
```

### Comparing `rstream-0.7.0/pyproject.toml` & `rstream-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [tool.poetry]
 name = "rstream"
-version = "0.7.0"
+version = "0.8.0"
 description = "A python client for RabbitMQ Streams"
 authors = ["George Fortunatov <qweeeze@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/qweeze/rstream"
 repository = "https://github.com/qweeze/rstream"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uamqp = "^1.6.3"
+requests = "^2.31.0"
+mmh3 = "^4.0.0"
 
 [tool.poetry.dev-dependencies]
 ipython = "^7.13.0"
 flake8 = "^3.9.2"
 isort = "^5.9.3"
 mypy = "^0.910"
 pytest = "^6.2.4"
 pytest-asyncio = "^0.15.1"
 black = "^21.9b0"
+requests = "^2.31.0"
+mmh3 = "^4.0.0"
 
 [tool.black]
 line-length = 110
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `rstream-0.7.0/rstream/__init__.py` & `rstream-0.8.0/rstream/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,35 @@
     __license__ = None
 
 del metadata
 
 from .amqp import AMQPMessage, amqp_decoder  # noqa: E402
 from .compression import CompressionType  # noqa: E402
 from .constants import OffsetType  # noqa: E402
-from .consumer import Consumer  # noqa: E402
+from .consumer import Consumer, MessageContext  # noqa: E402
 from .producer import (  # noqa: E402
     ConfirmationStatus,
     Producer,
     RawMessage,
 )
+from .superstream_consumer import (  # noqa: E402
+    SuperStreamConsumer,
+)
+from .superstream_producer import (  # noqa: E402
+    RouteType,
+    SuperStreamProducer,
+)
 
 __all__ = [
     "AMQPMessage",
     "amqp_decoder",
     "Consumer",
     "RawMessage",
     "Producer",
     "OffsetType",
     "ConfirmationStatus",
     "CompressionType",
+    "SuperStreamProducer",
+    "RouteType",
+    "SuperStreamConsumer",
+    "MessageContext",
 ]
```

### Comparing `rstream-0.7.0/rstream/amqp.py` & `rstream-0.8.0/rstream/amqp.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/client.py` & `rstream-0.8.0/rstream/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,14 +455,37 @@
         await self.send_frame(
             schema.Publish(
                 publisher_id=publisher_id,
                 messages=messages,
             ),
         )
 
+    async def partitions(self, super_stream: str) -> list[str]:
+        resp = await self.sync_request(
+            schema.SuperStreamPartitions(
+                self._corr_id_seq.next(),
+                super_stream=super_stream,
+            ),
+            resp_schema=schema.SuperStreamPartitionsResponse,
+            raise_exception=False,
+        )
+        return resp.streams
+
+    async def route(self, routing_key: str, super_stream: str) -> list[str]:
+        resp = await self.sync_request(
+            schema.SuperStreamRoute(
+                self._corr_id_seq.next(),
+                routing_key=routing_key,
+                super_stream=super_stream,
+            ),
+            resp_schema=schema.SuperStreamRouteResponse,
+            raise_exception=False,
+        )
+        return resp.streams
+
 
 class ClientPool:
     def __init__(
         self,
         host: str,
         port: int,
         *,
```

### Comparing `rstream-0.7.0/rstream/compression.py` & `rstream-0.8.0/rstream/compression.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/connection.py` & `rstream-0.8.0/rstream/connection.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/constants.py` & `rstream-0.8.0/rstream/constants.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/consumer.py` & `rstream-0.8.0/rstream/consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,36 @@
     Iterator,
     Optional,
     TypeVar,
     Union,
 )
 
 from . import exceptions, schema
+from .amqp import AMQPMessage
 from .client import Addr, Client, ClientPool
 from .constants import OffsetType
 
 MT = TypeVar("MT")
-CB = Annotated[Callable[[MT], Union[None, Awaitable[None]]], "Message callback type"]
+CB = Annotated[Callable[[MT, Any], Union[None, Awaitable[None]]], "Message callback type"]
+
+
+@dataclass
+class MessageContext:
+    stream: str
+    offset: int
+    timestamp: int
 
 
 @dataclass
 class _Subscriber:
     stream: str
     subscription_id: int
     reference: str
     client: Client
-    callback: CB[Any]
+    callback: Callable[[AMQPMessage, MessageContext], Union[None, Awaitable[None]]]
     decoder: Callable[[bytes], Any]
     offset_type: OffsetType
     offset: int
 
 
 class Consumer:
     def __init__(
@@ -112,15 +120,15 @@
 
         return self._clients[stream]
 
     async def _create_subscriber(
         self,
         stream: str,
         subscriber_name: Optional[str],
-        callback: CB[MT],
+        callback: Callable[[AMQPMessage, MessageContext], Union[None, Awaitable[None]]],
         decoder: Optional[Callable[[bytes], Any]],
         offset_type: OffsetType,
         offset: Optional[int],
     ) -> _Subscriber:
         client = await self._get_or_create_client(stream)
 
         # We can have multiple subscribers sharing same connection, so their ids must be distinct
@@ -139,15 +147,15 @@
             offset=offset or 0,
         )
         return subscriber
 
     async def subscribe(
         self,
         stream: str,
-        callback: CB[MT],
+        callback: Callable[[AMQPMessage, MessageContext], Union[None, Awaitable[None]]],
         *,
         decoder: Optional[Callable[[bytes], MT]] = None,
         offset: Optional[int] = None,
         offset_type: OffsetType = OffsetType.FIRST,
         initial_credit: int = 10,
         properties: Optional[dict[str, Any]] = None,
         subscriber_name: Optional[str] = None,
@@ -213,24 +221,26 @@
         for message in frame.get_messages():
             offset += 1
             if offset < min_deliverable_offset:
                 continue
 
             yield message
 
-        subscriber.offset = frame.chunk_first_offset + frame.num_entries
+        # subscriber.offset = frame.chunk_first_offset + frame.num_entries
 
     async def _on_deliver(self, frame: schema.Deliver, subscriber: _Subscriber) -> None:
         if frame.subscription_id != subscriber.subscription_id:
             return
 
         await subscriber.client.credit(subscriber.subscription_id, 1)
 
-        for message in self._filter_messages(frame, subscriber):
-            maybe_coro = subscriber.callback(subscriber.decoder(message))
+        for index, message in enumerate(self._filter_messages(frame, subscriber)):
+            subscriber.offset = frame.chunk_first_offset + frame.num_entries + index
+            message_context = MessageContext(subscriber.stream, subscriber.offset, frame.timestamp)
+            maybe_coro = subscriber.callback(subscriber.decoder(message), message_context)
             if maybe_coro is not None:
                 await maybe_coro
 
     async def create_stream(
         self,
         stream: str,
         arguments: Optional[dict[str, Any]] = None,
```

### Comparing `rstream-0.7.0/rstream/encoding.py` & `rstream-0.8.0/rstream/encoding.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/exceptions.py` & `rstream-0.8.0/rstream/exceptions.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/producer.py` & `rstream-0.8.0/rstream/producer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/rstream/schema.py` & `rstream-0.8.0/rstream/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -479,7 +479,40 @@
 
 
 @dataclass
 class CreditResponse(Frame, is_response=True):
     key = Key.Credit
     response_code: int = field(metadata={"type": T.uint16})
     subscription_id: int = field(metadata={"type": T.uint8})
+
+
+# For new super stream implementation
+@dataclass
+class SuperStreamRoute(Frame):
+    key = Key.Route
+    # version : int = field(metadata={"type": T.uint16})
+    correlation_id: int = field(metadata={"type": T.uint32})
+    routing_key: str = field(metadata={"type": T.string})
+    super_stream: str = field(metadata={"type": T.string})
+
+
+@dataclass
+class SuperStreamRouteResponse(Frame, is_response=True):
+    key = Key.Route
+    correlation_id: int = field(metadata={"type": T.uint32})
+    response_code: int = field(metadata={"type": T.uint16})
+    streams: list[str] = field(metadata={"type": [T.string]})
+
+
+@dataclass
+class SuperStreamPartitions(Frame):
+    key = Key.Partitions
+    correlation_id: int = field(metadata={"type": T.uint32})
+    super_stream: str = field(metadata={"type": T.string})
+
+
+@dataclass
+class SuperStreamPartitionsResponse(Frame, is_response=True):
+    key = Key.Partitions
+    correlation_id: int = field(metadata={"type": T.uint32})
+    response_code: int = field(metadata={"type": T.uint16})
+    streams: list[str] = field(metadata={"type": [T.string]})
```

### Comparing `rstream-0.7.0/rstream/utils.py` & `rstream-0.8.0/rstream/utils.py`

 * *Files identical despite different names*

### Comparing `rstream-0.7.0/PKG-INFO` & `rstream-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rstream
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python client for RabbitMQ Streams
 Home-page: https://github.com/qweeze/rstream
 License: MIT
 Author: George Fortunatov
 Author-email: qweeeze@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: mmh3 (>=4.0.0,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uamqp (>=1.6.3,<2.0.0)
 Project-URL: Repository, https://github.com/qweeze/rstream
 Description-Content-Type: text/markdown
 
 # RabbitMQ Stream Python Client
 
 A Python asyncio-based client for [RabbitMQ Streams](https://github.com/rabbitmq/rabbitmq-server/tree/master/deps/rabbitmq_stream)
@@ -173,38 +175,132 @@
 With `send_wait` instead will wait until the confirmation from the server is received.
 
 ### Consuming messages:
 
 ```python
 import asyncio
 import signal
-from rstream import Consumer, amqp_decoder, AMQPMessage
+from rstream import Consumer, amqp_decoder, AMQPMessage, MessageContext
 
 async def consume():
     consumer = Consumer(
         host='localhost',
         port=5552,
         vhost='/',
         username='guest',
         password='guest',
     )
 
     loop = asyncio.get_event_loop()
     loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
 
-    def on_message(msg: AMQPMessage):
-        print('Got message: {}'.format(msg.body))
+    def on_message(msg: AMQPMessage, message_context: MessageContext):
+        print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
 
     await consumer.start()
     await consumer.subscribe('mystream', on_message, decoder=amqp_decoder)
     await consumer.run()
 
 asyncio.run(consume())
 ```
 
+### Superstreams
+
+The client is also supporting superstream: https://blog.rabbitmq.com/posts/2022/07/rabbitmq-3-11-feature-preview-super-streams/
+A super stream is a logical stream made of individual, regular streams. It is a way to scale out publishing and consuming with RabbitMQ Streams: a large logical stream is divided into partition streams, splitting up the storage and the traffic on several cluster nodes.
+
+You can use superstream_producer and superstream_consumer classes which internally uses producers and consumers to operate on the componsing streams.
+
+How to create a superstream:
+
+```
+rabbitmq-streams add_super_stream orders  --routing-keys key1, key2,key3
+```
+
+How to send a message to a supersteream
+
+```python
+import asyncio
+import time
+import uamqp
+
+from rstream import Producer, AMQPMessage, ConfirmationStatus, CompressionType, SuperStreamProducer, RouteType
+
+async def routing_extractor(message: AMQPMessage) -> str:
+    return str(message.properties.message_id)
+
+async def publish():
+    global counter
+    counter = 0
+    sent = 0
+    async with SuperStreamProducer('localhost', username='guest', password='guest', super_stream='mixing', routing=RouteType.Hash, routing_extractor=routing_extractor) as producer:
+
+        messages = []
+        for i in range(1000):
+            amqp_message = AMQPMessage(
+                body='a:{}'.format(i),
+                properties=uamqp.message.MessageProperties(message_id=i),
+               
+            )
+           
+            await producer.send(message=amqp_message, on_publish_confirm=_on_publish_confirm_client)
+
+    
+        await asyncio.sleep(1)
+asyncio.run(publish())
+```
+
+How to consume from a superstream:
+
+```python
+import asyncio
+import signal
+from rstream import Consumer, amqp_decoder, AMQPMessage, SuperStreamConsumer, OffsetType, MessageContext
+from typing import Optional
+
+def on_message(msg: AMQPMessage, message_context: Optional[MessageContext]):
+    print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
+        
+async def consume():
+    print("consume")
+    consumer = SuperStreamConsumer(
+        host='localhost',
+        port=5552,
+        vhost='/',
+        username='guest',
+        password='guest',
+        super_stream='mixing'
+    )
+
+    loop = asyncio.get_event_loop()
+    loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
+
+    await consumer.start()
+    await consumer.subscribe(callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.FIRST)
+    await consumer.run()
+
+# main coroutine
+async def main():
+    print("starting")
+    # schedule the task
+    task = asyncio.create_task(consume())
+    # suspend a moment
+      # wait a moment
+    await asyncio.sleep(3)
+    # cancel the task
+    was_cancelled = task.cancel()
+   
+    # report a message
+    print('Main done')
+ 
+# run the asyncio program
+asyncio.run(main())
+```
+
+
 ### Connecting with SSL:
 
 ```python
 import ssl
 
 ssl_context = ssl.SSLContext()
 ssl_context.load_cert_chain('/path/to/certificate.pem', '/path/to/key.pem')
```

