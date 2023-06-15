# Comparing `tmp/x21e8-0.9.0.tar.gz` & `tmp/x21e8-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.9.0.tar", max compression
+gzip compressed data, was "x21e8-0.9.1.tar", max compression
```

## Comparing `x21e8-0.9.0.tar` & `x21e8-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     5223 2023-06-14 08:34:56.845137 x21e8-0.9.0/README.md
--rw-r--r--   0        0        0      823 2023-06-14 08:34:56.849137 x21e8-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6153 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2391 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/application/token.py
--rw-r--r--   0        0        0      837 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/config.py
--rw-r--r--   0        0        0     1096 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/data.py
--rw-r--r--   0        0        0     4145 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/utils.py
--rw-r--r--   0        0        0      997 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1123 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/eddsa_auth.py
--rw-r--r--   0        0        0     1035 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     2354 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4862 2023-06-14 08:34:56.853137 x21e8-0.9.0/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 x21e8-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     5223 2023-06-15 11:19:39.372072 x21e8-0.9.1/README.md
+-rw-r--r--   0        0        0      823 2023-06-15 11:19:39.376072 x21e8-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.376072 x21e8-0.9.1/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.376072 x21e8-0.9.1/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6153 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2391 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/application/token.py
+-rw-r--r--   0        0        0      837 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1096 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/data.py
+-rw-r--r--   0        0        0     4145 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      997 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1123 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/utils/eddsa_auth.py
+-rw-r--r--   0        0        0     1035 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2390 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4862 2023-06-15 11:19:39.380072 x21e8-0.9.1/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6322 1970-01-01 00:00:00.000000 x21e8-0.9.1/PKG-INFO
```

### Comparing `x21e8-0.9.0/README.md` & `x21e8-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/pyproject.toml` & `x21e8-0.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.9.0"
+version = "0.9.1"
 description = "x21e8 service to manage RDDL network identities on TrustAnchors and workflows."
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*"
```

### Comparing `x21e8-0.9.0/x21e8/application/liquid.py` & `x21e8-0.9.1/x21e8/application/liquid.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/application/planetmint.py` & `x21e8-0.9.1/x21e8/application/planetmint.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/application/token.py` & `x21e8-0.9.1/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/config.py` & `x21e8-0.9.1/x21e8/config.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/main.py` & `x21e8-0.9.1/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/network/liquid/__init__.py` & `x21e8-0.9.1/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/network/liquid/util.py` & `x21e8-0.9.1/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/assets.py` & `x21e8-0.9.1/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/data.py` & `x21e8-0.9.1/x21e8/routers/data.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/machine.py` & `x21e8-0.9.1/x21e8/routers/machine.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/seed.py` & `x21e8-0.9.1/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/utils.py` & `x21e8-0.9.1/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/routers/wallet.py` & `x21e8-0.9.1/x21e8/routers/wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/utils/eddsa_auth.py` & `x21e8-0.9.1/x21e8/utils/eddsa_auth.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/utils/encryption.py` & `x21e8-0.9.1/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/utils/storage.py` & `x21e8-0.9.1/x21e8/utils/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 def get_ipfs_link(cid: str):
     return "https://" + cid + ".ipfs.w3s.link"
 
 
 def register_cid_url(cid: str, url: str):
     http = urllib3.PoolManager()
     token = get_jwt_token()
-    cid_resp = http.request(
-        "POST",
-        CID_RESOLVER + "/entry?cid=" + cid + "&url=" + url,
-        headers={"Content-Type": "application/json", "Authorization": f"Bearer {token}"},
-    )
+    headers = {"Content-Type": "application/json", "accept": "application/json", "Authorization": f"Bearer {token}"}
+    url = CID_RESOLVER + "/entry/?cid=" + cid + "&url=" + url
+    cid_resp = http.request("POST", url, headers=headers)
     return cid_resp
 
 
 def decryption_layer(data, decrypt_data: bool = False):
     if decrypt_data:
         print(f"encrypted : {data}")
         decrypted_blob = decrypt_2_bytes(data)
```

### Comparing `x21e8-0.9.0/x21e8/wallet/base_wallet.py` & `x21e8-0.9.1/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.9.1/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.9.1/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/wallet/seed.py` & `x21e8-0.9.1/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/x21e8/wallet/sw_wallet.py` & `x21e8-0.9.1/x21e8/wallet/sw_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.9.0/PKG-INFO` & `x21e8-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.9.0
+Version: 0.9.1
 Summary: x21e8 service to manage RDDL network identities on TrustAnchors and workflows.
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

