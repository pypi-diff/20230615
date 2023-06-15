# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.3.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.3.tar", last modified: Mon Jun 12 09:17:46 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.4.tar", last modified: Thu Jun 15 03:38:12 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.3.tar` & `alibabacloud_btripopen20220520_py2-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     3343 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223194 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2002413 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223404 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2002899 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-15 03:38:12.000000 alibabacloud_btripopen20220520_py2-1.1.4/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.4/ChangeLog.md`

 * *Files 0% similar despite different names*

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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/README.md` & `alibabacloud_btripopen20220520_py2-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3413,14 +3413,16 @@
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
@@ -3497,14 +3499,16 @@
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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -36250,23 +36250,24 @@
         if m.get('x-acs-btrip-so-corp-token') is not None:
             self.x_acs_btrip_so_corp_token = m.get('x-acs-btrip-so-corp-token')
         return self
 
 
 class InvoiceAddRequest(TeaModel):
     def __init__(self, address=None, bank_name=None, bank_no=None, tax_no=None, tel=None, third_part_id=None,
-                 title=None, type=None):
+                 title=None, type=None, unit_type=None):
         self.address = address  # type: str
         self.bank_name = bank_name  # type: str
         self.bank_no = bank_no  # type: str
         self.tax_no = tax_no  # type: str
         self.tel = tel  # type: str
         self.third_part_id = third_part_id  # type: str
         self.title = title  # type: str
         self.type = type  # type: int
+        self.unit_type = unit_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InvoiceAddRequest, self).to_map()
         if _map is not None:
@@ -36285,14 +36286,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('address') is not None:
             self.address = m.get('address')
         if m.get('bank_name') is not None:
@@ -36305,14 +36308,16 @@
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
     def __init__(self, code=None, message=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.message = message  # type: str
@@ -36560,23 +36565,24 @@
         if m.get('x-acs-btrip-so-corp-token') is not None:
             self.x_acs_btrip_so_corp_token = m.get('x-acs-btrip-so-corp-token')
         return self
 
 
 class InvoiceModifyRequest(TeaModel):
     def __init__(self, address=None, bank_name=None, bank_no=None, tax_no=None, tel=None, third_part_id=None,
-                 title=None, type=None):
+                 title=None, type=None, unit_type=None):
         self.address = address  # type: str
         self.bank_name = bank_name  # type: str
         self.bank_no = bank_no  # type: str
         self.tax_no = tax_no  # type: str
         self.tel = tel  # type: str
         self.third_part_id = third_part_id  # type: str
         self.title = title  # type: str
         self.type = type  # type: int
+        self.unit_type = unit_type  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InvoiceModifyRequest, self).to_map()
         if _map is not None:
@@ -36595,14 +36601,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('address') is not None:
             self.address = m.get('address')
         if m.get('bank_name') is not None:
@@ -36615,14 +36623,16 @@
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
     def __init__(self, code=None, message=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.message = message  # type: str
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.4/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.3/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 12/06/2023
+Created on 15/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
```

