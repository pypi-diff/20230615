# Comparing `tmp/ayeaye-0.0.8.tar.gz` & `tmp/ayeaye-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/si/Documents/Progressive Logic/ContractData/Aye-Aye-Dev/AyeAye/dist/tmp0ott7gn0/ayeaye-0.0.8.tar", last modified: Tue Jun 29 14:25:47 2021, max compression
+gzip compressed data, was "/Users/si/Documents/Progressive Logic/ContractData/Aye-Aye-Dev/AyeAye/dist/tmpv6uqyy9s/ayeaye-0.0.9.tar", last modified: Wed Jun 30 16:49:18 2021, max compression
```

## Comparing `ayeaye-0.0.8.tar` & `ayeaye-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.967713 ayeaye-0.0.8/
--rw-r--r--   0 si         (501) staff       (20)    11357 2019-12-31 16:41:28.000000 ayeaye-0.0.8/LICENSE
--rw-r--r--   0 si         (501) staff       (20)      221 2020-01-21 12:18:40.000000 ayeaye-0.0.8/NOTICE
--rw-r--r--   0 si         (501) staff       (20)     3374 2021-06-29 14:25:47.967936 ayeaye-0.0.8/PKG-INFO
--rw-r--r--   0 si         (501) staff       (20)     2754 2021-06-29 14:09:43.000000 ayeaye-0.0.8/README.md
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.950382 ayeaye-0.0.8/lib/
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.954821 ayeaye-0.0.8/lib/ayeaye/
--rw-r--r--   0 si         (501) staff       (20)      263 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/__init__.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.957087 ayeaye-0.0.8/lib/ayeaye/common_pattern/
--rw-r--r--   0 si         (501) staff       (20)        0 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/common_pattern/__init__.py
--rw-r--r--   0 si         (501) staff       (20)    10763 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/common_pattern/manifest.py
--rw-r--r--   0 si         (501) staff       (20)    12356 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connect.py
--rw-r--r--   0 si         (501) staff       (20)    10369 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connect_resolve.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.967120 ayeaye-0.0.8/lib/ayeaye/connectors/
--rw-r--r--   0 si         (501) staff       (20)     2516 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     7369 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/base.py
--rw-r--r--   0 si         (501) staff       (20)     9173 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/bigquery.py
--rw-r--r--   0 si         (501) staff       (20)     6757 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/csv_connector.py
--rw-r--r--   0 si         (501) staff       (20)     4255 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/elasticsearch_connector.py
--rw-r--r--   0 si         (501) staff       (20)      774 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/fake.py
--rw-r--r--   0 si         (501) staff       (20)     4761 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/flowerpot.py
--rw-r--r--   0 si         (501) staff       (20)     3466 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/gcs_flowerpot.py
--rw-r--r--   0 si         (501) staff       (20)     4485 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/json_connector.py
--rw-r--r--   0 si         (501) staff       (20)    10054 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/kafka_connector.py
--rw-r--r--   0 si         (501) staff       (20)     6595 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/models_connector.py
--rw-r--r--   0 si         (501) staff       (20)     5162 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/multi_connector.py
--rw-r--r--   0 si         (501) staff       (20)     4259 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/ndjson_connector.py
--rw-r--r--   0 si         (501) staff       (20)     3648 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/parquet_connector.py
--rw-r--r--   0 si         (501) staff       (20)      646 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/placeholder.py
--rw-r--r--   0 si         (501) staff       (20)    10125 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/sqlalchemy_database.py
--rw-r--r--   0 si         (501) staff       (20)     4342 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/connectors/uncooked_connector.py
--rw-r--r--   0 si         (501) staff       (20)     4334 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/ignition.py
--rw-r--r--   0 si         (501) staff       (20)     9075 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/model.py
--rw-r--r--   0 si         (501) staff       (20)     5449 2021-06-29 14:01:34.000000 ayeaye-0.0.8/lib/ayeaye/pinnate.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-29 14:25:47.956298 ayeaye-0.0.8/lib/ayeaye.egg-info/
--rw-r--r--   0 si         (501) staff       (20)     3374 2021-06-29 14:25:47.000000 ayeaye-0.0.8/lib/ayeaye.egg-info/PKG-INFO
--rw-r--r--   0 si         (501) staff       (20)     1066 2021-06-29 14:25:47.000000 ayeaye-0.0.8/lib/ayeaye.egg-info/SOURCES.txt
--rw-r--r--   0 si         (501) staff       (20)        1 2021-06-29 14:25:47.000000 ayeaye-0.0.8/lib/ayeaye.egg-info/dependency_links.txt
--rw-r--r--   0 si         (501) staff       (20)        7 2021-06-29 14:25:47.000000 ayeaye-0.0.8/lib/ayeaye.egg-info/top_level.txt
--rw-r--r--   0 si         (501) staff       (20)      104 2021-06-03 13:41:58.000000 ayeaye-0.0.8/pyproject.toml
--rw-r--r--   0 si         (501) staff       (20)      676 2021-06-29 14:25:47.969085 ayeaye-0.0.8/setup.cfg
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.152500 ayeaye-0.0.9/
+-rw-r--r--   0 si         (501) staff       (20)    11357 2019-12-31 16:41:28.000000 ayeaye-0.0.9/LICENSE
+-rw-r--r--   0 si         (501) staff       (20)      221 2020-01-21 12:18:40.000000 ayeaye-0.0.9/NOTICE
+-rw-r--r--   0 si         (501) staff       (20)     3402 2021-06-30 16:49:18.152792 ayeaye-0.0.9/PKG-INFO
+-rw-r--r--   0 si         (501) staff       (20)     2782 2021-06-29 19:37:30.000000 ayeaye-0.0.9/README.md
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.129773 ayeaye-0.0.9/lib/
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.135196 ayeaye-0.0.9/lib/ayeaye/
+-rw-r--r--   0 si         (501) staff       (20)      281 2021-06-30 13:49:50.000000 ayeaye-0.0.9/lib/ayeaye/__init__.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.138587 ayeaye-0.0.9/lib/ayeaye/common_pattern/
+-rw-r--r--   0 si         (501) staff       (20)        0 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/common_pattern/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)    10763 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/common_pattern/manifest.py
+-rw-r--r--   0 si         (501) staff       (20)    12356 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connect.py
+-rw-r--r--   0 si         (501) staff       (20)    10369 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connect_resolve.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.151855 ayeaye-0.0.9/lib/ayeaye/connectors/
+-rw-r--r--   0 si         (501) staff       (20)     2516 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     7369 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/base.py
+-rw-r--r--   0 si         (501) staff       (20)     9173 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/bigquery.py
+-rw-r--r--   0 si         (501) staff       (20)     6757 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/csv_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     4255 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/elasticsearch_connector.py
+-rw-r--r--   0 si         (501) staff       (20)      774 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/fake.py
+-rw-r--r--   0 si         (501) staff       (20)     4761 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/flowerpot.py
+-rw-r--r--   0 si         (501) staff       (20)     3466 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/gcs_flowerpot.py
+-rw-r--r--   0 si         (501) staff       (20)     4485 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/json_connector.py
+-rw-r--r--   0 si         (501) staff       (20)    10054 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/kafka_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     6595 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/models_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     5162 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/multi_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     4259 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/ndjson_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     3648 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/parquet_connector.py
+-rw-r--r--   0 si         (501) staff       (20)      646 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/placeholder.py
+-rw-r--r--   0 si         (501) staff       (20)    10125 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/sqlalchemy_database.py
+-rw-r--r--   0 si         (501) staff       (20)     4342 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/connectors/uncooked_connector.py
+-rw-r--r--   0 si         (501) staff       (20)     4334 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/ignition.py
+-rw-r--r--   0 si         (501) staff       (20)    13347 2021-06-30 16:47:26.000000 ayeaye-0.0.9/lib/ayeaye/model.py
+-rw-r--r--   0 si         (501) staff       (20)     5449 2021-06-29 14:01:34.000000 ayeaye-0.0.9/lib/ayeaye/pinnate.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2021-06-30 16:49:18.137504 ayeaye-0.0.9/lib/ayeaye.egg-info/
+-rw-r--r--   0 si         (501) staff       (20)     3402 2021-06-30 16:49:18.000000 ayeaye-0.0.9/lib/ayeaye.egg-info/PKG-INFO
+-rw-r--r--   0 si         (501) staff       (20)     1066 2021-06-30 16:49:18.000000 ayeaye-0.0.9/lib/ayeaye.egg-info/SOURCES.txt
+-rw-r--r--   0 si         (501) staff       (20)        1 2021-06-30 16:49:18.000000 ayeaye-0.0.9/lib/ayeaye.egg-info/dependency_links.txt
+-rw-r--r--   0 si         (501) staff       (20)        7 2021-06-30 16:49:18.000000 ayeaye-0.0.9/lib/ayeaye.egg-info/top_level.txt
+-rw-r--r--   0 si         (501) staff       (20)      104 2021-06-03 13:41:58.000000 ayeaye-0.0.9/pyproject.toml
+-rw-r--r--   0 si         (501) staff       (20)      676 2021-06-30 16:49:18.154225 ayeaye-0.0.9/setup.cfg
```

### Comparing `ayeaye-0.0.8/LICENSE` & `ayeaye-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/PKG-INFO` & `ayeaye-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayeaye
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ETL (Extract, Transform, Load) framework
 Home-page: https://github.com/Aye-Aye-Dev/AyeAye
 Author: Si Parker
 Author-email: ayeaye@plogic.co.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Aye-Aye-Dev/AyeAye/issues
 Platform: UNKNOWN
