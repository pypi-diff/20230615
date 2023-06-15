# Comparing `tmp/DigiCore-1.0.4.tar.gz` & `tmp/DigiCore-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.4.tar", last modified: Wed Jun 14 08:48:52 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.5.tar", last modified: Thu Jun 15 02:47:21 2023, max compression
```

## Comparing `DigiCore-1.0.4.tar` & `DigiCore-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.009566 DigiCore-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.007058 DigiCore-1.0.4/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      585 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 08:48:51.000000 DigiCore-1.0.4/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 08:48:18.000000 DigiCore-1.0.4/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-06-14 08:48:52.009566 DigiCore-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:48:52.009566 DigiCore-1.0.4/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.4/digiCore/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3673 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.4/digiCore/dsd_redis.py
--rw-rw-rw-   0        0        0     4161 2023-06-14 08:34:47.000000 DigiCore-1.0.4/digiCore/lingxing_api_scheduler.py
--rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.4/digiCore/model.py
--rw-rw-rw-   0        0        0     3738 2023-06-14 08:39:17.000000 DigiCore-1.0.4/digiCore/send_to_group.py
--rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.4/digiCore/status_code.py
--rw-rw-rw-   0        0        0     5351 2023-06-14 02:12:46.000000 DigiCore-1.0.4/digiCore/utils.py
--rw-rw-rw-   0        0        0       42 2023-06-14 08:48:52.009566 DigiCore-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3015 2023-06-14 08:48:13.000000 DigiCore-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.177338 DigiCore-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.137715 DigiCore-1.0.5/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      585 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 02:47:21.000000 DigiCore-1.0.5/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-06-15 02:47:21.177338 DigiCore-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.151296 DigiCore-1.0.5/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-05-20 06:50:26.000000 DigiCore-1.0.5/digiCore/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.5/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3712 2023-06-15 01:40:35.000000 DigiCore-1.0.5/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.5/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     3919 2023-05-20 07:33:42.000000 DigiCore-1.0.5/digiCore/dsd_redis.py
+-rw-rw-rw-   0        0        0     4161 2023-06-14 08:34:47.000000 DigiCore-1.0.5/digiCore/lingxing_api_scheduler.py
+-rw-rw-rw-   0        0        0     1015 2023-05-23 01:25:52.000000 DigiCore-1.0.5/digiCore/model.py
+-rw-rw-rw-   0        0        0     3738 2023-06-14 08:39:17.000000 DigiCore-1.0.5/digiCore/send_to_group.py
+-rw-rw-rw-   0        0        0      786 2023-05-20 03:41:55.000000 DigiCore-1.0.5/digiCore/status_code.py
+-rw-rw-rw-   0        0        0     5191 2023-06-15 01:53:18.000000 DigiCore-1.0.5/digiCore/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.155306 DigiCore-1.0.5/k3cloud_webapi_sdk/
+-rw-rw-rw-   0        0        0       29 2023-06-15 02:44:53.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.159304 DigiCore-1.0.5/k3cloud_webapi_sdk/const/
+-rw-rw-rw-   0        0        0       16 2023-06-15 02:45:04.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-06-15 02:44:55.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/const/const_define.py
+-rw-rw-rw-   0        0        0      500 2023-06-15 02:44:57.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/const/header_param.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.161306 DigiCore-1.0.5/k3cloud_webapi_sdk/core/
+-rw-rw-rw-   0        0        0       15 2023-06-15 02:45:10.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/core/__init__.py
+-rw-rw-rw-   0        0        0     8162 2023-06-15 02:45:01.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/core/webapi_client.py
+-rw-rw-rw-   0        0        0     7910 2023-06-15 02:45:04.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.168724 DigiCore-1.0.5/k3cloud_webapi_sdk/model/
+-rw-rw-rw-   0        0        0       16 2023-06-15 02:45:07.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-06-15 02:45:03.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/api_config.py
+-rw-rw-rw-   0        0        0     1109 2023-06-15 02:45:03.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/cookie.py
+-rw-rw-rw-   0        0        0      327 2023-06-15 02:44:55.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/cookie_store.py
+-rw-rw-rw-   0        0        0      411 2023-06-15 02:44:57.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/identity.py
+-rw-rw-rw-   0        0        0      197 2023-06-15 02:44:57.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/model/query_param.py
+-rw-rw-rw-   0        0        0     4385 2023-06-15 02:44:56.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:47:21.176211 DigiCore-1.0.5/k3cloud_webapi_sdk/util/
+-rw-rw-rw-   0        0        0       15 2023-06-15 02:44:53.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-15 02:44:58.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/util/base64_util.py
+-rw-rw-rw-   0        0        0     2671 2023-06-15 02:45:06.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/util/config_util.py
+-rw-rw-rw-   0        0        0     1654 2023-06-15 02:44:54.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/util/encode_util.py
+-rw-rw-rw-   0        0        0      420 2023-06-15 02:44:56.000000 DigiCore-1.0.5/k3cloud_webapi_sdk/util/hmac_util.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:47:21.177338 DigiCore-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-06-15 02:46:44.000000 DigiCore-1.0.5/setup.py
```

### Comparing `DigiCore-1.0.4/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.5/DigiCore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.4
+Version: 1.0.5
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.4/DigiCore.egg-info/requires.txt` & `DigiCore-1.0.5/DigiCore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/LICENSE` & `DigiCore-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/PKG-INFO` & `DigiCore-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.4
+Version: 1.0.5
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.4/README.md` & `DigiCore-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/__init__.py` & `DigiCore-1.0.5/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/dsd_kafka.py` & `DigiCore-1.0.5/digiCore/dsd_kafka.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/dsd_mongodb.py` & `DigiCore-1.0.5/digiCore/dsd_mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,11 +104,12 @@
         批量保存数据到数据库
         如果数据存在则根据 自定义主键进行数据更新
         :param data_list: 数据列表
         :param field_list: 主键列表
         :return: 
         """
         table_ob = self.load_table_ob()
+        self.create_index(field_list)
         bulk_write_list = get_bulk_write_list(data_list, field_list)
         if not bulk_write_list:
             return
         table_ob.bulk_write(bulk_write_list, ordered=False)
```

### Comparing `DigiCore-1.0.4/digiCore/dsd_mysql.py` & `DigiCore-1.0.5/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/dsd_redis.py` & `DigiCore-1.0.5/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/lingxing_api_scheduler.py` & `DigiCore-1.0.5/digiCore/lingxing_api_scheduler.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/model.py` & `DigiCore-1.0.5/digiCore/model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/send_to_group.py` & `DigiCore-1.0.5/digiCore/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/status_code.py` & `DigiCore-1.0.5/digiCore/status_code.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.4/digiCore/utils.py` & `DigiCore-1.0.5/digiCore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,19 +108,15 @@
                 logger.error(f"{file_type} 文件类型错误。参数为：excel、csv")
                 return
         except Exception as e:
             logger.error(f'error file:{e.__traceback__.tb_frame.f_globals["__file__"]}')
             logger.error(f'error line:{e.__traceback__.tb_lineno}')
             logger.error(f'error message:{e.args}')
             return
-            # 将nan转化为None
-        df.fillna('None', inplace=True)
-        # 获取整个工作表数据
-        data_all = df.values.tolist()
-        return data_all
+        return df
 
 
 class EncryptTool:
     """
     加密工具包
     """
```

### Comparing `DigiCore-1.0.4/setup.py` & `DigiCore-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 "tzdata==2023.3",
 "urllib3==2.0.2",
 "win32-setctime==1.1.0"
 ]
 
 setup(
     name="DigiCore",
-    version="1.0.4",
+    version="1.0.5",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

