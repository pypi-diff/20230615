# Comparing `tmp/simple_aws_rds-0.1.2.tar.gz` & `tmp/simple_aws_rds-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_rds-0.1.2.tar", last modified: Wed May  3 17:20:20 2023, max compression
+gzip compressed data, was "simple_aws_rds-0.2.1.tar", last modified: Thu Jun 15 19:39:49 2023, max compression
```

## Comparing `simple_aws_rds-0.1.2.tar` & `simple_aws_rds-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.413216 simple_aws_rds-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 17:20:20.413054 simple_aws_rds-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3657 2023-05-03 16:15:22.000000 simple_aws_rds-0.1.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      736 2023-05-03 17:19:59.000000 simple_aws_rds-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-05-03 15:59:50.000000 simple_aws_rds-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 15:36:24.000000 simple_aws_rds-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 17:20:20.413275 simple_aws_rds-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 15:36:40.000000 simple_aws_rds-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.409819 simple_aws_rds-0.1.2/simple_aws_rds/
--rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.1.2/simple_aws_rds/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 17:19:02.000000 simple_aws_rds-0.1.2/simple_aws_rds/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      122 2023-05-03 16:11:07.000000 simple_aws_rds-0.1.2/simple_aws_rds/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.411908 simple_aws_rds-0.1.2/simple_aws_rds/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.1.2/simple_aws_rds/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6040 2023-05-03 17:18:56.000000 simple_aws_rds-0.1.2/simple_aws_rds/rds.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.411754 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4721 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 17:20:20.000000 simple_aws_rds-0.1.2/simple_aws_rds.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:20:20.412560 simple_aws_rds-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.1.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2733 2023-05-03 16:16:00.000000 simple_aws_rds-0.1.2/tests/test_rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.945490 simple_aws_rds-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:21.000000 simple_aws_rds-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-15 19:39:49.945330 simple_aws_rds-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3833 2023-06-15 18:43:35.000000 simple_aws_rds-0.2.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1048 2023-06-15 18:59:50.000000 simple_aws_rds-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-15 16:48:33.000000 simple_aws_rds-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-15 16:48:10.000000 simple_aws_rds-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-15 19:39:49.945536 simple_aws_rds-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7563 2023-06-15 18:42:44.000000 simple_aws_rds-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.943403 simple_aws_rds-0.2.1/simple_aws_rds/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.2.1/simple_aws_rds/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 19:01:48.000000 simple_aws_rds-0.2.1/simple_aws_rds/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      122 2023-05-03 16:11:07.000000 simple_aws_rds-0.2.1/simple_aws_rds/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944151 simple_aws_rds-0.2.1/simple_aws_rds/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.2.1/simple_aws_rds/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    22301 2023-06-15 19:01:15.000000 simple_aws_rds-0.2.1/simple_aws_rds/rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944564 simple_aws_rds-0.2.1/simple_aws_rds/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_rds-0.2.1/simple_aws_rds/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_rds-0.2.1/simple_aws_rds/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.944031 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-15 19:39:49.000000 simple_aws_rds-0.2.1/simple_aws_rds.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 19:39:49.945010 simple_aws_rds-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3343 2023-06-15 19:00:20.000000 simple_aws_rds-0.2.1/tests/test_rds.py
```

### Comparing `simple_aws_rds-0.1.2/LICENSE.txt` & `simple_aws_rds-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.2/PKG-INFO` & `simple_aws_rds-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_rds
-Version: 0.1.2
+Version: 0.2.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -19,14 +19,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 
@@ -45,14 +46,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_rds-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_rds-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `simple_aws_rds-0.1.2/README.rst` & `simple_aws_rds-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_rds-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_rds-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `simple_aws_rds-0.1.2/requirements-doc.txt` & `simple_aws_rds-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.1.2/setup.py` & `simple_aws_rds-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ]
     """
     Full list can be found at: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     """
 
     def read_requirements_file(path):
