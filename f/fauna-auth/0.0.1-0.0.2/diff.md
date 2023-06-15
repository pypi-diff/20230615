# Comparing `tmp/fauna_auth-0.0.1-py3-none-any.whl.zip` & `tmp/fauna_auth-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5195 bytes, number of entries: 7
+Zip file size: 5308 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 fauna_auth/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 fauna_auth/accounts.py
--rw-r--r--  2.0 unx     2090 b- defN 80-Jan-01 00:00 fauna_auth/oauth.py
--rw-r--r--  2.0 unx     3812 b- defN 80-Jan-01 00:00 fauna_auth/public_key.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      525 b- defN 16-Jan-01 00:00 fauna_auth-0.0.1.dist-info/RECORD
-7 files, 7182 bytes uncompressed, 4267 bytes compressed:  40.6%
+-rw-r--r--  2.0 unx     2372 b- defN 80-Jan-01 00:00 fauna_auth/oauth.py
+-rw-r--r--  2.0 unx     3813 b- defN 80-Jan-01 00:00 fauna_auth/public_key.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx      525 b- defN 16-Jan-01 00:00 fauna_auth-0.0.2.dist-info/RECORD
+7 files, 7465 bytes uncompressed, 4380 bytes compressed:  41.3%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: fauna_auth/oauth.py
 Comment: 
 
 Filename: fauna_auth/public_key.py
 Comment: 
 
-Filename: fauna_auth-0.0.1.dist-info/WHEEL
+Filename: fauna_auth-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: fauna_auth-0.0.1.dist-info/METADATA
+Filename: fauna_auth-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: fauna_auth-0.0.1.dist-info/RECORD
+Filename: fauna_auth-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fauna_auth/oauth.py

```diff
@@ -1,18 +1,21 @@
 import json
+import re
 from enum import Enum
 from typing import Optional
 
 from fastapi import Request, Depends, HTTPException, status
 from fastapi.security import OAuth2AuthorizationCodeBearer
 from jwcrypto import jwt, jwk
 from pydantic import BaseModel
 
 from .public_key import FAUNA_PUBLIC_KEY
 
+USER_ID_PATTERN = re.compile(r"^[a-z0-9]{48}$")
+
 public_key = jwk.JWK.from_pem(FAUNA_PUBLIC_KEY.encode())
 
 
 class ClientType(str, Enum):
     User = "user"  # An active user session
     Delegate = "delegate"  # a delegated user session
     App = "app"  # an app session
@@ -31,48 +34,56 @@
             return fauna
         return await super().__call__(request)
 
 
 fauna_auth_scheme = FaunaAuthorizationScheme(authorizationUrl="", tokenUrl="token")
 
 
-def parse_user_token(token: str) -> Optional[str]:
+def _parse_token(token: str) -> Optional[Client]:
     try:
         jwt_token = jwt.JWT(
             key=public_key,
             jwt=token,
             check_claims={"exp": None, "iss": "fetch.ai", "sub": None, "iat": None},
         )
 
+        # parse the claims
         claims = json.loads(jwt_token.claims)
-        print('CLAIMS', claims)
 
-        return claims["sub"]
+        # extract the elements
+        subject = str(claims["sub"])
+        group = claims.get("grp")
+
+        # ensure that we match the user id pattern
+        if USER_ID_PATTERN.match(subject) is None:
+            return None
+
+        return Client(
+            client_type=ClientType.User,
+            client_id=subject,
+            group=group,
+        )
 
     except jwt.JWException as e:
         return None
 
 
 def get_fauna_client(token: Optional[str] = Depends(fauna_auth_scheme)) -> Client:
     credentials_exception = HTTPException(
         status_code=status.HTTP_401_UNAUTHORIZED,
         detail="Could not validate credentials",
     )
 
     if token is None:
         raise credentials_exception
 
-    user_id = parse_user_token(token)
-    if user_id is None:
+    client = _parse_token(token)
+    if client is None:
         raise credentials_exception
 
-    return Client(
-        client_type=ClientType.User,
-        client_id=str(user_id),
-        group=None,
-    )
+    return client
 
 
 def get_fauna_user(client: Client = Depends(get_fauna_client)) -> Client:
     if client.client_type != ClientType.User:
         raise HTTPException(status_code=401, detail="Invalid token")
     return client
```

## fauna_auth/public_key.py

 * *Ordering differences only*

```diff
@@ -57,8 +57,8 @@
 QenA+Kn12bURjOeI/zdbrvH0Fd0CpfsdmtxMkawkwNBdT6LuiX2U0aHv05aAkl1R
 gDC4RpsmauTp+EnGBNUBufNIkY1awwQckgZqTHD7jM89qXZIuH3mlVpghBgJxJ0O
 UquNrYU9ps3311BGnru1XAAVbEUUNvMYtuxFf6b4SRpuMbdzuKrxH3/3sh/aob9Y
 s7NfPQr+ii8R+Pgh+8XMAKuWm9y//Hg2X45PU0BsxWMBJMCsqf+AuAcidfJrqoV0
 fWh5NAV5o3O30mMRIKBGuBaIvodlbhxOKYHo1wdtvhLSrmswDdVoWgO9uJt0j6/b
 FqMBAQ1y
 -----END CERTIFICATE-----
-"""
+"""
```

## Comparing `fauna_auth-0.0.1.dist-info/METADATA` & `fauna_auth-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fauna-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: Helper library
 Author: Edward FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

