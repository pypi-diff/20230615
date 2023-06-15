# Comparing `tmp/repleno-0.0.5-py3-none-any.whl.zip` & `tmp/repleno-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 22634 bytes, number of entries: 11
+Zip file size: 22647 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      175 b- defN 23-Feb-28 13:50 repleno/__init__.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Feb-22 11:30 repleno/__main__.py
 -rw-rw-rw-  2.0 fat    31425 b- defN 23-May-13 20:31 repleno/factory.py
--rw-rw-rw-  2.0 fat    17458 b- defN 23-Jun-15 12:59 repleno/factory_str.py
+-rw-rw-rw-  2.0 fat    17458 b- defN 23-Jun-15 15:09 repleno/factory_str.py
 -rw-rw-rw-  2.0 fat    23779 b- defN 23-May-05 08:37 repleno/item.py
 -rw-rw-rw-  2.0 fat     2095 b- defN 23-Mar-05 12:10 repleno/order.py
 -rw-rw-rw-  2.0 fat    11183 b- defN 23-May-28 17:35 repleno/utils.py
--rw-rw-rw-  2.0 fat      608 b- defN 23-Jun-15 14:04 repleno-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 14:04 repleno-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-15 14:04 repleno-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      821 b- defN 23-Jun-15 14:04 repleno-0.0.5.dist-info/RECORD
-11 files, 87740 bytes uncompressed, 21270 bytes compressed:  75.8%
+-rw-rw-rw-  2.0 fat      640 b- defN 23-Jun-15 15:11 repleno-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 15:11 repleno-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-15 15:11 repleno-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      821 b- defN 23-Jun-15 15:11 repleno-0.0.6.dist-info/RECORD
+11 files, 87772 bytes uncompressed, 21283 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: repleno/order.py
 Comment: 
 
 Filename: repleno/utils.py
 Comment: 
 
-Filename: repleno-0.0.5.dist-info/METADATA
+Filename: repleno-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: repleno-0.0.5.dist-info/WHEEL
+Filename: repleno-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: repleno-0.0.5.dist-info/top_level.txt
+Filename: repleno-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: repleno-0.0.5.dist-info/RECORD
+Filename: repleno-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `repleno-0.0.5.dist-info/METADATA` & `repleno-0.0.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.5
+Version: 0.0.6
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pptree (>=3.1)
+Requires-Dist: tqdm (>=4.65.0)
 Provides-Extra: tests
 Requires-Dist: pytest ; extra == 'tests'
```

## Comparing `repleno-0.0.5.dist-info/RECORD` & `repleno-0.0.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 repleno/__init__.py,sha256=VjpZCtQMHgZ3t_egCL5K4a4p2pDu_D_KTVYLuFsGKOE,175
 repleno/__main__.py,sha256=1e9iXv9yqSGG5P0yHDK8c6boEQ_eDB8NkkEoBn-dqgc,96
 repleno/factory.py,sha256=HkTmV-5Atq8HSQJEeiFz-YbRWICvZFF-JDBOvBu-39I,31425
 repleno/factory_str.py,sha256=S3HXNr1VNH7GrcWqOpbBlxZFwwosFzNw-HxkaBuviiw,17458
 repleno/item.py,sha256=2OV1cVAOAM7GBerlXciw-l0iN0nLg2ehwLW7rkZ2UrE,23779
 repleno/order.py,sha256=u114s35ogN4BJrpBg73w-u6ZS7-aQjGbQqe6Q_bVuS0,2095
 repleno/utils.py,sha256=clUB2y67ZcSl2DZUJi2Gu22SpxUEczPzfYw6yvUevzo,11183
-repleno-0.0.5.dist-info/METADATA,sha256=opOVGU7fIts6nG3ZDufXG6qMA1wa4brruibp3zTykbU,608
-repleno-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-repleno-0.0.5.dist-info/top_level.txt,sha256=JoxJRcRjfYiR-s-R-SCXxJXSmuakgXJbQyfBpZ7EjeY,8
-repleno-0.0.5.dist-info/RECORD,,
+repleno-0.0.6.dist-info/METADATA,sha256=fbcPm4UZVl9l9aGJaPRPuzvW7oD8IyK-0pghgwzSO8k,640
+repleno-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+repleno-0.0.6.dist-info/top_level.txt,sha256=JoxJRcRjfYiR-s-R-SCXxJXSmuakgXJbQyfBpZ7EjeY,8
+repleno-0.0.6.dist-info/RECORD,,
```

