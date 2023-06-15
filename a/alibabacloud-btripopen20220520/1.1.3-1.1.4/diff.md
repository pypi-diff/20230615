# Comparing `tmp/alibabacloud_btripopen20220520-1.1.3.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.3.tar", last modified: Mon Jun 12 09:18:20 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.4.tar", last modified: Thu Jun 15 03:38:22 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.3.tar` & `alibabacloud_btripopen20220520-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     3469 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   525206 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1980376 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     3506 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525626 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1980866 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-06-15 03:38:22.000000 alibabacloud_btripopen20220520-1.1.4/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.4/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-12 Version: 1.1.3
+- Update.
+
 2023-06-09 Version: 1.1.2
 - Update.
 
 2023-06-06 Version: 1.0.74
 - Update.
 
 2023-06-05 Version: 1.0.73
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/LICENSE` & `alibabacloud_btripopen20220520-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.3/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/README-CN.md` & `alibabacloud_btripopen20220520-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.3/README.md` & `alibabacloud_btripopen20220520-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7923,14 +7923,16 @@
             body['tel'] = request.tel
         if not UtilClient.is_unset(request.third_part_id):
             body['third_part_id'] = request.third_part_id
         if not UtilClient.is_unset(request.title):
             body['title'] = request.title
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
+        if not UtilClient.is_unset(request.unit_type):
+            body['unit_type'] = request.unit_type
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_so_corp_token):
             real_headers['x-acs-btrip-so-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_so_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -7972,14 +7974,16 @@
             body['tel'] = request.tel
         if not UtilClient.is_unset(request.third_part_id):
             body['third_part_id'] = request.third_part_id
         if not UtilClient.is_unset(request.title):
             body['title'] = request.title
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
+        if not UtilClient.is_unset(request.unit_type):
+            body['unit_type'] = request.unit_type
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_so_corp_token):
             real_headers['x-acs-btrip-so-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_so_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -8123,14 +8127,16 @@
             body['tel'] = request.tel
         if not UtilClient.is_unset(request.third_part_id):
             body['third_part_id'] = request.third_part_id
         if not UtilClient.is_unset(request.title):
             body['title'] = request.title
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
+        if not UtilClient.is_unset(request.unit_type):
+            body['unit_type'] = request.unit_type
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_so_corp_token):
             real_headers['x-acs-btrip-so-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_so_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -8172,14 +8178,16 @@
             body['tel'] = request.tel
         if not UtilClient.is_unset(request.third_part_id):
             body['third_part_id'] = request.third_part_id
         if not UtilClient.is_unset(request.title):
             body['title'] = request.title
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
+        if not UtilClient.is_unset(request.unit_type):
+            body['unit_type'] = request.unit_type
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_so_corp_token):
             real_headers['x-acs-btrip-so-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_so_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -41320,23 +41320,25 @@
         bank_name: str = None,
         bank_no: str = None,
         tax_no: str = None,
         tel: str = None,
         third_part_id: str = None,
         title: str = None,
         type: int = None,
+        unit_type: int = None,
     ):
         self.address = address
         self.bank_name = bank_name
         self.bank_no = bank_no
         self.tax_no = tax_no
         self.tel = tel
         self.third_part_id = third_part_id
         self.title = title
         self.type = type
+        self.unit_type = unit_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -41355,14 +41357,16 @@
             result['tel'] = self.tel
         if self.third_part_id is not None:
             result['third_part_id'] = self.third_part_id
         if self.title is not None:
             result['title'] = self.title
         if self.type is not None:
             result['type'] = self.type
+        if self.unit_type is not None:
+            result['unit_type'] = self.unit_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('address') is not None:
             self.address = m.get('address')
         if m.get('bank_name') is not None:
@@ -41375,14 +41379,16 @@
             self.tel = m.get('tel')
         if m.get('third_part_id') is not None:
             self.third_part_id = m.get('third_part_id')
         if m.get('title') is not None:
             self.title = m.get('title')
         if m.get('type') is not None:
             self.type = m.get('type')
+        if m.get('unit_type') is not None:
+            self.unit_type = m.get('unit_type')
         return self
 
 
 class InvoiceAddResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -41674,23 +41680,25 @@
         bank_name: str = None,
         bank_no: str = None,
         tax_no: str = None,
         tel: str = None,
         third_part_id: str = None,
         title: str = None,
         type: int = None,
+        unit_type: int = None,
     ):
         self.address = address
         self.bank_name = bank_name
         self.bank_no = bank_no
         self.tax_no = tax_no
         self.tel = tel
         self.third_part_id = third_part_id
         self.title = title
         self.type = type
+        self.unit_type = unit_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -41709,14 +41717,16 @@
             result['tel'] = self.tel
         if self.third_part_id is not None:
             result['third_part_id'] = self.third_part_id
         if self.title is not None:
             result['title'] = self.title
         if self.type is not None:
             result['type'] = self.type
+        if self.unit_type is not None:
+            result['unit_type'] = self.unit_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('address') is not None:
             self.address = m.get('address')
         if m.get('bank_name') is not None:
@@ -41729,14 +41739,16 @@
             self.tel = m.get('tel')
         if m.get('third_part_id') is not None:
             self.third_part_id = m.get('third_part_id')
         if m.get('title') is not None:
             self.title = m.get('title')
         if m.get('type') is not None:
             self.type = m.get('type')
+        if m.get('unit_type') is not None:
+            self.unit_type = m.get('unit_type')
         return self
 
 
 class InvoiceModifyResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.4/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.3/setup.py` & `alibabacloud_btripopen20220520-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 12/06/2023
+Created on 15/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
```

