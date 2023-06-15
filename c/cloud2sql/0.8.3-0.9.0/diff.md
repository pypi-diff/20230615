# Comparing `tmp/cloud2sql-0.8.3.tar.gz` & `tmp/cloud2sql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud2sql-0.8.3.tar", last modified: Tue May 23 16:21:14 2023, max compression
+gzip compressed data, was "cloud2sql-0.9.0.tar", last modified: Thu Jun 15 07:56:27 2023, max compression
```

## Comparing `cloud2sql-0.8.3.tar` & `cloud2sql-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.370772 cloud2sql-0.8.3/cloud2sql/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/cloud2sql/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/remote_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/cloud2sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/cloud2sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 16:21:14.000000 cloud2sql-0.8.3/cloud2sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-parquet.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-snowflake.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 16:21:14.374772 cloud2sql-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-23 16:17:42.000000 cloud2sql-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:56:27.254089 cloud2sql-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-15 07:56:27.254089 cloud2sql-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:56:27.250089 cloud2sql-0.9.0/cloud2sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/cloud2sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/cloud2sql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/cloud2sql/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/cloud2sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:56:27.254089 cloud2sql-0.9.0/cloud2sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 07:56:27.000000 cloud2sql-0.9.0/cloud2sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements-mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements-parquet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements-postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements-snowflake.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 07:56:27.254089 cloud2sql-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-15 07:53:01.000000 cloud2sql-0.9.0/setup.py
```

### Comparing `cloud2sql-0.8.3/LICENSE` & `cloud2sql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.3/PKG-INFO` & `cloud2sql-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.3
+Version: 0.9.0
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
@@ -42,15 +42,15 @@
 ```
 
 This will install the executable to the user install directory of your platform. Please make sure this installation directory is listed in `PATH`.
 
 
 ## Usage
 
-The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](./config-template.yaml).
+The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](config-template.yaml).
 
 You can safely delete the sections that are not relevant to you (e.g. if you do not use AWS, you can delete the `aws` section).
 All sections refer to cloud providers and are enabled if a configuration section is provided.
 
 In the next section you will create a YAML configuration file. Once you have created your configuration file, you can run `cloud2sql` with the following command:
 
 ```bash
@@ -117,19 +117,19 @@
     configs: []
 ```
 
 #### DigitalOcean
 
 ```yaml
 sources:
-digitalocean:
-  # DigitalOcean API tokens for the teams to be collected
-  api_tokens: []
-  # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
-  spaces_access_keys: []
+  digitalocean:
+    # DigitalOcean API tokens for the teams to be collected
+    api_tokens: []
+    # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
+    spaces_access_keys: []
 ```
 
 ### Destinations
 
 #### SQLite
 
 ```yaml
