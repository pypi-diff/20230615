# Comparing `tmp/webhdfs_py_client-0.0b5-py2.py3-none-any.whl.zip` & `tmp/webhdfs_py_client-0.0b6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12029 bytes, number of entries: 14
+Zip file size: 12026 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-15 20:24 webhdfs_py/__init__.py
 -rw-rw-rw-  2.0 fat      493 b- defN 23-Jun-01 19:50 webhdfs_py/errors.py
 -rw-rw-rw-  2.0 fat      406 b- defN 23-Jun-07 19:36 webhdfs_py/operations.py
 -rw-rw-rw-  2.0 fat    27368 b- defN 23-Jun-15 20:27 webhdfs_py/webhdfs.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-15 20:46 webhdfs_py/example/__init__.py
 -rw-rw-rw-  2.0 fat     2483 b- defN 23-Jun-15 15:14 webhdfs_py/example/example.py
 -rw-rw-rw-  2.0 fat     1160 b- defN 23-Jun-01 02:02 webhdfs_py/example/hello.py
 -rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-15 20:42 webhdfs_py/example/run.py
 -rw-rw-rw-  2.0 fat      390 b- defN 23-Jun-01 02:08 webhdfs_py/example/utils.py
--rw-rw-rw-  2.0 fat     1649 b- defN 23-Jun-15 20:17 webhdfs_py/example/pages/dataframe.py
--rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1164 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/RECORD
-14 files, 39268 bytes uncompressed, 10083 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat     1651 b- defN 23-Jun-15 21:25 webhdfs_py/example/pages/dataframe.py
+-rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-15 21:26 webhdfs_py_client-0.0b6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-15 21:26 webhdfs_py_client-0.0b6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-15 21:26 webhdfs_py_client-0.0b6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1164 b- defN 23-Jun-15 21:26 webhdfs_py_client-0.0b6.dist-info/RECORD
+14 files, 39270 bytes uncompressed, 10080 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: webhdfs_py/example/utils.py
 Comment: 
 
 Filename: webhdfs_py/example/pages/dataframe.py
 Comment: 
 
-Filename: webhdfs_py_client-0.0b5.dist-info/METADATA
+Filename: webhdfs_py_client-0.0b6.dist-info/METADATA
 Comment: 
 
-Filename: webhdfs_py_client-0.0b5.dist-info/WHEEL
+Filename: webhdfs_py_client-0.0b6.dist-info/WHEEL
 Comment: 
 
-Filename: webhdfs_py_client-0.0b5.dist-info/top_level.txt
+Filename: webhdfs_py_client-0.0b6.dist-info/top_level.txt
 Comment: 
 
-Filename: webhdfs_py_client-0.0b5.dist-info/RECORD
+Filename: webhdfs_py_client-0.0b6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webhdfs_py/example/pages/dataframe.py

```diff
@@ -43,8 +43,8 @@
             st.markdown(f"se subio correctamente: **{home_path+uploaded_file.name}** ")
 with t2:
     
     json_data = hdfs.list_dir(home_path)
     expander = st.expander(home_path)
     expander.write(json_data)
     # show_code( hdfs)
-    st.download_button()
+    # st.download_button()
```

## Comparing `webhdfs_py_client-0.0b5.dist-info/METADATA` & `webhdfs_py_client-0.0b6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0b5
+Version: 0.0b6
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `webhdfs_py_client-0.0b5.dist-info/RECORD` & `webhdfs_py_client-0.0b6.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 webhdfs_py/operations.py,sha256=GVO-aG97iiMB0HGKvnPBtpZiVsPAuzYxaYbSmKZyH1o,406
 webhdfs_py/webhdfs.py,sha256=_rHrcrWJQPBg4Dx4JUENY1TQEmOJcrjza4PCwdiCBMk,27368
 webhdfs_py/example/__init__.py,sha256=V0cl8MZIMc93oz3NIgy3qBw_oNUtGxOcdZ0uCTE7QIQ,38
 webhdfs_py/example/example.py,sha256=J_4H6cNbgkrV-9ebeO4dSafct885_INeZX5FGuCVGnE,2483
 webhdfs_py/example/hello.py,sha256=Z77VQ8JSZq0-bT129HVCkH8vqMMBPFWBFX9b5IlKA58,1160
 webhdfs_py/example/run.py,sha256=_oL1tj8ejl9Hc-xtgGIKDMrPKc5QfMq1LtKsrQcJl5E,364
 webhdfs_py/example/utils.py,sha256=TpXLcEeK1zmPAwyWCYh3TZL2BWl0Pp1_H19f1Fpcihc,390
-webhdfs_py/example/pages/dataframe.py,sha256=KJt_NUoOtdoRZqWAXUYqyhdw9hcRM8wTaNuHgGSDwUM,1649
-webhdfs_py_client-0.0b5.dist-info/METADATA,sha256=o6DgLcg4OG23SdeZ1VoyJEUyYkrXBdElkFnaklIxDq0,3586
-webhdfs_py_client-0.0b5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-webhdfs_py_client-0.0b5.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
-webhdfs_py_client-0.0b5.dist-info/RECORD,,
+webhdfs_py/example/pages/dataframe.py,sha256=YAWElNV6wCXzsSyifx4gc3WbtUTJZzyxKGrwdQ79eQ8,1651
+webhdfs_py_client-0.0b6.dist-info/METADATA,sha256=GEOFr7fAOPf4-gOAn-6rgpPAlAOa594OFhD5vk845_g,3586
+webhdfs_py_client-0.0b6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+webhdfs_py_client-0.0b6.dist-info/top_level.txt,sha256=U-g45ZCFQMp3TX9DsicMZluP7m5tVb_V88Xs3Wj5A1Q,11
+webhdfs_py_client-0.0b6.dist-info/RECORD,,
```

