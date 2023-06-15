# Comparing `tmp/hugegraph-python-1.0.0.7.tar.gz` & `tmp/hugegraph-python-1.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.7.tar", last modified: Thu Jun 15 08:52:19 2023, max compression
+gzip compressed data, was "dist/hugegraph-python-1.0.0.8.tar", last modified: Thu Jun 15 09:03:08 2023, max compression
```

## Comparing `hugegraph-python-1.0.0.7.tar` & `hugegraph-python-1.0.0.8.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.656998 hugegraph-python-1.0.0.7/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.7/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:52:19.656350 hugegraph-python-1.0.0.7/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-06-15 08:14:41.000000 hugegraph-python-1.0.0.7/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.641319 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      787 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)       26 2023-06-15 08:52:19.000000 hugegraph-python-1.0.0.7/hugegraph_python.egg-info/top_level.txt
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.643515 hugegraph-python-1.0.0.7/manager/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/manager/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     2126 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/common.py
--rw-rw-r--   0 zsm        (501) staff       (20)    13726 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/graph_manager.py
--rw-r--r--   0 zsm        (501) staff       (20)     1677 2023-06-15 02:47:44.000000 hugegraph-python-1.0.0.7/manager/gremlin_manager.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.645598 hugegraph-python-1.0.0.7/manager/schema/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/manager/schema/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     6471 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/manager/schema/edge_label.py
--rw-r--r--   0 zsm        (501) staff       (20)     4158 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.7/manager/schema/index_label.py
--rw-r--r--   0 zsm        (501) staff       (20)     6540 2023-04-14 07:47:12.000000 hugegraph-python-1.0.0.7/manager/schema/property_key.py
--rw-r--r--   0 zsm        (501) staff       (20)     6555 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/manager/schema/vertex_label.py
--rw-rw-r--   0 zsm        (501) staff       (20)     6366 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.7/manager/schema_manager.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.649771 hugegraph-python-1.0.0.7/models/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/models/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     2038 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/edge_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     2203 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/edge_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1973 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.7/models/index_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1609 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.7/models/property_key_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1317 2023-04-18 04:39:59.000000 hugegraph-python-1.0.0.7/models/respon_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1503 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/vertex_data.py
--rw-r--r--   0 zsm        (501) staff       (20)     1989 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.7/models/vertex_label_data.py
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 08:52:19.657220 hugegraph-python-1.0.0.7/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 08:52:17.000000 hugegraph-python-1.0.0.7/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.651554 hugegraph-python-1.0.0.7/test/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/test/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)      611 2023-06-15 08:14:41.000000 hugegraph-python-1.0.0.7/test/test.py
--rw-r--r--   0 zsm        (501) staff       (20)     1964 2023-06-15 08:22:59.000000 hugegraph-python-1.0.0.7/test/test_df.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:52:19.655649 hugegraph-python-1.0.0.7/utils/
--rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.7/utils/__init__.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1532 2023-04-14 04:34:09.000000 hugegraph-python-1.0.0.7/utils/exceptions.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1745 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/utils/huge_decorator.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1221 2023-04-13 11:39:44.000000 hugegraph-python-1.0.0.7/utils/huge_requests.py
--rw-rw-r--   0 zsm        (501) staff       (20)     1474 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.7/utils/util.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.776270 hugegraph-python-1.0.0.8/
+-rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.8/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     1350 2023-06-15 09:03:08.775883 hugegraph-python-1.0.0.8/PKG-INFO
+-rw-rw-r--   0 zsm        (501) staff       (20)      866 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.8/README.md
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.761348 hugegraph-python-1.0.0.8/hugegraph/
+-rw-rw-r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/hugegraph/__init__.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     3721 2023-06-15 09:02:12.000000 hugegraph-python-1.0.0.8/hugegraph/connection.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1070 2023-04-14 07:32:18.000000 hugegraph-python-1.0.0.8/hugegraph/constants.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.764415 hugegraph-python-1.0.0.8/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     1350 2023-06-15 09:03:08.000000 hugegraph-python-1.0.0.8/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      856 2023-06-15 09:03:08.000000 hugegraph-python-1.0.0.8/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 09:03:08.000000 hugegraph-python-1.0.0.8/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       36 2023-06-15 09:03:08.000000 hugegraph-python-1.0.0.8/hugegraph_python.egg-info/top_level.txt
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.766329 hugegraph-python-1.0.0.8/manager/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/manager/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2136 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.8/manager/common.py
+-rw-rw-r--   0 zsm        (501) staff       (20)    13726 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.8/manager/graph_manager.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1677 2023-06-15 02:47:44.000000 hugegraph-python-1.0.0.8/manager/gremlin_manager.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.768297 hugegraph-python-1.0.0.8/manager/schema/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/manager/schema/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6471 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.8/manager/schema/edge_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     4158 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.8/manager/schema/index_label.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6540 2023-04-14 07:47:12.000000 hugegraph-python-1.0.0.8/manager/schema/property_key.py
+-rw-r--r--   0 zsm        (501) staff       (20)     6555 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.8/manager/schema/vertex_label.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     6366 2023-04-14 07:49:55.000000 hugegraph-python-1.0.0.8/manager/schema_manager.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.771579 hugegraph-python-1.0.0.8/models/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/models/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2038 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.8/models/edge_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     2203 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.8/models/edge_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1973 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.8/models/index_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1609 2023-04-14 01:24:51.000000 hugegraph-python-1.0.0.8/models/property_key_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1317 2023-04-18 04:39:59.000000 hugegraph-python-1.0.0.8/models/respon_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1503 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.8/models/vertex_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1989 2023-04-14 02:01:36.000000 hugegraph-python-1.0.0.8/models/vertex_label_data.py
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 09:03:08.776483 hugegraph-python-1.0.0.8/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 09:03:06.000000 hugegraph-python-1.0.0.8/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.772715 hugegraph-python-1.0.0.8/test/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/test/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)      624 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.8/test/test.py
+-rw-r--r--   0 zsm        (501) staff       (20)     1959 2023-06-15 09:02:39.000000 hugegraph-python-1.0.0.8/test/test_df.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 09:03:08.775188 hugegraph-python-1.0.0.8/utils/
+-rw-r--r--   0 zsm        (501) staff       (20)      801 2023-04-14 02:23:11.000000 hugegraph-python-1.0.0.8/utils/__init__.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1532 2023-04-14 04:34:09.000000 hugegraph-python-1.0.0.8/utils/exceptions.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1745 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.8/utils/huge_decorator.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1221 2023-04-13 11:39:44.000000 hugegraph-python-1.0.0.8/utils/huge_requests.py
+-rw-rw-r--   0 zsm        (501) staff       (20)     1474 2023-04-14 07:33:45.000000 hugegraph-python-1.0.0.8/utils/util.py
```

### Comparing `hugegraph-python-1.0.0.7/LICENSE` & `hugegraph-python-1.0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/PKG-INFO` & `hugegraph-python-1.0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.7
+Version: 1.0.0.8
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -26,18 +26,18 @@
 
 ## Install from source
 release soon
 
 # Examples
 
 ```python
-from hugegraph import PHugeGraph
+from hugegraph.connection import PyHugeGraph
 
 # init client
-client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.7/README.md` & `hugegraph-python-1.0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 ## Install from source
 release soon
 
 # Examples
 
 ```python