@@ -75,14 +75,15 @@
 
 
 ## Unit tests
 
 Ensure the working directory is the base Aye Aye directory (i.e. the same directory as the Pipfile):
 ```shell
 pipenv install --dev
+export PYTHONPATH=`pwd`/lib
 pipenv run python -m unittest discover
 ```
 
 ## Development version
 
 To use the latest code in editable mode-
```

### Comparing `ayeaye-0.0.8/README.md` & `ayeaye-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 
 ## Unit tests
 
 Ensure the working directory is the base Aye Aye directory (i.e. the same directory as the Pipfile):
 ```shell
 pipenv install --dev
+export PYTHONPATH=`pwd`/lib
 pipenv run python -m unittest discover
 ```
 
 ## Development version
 
 To use the latest code in editable mode-
```

### Comparing `ayeaye-0.0.8/lib/ayeaye/common_pattern/manifest.py` & `ayeaye-0.0.9/lib/ayeaye/common_pattern/manifest.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connect.py` & `ayeaye-0.0.9/lib/ayeaye/connect.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connect_resolve.py` & `ayeaye-0.0.9/lib/ayeaye/connect_resolve.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/__init__.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/base.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/base.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/bigquery.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/csv_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/csv_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/elasticsearch_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/fake.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/fake.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/flowerpot.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/flowerpot.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/gcs_flowerpot.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/gcs_flowerpot.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/json_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/json_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/kafka_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/models_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/models_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/multi_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/multi_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/ndjson_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/ndjson_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/parquet_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/parquet_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/placeholder.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/placeholder.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/sqlalchemy_database.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/sqlalchemy_database.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/connectors/uncooked_connector.py` & `ayeaye-0.0.9/lib/ayeaye/connectors/uncooked_connector.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/ignition.py` & `ayeaye-0.0.9/lib/ayeaye/ignition.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye/pinnate.py` & `ayeaye-0.0.9/lib/ayeaye/pinnate.py`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/lib/ayeaye.egg-info/PKG-INFO` & `ayeaye-0.0.9/lib/ayeaye.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayeaye
-Version: 0.0.8
+Version: 0.0.9
 Summary: An ETL (Extract, Transform, Load) framework
 Home-page: https://github.com/Aye-Aye-Dev/AyeAye
 Author: Si Parker
 Author-email: ayeaye@plogic.co.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Aye-Aye-Dev/AyeAye/issues
 Platform: UNKNOWN
@@ -75,14 +75,15 @@
 
 
 ## Unit tests
 
 Ensure the working directory is the base Aye Aye directory (i.e. the same directory as the Pipfile):
 ```shell
 pipenv install --dev
+export PYTHONPATH=`pwd`/lib
 pipenv run python -m unittest discover
 ```
 
 ## Development version
 
 To use the latest code in editable mode-
```

### Comparing `ayeaye-0.0.8/lib/ayeaye.egg-info/SOURCES.txt` & `ayeaye-0.0.9/lib/ayeaye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayeaye-0.0.8/setup.cfg` & `ayeaye-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ayeaye
-version = 0.0.8
+version = 0.0.9
 author = Si Parker
 author_email = ayeaye@plogic.co.uk
 description = An ETL (Extract, Transform, Load) framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Aye-Aye-Dev/AyeAye
 project_urls =
```

