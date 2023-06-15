# Comparing `tmp/gremlin_python_tutorial-0.0.2.tar.gz` & `tmp/gremlin_python_tutorial-0.0.3.tar.gz`

## Comparing `gremlin_python_tutorial-0.0.2.tar` & `gremlin_python_tutorial-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.project
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.pydevproject
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.travis.yml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/setServer.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.github/workflows/build.yaml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/config/DataStax.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/config/Neo4j.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/config/OrientDB.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/config/TinkerGraph.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/config/server.yaml
--rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/data/air-routes-small.xml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/data/tinkerpop-modern.xml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/gremlin/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/gremlin/draw.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/gremlin/examples.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/gremlin/remote.py
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/install
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/installAndTest
--rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/run
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/runDataStax
--rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/runNeo4j
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/runOrientDB
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/base_gremlin_test.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/basetest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_003_connection.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_004_io.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_005_graphviz.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_draw.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_examples.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_modern.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_server.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/tests/test_tutorial.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/LICENSE
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.project
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.pydevproject
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.travis.yml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/setServer.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/DataStax.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/Neo4j.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/OrientDB.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/TinkerGraph.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/config/server.yaml
+-rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/data/air-routes-small.xml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/data/tinkerpop-modern.xml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/__init__.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/draw.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/examples.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/gremlin/remote.py
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/install
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/installAndTest
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/run
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runDataStax
+-rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runNeo4j
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/runOrientDB
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/base_gremlin_test.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/basetest.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_003_connection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_004_io.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_005_graphviz.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_draw.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_examples.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_modern.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_server.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/tests/test_tutorial.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.3/PKG-INFO
```

### Comparing `gremlin_python_tutorial-0.0.2/.project` & `gremlin_python_tutorial-0.0.3/.project`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/.travis.yml` & `gremlin_python_tutorial-0.0.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/setServer.py` & `gremlin_python_tutorial-0.0.3/setServer.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/.github/workflows/build.yaml` & `gremlin_python_tutorial-0.0.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/.github/workflows/upload-to-pypi.yml` & `gremlin_python_tutorial-0.0.3/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/data/air-routes-small.xml` & `gremlin_python_tutorial-0.0.3/data/air-routes-small.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/data/tinkerpop-modern.xml` & `gremlin_python_tutorial-0.0.3/data/tinkerpop-modern.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/gremlin/draw.py` & `gremlin_python_tutorial-0.0.3/gremlin/draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/gremlin/examples.py` & `gremlin_python_tutorial-0.0.3/gremlin/examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/gremlin/remote.py` & `gremlin_python_tutorial-0.0.3/gremlin/remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,33 @@
 from contextlib import closing
 
 class RemoteTraversal:
     """
     helper class for Apache Tinkerpop Gremlin Python GLV remote access
     """
 
-    def __init__(self,serverName='server',config_path:str=None):
+    def __init__(self,server):
         """
         constructor
         
+        """
+        self.server=server
+        
+    @classmethod
+    def fromYaml(cls,serverName='server',config_path:str=None)->"RemoteTraversal":
+        """
+        create a server from the given yaml file
+        
         Args:
             serverName(str): the servername to use
+            config_path(str): the path to the server configuration file
         """
-        self.server=Server.read(serverName,config_path)
+        server=Server.read(serverName,config_path)
+        rt=RemoteTraversal(server)
+        return rt
    
     def g(self):
         """
         get the graph traversal
         """
         server=self.server
         url=f'ws://{server.host}:{server.port}/gremlin'
```