-from hugegraph import PHugeGraph
+from hugegraph.connection import PyHugeGraph
 
 # init client
-client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.7/hugegraph_python.egg-info/PKG-INFO` & `hugegraph-python-1.0.0.8/hugegraph_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.7
+Version: 1.0.0.8
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -26,18 +26,18 @@
 
 ## Install from source
 release soon
 
 # Examples
 
 ```python
-from hugegraph import PHugeGraph
+from hugegraph.connection import PyHugeGraph
 
 # init client
-client = PHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
+client = PyHugeGraph("127.0.0.1", "8080", user="admin", pwd="pwd", graph="hugegraph")
 
 # schema
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
```

### Comparing `hugegraph-python-1.0.0.7/hugegraph_python.egg-info/SOURCES.txt` & `hugegraph-python-1.0.0.8/hugegraph_python.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 LICENSE
 README.md
 setup.py
+hugegraph/__init__.py
+hugegraph/connection.py
+hugegraph/constants.py
 hugegraph_python.egg-info/PKG-INFO
 hugegraph_python.egg-info/SOURCES.txt
 hugegraph_python.egg-info/dependency_links.txt
 hugegraph_python.egg-info/top_level.txt
 manager/__init__.py
 manager/common.py
 manager/graph_manager.py
```

### Comparing `hugegraph-python-1.0.0.7/manager/__init__.py` & `hugegraph-python-1.0.0.8/hugegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/common.py` & `hugegraph-python-1.0.0.8/manager/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-from constants import Graph
+from hugegraph.constants import Graph
 
 
 class ParameterHolder:
     def __init__(self):
         self._dic = {}
 
     def set(self, key, value):
