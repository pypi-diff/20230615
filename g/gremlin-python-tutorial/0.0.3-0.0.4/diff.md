# Comparing `tmp/gremlin_python_tutorial-0.0.3.tar.gz` & `tmp/gremlin_python_tutorial-0.0.4.tar.gz`

## Comparing `gremlin_python_tutorial-0.0.3.tar` & `gremlin_python_tutorial-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.project
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.pydevproject
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.travis.yml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/setServer.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.github/workflows/build.yaml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/DataStax.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/Neo4j.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/OrientDB.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/TinkerGraph.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/server.yaml
--rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/data/air-routes-small.xml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/data/tinkerpop-modern.xml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/draw.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/examples.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/remote.py
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/install
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/installAndTest
--rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/run
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runDataStax
--rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runNeo4j
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runOrientDB
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/base_gremlin_test.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/basetest.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_003_connection.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_004_io.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_005_graphviz.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_draw.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_examples.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_modern.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_server.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_tutorial.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/LICENSE
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.project
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.pydevproject
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.travis.yml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/setServer.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/DataStax.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/Neo4j.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/OrientDB.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/TinkerGraph.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/config/server.yaml
+-rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/data/air-routes-small.xml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/data/tinkerpop-modern.xml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/draw.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/examples.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/gremlin/remote.py
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/install
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/installAndTest
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/run
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runDataStax
+-rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runNeo4j
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/runOrientDB
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/base_gremlin_test.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/basetest.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_003_connection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_004_io.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_005_graphviz.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_draw.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_examples.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_modern.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_server.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/tests/test_tutorial.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.4/PKG-INFO
```

### Comparing `gremlin_python_tutorial-0.0.3/.project` & `gremlin_python_tutorial-0.0.4/.project`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/.travis.yml` & `gremlin_python_tutorial-0.0.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/setServer.py` & `gremlin_python_tutorial-0.0.4/setServer.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/.github/workflows/build.yaml` & `gremlin_python_tutorial-0.0.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/.github/workflows/upload-to-pypi.yml` & `gremlin_python_tutorial-0.0.4/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/data/air-routes-small.xml` & `gremlin_python_tutorial-0.0.4/data/air-routes-small.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/data/tinkerpop-modern.xml` & `gremlin_python_tutorial-0.0.4/data/tinkerpop-modern.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/gremlin/draw.py` & `gremlin_python_tutorial-0.0.4/gremlin/draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/gremlin/examples.py` & `gremlin_python_tutorial-0.0.4/gremlin/examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/gremlin/remote.py` & `gremlin_python_tutorial-0.0.4/gremlin/remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Created on 2019-09-17
 
 @author: wf
 '''
 from gremlin_python.process.anonymous_traversal import traversal
 from gremlin_python.driver.driver_remote_connection import DriverRemoteConnection
+from gremlin_python.driver.aiohttp.transport import AiohttpTransport
 import os.path
 from os.path import dirname, abspath
 import io
 import yaml
 import socket
 from contextlib import closing
 
@@ -42,15 +43,15 @@
         get the graph traversal
         """
         server=self.server
         url=f'ws://{server.host}:{server.port}/gremlin' 
         # https://github.com/orientechnologies/orientdb-gremlin/issues/143
         #username="root"
         #password="rootpwd"
-        self.remoteConnection=DriverRemoteConnection(url,server.alias,username=server.username,password=server.password)
+        self.remoteConnection=DriverRemoteConnection(url,server.alias,username=server.username,password=server.password, transport_factory=lambda:AiohttpTransport(call_from_event_loop=True))
         g = traversal().with_remote(self.remoteConnection)
         return g
     
     def close(self):
         """
         close my connection
         """
```

### Comparing `gremlin_python_tutorial-0.0.3/scripts/installAndTest` & `gremlin_python_tutorial-0.0.4/scripts/installAndTest`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/scripts/run` & `gremlin_python_tutorial-0.0.4/scripts/run`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/scripts/runNeo4j` & `gremlin_python_tutorial-0.0.4/scripts/runNeo4j`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/base_gremlin_test.py` & `gremlin_python_tutorial-0.0.4/tests/base_gremlin_test.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/basetest.py` & `gremlin_python_tutorial-0.0.4/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_003_connection.py` & `gremlin_python_tutorial-0.0.4/tests/test_003_connection.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_004_io.py` & `gremlin_python_tutorial-0.0.4/tests/test_004_io.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_005_graphviz.py` & `gremlin_python_tutorial-0.0.4/tests/test_005_graphviz.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_draw.py` & `gremlin_python_tutorial-0.0.4/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_examples.py` & `gremlin_python_tutorial-0.0.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_modern.py` & `gremlin_python_tutorial-0.0.4/tests/test_modern.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/tests/test_tutorial.py` & `gremlin_python_tutorial-0.0.4/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/.gitignore` & `gremlin_python_tutorial-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/LICENSE` & `gremlin_python_tutorial-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/README.md` & `gremlin_python_tutorial-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/pyproject.toml` & `gremlin_python_tutorial-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.3/PKG-INFO` & `gremlin_python_tutorial-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlin-python-tutorial
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Home, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Gremlin_python
 Project-URL: Source, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Author-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

