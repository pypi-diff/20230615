# Comparing `tmp/laningapi-0.0.6.tar.gz` & `tmp/laningapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laningapi-0.0.6.tar", last modified: Wed May 24 08:30:59 2023, max compression
+gzip compressed data, was "laningapi-0.0.7.tar", last modified: Thu Jun 15 02:52:23 2023, max compression
```

## Comparing `laningapi-0.0.6.tar` & `laningapi-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769670 laningapi-0.0.6/
--rw-r--r--   0 changwei   (501) staff       (20)       94 2023-04-04 01:34:16.000000 laningapi-0.0.6/MANIFEST.in
--rw-r--r--   0 changwei   (501) staff       (20)      181 2023-05-24 08:30:59.769565 laningapi-0.0.6/PKG-INFO
--rw-r--r--   0 changwei   (501) staff       (20)      395 2022-12-08 06:35:53.000000 laningapi-0.0.6/README.md
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769364 laningapi-0.0.6/laningapi/
--rw-r--r--   0 changwei   (501) staff       (20)      174 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/__init__.py
--rw-r--r--   0 changwei   (501) staff       (20)     1025 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/_mock.py
--rw-r--r--   0 changwei   (501) staff       (20)     3144 2023-05-24 08:27:18.000000 laningapi-0.0.6/laningapi/base.py
--rw-r--r--   0 changwei   (501) staff       (20)     1171 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/dictionary.py
--rw-r--r--   0 changwei   (501) staff       (20)     1061 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/oplog.py
--rw-r--r--   0 changwei   (501) staff       (20)     1324 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/series.py
--rw-r--r--   0 changwei   (501) staff       (20)     3802 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/target.py
--rw-r--r--   0 changwei   (501) staff       (20)        0 2022-12-08 06:35:50.000000 laningapi-0.0.6/laningapi/task.py
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769443 laningapi-0.0.6/laningapi.egg-info/
--rwx------   0 changwei   (501) staff       (20)      190 2023-05-24 08:30:59.000000 laningapi-0.0.6/laningapi.egg-info/SOURCES.txt
--rw-r--r--   0 changwei   (501) staff       (20)       38 2023-05-24 08:30:59.769725 laningapi-0.0.6/setup.cfg
--rw-r--r--   0 changwei   (501) staff       (20)      724 2023-05-24 08:30:40.000000 laningapi-0.0.6/setup.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-06-15 02:52:23.305652 laningapi-0.0.7/
+-rw-r--r--   0 changwei   (501) staff       (20)       94 2023-04-04 01:34:16.000000 laningapi-0.0.7/MANIFEST.in
+-rw-r--r--   0 changwei   (501) staff       (20)      181 2023-06-15 02:52:23.305540 laningapi-0.0.7/PKG-INFO
+-rw-r--r--   0 changwei   (501) staff       (20)      395 2022-12-08 06:35:53.000000 laningapi-0.0.7/README.md
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-06-15 02:52:23.305333 laningapi-0.0.7/laningapi/
+-rw-r--r--   0 changwei   (501) staff       (20)      174 2023-04-04 01:34:16.000000 laningapi-0.0.7/laningapi/__init__.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1308 2023-06-15 02:51:54.000000 laningapi-0.0.7/laningapi/_mock.py
+-rw-r--r--   0 changwei   (501) staff       (20)     3146 2023-06-15 02:51:54.000000 laningapi-0.0.7/laningapi/base.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1171 2023-04-04 01:34:16.000000 laningapi-0.0.7/laningapi/dictionary.py
+-rw-r--r--   0 changwei   (501) staff       (20)      362 2023-06-15 02:51:54.000000 laningapi-0.0.7/laningapi/ner.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1061 2023-04-04 01:34:16.000000 laningapi-0.0.7/laningapi/oplog.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1324 2023-04-04 01:34:16.000000 laningapi-0.0.7/laningapi/series.py
+-rw-r--r--   0 changwei   (501) staff       (20)     4012 2023-06-15 02:51:54.000000 laningapi-0.0.7/laningapi/target.py
+-rw-r--r--   0 changwei   (501) staff       (20)        0 2022-12-08 06:35:50.000000 laningapi-0.0.7/laningapi/task.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-06-15 02:52:23.305414 laningapi-0.0.7/laningapi.egg-info/
+-rwx------   0 changwei   (501) staff       (20)      207 2023-06-15 02:52:23.000000 laningapi-0.0.7/laningapi.egg-info/SOURCES.txt
+-rw-r--r--   0 changwei   (501) staff       (20)       38 2023-06-15 02:52:23.305686 laningapi-0.0.7/setup.cfg
+-rw-r--r--   0 changwei   (501) staff       (20)      724 2023-06-15 02:52:18.000000 laningapi-0.0.7/setup.py
```

### Comparing `laningapi-0.0.6/laningapi/_mock.py` & `laningapi-0.0.7/laningapi/_mock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import functools
 
 mocking = {}
 
 
 class Mock:
+    """NOTE:
+    Example:
+
+    dict_api = Dictionary(baseurl="http://mock/", transport=te)
+
+    with Mock("Dictionary", "get_dict_info") as m:
+        m.register("my mocking")
+        data = dict_api.get_dict_info(name="dict_name")
+        print(data)  # Output: my mocking
+    """
+
     def __init__(self, module, method):
         self.module = module.lower()
         self.method = method.lower()
 
     def __enter__(self):
         mocking[(self.module, self.method)] = None
         return self
```

### Comparing `laningapi-0.0.6/laningapi/base.py` & `laningapi-0.0.7/laningapi/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class TransportInternal(Transport):
     def init(self):
         pass
 
     def post(self, url, *, json) -> Response:
         headers = {
             "x-forwarded-for-zl": "127.0.0.1",
-            "x-current-user-id": 1,
+            "x-current-user-id": "1",
             "x-current-username": "laningapi"
         }
         return requests.post(url, json=json, headers=headers)
 
 
 class TransportExternal(Transport):
     def __init__(self):
```

### Comparing `laningapi-0.0.6/laningapi/dictionary.py` & `laningapi-0.0.7/laningapi/dictionary.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.6/laningapi/oplog.py` & `laningapi-0.0.7/laningapi/oplog.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.6/laningapi/series.py` & `laningapi-0.0.7/laningapi/series.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.6/laningapi/target.py` & `laningapi-0.0.7/laningapi/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .base import Base
 from ._mock import MockType
+from .base import Base
+
 
 # class TargetSearch(BaseModel):
 #     keyword: str = ""
 #     person_name: str = ""
 #     person_level_ids: list = []
 #     person_type_ids: list = []
 #     sack_start_time: str = ""
@@ -100,7 +101,14 @@
         return result["success"]
 
     def remove_include(self, *, person_feature: list) -> list:
         data = person_feature
         # self.baseurl = "http://targetapi-feature-prod:8000"
         result = self._do_post('feature/include/remove', data)
         return result["success"]
+
+    def base64_feature(self, *, img_base64: str):
+        data = {
+            "img_base64": img_base64
+        }
+        result = self._do_post('picture/base64_feature', data)
+        return result["faces"]
```

### Comparing `laningapi-0.0.6/setup.py` & `laningapi-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- encoding: UTF-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name="laningapi",  # 包名
     author="laning",
     author_email="nkchwfree@163.com",
-    version="0.0.6",  # 版本信息
+    version="0.0.7",  # 版本信息
     packages=["laningapi"],
     include_package_data=True,  # 自动打包文件夹内所有数据
     zip_safe=True,  # 设定项目包为安全，不用每次都检测其安全性
     install_requires=[  # 安装依赖的其他包（测试数据）
     ],
 
     # 设置程序的入口为path
```

