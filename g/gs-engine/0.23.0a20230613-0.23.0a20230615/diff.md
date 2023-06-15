# Comparing `tmp/gs_engine-0.23.0a20230613-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.23.0a20230615-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11893 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 23-Jun-13 19:02 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-13 19:02 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 23-Jun-13 19:02 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-13 19:02 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-13 19:02 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    21680 b- defN 23-Jun-13 20:50 gs_engine-0.23.0a20230613.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 20:50 gs_engine-0.23.0a20230613.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-13 20:50 gs_engine-0.23.0a20230613.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 23-Jun-13 20:50 gs_engine-0.23.0a20230613.dist-info/RECORD
-9 files, 26013 bytes uncompressed, 10431 bytes compressed:  59.9%
+Zip file size: 11892 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Jun-15 02:15 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      505 b- defN 23-Jun-15 02:15 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jun-15 02:15 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-15 02:15 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-15 02:15 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jun-15 04:04 gs_engine-0.23.0a20230615.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 04:04 gs_engine-0.23.0a20230615.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-15 04:04 gs_engine-0.23.0a20230615.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jun-15 04:04 gs_engine-0.23.0a20230615.dist-info/RECORD
+9 files, 26014 bytes uncompressed, 10430 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.23.0a20230613.dist-info/METADATA
+Filename: gs_engine-0.23.0a20230615.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.23.0a20230613.dist-info/WHEEL
+Filename: gs_engine-0.23.0a20230615.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.23.0a20230613.dist-info/top_level.txt
+Filename: gs_engine-0.23.0a20230615.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.23.0a20230613.dist-info/RECORD
+Filename: gs_engine-0.23.0a20230615.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## graphscope.runtime/conf/frontend.vineyard.properties

 * *Ordering differences only*

```diff
@@ -14,8 +14,8 @@
 graph.schema = GRAPH_SCHEMA
 
 ## Frontend Config
 frontend.service.port = FRONTEND_SERVICE_PORT
 
 # disable the authentication if username or password is not set
 #auth.username = default
-#auth.password = default
+#auth.password = default
```

## Comparing `gs_engine-0.23.0a20230613.dist-info/METADATA` & `gs_engine-0.23.0a20230615.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.23.0a20230613
+Version: 0.23.0a20230615
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `gs_engine-0.23.0a20230613.dist-info/RECORD` & `gs_engine-0.23.0a20230615.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
-graphscope.runtime/conf/frontend.vineyard.properties,sha256=eIDnFSXj53FD5KWKOg_keg6pA-OrNUg9BsQP-gxslHU,504
+graphscope.runtime/conf/frontend.vineyard.properties,sha256=1mILl2P2oiLAIzc4R23zLzwT7fod-y4kj0Pa2ne3bl0,505
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.23.0a20230613.dist-info/METADATA,sha256=0qxx_B5AqTCtFUYAcDcm92iCDa8m-xpLc0TaxsQBolE,21680
-gs_engine-0.23.0a20230613.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-gs_engine-0.23.0a20230613.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.23.0a20230613.dist-info/RECORD,,
+gs_engine-0.23.0a20230615.dist-info/METADATA,sha256=Md_2JQnmN3ydOj-iYq3iiS6f7jjGapz5s2D009dng_8,21680
+gs_engine-0.23.0a20230615.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+gs_engine-0.23.0a20230615.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.23.0a20230615.dist-info/RECORD,,
```