### Comparing `gremlin_python_tutorial-0.0.2/scripts/installAndTest` & `gremlin_python_tutorial-0.0.3/scripts/installAndTest`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/scripts/run` & `gremlin_python_tutorial-0.0.3/scripts/run`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/scripts/runNeo4j` & `gremlin_python_tutorial-0.0.3/scripts/runNeo4j`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/base_gremlin_test.py` & `gremlin_python_tutorial-0.0.3/tests/base_gremlin_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 '''
 Created on 2023-03-23
 
 @author: wf
 '''
 from tests.basetest import Basetest
-from gremlin.remote import RemoteTraversal
+from gremlin.remote import RemoteTraversal, Server
 from gremlin.examples import Examples, Volume
 
 class BaseGremlinTest(Basetest):
     """
     Basetest for Gremlin Python
     """
     
     def setUp(self, debug=False, profile=True):
         """
         prepare the test environment
         """
         Basetest.setUp(self, debug, profile)
-        self.remote_traversal=RemoteTraversal()
+        self.server=Server()
+        self.remote_traversal=RemoteTraversal(self.server)
         self.g=self.remote_traversal.g()
         self.volume=Volume.docker()
         self.examples=Examples(volume=self.volume,debug=self.debug)
         
     def tearDown(self):
         """
         tear down
```

### Comparing `gremlin_python_tutorial-0.0.2/tests/basetest.py` & `gremlin_python_tutorial-0.0.3/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_003_connection.py` & `gremlin_python_tutorial-0.0.3/tests/test_003_connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # see https://github.com/apache/tinkerpop/blob/master/gremlin-python/src/main/jython/tests/driver/test_client.py
 from gremlin_python.driver.request import RequestMessage
-from gremlin.remote import RemoteTraversal
+from gremlin.remote import RemoteTraversal, Server
 from tests.basetest import Basetest
 
 class TestConnection(Basetest):
     """
     test connection handling
     """
     # test a connection
     def test_connection(self):
         # see https://github.com/apache/tinkerpop/blob/master/gremlin-python/src/main/jython/gremlin_python/driver/driver_remote_connection.py
-        remoteTraversal=RemoteTraversal()
-        g = remoteTraversal.g()
+        server=Server()
+        remote_traversal=RemoteTraversal(server)
+        g = remote_traversal.g()
         t=g.V()
-        remoteConnection=remoteTraversal.remoteConnection
+        remoteConnection=remote_traversal.remoteConnection
         # see https://github.com/apache/tinkerpop/blob/master/gremlin-python/src/main/jython/gremlin_python/driver/client.py
         client=remoteConnection._client
     
         connection=client._get_connection()
         message = RequestMessage('traversal', 'bytecode', {'gremlin': t.bytecode, 'aliases': {'g': client._traversal_source}})
         results_set = connection.write(message).result()
         future = results_set.all()
```

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_004_io.py` & `gremlin_python_tutorial-0.0.3/tests/test_004_io.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_005_graphviz.py` & `gremlin_python_tutorial-0.0.3/tests/test_005_graphviz.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_draw.py` & `gremlin_python_tutorial-0.0.3/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_examples.py` & `gremlin_python_tutorial-0.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_modern.py` & `gremlin_python_tutorial-0.0.3/tests/test_modern.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/tests/test_tutorial.py` & `gremlin_python_tutorial-0.0.3/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/.gitignore` & `gremlin_python_tutorial-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/LICENSE` & `gremlin_python_tutorial-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/README.md` & `gremlin_python_tutorial-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![pypi](https://img.shields.io/pypi/pyversions/gremlin-python-tutorial)](https://pypi.org/project/gremlin-python-tutorial/)
+[![PyPI Status](https://img.shields.io/pypi/v/gremlin-python-tutorial)](https://pypi.org/project/gremlin-python-tutorial/)
 [![Github Actions - build](https://github.com/WolfgangFahl/gremlin-python-tutorial/actions/workflows/build.yaml/badge.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/actions/workflows/build.yaml)
 [![GitHub issues](https://img.shields.io/github/issues/WolfgangFahl/gremlin-python-tutorial.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/issues)
 [![GitHub issues](https://img.shields.io/github/issues-closed/WolfgangFahl/gremlin-python-tutorial.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/issues/?q=is%3Aissue+is%3Aclosed)
 [![GitHub](https://img.shields.io/github/license/WolfgangFahl/gremlin-python-tutorial.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [<img alt="BITPlan" width="8%" src="http://wiki.bitplan.com/images/wiki/thumb/3/38/BITPlanLogoFontLessTransparent.png/198px-BITPlanLogoFontLessTransparent.png" />](http://www.bitplan.com)
 # gremlin-python-tutorial
 Gremlin-Python tutorial
```

### Comparing `gremlin_python_tutorial-0.0.2/pyproject.toml` & `gremlin_python_tutorial-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.2/PKG-INFO` & `gremlin_python_tutorial-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlin-python-tutorial
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Home, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Gremlin_python
 Project-URL: Source, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Author-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -224,14 +224,16 @@
 Requires-Dist: graphviz>=0.20.1
 Requires-Dist: gremlinpython>=3.6.4
 Requires-Dist: pyyaml>=6.0
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
+[![pypi](https://img.shields.io/pypi/pyversions/gremlin-python-tutorial)](https://pypi.org/project/gremlin-python-tutorial/)
+[![PyPI Status](https://img.shields.io/pypi/v/gremlin-python-tutorial)](https://pypi.org/project/gremlin-python-tutorial/)
 [![Github Actions - build](https://github.com/WolfgangFahl/gremlin-python-tutorial/actions/workflows/build.yaml/badge.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/actions/workflows/build.yaml)
 [![GitHub issues](https://img.shields.io/github/issues/WolfgangFahl/gremlin-python-tutorial.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/issues)
 [![GitHub issues](https://img.shields.io/github/issues-closed/WolfgangFahl/gremlin-python-tutorial.svg)](https://github.com/WolfgangFahl/gremlin-python-tutorial/issues/?q=is%3Aissue+is%3Aclosed)
 [![GitHub](https://img.shields.io/github/license/WolfgangFahl/gremlin-python-tutorial.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [<img alt="BITPlan" width="8%" src="http://wiki.bitplan.com/images/wiki/thumb/3/38/BITPlanLogoFontLessTransparent.png/198px-BITPlanLogoFontLessTransparent.png" />](http://www.bitplan.com)
 # gremlin-python-tutorial
 Gremlin-Python tutorial
```

