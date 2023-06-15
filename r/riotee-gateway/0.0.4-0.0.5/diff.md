# Comparing `tmp/riotee_gateway-0.0.4.tar.gz` & `tmp/riotee_gateway-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_gateway-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_gateway-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_gateway-0.0.4.tar` & `riotee_gateway-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1101 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      518 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      514 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/__init__.py
--rw-r--r--   0        0        0     2675 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/cli.py
--rw-r--r--   0        0        0     2910 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/client.py
--rw-r--r--   0        0        0     3876 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/packet_model.py
--rw-r--r--   0        0        0     2544 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/server.py
--rw-r--r--   0        0        0     1827 2023-06-13 13:21:36.443366 riotee_gateway-0.0.4/riotee_gateway/transceiver.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      518 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      514 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/__init__.py
+-rw-r--r--   0        0        0     2904 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/cli.py
+-rw-r--r--   0        0        0     2910 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/client.py
+-rw-r--r--   0        0        0     3876 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/packet_model.py
+-rw-r--r--   0        0        0     2547 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/server.py
+-rw-r--r--   0        0        0     1827 2023-06-15 10:03:38.367715 riotee_gateway-0.0.5/riotee_gateway/transceiver.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.5/PKG-INFO
```

### Comparing `riotee_gateway-0.0.4/LICENSE.txt` & `riotee_gateway-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.4/pyproject.toml` & `riotee_gateway-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.4/riotee_gateway/__init__.py` & `riotee_gateway-0.0.5/riotee_gateway/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Riotee Gateway Python package"""
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 import base64
 import numpy as np
 
 from riotee_gateway.client import GatewayClient
 from riotee_gateway.transceiver import Transceiver
```

### Comparing `riotee_gateway-0.0.4/riotee_gateway/cli.py` & `riotee_gateway-0.0.5/riotee_gateway/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 import logging
 import uvicorn
 from riotee_gateway.client import GatewayClient
+import riotee_gateway.server
+from riotee_gateway import Transceiver
 import time
 import signal
 import sys
 import json
 
 @click.option("-v", "--verbose", count=True, default=2)
 @click.option("-p", "--port", type=int, default=8000, help="Port for API server")
@@ -23,17 +25,24 @@
         logging.basicConfig(level=logging.DEBUG)
 
     ctx.obj["host"] = host
     ctx.obj["port"] = port
 
 
 @cli.command(short_help="server stuff")
+@click.option(
+    "--device",
+    "-d",
+    type=click.Path(exists=True),
+    required=False,
+    help="Path to USB device",
+)
 @click.pass_context
-def server(ctx):
-    click.echo("Here to serve")
+def server(ctx, device):
+    riotee_gateway.server.tcv = Transceiver(port=device)
     uvicorn.run("riotee_gateway.server:app", port=ctx.obj["port"], host=ctx.obj["host"])
 
 
 @cli.group(short_help="client stuff")
 @click.pass_context
 def client(ctx):
     ctx.obj["client"] = GatewayClient(ctx.obj["host"], ctx.obj["port"])
```

### Comparing `riotee_gateway-0.0.4/riotee_gateway/client.py` & `riotee_gateway-0.0.5/riotee_gateway/client.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.4/riotee_gateway/packet_model.py` & `riotee_gateway-0.0.5/riotee_gateway/packet_model.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.4/riotee_gateway/server.py` & `riotee_gateway-0.0.5/riotee_gateway/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     while True:
         pkt = await tcv.read_packet()
         db.add(pkt)
         logging.debug(
             f"Got packet from {pkt.dev_id} with ID {pkt.pkt_id} @{pkt.timestamp}"
         )
 
-
-tcv = Transceiver()
+tcv: Transceiver = None
 db = PacketDatabase()
 app = FastAPI()
 
 
 @app.get("/")
 async def get_root():
     return "Welcome to the Riotee Gateway!"
```

### Comparing `riotee_gateway-0.0.4/riotee_gateway/transceiver.py` & `riotee_gateway-0.0.5/riotee_gateway/transceiver.py`

 * *Files identical despite different names*