```

### Comparing `simple_aws_rds-0.1.2/simple_aws_rds.egg-info/PKG-INFO` & `simple_aws_rds-0.2.1/simple_aws_rds.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-rds
-Version: 0.1.2
+Version: 0.2.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -19,14 +19,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 
@@ -45,14 +46,17 @@
 
 .. image:: https://img.shields.io/pypi/l/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
 .. image:: https://img.shields.io/pypi/pyversions/simple_aws_rds.svg
     :target: https://pypi.python.org/pypi/simple_aws_rds
 
+.. image:: https://img.shields.io/badge/Release_History!--None.svg?style=social
+    :target: https://github.com/MacHu-GWU/simple_aws_rds-project/blob/main/release-history.rst
+
 .. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
     :target: https://github.com/MacHu-GWU/simple_aws_rds-project
 
 ------
 
 
 .. .. image:: https://img.shields.io/badge/Link-Document-blue.svg
```

### Comparing `simple_aws_rds-0.1.2/tests/test_rds.py` & `simple_aws_rds-0.2.1/tests/test_rds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import pytest
 import moto
 from boto_session_manager import BotoSesManager
 
-from simple_aws_rds.rds import RDSDBInstance
+from simple_aws_rds.rds import RDSDBInstanceStatusEnum, RDSDBInstance
 
 
 class TestRds:
     mock_rds = None
     bsm: BotoSesManager = None
 
     @classmethod
@@ -42,48 +42,61 @@
 
     def _test(self):
         inst_id_list = [
             self.inst_id_1,
             self.inst_id_2,
         ]
         for inst_id in inst_id_list:
-            db_inst = RDSDBInstance.from_id(self.bsm, inst_id)
+            db_inst = RDSDBInstance.from_id(self.bsm.rds_client, inst_id)
             assert db_inst.is_available() is True
             assert db_inst.is_stopped() is False
             assert db_inst.is_ready_to_start() is False
             assert db_inst.is_ready_to_stop() is True
             assert db_inst.id == inst_id
 
-        db_inst_list = RDSDBInstance.query(self.bsm).all()
+        db_inst_list = RDSDBInstance.query(self.bsm.rds_client).all()
         assert len(db_inst_list) == 2
 
         db_inst_list = RDSDBInstance.from_tag_key_value(
-            self.bsm, key="Name", value="my-db"
+            self.bsm.rds_client, key="Name", value="my-db"
         ).all()
         assert len(db_inst_list) == 1
         db_inst = db_inst_list[0]
         assert db_inst.id == self.inst_id_2
         assert db_inst.tags["Name"] == "my-db"
 
-        db_inst = RDSDBInstance.from_id(self.bsm, self.inst_id_1)
-        db_inst.stop_db_instance(self.bsm)
-        db_inst = RDSDBInstance.from_id(self.bsm, self.inst_id_1)
+        db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
+        db_inst.stop_db_instance(self.bsm.rds_client)
+        db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
         assert db_inst.is_available() is False
         assert db_inst.is_stopped() is True
 
-        db_inst.start_db_instance(self.bsm)
-        db_inst = RDSDBInstance.from_id(self.bsm, self.inst_id_1)
+        db_inst.start_db_instance(self.bsm.rds_client)
+        db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
         assert db_inst.is_stopped() is False
         assert db_inst.is_available() is True
 
         db_inst_list = RDSDBInstance.from_tag_key_value(
-            self.bsm, key="Env", value="sandbox"
+            self.bsm.rds_client, key="Env", value="sandbox"
         ).all()
         assert len(db_inst_list) == 0
 
+    def _test_wait_for_status(self):
+        db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
+        assert db_inst.is_available() is True
+
+        db_inst.stop_db_instance(self.bsm.rds_client)
+        new_db_inst = db_inst.wait_for_status(
+            rds_client=self.bsm.rds_client,
+            stop_status=RDSDBInstanceStatusEnum.stopped,
+            verbose=False,
+        )
+        assert new_db_inst.is_stopped() is True
+
     def test(self):
         self._test()
+        self._test_wait_for_status()
 
 
 if __name__ == "__main__":
     basename = os.path.basename(__file__)
     pytest.main([basename, "-s", "--tb=native"])
```

