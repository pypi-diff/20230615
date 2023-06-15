# Comparing `tmp/addereq-1.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/addereq-1.0.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 207237 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-14 08:05 addereq/__init__.py
--rw-rw-rw-  2.0 fat    47616 b- defN 23-Jun-14 08:06 addereq/cleaning.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   123904 b- defN 23-Jun-14 08:06 addereq/fetching.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   111616 b- defN 23-Jun-14 08:06 addereq/fetching_mysql.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   151552 b- defN 23-Jun-14 08:06 addereq/plotting.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-14 08:06 addereq-1.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3175 b- defN 23-Jun-14 08:06 addereq-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 08:06 addereq-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 08:05 addereq-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      841 b- defN 23-Jun-14 08:06 addereq-1.0.4.dist-info/RECORD
-10 files, 474635 bytes uncompressed, 205807 bytes compressed:  56.6%
+Zip file size: 207336 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-15 02:50 addereq/__init__.py
+-rw-rw-rw-  2.0 fat    47616 b- defN 23-Jun-15 02:54 addereq/cleaning.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   123904 b- defN 23-Jun-15 02:54 addereq/fetching.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   111616 b- defN 23-Jun-15 02:54 addereq/fetching_mysql.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   151552 b- defN 23-Jun-15 02:54 addereq/plotting.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-15 02:54 addereq-1.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-Jun-15 02:54 addereq-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-15 02:54 addereq-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-15 02:51 addereq-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      841 b- defN 23-Jun-15 02:54 addereq-1.0.5.dist-info/RECORD
+10 files, 474876 bytes uncompressed, 205906 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: addereq/fetching_mysql.cp39-win_amd64.pyd
 Comment: 
 
 Filename: addereq/plotting.cp39-win_amd64.pyd
 Comment: 
 
-Filename: addereq-1.0.4.dist-info/LICENSE
+Filename: addereq-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: addereq-1.0.4.dist-info/METADATA
+Filename: addereq-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: addereq-1.0.4.dist-info/WHEEL
+Filename: addereq-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: addereq-1.0.4.dist-info/top_level.txt
+Filename: addereq-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: addereq-1.0.4.dist-info/RECORD
+Filename: addereq-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `addereq-1.0.4.dist-info/LICENSE` & `addereq-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `addereq-1.0.4.dist-info/METADATA` & `addereq-1.0.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 Metadata-Version: 2.1
 Name: addereq
-Version: 1.0.4
+Version: 1.0.5
 Summary: 地震前兆数据自动处理框架
 Author-email: WANG Qinglin <chd_wql@qq.com>
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymysql
+Requires-Dist: cx-Oracle
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: openpyxl
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: SQLAlchemy (==1.4.48)
 
 # addereq（地震前兆数据自动分析框架）
 
 地震前兆分析手段长期积弱，数据源是一个很大的原因，没有文件存储标准，数据库接入门槛也比较高。
 
 为了突破数据源的壁垒，助力地震前兆科研发展，开发上线了该框架。
```

