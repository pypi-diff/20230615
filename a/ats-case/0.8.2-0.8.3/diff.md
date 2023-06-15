# Comparing `tmp/ats_case-0.8.2.tar.gz` & `tmp/ats_case-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.2.tar", last modified: Tue May 30 00:58:05 2023, max compression
+gzip compressed data, was "ats_case-0.8.3.tar", last modified: Wed Jun 14 05:53:26 2023, max compression
```

## Comparing `ats_case-0.8.2.tar` & `ats_case-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.594403 ats_case-0.8.2/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-30 00:58:05.592409 ats_case-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.189480 ats_case-0.8.2/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.2/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.406902 ats_case-0.8.2/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.2/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18767 2023-05-30 00:52:23.000000 ats_case-0.8.2/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11494 2023-05-30 00:50:05.000000 ats_case-0.8.2/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.2/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.2/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.486689 ats_case-0.8.2/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.2/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.2/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.2/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.548525 ats_case-0.8.2/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.2/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.2/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3771 2023-05-30 00:49:20.000000 ats_case-0.8.2/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.583432 ats_case-0.8.2/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.2/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.2/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.287221 ats_case-0.8.2/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 00:58:05.594403 ats_case-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-30 00:57:57.000000 ats_case-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.790440 ats_case-0.8.3/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-14 05:53:26.788432 ats_case-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.381917 ats_case-0.8.3/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.3/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.620241 ats_case-0.8.3/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.3/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18831 2023-06-14 05:51:39.000000 ats_case-0.8.3/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11494 2023-05-30 00:50:05.000000 ats_case-0.8.3/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.3/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.3/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.677798 ats_case-0.8.3/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.3/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.3/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.3/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.741151 ats_case-0.8.3/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.3/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.3/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3771 2023-05-30 00:49:20.000000 ats_case-0.8.3/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.781111 ats_case-0.8.3/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.3/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.3/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-14 05:53:26.492622 ats_case-0.8.3/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-14 05:53:25.000000 ats_case-0.8.3/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-14 05:53:26.000000 ats_case-0.8.3/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 05:53:25.000000 ats_case-0.8.3/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-14 05:53:25.000000 ats_case-0.8.3/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 05:53:25.000000 ats_case-0.8.3/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 05:53:26.791425 ats_case-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-14 05:52:52.000000 ats_case-0.8.3/setup.py
```

### Comparing `ats_case-0.8.2/PKG-INFO` & `ats_case-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.2
+Version: 0.8.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.2/README.md` & `ats_case-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/case/command.py` & `ats_case-0.8.3/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,17 @@
 
         self._frame = parse.get('frame')
         return self._frame
 
     def decode(self, context: Context, index=0):
         # 异常判断 - 客户端返回结果
         if self._frame is None or len(self._frame) <= 0:
-            raise ClientError(self._frame)
+            # raise ClientError(self._frame)
+            self._parse = '无响应帧'
+            return
 
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(
             func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.test_sn))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         # 异常判断 - 协议服务返回结果
```

### Comparing `ats_case-0.8.2/ats_case/case/context.py` & `ats_case-0.8.3/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/case/executor.py` & `ats_case-0.8.3/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/case/translator.py` & `ats_case-0.8.3/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/common/error.py` & `ats_case-0.8.3/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/manage/core.py` & `ats_case-0.8.3/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/manage/start.py` & `ats_case-0.8.3/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.3/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.3/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.2
+Version: 0.8.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.2/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.3/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.2/setup.py` & `ats_case-0.8.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.2",
+    version="0.8.3",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

