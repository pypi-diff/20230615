# Comparing `tmp/webhdfs_py_client-0.0b4-py2.py3-none-any.whl.zip` & `tmp/webhdfs_py_client-0.0b5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11985 bytes, number of entries: 14
+Zip file size: 12029 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jun-15 20:24 webhdfs_py/__init__.py
 -rw-rw-rw-  2.0 fat      493 b- defN 23-Jun-01 19:50 webhdfs_py/errors.py
 -rw-rw-rw-  2.0 fat      406 b- defN 23-Jun-07 19:36 webhdfs_py/operations.py
 -rw-rw-rw-  2.0 fat    27368 b- defN 23-Jun-15 20:27 webhdfs_py/webhdfs.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-15 14:38 webhdfs_py/example/__init__.py
+-rw-rw-rw-  2.0 fat       38 b- defN 23-Jun-15 20:46 webhdfs_py/example/__init__.py
 -rw-rw-rw-  2.0 fat     2483 b- defN 23-Jun-15 15:14 webhdfs_py/example/example.py
 -rw-rw-rw-  2.0 fat     1160 b- defN 23-Jun-01 02:02 webhdfs_py/example/hello.py
--rw-rw-rw-  2.0 fat      360 b- defN 23-Jun-15 14:45 webhdfs_py/example/run.py
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-15 20:42 webhdfs_py/example/run.py
 -rw-rw-rw-  2.0 fat      390 b- defN 23-Jun-01 02:08 webhdfs_py/example/utils.py
 -rw-rw-rw-  2.0 fat     1649 b- defN 23-Jun-15 20:17 webhdfs_py/example/pages/dataframe.py
--rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-15 20:34 webhdfs_py_client-0.0b4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-15 20:34 webhdfs_py_client-0.0b4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-15 20:34 webhdfs_py_client-0.0b4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1163 b- defN 23-Jun-15 20:34 webhdfs_py_client-0.0b4.dist-info/RECORD
-14 files, 39225 bytes uncompressed, 10039 bytes compressed:  74.4%
+-rw-rw-rw-  2.0 fat     3586 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1164 b- defN 23-Jun-15 20:49 webhdfs_py_client-0.0b5.dist-info/RECORD
+14 files, 39268 bytes uncompressed, 10083 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: webhdfs_py/example/utils.py
 Comment: 
 
 Filename: webhdfs_py/example/pages/dataframe.py
 Comment: 
 
-Filename: webhdfs_py_client-0.0b4.dist-info/METADATA
+Filename: webhdfs_py_client-0.0b5.dist-info/METADATA
 Comment: 
 
-Filename: webhdfs_py_client-0.0b4.dist-info/WHEEL
+Filename: webhdfs_py_client-0.0b5.dist-info/WHEEL
 Comment: 
 
-Filename: webhdfs_py_client-0.0b4.dist-info/top_level.txt
+Filename: webhdfs_py_client-0.0b5.dist-info/top_level.txt
 Comment: 
 
-Filename: webhdfs_py_client-0.0b4.dist-info/RECORD
+Filename: webhdfs_py_client-0.0b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webhdfs_py/example/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 6672 6f6d 2077 6562 6864 6673 5f70 792e  from webhdfs_py.
+00000010: 6578 616d 706c 652e 7275 6e20 696d 706f  example.run impo
+00000020: 7274 2072 756e                           rt run
```

## webhdfs_py/example/run.py

```diff
@@ -7,9 +7,9 @@
     file_path = os.path.join(dir_path, "hello.py")
 
     _config.set_option("server.headless", False)
     args = []
 
     bootstrap.run(file_path,'',args, flag_options={})
 
-if __name__ == "__main__":
-    run()
+# if __name__ == "__main__":
+#     run()
```

## Comparing `webhdfs_py_client-0.0b4.dist-info/METADATA` & `webhdfs_py_client-0.0b5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0b4
+Version: 0.0b5
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

