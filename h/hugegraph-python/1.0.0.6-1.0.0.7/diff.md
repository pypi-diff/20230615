# Comparing `tmp/hugegraph-python-1.0.0.6.tar.gz` & `tmp/hugegraph-python-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.6.tar", last modified: Thu Jun 15 08:07:07 2023, max compression
+gzip compressed data, was "dist/hugegraph-python-1.0.0.7.tar", last modified: Thu Jun 15 08:52:19 2023, max compression
```

## Comparing `hugegraph-python-1.0.0.6.tar` & `hugegraph-python-1.0.0.7.tar`

### file list

```diff
@@ -1,13 +1,42 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.199756 hugegraph-python-1.0.0.6/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.6/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:07:07.199341 hugegraph-python-1.0.0.6/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-04-18 04:57:38.000000 hugegraph-python-1.0.0.6/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.197877 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      199 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/top_level.txt
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 08:07:07.199876 hugegraph-python-1.0.0.6/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 08:05:26.000000 hugegraph-python-1.0.0.6/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.198428 hugegraph-python-1.0.0.6/test/
--rw-r--r--   0 zsm        (501) staff       (20)      613 2023-06-15 08:01:51.000000 hugegraph-python-1.0.0.6/test/test.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.656998 hugegraph-python-1.0.0.7/
+-rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.7/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:52:19.656350 hugegraph-python-1.0.0.7/PKG-INFO
+-rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-06-15 08:14:41.000000 hugegraph-python-1.0.0.7/README.md
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.641319 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      787 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       26 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/top_level.txt
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.643515 hugegraph-python-1.0.0.7/manager/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/manager/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2126 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/common.py
+-rw-rw-r--   0 zsm        (501) staff       (20)    13726 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/graph_manager.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1677 2023-06-15 02:47:44.000000 hugegraph-python-1.0.0.7/manager/gremlin_manager.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.645598 hugegraph-python-1.0.0.7/manager/schema/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/manager/schema/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6471 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/manager/schema/edge_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     4158 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.7/manager/schema/index_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6540 2023-04-14 07:47:12.000000 hugegraph-python-1.0.0.7/manager/schema/property_key.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6555 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/manager/schema/vertex_label.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     6366 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/schema_manager.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.649771 hugegraph-python-1.0.0.7/models/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/models/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2038 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/edge_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2203 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/edge_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1973 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.7/models/index_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1609 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.7/models/property_key_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1317 2023-04-18 04:39:59.000000 hugegraph-python-1.0.0.7/models/respon_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1503 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/vertex_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1989 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/vertex_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 08:52:19.657220 hugegraph-python-1.0.0.7/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 08:52:17.000000 hugegraph-python-1.0.0.7/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.651554 hugegraph-python-1.0.0.7/test/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/test/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)      611 2023-06-15 08:14:41.000000 hugegraph-python-1.0.0.7/test/test.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1964 2023-06-15 08:22:59.000000 hugegraph-python-1.0.0.7/test/test_df.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.655649 hugegraph-python-1.0.0.7/utils/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/utils/__init__.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1532 2023-04-14 04:34:09.000000 hugegraph-python-1.0.0.7/utils/exceptions.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1745 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/utils/huge_decorator.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1221 2023-04-13 11:39:44.000000 hugegraph-python-1.0.0.7/utils/huge_requests.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1474 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/utils/util.py
```

### Comparing `hugegraph-python-1.0.0.6/LICENSE` & `hugegraph-python-1.0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.6/PKG-INFO` & `hugegraph-python-1.0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.6
+Version: 1.0.0.7
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,20 @@
 pip3 install hugegraph-python
 ```
 
 ## Install from source
 release soon
 
 # Examples
+
 ```python
-from hugegraph import PyHugeGraph
+from hugegraph import PHugeGraph
+
 # init client
-client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.6/README.md` & `hugegraph-python-1.0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 pip3 install hugegraph-python
 ```
 
 ## Install from source
 release soon
 
 # Examples
+
 ```python
-from hugegraph import PyHugeGraph
+from hugegraph import PHugeGraph
+
 # init client
-client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.6/hugegraph_python.egg-info/PKG-INFO` & `hugegraph-python-1.0.0.7/hugegraph_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.6
+Version: 1.0.0.7
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,20 @@
 pip3 install hugegraph-python
 ```
 
 ## Install from source
 release soon
 
 # Examples
+
 ```python
-from hugegraph import PyHugeGraph
+from hugegraph import PHugeGraph
+
 # init client
-client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.6/setup.py` & `hugegraph-python-1.0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hugegraph-python",
-    version="1.0.0.6",
+    version="1.0.0.7",
     author="cvte-research-datamining",
     author_email="ming@apache.org",
     description="A Python SDK for Apache HugeGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cvte-research-datamining/hugegraph-python",
     packages=setuptools.find_packages(),
```

### Comparing `hugegraph-python-1.0.0.6/test/test.py` & `hugegraph-python-1.0.0.7/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hugegraph import PyHugeGraph
+from hugegraph import PHugeGraph
 
 if __name__ == '__main__':
-    client = PyHugeGraph("10.21.3.10", "8080", user="admin", pwd="admin", graph="hugegraph")
+    client = PHugeGraph("10.21.3.10", "8080", user="admin", pwd="admin", graph="hugegraph")
 
     """system"""
     res = client.get_graphinfo()
     print(res)
 
     res = client.get_all_graphs()
     print(res)
```

