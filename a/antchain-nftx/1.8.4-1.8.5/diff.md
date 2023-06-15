# Comparing `tmp/antchain_nftx-1.8.4.tar.gz` & `tmp/antchain_nftx-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.8.4.tar", last modified: Thu Jun 15 03:30:29 2023, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.5.tar", last modified: Thu Jun 15 11:09:16 2023, max compression
```

## Comparing `antchain_nftx-1.8.4.tar` & `antchain_nftx-1.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52197 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)   107671 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 03:30:29.000000 antchain_nftx-1.8.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-15 03:30:28.000000 antchain_nftx-1.8.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 11:09:15.000000 antchain_nftx-1.8.5/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52197 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)   108031 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 11:09:16.000000 antchain_nftx-1.8.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-15 11:09:13.000000 antchain_nftx-1.8.5/setup.py
```

### Comparing `antchain_nftx-1.8.4/LICENSE` & `antchain_nftx-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.4/PKG-INFO` & `antchain_nftx-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.8.4
+Version: 1.8.5
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.4/README-CN.md` & `antchain_nftx-1.8.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.4/README.md` & `antchain_nftx-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.4/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.5/antchain_nftx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.8.4
+Version: 1.8.5
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.4/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.5/antchain_sdk_nftx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.4',
+                    'sdk_version': '1.8.5',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.4',
+                    'sdk_version': '1.8.5',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_nftx-1.8.4/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.5/antchain_sdk_nftx/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2555,31 +2555,35 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         access_token: str = None,
         type: str = None,
         resource_id: str = None,
         nft_id: str = None,
+        need_hd_img: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # access_token
         self.access_token = access_token
         # 素材的类型（AIGC/NFT）
         self.type = type
         # 资源ID
         self.resource_id = resource_id
         # type为NFT必填
         self.nft_id = nft_id
+        # 是否需要高清图
+        self.need_hd_img = need_hd_img
 
     def validate(self):
         self.validate_required(self.access_token, 'access_token')
         self.validate_required(self.type, 'type')
         self.validate_required(self.resource_id, 'resource_id')
+        self.validate_required(self.need_hd_img, 'need_hd_img')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2591,14 +2595,16 @@
             result['access_token'] = self.access_token
         if self.type is not None:
             result['type'] = self.type
         if self.resource_id is not None:
             result['resource_id'] = self.resource_id
         if self.nft_id is not None:
             result['nft_id'] = self.nft_id
+        if self.need_hd_img is not None:
+            result['need_hd_img'] = self.need_hd_img
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -2607,14 +2613,16 @@
             self.access_token = m.get('access_token')
         if m.get('type') is not None:
             self.type = m.get('type')
         if m.get('resource_id') is not None:
             self.resource_id = m.get('resource_id')
         if m.get('nft_id') is not None:
             self.nft_id = m.get('nft_id')
+        if m.get('need_hd_img') is not None:
+            self.need_hd_img = m.get('need_hd_img')
         return self
 
 
 class QueryResourceImageResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_nftx-1.8.4/setup.py` & `antchain_nftx-1.8.5/setup.py`

 * *Files identical despite different names*

