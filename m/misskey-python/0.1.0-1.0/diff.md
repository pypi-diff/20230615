# Comparing `tmp/misskey_python-0.1.0.tar.gz` & `tmp/misskey_python-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misskey_python-0.1.0.tar", max compression
+gzip compressed data, was "misskey_python-1.0.tar", max compression
```

## Comparing `misskey_python-0.1.0.tar` & `misskey_python-1.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0       53 2023-06-04 09:10:27.546250 misskey_python-0.1.0/MiPC/__init__.py
--rw-r--r--   0        0        0      183 2023-06-03 18:49:17.222680 misskey_python-0.1.0/MiPC/exceptions.py
--rw-r--r--   0        0        0       29 2023-06-04 09:12:14.258816 misskey_python-0.1.0/MiPC/MiAuth/__init__.py
--rw-r--r--   0        0        0      199 2023-06-04 09:12:18.906910 misskey_python-0.1.0/MiPC/MiAuth/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2190 2023-06-04 22:35:30.851148 misskey_python-0.1.0/MiPC/MiAuth/__pycache__/create_session.cpython-311.pyc
--rw-r--r--   0        0        0     1295 2023-06-04 22:34:31.448822 misskey_python-0.1.0/MiPC/MiAuth/create_session.py
--rw-r--r--   0        0        0     8135 2023-06-05 07:22:38.772929 misskey_python-0.1.0/MiPC/MiAuth/example.json
--rw-r--r--   0        0        0      198 2023-06-05 07:22:37.533993 misskey_python-0.1.0/MiPC/MiAuth/新規 Python File.py
--rw-r--r--   0        0        0     7942 2023-06-08 16:08:31.039028 misskey_python-0.1.0/MiPC/Misskey.py
--rw-r--r--   0        0        0      530 2023-06-08 21:47:57.036069 misskey_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 18:57:26.461287 misskey_python-0.1.0/README.md
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 misskey_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      137 2023-06-14 21:45:27.869305 misskey_python-1.0/MiPC/__init__.py
+-rw-r--r--   0        0        0      273 2023-06-11 18:10:32.427114 misskey_python-1.0/MiPC/exceptions.py
+-rw-r--r--   0        0        0     1303 2023-06-14 19:33:02.951882 misskey_python-1.0/MiPC/MiAuth/__main__.py
+-rw-r--r--   0        0        0     2201 2023-06-14 21:45:31.410385 misskey_python-1.0/MiPC/MiAuth/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     1300 2023-06-14 18:17:15.540066 misskey_python-1.0/MiPC/mihttp.py
+-rw-r--r--   0        0        0    12490 2023-06-14 22:33:40.585384 misskey_python-1.0/MiPC/Misskey.py
+-rw-r--r--   0        0        0      498 2023-06-14 21:55:10.887744 misskey_python-1.0/MiPC/新規 Python File.py
+-rw-r--r--   0        0        0      495 2023-06-11 17:37:48.981322 misskey_python-1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 18:57:26.461287 misskey_python-1.0/README.md
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 misskey_python-1.0/PKG-INFO
```

### Comparing `misskey_python-0.1.0/MiPC/MiAuth/__pycache__/create_session.cpython-311.pyc` & `misskey_python-1.0/MiPC/MiAuth/__pycache__/__main__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x77117d64 (Sun Jun  4 22:34:31 2023 UTC)
-files sz: 1295
+moddate:  0xee158a64 (Wed Jun 14 19:33:02 2023 UTC)
+files sz: 1303
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -37,15 +37,15 @@
                 38 IMPORT_NAME              4 (MiPC.exceptions)
                 40 IMPORT_FROM              5 (MisskeyMiAuthFailedException)
                 42 STORE_NAME               5 (MisskeyMiAuthFailedException)
                 44 POP_TOP
    
      9          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               3 (<code object MiAuth, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\create_session.py", line 9>)
+                50 LOAD_CONST               3 (<code object MiAuth, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\__main__.py", line 9>)
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               4 ('MiAuth')
                 56 PRECALL                  2
                 60 CALL                     2
                 70 STORE_NAME               6 (MiAuth)
                 72 LOAD_CONST               1 (None)
                 74 RETURN_VALUE
@@ -55,42 +55,45 @@
       ('MisskeyMiAuthFailedException',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
-            0x970065005a0164005a02640184005a0367006402a2016601640384015a
-            04640484005a0564055300
+            0x970065005a0164005a026408640384015a0367006404a2016601640584
+            015a04640684005a0564075300
            9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MiAuth')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               1 (<code object __init__, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\create_session.py", line 11>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (__init__)
+          11          10 LOAD_CONST               8 (('misskey.io', 'MiPC App'))
+                      12 LOAD_CONST               3 (<code object __init__, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\__main__.py", line 11>)
+                      14 MAKE_FUNCTION            1 (defaults)
+                      16 STORE_NAME               3 (__init__)
          
-          17          16 BUILD_LIST               0
-                      18 LOAD_CONST               2 (('read:account', 'write:account', 'read:blocks', 'write:blocks', 'read:drive', 'write:drive', 'read:favorites', 'write:favorites', 'read:following', 'write:following', 'read:messaging', 'write:messaging', 'read:mutes', 'write:mutes', 'write:notes', 'read:notifications', 'write:notifications', 'write:reactions', 'write:votes', 'read:pages', 'write:pages', 'write:page-likes', 'read:page-likes', 'write:gallery-likes', 'read:gallery-likes'))
-                      20 LIST_EXTEND              1
+          17          18 BUILD_LIST               0
+                      20 LOAD_CONST               4 (('read:account', 'write:account', 'read:blocks', 'write:blocks', 'read:drive', 'write:drive', 'read:favorites', 'write:favorites', 'read:following', 'write:following', 'read:messaging', 'write:messaging', 'read:mutes', 'write:mutes', 'write:notes', 'read:notifications', 'write:notifications', 'write:reactions', 'write:votes', 'read:pages', 'write:pages', 'write:page-likes', 'read:page-likes', 'write:gallery-likes', 'read:gallery-likes'))
+                      22 LIST_EXTEND              1
          
-          15          22 BUILD_TUPLE              1
-                      24 LOAD_CONST               3 (<code object generate_url, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\create_session.py", line 15>)
-                      26 MAKE_FUNCTION            1 (defaults)
-                      28 STORE_NAME               4 (generate_url)
+          15          24 BUILD_TUPLE              1
+                      26 LOAD_CONST               5 (<code object generate_url, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\__main__.py", line 15>)
+                      28 MAKE_FUNCTION            1 (defaults)
+                      30 STORE_NAME               4 (generate_url)
          
-          23          30 LOAD_CONST               4 (<code object get_token, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\create_session.py", line 23>)
-                      32 MAKE_FUNCTION            0
-                      34 STORE_NAME               5 (get_token)
-                      36 LOAD_CONST               5 (None)
-                      38 RETURN_VALUE
+          23          32 LOAD_CONST               6 (<code object get_token, file "C:\Users\hm74c\Desktop\MiPC\MiPC\MiAuth\__main__.py", line 23>)
+                      34 MAKE_FUNCTION            0
+                      36 STORE_NAME               5 (get_token)
+                      38 LOAD_CONST               7 (None)
+                      40 RETURN_VALUE
          consts
             'MiAuth'
+            'misskey.io'
+            'MiPC App'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
@@ -108,161 +111,157 @@
                             32 RETURN_VALUE
                consts
                   None
                names      ('server', 'name')
                varnames   ('self', 'server', 'name')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\create_session.py'
+               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\__main__.py'
                name       '__init__'
                firstlineno 11
                lnotab 0x02010e01
             ('read:account', 'write:account', 'read:blocks', 'write:blocks', 'read:drive', 'write:drive', 'read:favorites', 'write:favorites', 'read:following', 'write:following', 'read:messaging', 'write:messaging', 'read:mutes', 'write:mutes', 'write:notes', 'read:notifications', 'write:notifications', 'write:reactions', 'write:votes', 'read:pages', 'write:pages', 'write:page-likes', 'read:page-likes', 'write:gallery-likes', 'read:gallery-likes')
             code
                argcount  : 2
                nlocals   : 3
-               stacksize : 10
+               stacksize : 9
                flags     : 3
                code
                   0x97007401000000000000000000006a010000000000000000a6000000ab
-                  0000000000000000007c005f02000000000000000064017c006a03000000
-                  00000000009b0064027c006a0200000000000000009b0064037c006a0400
-                  000000000000009b0064046405a005000000000000000000000000000000
-                  00000000007c01a6010000ab0100000000000000009b009d087d027c0253
-                  00
+                  0000000000000000007c005f0200000000000000007c006a030000000000
+                  0000009b0064017c006a0200000000000000009b0064027c006a04000000
+                  00000000009b0064036404a0050000000000000000000000000000000000
+                  0000007c01a6010000ab0100000000000000009b009d077d027c025300
                 15           0 RESUME                   0
                
                 19           2 LOAD_GLOBAL              1 (NULL + uuid)
                             14 LOAD_ATTR                1 (uuid4)
                             24 PRECALL                  0
                             28 CALL                     0
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               2 (session_id)
                
-                20          50 LOAD_CONST               1 ('https://')
-                            52 LOAD_FAST                0 (self)
-                            54 LOAD_ATTR                3 (server)
-                            64 FORMAT_VALUE             0
-                            66 LOAD_CONST               2 ('/miauth/')
-                            68 LOAD_FAST                0 (self)
-                            70 LOAD_ATTR                2 (session_id)
-                            80 FORMAT_VALUE             0
-                            82 LOAD_CONST               3 ('?name=')
-                            84 LOAD_FAST                0 (self)
-                            86 LOAD_ATTR                4 (name)
-                            96 FORMAT_VALUE             0
-                            98 LOAD_CONST               4 ('&permission=')
-                           100 LOAD_CONST               5 (',')
-                           102 LOAD_METHOD              5 (join)
-                           124 LOAD_FAST                1 (permission)
-                           126 PRECALL                  1
-                           130 CALL                     1
-                           140 FORMAT_VALUE             0
-                           142 BUILD_STRING             8
-                           144 STORE_FAST               2 (url)
+                20          50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                3 (server)
+                            62 FORMAT_VALUE             0
+                            64 LOAD_CONST               1 ('/miauth/')
+                            66 LOAD_FAST                0 (self)
+                            68 LOAD_ATTR                2 (session_id)
+                            78 FORMAT_VALUE             0
+                            80 LOAD_CONST               2 ('?name=')
+                            82 LOAD_FAST                0 (self)
+                            84 LOAD_ATTR                4 (name)
+                            94 FORMAT_VALUE             0
+                            96 LOAD_CONST               3 ('&permission=')
+                            98 LOAD_CONST               4 (',')
+                           100 LOAD_METHOD              5 (join)
+                           122 LOAD_FAST                1 (permission)
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 FORMAT_VALUE             0
+                           140 BUILD_STRING             7
+                           142 STORE_FAST               2 (url)
                
-                21         146 LOAD_FAST                2 (url)
-                           148 RETURN_VALUE
+                21         144 LOAD_FAST                2 (url)
+                           146 RETURN_VALUE
                consts
                   None
-                  'https://'
                   '/miauth/'
                   '?name='
                   '&permission='
                   ','
                names      ('uuid', 'uuid4', 'session_id', 'server', 'name', 'join')
                varnames   ('self', 'permission', 'url')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\create_session.py'
+               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\__main__.py'
                name       'generate_url'
                firstlineno 15
-               lnotab 0x020430016001
+               lnotab 0x020430015e01
             code
                argcount  : 1
                nlocals   : 4
-               stacksize : 5
+               stacksize : 4
                flags     : 3
                code
-                  0x970064017c006a0000000000000000009b0064027c006a010000000000
-                  0000009b0064039d057d017405000000000000000000006a030000000000
-                  0000007c01a6010000ab0100000000000000007d027c02a0040000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007d
-                  037c0364041900000000000000000072087c036405190000000000000000
-                  005300740b000000000000000000006406a6010000ab0100000000000000
-                  008201
+                  0x97007c006a0000000000000000009b0064017c006a0100000000000000
+                  009b0064029d047d017405000000000000000000006a0300000000000000
+                  007c01a6010000ab0100000000000000007d027c02a00400000000000000
+                  00000000000000000000000000a6000000ab0000000000000000007d037c
+                  0364031900000000000000000072087c0364041900000000000000000053
+                  00740b000000000000000000006405a6010000ab01000000000000000082
+                  01
                 23           0 RESUME                   0
                
-                26           2 LOAD_CONST               1 ('https://')
-                             4 LOAD_FAST                0 (self)
-                             6 LOAD_ATTR                0 (server)
-                            16 FORMAT_VALUE             0
-                            18 LOAD_CONST               2 ('/api/miauth/')
-                            20 LOAD_FAST                0 (self)
-                            22 LOAD_ATTR                1 (session_id)
-                            32 FORMAT_VALUE             0
-                            34 LOAD_CONST               3 ('/check')
-                            36 BUILD_STRING             5
-                            38 STORE_FAST               1 (url)
-               
-                27          40 LOAD_GLOBAL              5 (NULL + httpx)
-                            52 LOAD_ATTR                3 (post)
-                            62 LOAD_FAST                1 (url)
-                            64 PRECALL                  1
-                            68 CALL                     1
-                            78 STORE_FAST               2 (response)
-               
-                28          80 LOAD_FAST                2 (response)
-                            82 LOAD_METHOD              4 (json)
-                           104 PRECALL                  0
-                           108 CALL                     0
-                           118 STORE_FAST               3 (response_json)
-               
-                29         120 LOAD_FAST                3 (response_json)
-                           122 LOAD_CONST               4 ('ok')
-                           124 BINARY_SUBSCR
-                           134 POP_JUMP_FORWARD_IF_FALSE     8 (to 152)
-               
-                30         136 LOAD_FAST                3 (response_json)
-                           138 LOAD_CONST               5 ('token')
-                           140 BINARY_SUBSCR
-                           150 RETURN_VALUE
-               
-                32     >>  152 LOAD_GLOBAL             11 (NULL + MisskeyMiAuthFailedException)
-                           164 LOAD_CONST               6 ('ログイン失敗')
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 RAISE_VARARGS            1
+                26           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (server)
+                            14 FORMAT_VALUE             0
+                            16 LOAD_CONST               1 ('/api/miauth/')
+                            18 LOAD_FAST                0 (self)
+                            20 LOAD_ATTR                1 (session_id)
+                            30 FORMAT_VALUE             0
+                            32 LOAD_CONST               2 ('/check')
+                            34 BUILD_STRING             4
+                            36 STORE_FAST               1 (url)
+               
+                27          38 LOAD_GLOBAL              5 (NULL + httpx)
+                            50 LOAD_ATTR                3 (post)
+                            60 LOAD_FAST                1 (url)
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 STORE_FAST               2 (response)
+               
+                28          78 LOAD_FAST                2 (response)
+                            80 LOAD_METHOD              4 (json)
+                           102 PRECALL                  0
+                           106 CALL                     0
+                           116 STORE_FAST               3 (response_json)
+               
+                29         118 LOAD_FAST                3 (response_json)
+                           120 LOAD_CONST               3 ('ok')
+                           122 BINARY_SUBSCR
+                           132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
+               
+                30         134 LOAD_FAST                3 (response_json)
+                           136 LOAD_CONST               4 ('token')
+                           138 BINARY_SUBSCR
+                           148 RETURN_VALUE
+               
+                32     >>  150 LOAD_GLOBAL             11 (NULL + MisskeyMiAuthFailedException)
+                           162 LOAD_CONST               5 ('ログイン失敗')
+                           164 PRECALL                  1
+                           168 CALL                     1
+                           178 RAISE_VARARGS            1
                consts
                   None
-                  'https://'
                   '/api/miauth/'
                   '/check'
                   'ok'
                   'token'
                   'ログイン失敗'
                names      ('server', 'session_id', 'httpx', 'post', 'json', 'MisskeyMiAuthFailedException')
                varnames   ('self', 'url', 'response', 'response_json')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\create_session.py'
+               filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\__main__.py'
                name       'get_token'
                firstlineno 23
-               lnotab 0x020326012801280110011002
+               lnotab 0x020324012801280110011002
             None
+            ('misskey.io', 'MiPC App')
          names      ('__name__', '__module__', '__qualname__', '__init__', 'generate_url', 'get_token')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\create_session.py'
+         filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\__main__.py'
          name       'MiAuth'
          firstlineno 9
-         lnotab 0x0a02060606fe0808
+         lnotab 0x0a02080606fe0808
       'MiAuth'
    names      ('uuid', 'asyncio', 'json', 'httpx', 'MiPC.exceptions', 'MisskeyMiAuthFailedException', 'MiAuth')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\create_session.py'
+   filename   'C:\\Users\\hm74c\\Desktop\\MiPC\\MiPC\\MiAuth\\__main__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010801080208020c02
```

### Comparing `misskey_python-0.1.0/MiPC/MiAuth/create_session.py` & `misskey_python-1.0/MiPC/MiAuth/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 import httpx
 
 from MiPC.exceptions import MisskeyMiAuthFailedException
 
 class MiAuth:
 
-    def __init__(self, server, name):
+    def __init__(self, server="misskey.io", name="MiPC App"):
         self.server = server
         self.name = name
     
     def generate_url(
             self, 
             permission=["read:account", "write:account", "read:blocks", "write:blocks", "read:drive", "write:drive", "read:favorites", "write:favorites", "read:following", "write:following", "read:messaging", "write:messaging", "read:mutes", "write:mutes", "write:notes", "read:notifications", "write:notifications", "write:reactions", "write:votes", "read:pages", "write:pages", "write:page-likes", "read:page-likes", "write:gallery-likes", "read:gallery-likes"]
     ):
         self.session_id = uuid.uuid4()
-        url = f"https://{self.server}/miauth/{self.session_id}?name={self.name}&permission={','.join(permission)}"
+        url = f"{self.server}/miauth/{self.session_id}?name={self.name}&permission={','.join(permission)}"
         return url
     
     def get_token(
             self
     ):
-        url = f"https://{self.server}/api/miauth/{self.session_id}/check"
+        url = f"{self.server}/api/miauth/{self.session_id}/check"
         response = httpx.post(url)
         response_json = response.json()
         if response_json["ok"]:
             return response_json["token"]
         else:
             raise MisskeyMiAuthFailedException("ログイン失敗")
```

### Comparing `misskey_python-0.1.0/PKG-INFO` & `misskey_python-1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: misskey-python
-Version: 0.1.0
+Version: 1.0
 Summary: MiPC is the Misskey API framework for Python.
 License: MIT
 Author: sonyakun
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
```

