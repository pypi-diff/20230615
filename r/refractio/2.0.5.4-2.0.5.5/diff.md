# Comparing `tmp/refractio-2.0.5.4.tar.gz` & `tmp/refractio-2.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.4.tar", last modified: Wed Jun 14 18:03:20 2023, max compression
+gzip compressed data, was "refractio-2.0.5.5.tar", last modified: Thu Jun 15 18:11:03 2023, max compression
```

## Comparing `refractio-2.0.5.4.tar` & `refractio-2.0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 18:03:20.688806 refractio-2.0.5.4/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-14 18:03:20.688806 refractio-2.0.5.4/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-14 14:53:40.000000 refractio-2.0.5.4/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 18:03:20.686806 refractio-2.0.5.4/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-14 13:25:53.000000 refractio-2.0.5.4/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4797 2023-06-14 14:53:40.000000 refractio-2.0.5.4/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16636 2023-06-14 17:59:29.000000 refractio-2.0.5.4/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.4/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 18:03:20.688806 refractio-2.0.5.4/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-14 18:03:20.000000 refractio-2.0.5.4/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-14 18:03:20.000000 refractio-2.0.5.4/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-14 18:03:20.000000 refractio-2.0.5.4/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-14 18:03:20.000000 refractio-2.0.5.4/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-14 18:03:20.000000 refractio-2.0.5.4/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-14 18:03:20.688806 refractio-2.0.5.4/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-14 18:01:03.000000 refractio-2.0.5.4/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.984468 refractio-2.0.5.5/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-15 18:11:03.984468 refractio-2.0.5.5/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-14 14:53:40.000000 refractio-2.0.5.5/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.982468 refractio-2.0.5.5/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-14 13:25:53.000000 refractio-2.0.5.5/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-15 18:10:28.000000 refractio-2.0.5.5/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16632 2023-06-15 18:10:28.000000 refractio-2.0.5.5/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.5/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-15 18:11:03.984468 refractio-2.0.5.5/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-15 18:11:03.000000 refractio-2.0.5.5/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-15 18:11:03.984468 refractio-2.0.5.5/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-15 18:10:28.000000 refractio-2.0.5.5/setup.py
```

### Comparing `refractio-2.0.5.4/PKG-INFO` & `refractio-2.0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.4
+Version: 2.0.5.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.4/README.md` & `refractio-2.0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/amazons3.py` & `refractio-2.0.5.5/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/azure.py` & `refractio-2.0.5.5/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/hive.py` & `refractio-2.0.5.5/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/manager.py` & `refractio-2.0.5.5/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/mysql.py` & `refractio-2.0.5.5/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/postgres.py` & `refractio-2.0.5.5/refractio/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
-            query = get_dataframe_query(f"{self.__connection_details['params']['READER']['database']}."
+            query = get_dataframe_query(f"{self.__connection_details['params']['READER']['schema']}."
                                         f"{self.__connection_details['params']['READER']['tables']}",
                                         row_count, filter_condition)     # Get query to fetch details
 
             data_frame = sqlio.read_sql_query(query, con=self.con_obj)   # Read data from postgres
 
             self.con_obj.close()    # Closing the connection used for reading dataset.
             return data_frame
```

### Comparing `refractio-2.0.5.4/refractio/refractio.py` & `refractio-2.0.5.5/refractio/refractio.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,17 +247,17 @@
                             port=int(connection_details["params"]["READER"]["port"]),
                             user=connection_details["params"]["READER"]["user"],
                             password=connection_details["params"]["READER"]["password"],
                             database=connection_details["params"]["READER"]["database"])
 
     if int(row_count) > 0:
         # Generate query
-        query = f"SELECT * FROM {connection_details['params']['READER']['database']}.{connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
+        query = f"SELECT * FROM {connection_details['params']['READER']['schema']}.{connection_details['params']['READER']['tables']} LIMIT {int(row_count)}"
     else:
-        query = f"SELECT * FROM {connection_details['params']['READER']['database']}.{connection_details['params']['READER']['tables']}"
+        query = f"SELECT * FROM {connection_details['params']['READER']['schema']}.{connection_details['params']['READER']['tables']}"
     # Read data fromm postgres
     data_frame = sqlio.read_sql_query(query, con=conn)
     # Close connection
     conn.close()
     return data_frame
```

### Comparing `refractio-2.0.5.4/refractio/sftp.py` & `refractio-2.0.5.5/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/snowflake.py` & `refractio-2.0.5.5/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio/sqlserver.py` & `refractio-2.0.5.5/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.5/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.4
+Version: 2.0.5.5
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.4/refractio.egg-info/requires.txt` & `refractio-2.0.5.5/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.4/setup.py` & `refractio-2.0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.4'
+VERSION = '2.0.5.5'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