```

### Comparing `hugegraph-python-1.0.0.7/manager/graph_manager.py` & `hugegraph-python-1.0.0.8/manager/graph_manager.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/gremlin_manager.py` & `hugegraph-python-1.0.0.8/manager/gremlin_manager.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema/__init__.py` & `hugegraph-python-1.0.0.8/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema/edge_label.py` & `hugegraph-python-1.0.0.8/manager/schema/edge_label.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema/index_label.py` & `hugegraph-python-1.0.0.8/manager/schema/index_label.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema/property_key.py` & `hugegraph-python-1.0.0.8/manager/schema/property_key.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema/vertex_label.py` & `hugegraph-python-1.0.0.8/manager/schema/vertex_label.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/manager/schema_manager.py` & `hugegraph-python-1.0.0.8/manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/__init__.py` & `hugegraph-python-1.0.0.8/manager/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/edge_data.py` & `hugegraph-python-1.0.0.8/models/edge_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/edge_label_data.py` & `hugegraph-python-1.0.0.8/models/edge_label_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/index_label_data.py` & `hugegraph-python-1.0.0.8/models/index_label_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/property_key_data.py` & `hugegraph-python-1.0.0.8/models/property_key_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/respon_data.py` & `hugegraph-python-1.0.0.8/models/respon_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/vertex_data.py` & `hugegraph-python-1.0.0.8/models/vertex_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/models/vertex_label_data.py` & `hugegraph-python-1.0.0.8/models/vertex_label_data.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/setup.py` & `hugegraph-python-1.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hugegraph-python",
-    version="1.0.0.7",
+    version="1.0.0.8",
     author="cvte-research-datamining",
     author_email="ming@apache.org",
     description="A Python SDK for Apache HugeGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cvte-research-datamining/hugegraph-python",
     packages=setuptools.find_packages(),
```

### Comparing `hugegraph-python-1.0.0.7/test/__init__.py` & `hugegraph-python-1.0.0.8/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/test/test.py` & `hugegraph-python-1.0.0.8/test/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hugegraph import PHugeGraph
+from hugegraph.connection import PyHugeGraph
 
 if __name__ == '__main__':
-    client = PHugeGraph("10.21.3.10", "8080", user="admin", pwd="admin", graph="hugegraph")
+    client = PyHugeGraph("10.21.3.10", "8080", user="admin", pwd="admin", graph="hugegraph")
 
     """system"""
     res = client.get_graphinfo()
     print(res)
 
     res = client.get_all_graphs()
     print(res)
```

### Comparing `hugegraph-python-1.0.0.7/test/test_df.py` & `hugegraph-python-1.0.0.8/test/test_df.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import time
 import eventlet  # 导入eventlet这个模块
-from hugegraph import PyHugeGraph
-import gremlinapi
 
-hugegraph_conn = PHugeGraph("10.22.32.24", "8080",
+from hugegraph.connection import PyHugeGraph
+
+hugegraph_conn = PyHugeGraph("10.22.32.24", "8080",
                             user="admin", pwd="admin", graph="exercise")
 
 
 # hugegraph_conn = PyHugeGraph(kv_dict['graph_host'], kv_dict['graph_port'],
 #                      user=kv_dict['graph_user'], pwd=kv_dict['graph_pwd'], graph="exercise")
 def get_date_from_hugegraph(student_id, chapter_id_list):
     chapter_ids = '\',\''.join(chapter_id_list)
```

### Comparing `hugegraph-python-1.0.0.7/utils/__init__.py` & `hugegraph-python-1.0.0.8/test/__init__.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/utils/exceptions.py` & `hugegraph-python-1.0.0.8/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/utils/huge_decorator.py` & `hugegraph-python-1.0.0.8/utils/huge_decorator.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/utils/huge_requests.py` & `hugegraph-python-1.0.0.8/utils/huge_requests.py`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.7/utils/util.py` & `hugegraph-python-1.0.0.8/utils/util.py`

 * *Files identical despite different names*