@@ -238,15 +238,15 @@
 #### My database is not listed here
 
 Cloud2SQL uses SQLAlchemy to connect to the database. If your database is not listed here, you can check if it is supported in [SQLAlchemy Dialects](https://docs.sqlalchemy.org/en/20/dialects/index.html).
 Install the relevant driver and use the connection string from the documentation.
 
 #### Example
 
-We use a minimal configuration [example](./config-example.yaml) and export the data to a SQLite database.
+We use a minimal configuration [example](config-example.yaml) and export the data to a SQLite database.
 The example uses our AWS default credentials and the default kubernetes config.
 
 ```bash
 cloud2sql --config config-example.yaml
 ```
 
 For a more in-depth example, check out our [blog post](https://resoto.com/blog/2022/12/21/installing-cloud2sql).
```

### Comparing `cloud2sql-0.8.3/README.md` & `cloud2sql-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```
 
 This will install the executable to the user install directory of your platform. Please make sure this installation directory is listed in `PATH`.
 
 
 ## Usage
 
-The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](./config-template.yaml).
+The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](config-template.yaml).
 
 You can safely delete the sections that are not relevant to you (e.g. if you do not use AWS, you can delete the `aws` section).
 All sections refer to cloud providers and are enabled if a configuration section is provided.
 
 In the next section you will create a YAML configuration file. Once you have created your configuration file, you can run `cloud2sql` with the following command:
 
 ```bash
@@ -100,19 +100,19 @@
     configs: []
 ```
 
 #### DigitalOcean
 
 ```yaml
 sources:
-digitalocean:
-  # DigitalOcean API tokens for the teams to be collected
-  api_tokens: []
-  # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
-  spaces_access_keys: []
+  digitalocean:
+    # DigitalOcean API tokens for the teams to be collected
+    api_tokens: []
+    # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
+    spaces_access_keys: []
 ```
 
 ### Destinations
 
 #### SQLite
 
 ```yaml
@@ -221,15 +221,15 @@
 #### My database is not listed here
 
 Cloud2SQL uses SQLAlchemy to connect to the database. If your database is not listed here, you can check if it is supported in [SQLAlchemy Dialects](https://docs.sqlalchemy.org/en/20/dialects/index.html).
 Install the relevant driver and use the connection string from the documentation.
 
 #### Example
 
-We use a minimal configuration [example](./config-example.yaml) and export the data to a SQLite database.
+We use a minimal configuration [example](config-example.yaml) and export the data to a SQLite database.
 The example uses our AWS default credentials and the default kubernetes config.
 
 ```bash
 cloud2sql --config config-example.yaml
 ```
 
 For a more in-depth example, check out our [blog post](https://resoto.com/blog/2022/12/21/installing-cloud2sql).
```

### Comparing `cloud2sql-0.8.3/cloud2sql/__main__.py` & `cloud2sql-0.9.0/cloud2sql/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import yaml
 from resotolib.args import Namespace, ArgumentParser
 from resotolib.logger import setup_logger
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 
 from cloud2sql import __version__
-from cloud2sql.analytics import PosthogEventSender, NoEventSender, AnalyticsEventSender
-from cloud2sql.collect_plugins import collect_from_plugins, configure, default_config
+from resotodatalink.analytics import PosthogEventSender, NoEventSender, AnalyticsEventSender
+from cloud2sql.collect import collect_from_plugins, configure, default_config
 from cloud2sql.util import db_string_from_config, check_parquet_driver
 
 # Will fail in case snowflake is not installed - which is fine.
 try:
     from cloud2sql.snowflake import SnowflakeUpdater  # noqa:F401
 except ImportError:
     pass
```

### Comparing `cloud2sql-0.8.3/cloud2sql/util.py` & `cloud2sql-0.9.0/cloud2sql/util.py`

 * *Files identical despite different names*

### Comparing `cloud2sql-0.8.3/cloud2sql.egg-info/PKG-INFO` & `cloud2sql-0.9.0/cloud2sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud2sql
-Version: 0.8.3
+Version: 0.9.0
 Summary: Read infrastructure data from your cloud and export it to a SQL database.
 Home-page: https://github.com/someengineering/cloud2sql
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
@@ -42,15 +42,15 @@
 ```
 
 This will install the executable to the user install directory of your platform. Please make sure this installation directory is listed in `PATH`.
 
 
 ## Usage
 
-The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](./config-template.yaml).
+The sources and destinations for `cloud2sql` are configured via a configuration file. Create your own configuration by adjusting the [config template file](config-template.yaml).
 
 You can safely delete the sections that are not relevant to you (e.g. if you do not use AWS, you can delete the `aws` section).
 All sections refer to cloud providers and are enabled if a configuration section is provided.
 
 In the next section you will create a YAML configuration file. Once you have created your configuration file, you can run `cloud2sql` with the following command:
 
 ```bash
@@ -117,19 +117,19 @@
     configs: []
 ```
 
 #### DigitalOcean
 
 ```yaml
 sources:
-digitalocean:
-  # DigitalOcean API tokens for the teams to be collected
-  api_tokens: []
-  # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
-  spaces_access_keys: []
+  digitalocean:
+    # DigitalOcean API tokens for the teams to be collected
+    api_tokens: []
+    # DigitalOcean Spaces access keys for the teams to be collected, separated by colons
+    spaces_access_keys: []
 ```
 
 ### Destinations
 
 #### SQLite
 
 ```yaml
@@ -238,15 +238,15 @@
 #### My database is not listed here
 
 Cloud2SQL uses SQLAlchemy to connect to the database. If your database is not listed here, you can check if it is supported in [SQLAlchemy Dialects](https://docs.sqlalchemy.org/en/20/dialects/index.html).
 Install the relevant driver and use the connection string from the documentation.
 
 #### Example
 
-We use a minimal configuration [example](./config-example.yaml) and export the data to a SQLite database.
+We use a minimal configuration [example](config-example.yaml) and export the data to a SQLite database.
 The example uses our AWS default credentials and the default kubernetes config.
 
 ```bash
 cloud2sql --config config-example.yaml
 ```
 
 For a more in-depth example, check out our [blog post](https://resoto.com/blog/2022/12/21/installing-cloud2sql).
```

### Comparing `cloud2sql-0.8.3/setup.py` & `cloud2sql-0.9.0/setup.py`

 * *Files identical despite different names*

