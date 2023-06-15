# Comparing `tmp/fauna_auth-0.0.3-py3-none-any.whl.zip` & `tmp/fauna_auth-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5310 bytes, number of entries: 7
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 fauna_auth/__init__.py
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 fauna_auth/accounts.py
--rw-r--r--  2.0 unx     2372 b- defN 80-Jan-01 00:00 fauna_auth/oauth.py
+Zip file size: 6011 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 fauna_auth/__init__.py
+-rw-r--r--  2.0 unx     2493 b- defN 80-Jan-01 00:00 fauna_auth/oauth.py
 -rw-r--r--  2.0 unx     3813 b- defN 80-Jan-01 00:00 fauna_auth/public_key.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.3.dist-info/METADATA
-?rw-r--r--  2.0 unx      525 b- defN 16-Jan-01 00:00 fauna_auth-0.0.3.dist-info/RECORD
-7 files, 7465 bytes uncompressed, 4382 bytes compressed:  41.3%
+-rw-r--r--  2.0 unx      812 b- defN 80-Jan-01 00:00 fauna_auth/testing.py
+-rw-r--r--  2.0 unx      351 b- defN 80-Jan-01 00:00 fauna_auth/types.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.4.dist-info/METADATA
+?rw-r--r--  2.0 unx      600 b- defN 16-Jan-01 00:00 fauna_auth-0.0.4.dist-info/RECORD
+8 files, 8807 bytes uncompressed, 4971 bytes compressed:  43.6%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: fauna_auth/__init__.py
 Comment: 
 
-Filename: fauna_auth/accounts.py
-Comment: 
-
 Filename: fauna_auth/oauth.py
 Comment: 
 
 Filename: fauna_auth/public_key.py
 Comment: 
 
-Filename: fauna_auth-0.0.3.dist-info/WHEEL
+Filename: fauna_auth/testing.py
+Comment: 
+
+Filename: fauna_auth/types.py
+Comment: 
+
+Filename: fauna_auth-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: fauna_auth-0.0.3.dist-info/METADATA
+Filename: fauna_auth-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: fauna_auth-0.0.3.dist-info/RECORD
+Filename: fauna_auth-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fauna_auth/__init__.py

```diff
@@ -1 +1,2 @@
-from .oauth import Client, get_fauna_user, get_fauna_client
+from .oauth import get_fauna_user, get_fauna_client
+from .types import Client, ClientType
```

## fauna_auth/oauth.py

```diff
@@ -1,41 +1,31 @@
 import json
+import logging
 import re
-from enum import Enum
 from typing import Optional
 
 from fastapi import Request, Depends, HTTPException, status
 from fastapi.security import OAuth2AuthorizationCodeBearer
 from jwcrypto import jwt, jwk
-from pydantic import BaseModel
 
 from .public_key import FAUNA_PUBLIC_KEY
+from .testing import mocked_auth
+from .types import Client, ClientType
 
 USER_ID_PATTERN = re.compile(r"^[a-z0-9]{48}$")
 
 public_key = jwk.JWK.from_pem(FAUNA_PUBLIC_KEY.encode())
 
 
-class ClientType(str, Enum):
-    User = "user"  # An active user session
-    Delegate = "delegate"  # a delegated user session
-    App = "app"  # an app session
-
-
-class Client(BaseModel):
-    client_type: ClientType
-    client_id: str
-    group: Optional[str] = None
-
-
 class FaunaAuthorizationScheme(OAuth2AuthorizationCodeBearer):
     async def __call__(self, request: Request) -> Optional[str]:
         fauna = request.cookies.get("fauna")
         if fauna is not None:
             return fauna
+
         return await super().__call__(request)
 
 
 fauna_auth_scheme = FaunaAuthorizationScheme(authorizationUrl="", tokenUrl="token")
 
 
 def _parse_token(token: str) -> Optional[Client]:
@@ -63,27 +53,41 @@
             group=group,
         )
 
     except jwt.JWException as e:
         return None
 
 
-def get_fauna_client(token: Optional[str] = Depends(fauna_auth_scheme)) -> Client:
+def _is_authorization_mocked(request: Request) -> bool:
+    return request.app.state._state.get("authorization_mocked", False)
+
+
+def _auth(token: str) -> Client:
+    client = _parse_token(token)
+    if client is None:
+        raise credentials_exception
+
+    return client
+
+
+def get_fauna_client(
+    request: Request, token: Optional[str] = Depends(fauna_auth_scheme)
+) -> Client:
     credentials_exception = HTTPException(
         status_code=status.HTTP_401_UNAUTHORIZED,
         detail="Could not validate credentials",
     )
 
     if token is None:
         raise credentials_exception
 
-    client = _parse_token(token)
-    if client is None:
-        raise credentials_exception
-
-    return client
+    if _is_authorization_mocked(request):
+        logging.warning("Using mocked authorization")
+        return mocked_auth(token)
+    else:
+        return _auth(token)
 
 
 def get_fauna_user(client: Client = Depends(get_fauna_client)) -> Client:
     if client.client_type != ClientType.User:
         raise HTTPException(status_code=401, detail="Invalid token")
     return client
```

## Comparing `fauna_auth-0.0.3.dist-info/METADATA` & `fauna_auth-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fauna-auth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Helper library
 Author: Edward FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `fauna_auth-0.0.3.dist-info/RECORD` & `fauna_auth-0.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-fauna_auth/__init__.py,sha256=8MKiYFv6Krd2XPUNwKZA2_6ZAhbTkSZsMShf4YsggKQ,60
-fauna_auth/accounts.py,sha256=vw98q6vcm3338yAgfagQO8nWHBKdB5_LJBlrep0TFkQ,47
-fauna_auth/oauth.py,sha256=BTGppqmwrUlwnci9M82T-hvjMQhg7X-kvxiVzr3aOfc,2372
+fauna_auth/__init__.py,sha256=NyW32VMOgYZS-Hb6ApRksPGvRy3WMkbxYTvoGvBdBhs,90
+fauna_auth/oauth.py,sha256=o_2nwwcieLv2JHQOS5HidnuB-wMcq9xMohBL64xQIiQ,2493
 fauna_auth/public_key.py,sha256=1aCrm0X7zWs3k22EW7_E9q9LZSMQIUVygPSAY1vXGi4,3813
-fauna_auth-0.0.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-fauna_auth-0.0.3.dist-info/METADATA,sha256=UZek3POMnCytbmFHmtr3-pqgKxFkWbGBtGUNWlqpIDs,560
-fauna_auth-0.0.3.dist-info/RECORD,,
+fauna_auth/testing.py,sha256=FxWg2Qy1QE-9IgaWPnLdSf4fVJjnoLKxAKcZ6ungosA,812
+fauna_auth/types.py,sha256=xBX95B-nmTYYAdEYzvE45LpxXpKXhCvWd3swi_uXEUM,351
+fauna_auth-0.0.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+fauna_auth-0.0.4.dist-info/METADATA,sha256=ovKkXgq7bFv9_99YOSMJGQuZ9B71Bm0zF67-ySZEua4,560
+fauna_auth-0.0.4.dist-info/RECORD,,
```

