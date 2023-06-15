# Comparing `tmp/ALMAFE-Lib-0.0.8.tar.gz` & `tmp/ALMAFE-Lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ALMAFE-Lib-0.0.8.tar", last modified: Fri Dec 17 16:48:11 2021, max compression
+gzip compressed data, was "dist\ALMAFE-Lib-0.0.9.tar", last modified: Thu Jan 20 21:47:36 2022, max compression
```

## Comparing `ALMAFE-Lib-0.0.8.tar` & `ALMAFE-Lib-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:11.000000 ALMAFE-Lib-0.0.8/
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/
--rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.8/ALMAFE/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/basic/
--rw-rw-rw-   0        0        0     3490 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/basic/ParseTimeStamp.py
--rw-rw-rw-   0        0        0      276 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/basic/StripQuotes.py
--rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.8/ALMAFE/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/common/
--rw-rw-rw-   0        0        0      896 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/common/GitVersion.py
--rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.8/ALMAFE/common/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/database/
--rw-rw-rw-   0        0        0     4608 2021-11-17 17:06:01.000000 ALMAFE-Lib-0.0.8/ALMAFE/database/DriverMySQL.py
--rw-rw-rw-   0        0        0     4628 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/database/DriverOracle.py
--rw-rw-rw-   0        0        0     2621 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/database/DriverSQLite.py
--rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.8/ALMAFE/database/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/
--rw-rw-rw-   0        0        0     3647 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/NWayTree.py
--rw-rw-rw-   0        0        0        0 2021-02-16 21:19:03.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/test/
--rw-rw-rw-   0        0        0        0 2021-02-16 21:19:03.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/test/__init__.py
--rw-rw-rw-   0        0        0     1724 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/ALMAFE/datastruct/test/t_NWayTree.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE/tests/
--rw-rw-rw-   0        0        0        0 2021-02-16 21:19:02.000000 ALMAFE-Lib-0.0.8/ALMAFE/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-17 16:48:11.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/
--rw-rw-rw-   0        0        0     1573 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-12-17 16:48:10.000000 ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      571 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1573 2021-12-17 16:48:11.000000 ALMAFE-Lib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      970 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-12-17 16:48:11.000000 ALMAFE-Lib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      895 2021-12-17 16:44:41.000000 ALMAFE-Lib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/
+-rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.9/ALMAFE/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/basic/
+-rw-rw-rw-   0        0        0     3490 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/basic/ParseTimeStamp.py
+-rw-rw-rw-   0        0        0      276 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/basic/StripQuotes.py
+-rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.9/ALMAFE/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/common/
+-rw-rw-rw-   0        0        0      896 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/common/GitVersion.py
+-rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.9/ALMAFE/common/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/database/
+-rw-rw-rw-   0        0        0     4835 2022-01-05 21:49:58.000000 ALMAFE-Lib-0.0.9/ALMAFE/database/DriverMySQL.py
+-rw-rw-rw-   0        0        0     4628 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/database/DriverOracle.py
+-rw-rw-rw-   0        0        0     2621 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/database/DriverSQLite.py
+-rw-rw-rw-   0        0        0        0 2020-12-16 19:28:58.000000 ALMAFE-Lib-0.0.9/ALMAFE/database/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/
+-rw-rw-rw-   0        0        0     3647 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/NWayTree.py
+-rw-rw-rw-   0        0        0        0 2021-02-16 21:19:03.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/test/
+-rw-rw-rw-   0        0        0        0 2021-02-16 21:19:03.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/test/__init__.py
+-rw-rw-rw-   0        0        0     1724 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/ALMAFE/datastruct/test/t_NWayTree.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE/tests/
+-rw-rw-rw-   0        0        0        0 2021-02-16 21:19:02.000000 ALMAFE-Lib-0.0.9/ALMAFE/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/
+-rw-rw-rw-   0        0        0     1573 2022-01-20 21:47:33.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2022-01-20 21:47:33.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-20 21:47:33.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2022-01-20 21:47:33.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-01-20 21:47:33.000000 ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      571 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1573 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      970 2021-10-25 21:19:11.000000 ALMAFE-Lib-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-01-20 21:47:36.000000 ALMAFE-Lib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      895 2022-01-20 21:23:26.000000 ALMAFE-Lib-0.0.9/setup.py
```

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/basic/ParseTimeStamp.py` & `ALMAFE-Lib-0.0.9/ALMAFE/basic/ParseTimeStamp.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/common/GitVersion.py` & `ALMAFE-Lib-0.0.9/ALMAFE/common/GitVersion.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/database/DriverMySQL.py` & `ALMAFE-Lib-0.0.9/ALMAFE/database/DriverMySQL.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Driver wrapper for mysql-connector-python
 '''
 import mysql.connector
-from mysql.connector import Error, InterfaceError
+from mysql.connector import Error
 
 class DriverMySQL():
     '''
     Driver wrapper for mysql-connector-python
     Provides a uniform interface to SQL user code
     '''
     TIMESTAMP_FORMAT = '%Y-%m-%d %H:%M:%S'
@@ -56,36 +56,44 @@
     def execute(self, query, params = None, commit = False, reconnect = True):
         '''
         Execute an SQL query.
         :param query: str
         :param params: tuple or dictionary params are bound to the variables in the operation. 
                        Specify variables using %s or %(name)s parameter style (that is, using format or pyformat style).
         :param commit: If True, commit INSERT/UPDATE/DELETE queries immediately.
+        :param reconnect: If True and the connection seems to have gone away, reconnect and retry the query.
         :return True/False
         '''
+        doRetry = False
         try:
-            try:
-                self.cursor.execute(query, params)                
-            # if we should reconnect:
-            except InterfaceError as e:
-                if not reconnect:
-                    raise 
-                # this calls reconnect() internally:
-                self.connection.ping(reconnect = True, attempts = 2)
-                # get the cursor again:
-                self.cursor = self.connection.cursor()
-                # and retry the query:
-                self.cursor.execute(query, params)
+            self.cursor.execute(query, params)
             if commit:
                 self.connection.commit()
-            return True
         except Error as e:
-            print(f"MySQL error: {e}")
-            print(query)
-            return False
+            if not reconnect:
+                print(f"MySQL error: {e}")
+                print(query)
+                return False
+            # this calls reconnect() internally:
+            self.connection.ping(reconnect = True, attempts = 2)
+            # get the cursor again:
+            self.cursor = self.connection.cursor()
+            doRetry = True
+
+        if doRetry:
+            # and retry the query
+            try:
+                self.cursor.execute(query, params)
+                if commit:
+                    self.connection.commit()
+            except Error as e:
+                print(f"MySQL error: {e}")
+                print(query)
+                return False
+        return True
     
     def commit(self):
         '''
         Commit any previously executed but not yet committed INSERT/UPDATE/DELETE queries.
         :return True/False
         '''
         try:
```

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/database/DriverOracle.py` & `ALMAFE-Lib-0.0.9/ALMAFE/database/DriverOracle.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/database/DriverSQLite.py` & `ALMAFE-Lib-0.0.9/ALMAFE/database/DriverSQLite.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/datastruct/NWayTree.py` & `ALMAFE-Lib-0.0.9/ALMAFE/datastruct/NWayTree.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE/datastruct/test/t_NWayTree.py` & `ALMAFE-Lib-0.0.9/ALMAFE/datastruct/test/t_NWayTree.py`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/PKG-INFO` & `ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMAFE-Lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains reusable tools which are required by other ALMAFE packages.
 Home-page: https://github.com/morganmcleod/ALMAFE-Lib
 Author: Morgan McLeod
 Author-email: mmcleod@nrao.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ALMAFE-Lib-0.0.8/ALMAFE_Lib.egg-info/SOURCES.txt` & `ALMAFE-Lib-0.0.9/ALMAFE_Lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/LICENSE` & `ALMAFE-Lib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/PKG-INFO` & `ALMAFE-Lib-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMAFE-Lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains reusable tools which are required by other ALMAFE packages.
 Home-page: https://github.com/morganmcleod/ALMAFE-Lib
 Author: Morgan McLeod
 Author-email: mmcleod@nrao.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ALMAFE-Lib-0.0.8/README.md` & `ALMAFE-Lib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ALMAFE-Lib-0.0.8/setup.py` & `ALMAFE-Lib-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ALMAFE-Lib",
-    version="0.0.8",
+    version="0.0.9",
     author="Morgan McLeod",
     author_email="mmcleod@nrao.edu",
     description="Contains reusable tools which are required by other ALMAFE packages.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/morganmcleod/ALMAFE-Lib",
     packages=setuptools.find_packages(),
```

