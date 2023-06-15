# Comparing `tmp/misskey_python-1.0.tar.gz` & `tmp/misskey_python-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misskey_python-1.0.tar", max compression
+gzip compressed data, was "misskey_python-1.1.tar", max compression
```

## Comparing `misskey_python-1.0.tar` & `misskey_python-1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      137 2023-06-14 21:45:27.869305 misskey_python-1.0/MiPC/__init__.py
--rw-r--r--   0        0        0      273 2023-06-11 18:10:32.427114 misskey_python-1.0/MiPC/exceptions.py
--rw-r--r--   0        0        0     1303 2023-06-14 19:33:02.951882 misskey_python-1.0/MiPC/MiAuth/__main__.py
--rw-r--r--   0        0        0     2201 2023-06-14 21:45:31.410385 misskey_python-1.0/MiPC/MiAuth/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     1300 2023-06-14 18:17:15.540066 misskey_python-1.0/MiPC/mihttp.py
--rw-r--r--   0        0        0    12490 2023-06-14 22:33:40.585384 misskey_python-1.0/MiPC/Misskey.py
--rw-r--r--   0        0        0      498 2023-06-14 21:55:10.887744 misskey_python-1.0/MiPC/新規 Python File.py
--rw-r--r--   0        0        0      495 2023-06-11 17:37:48.981322 misskey_python-1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 18:57:26.461287 misskey_python-1.0/README.md
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 misskey_python-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-15 06:34:58.016922 misskey_python-1.1/LICENSE
+-rw-r--r--   0        0        0      133 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/exceptions.py
+-rw-r--r--   0        0        0     1300 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/http.py
+-rw-r--r--   0        0        0     1303 2023-06-15 06:34:58.017435 misskey_python-1.1/MiPC/MiAuth/__main__.py
+-rw-r--r--   0        0        0    11502 2023-06-15 06:34:58.017435 misskey_python-1.1/MiPC/Misskey.py
+-rw-r--r--   0        0        0      495 2023-06-15 06:34:58.025449 misskey_python-1.1/pyproject.toml
+-rw-r--r--   0        0        0      634 2023-06-15 06:34:58.019447 misskey_python-1.1/README.md
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 misskey_python-1.1/PKG-INFO
```

### Comparing `misskey_python-1.0/MiPC/MiAuth/__main__.py` & `misskey_python-1.1/MiPC/MiAuth/__main__.py`

 * *Files identical despite different names*

### Comparing `misskey_python-1.0/MiPC/mihttp.py` & `misskey_python-1.1/MiPC/http.py`

 * *Files identical despite different names*

### Comparing `misskey_python-1.0/MiPC/Misskey.py` & `misskey_python-1.1/MiPC/Misskey.py`

 * *Files 5% similar despite different names*

```diff
@@ -239,101 +239,69 @@
                         headers=head
                     )
                     return r.json()
                 
 class StreamingClient():
 
     class context:
-        
-        class nt:
-            id = ""
-        
-        class auth:
-            class hst:
-                name = ""
-                software = ""
-                softwareversion = ""
-                icon = ""
-                favicon = ""
-                color = ""
-            id = ""
-            name = ""
-            username = ""
-            host = hst()
-        
-        class rid:
-            id = ""
-            
-        class rnid:
-            id = ""
-        
-        note = nt()
-        author = auth()
-        reply = rid()
-        renote = rnid()
+        pass
 
     def __init__(self, server, token):
         self.__token = token
         self.__pattern = "^ws:\/\/.*"
         if re.match(self.__pattern, server):
             self.__server = server
         else:
             self.__server = "wss://" + server
 
     def run(self):
         async def runner(self):
-            self.__ws = await websockets.connect(f'{self.__server}/streaming?i={self.__token}')
+            self.__ws = await websockets.connect(f{self.__server}/streaming?i={self.__token}')
             try:
                 await self.on_ready()
             except AttributeError:
                 pass
             while True:
-                response = await self.__ws.recv()
+                response = await self.recv()
                 response = json.loads(response)
                 if response["body"]["type"] == "note":
                     try:
                         ctx = self.context()
                         ctx.note.id = response["body"]["body"]["id"]
                         ctx.author.id = response["body"]["body"]["userId"]
-                        if not response["body"]["body"]["user"]["name"] == '':
-                            ctx.author.name = response["body"]["body"]["user"]["name"]
-                        else:
-                            ctx.author.name = "null"
+                        ctx.author.name = response["body"]["body"]["user"]["name"]
                         ctx.author.username = response["body"]["body"]["user"]["username"]
                         ctx.text = response["body"]["body"]["text"]
                         ctx.reactions = response["body"]["body"]["reactions"]
                         ctx.files = response["body"]["body"]["files"]
                         ctx.fileId = response["body"]["body"]["fileIds"]
                         ctx.reply.id = response["body"]["body"]["replyId"]
                         ctx.renote.id = response["body"]["body"]["renoteId"]
-                        try:
-                            ctx.mention = response["body"]["body"]["mentions"]
-                        except KeyError:
-                            ctx.mention = None
+                        ctx.uri = response["body"]["body"]["uri"]
+                        ctx.url = response["body"]["body"]["url"]
                         if response["body"]["body"]["user"]["host"] is not None:
                             ctx.author.host = response["body"]["body"]["user"]["host"]
                             ctx.author.host.name = response["body"]["body"]["user"]["instance"]["name"]
                             ctx.author.host.software = response["body"]["body"]["user"]["instance"]["softwareName"]
                             ctx.author.host.softwareversion = response["body"]["body"]["user"]["instance"]["softwareVersion"]
                             ctx.author.host.icon = response["body"]["body"]["user"]["instance"]["iconUrl"]
                             ctx.author.host.favicon = response["body"]["body"]["user"]["instance"]["faviconUrl"]
                             ctx.author.host.color = response["body"]["body"]["user"]["instance"]["themeColor"]
-                            ctx.uri = response["body"]["body"]["uri"]
-                            ctx.url = response["body"]["body"]["url"]
                         else:
                             ctx.author.host = None
                         await self.on_note(ctx)
-                    except AttributeError as e:
-                        print(traceback.format_exc())
+                    except AttributeError:
+                        pass
         asyncio.run(runner(self))
 
     async def send(self, message):
         await self.__ws.send(json.dumps(message, indent=4, ensure_ascii=False))
 
     async def connect(self, channel):
-        await self.__ws.send(json.dumps({"type": "connect", "body": {"channel": channel,"id": channel}}, indent=4, ensure_ascii=False))
+        await self.__ws.send(json.dumps({"type": "connect", "body": {"channel": channel, "id": channel}}, indent=4, ensure_ascii=False))
 
     async def disconnect(self, channel):
         await self.__ws.send(json.dumps({"type": "disconnect", "body": {"id": channel}}, indent=4, ensure_ascii=False))
 
+
     async def recv(self):
-        return await self.__ws.recv()
+        return await self.__ws.recv()
```

