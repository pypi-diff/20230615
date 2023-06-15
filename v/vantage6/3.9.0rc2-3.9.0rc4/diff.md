# Comparing `tmp/vantage6-3.9.0rc2.tar.gz` & `tmp/vantage6-3.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-3.9.0rc2.tar", last modified: Tue May  9 13:37:05 2023, max compression
+gzip compressed data, was "vantage6-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
```

## Comparing `vantage6-3.9.0rc2.tar` & `vantage6-3.9.0rc4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.322882 vantage6-3.9.0rc2/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    37859 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.330882 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    29886 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-09 13:36:37.000000 vantage6-3.9.0rc2/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.326882 vantage6-3.9.0rc2/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 13:37:05.000000 vantage6-3.9.0rc2/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37859 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.521727 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    29887 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-24 09:33:56.000000 vantage6-3.9.0rc4/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.517727 vantage6-3.9.0rc4/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 09:34:09.000000 vantage6-3.9.0rc4/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-3.9.0rc2/PKG-INFO` & `vantage6-3.9.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc2 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc4 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-3.9.0rc2/setup.py` & `vantage6-3.9.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_description_content_type="text/markdown",
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'click==8.1.3',
         'colorama==0.4.6',
-        'docker==6.0.1',
+        'docker==6.1.2',
         'ipython==8.10.0',
         'questionary==1.10.0',
         'schema==0.7.5',
         'SQLAlchemy==1.4.46',
         f'vantage6-common == {version_ns["__version__"]}',
         f'vantage6-client == {version_ns["__version__"]}',
     ],
```

### Comparing `vantage6-3.9.0rc2/tests_cli/test_node_cli.py` & `vantage6-3.9.0rc4/tests_cli/test_node_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/tests_cli/test_server_cli.py` & `vantage6-3.9.0rc4/tests_cli/test_server_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/tests_cli/test_wizard.py` & `vantage6-3.9.0rc4/tests_cli/test_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/_version.py` & `vantage6-3.9.0rc4/vantage6/cli/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/configuration_manager.py` & `vantage6-3.9.0rc4/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/configuration_wizard.py` & `vantage6-3.9.0rc4/vantage6/cli/configuration_wizard.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,22 @@
 
     config["logging"] = {
         "level": res,
         "use_console": True,
         "backup_count": 5,
         "max_size": 1024,
         "format": "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s",
-        "datefmt": "%Y-%m-%d %H:%M:%S"
+        "datefmt": "%Y-%m-%d %H:%M:%S",
+        "loggers": [
+            {"name": "urllib3", "level": "warning"},
+            {"name": "requests", "level": "warning"},
+            {"name": "engineio.client", "level": "warning"},
+            {"name": "docker.utils.config", "level": "warning"},
+            {"name": "docker.auth", "level": "warning"},
+        ]
     }
 
     encryption = q.confirm("Enable encryption?", default=True).ask()
 
     private_key = "" if not encryption else \
         q.text("Path to private key file:").ask()
 
@@ -236,15 +243,23 @@
     config["logging"] = {
         "level": res,
         "file": f"{instance_name}.log",
         "use_console": True,
         "backup_count": 5,
         "max_size": 1024,
         "format": "%(asctime)s - %(name)-14s - %(levelname)-8s - %(message)s",
-        "datefmt": "%Y-%m-%d %H:%M:%S"
+        "datefmt": "%Y-%m-%d %H:%M:%S",
+        "loggers": [
+            {"name": "urllib3", "level": "warning"},
+            {"name": "socketIO-client", "level": "warning"},
+            {"name": "socketio.server", "level": "warning"},
+            {"name": "engineio.server", "level": "warning"},
+            {"name": "sqlalchemy.engine", "level": "warning"},
+            {"name": "requests_oauthlib.oauth2_session", "level": "warning"},
+        ]
     }
 
     return config
 
 
 def configuration_wizard(type_: str, instance_name: str, environment: str,
                          system_folders: bool) -> Path:
```

### Comparing `vantage6-3.9.0rc2/vantage6/cli/context.py` & `vantage6-3.9.0rc4/vantage6/cli/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,18 +76,26 @@
         -------
         str
             string representation of the database uri
         """
         uri = os.environ.get("VANTAGE6_DB_URI") or self.config['uri']
         url = make_url(uri)
 
-        if (url.host is None) and (not os.path.isabs(url.database)):
-            # We're dealing with a relative path here.
-            url.database = str(self.data_dir / url.database)
-            uri = str(url)
+        if url.host is None and not os.path.isabs(url.database):
+            # We're dealing with a relative path here of a local database, when
+            # we're running the server outside of docker. Therefore we need to
+            # prepend the data directory to the database name, but after the
+            # driver name (e.g. sqlite:////db.sqlite ->
+            # sqlite:////data_dir>/db.sqlite)
+
+            # find index of database name
+            idx_db_name = str(url).find(url.database)
+
+            # add the datadir to the right location in the database uri
+            return str(url)[:idx_db_name] + str(self.data_dir / url.database)
 
         return uri
 
     @property
     def docker_container_name(self) -> str:
         """
         Name of the docker container that the server is running in.
```

### Comparing `vantage6-3.9.0rc2/vantage6/cli/globals.py` & `vantage6-3.9.0rc4/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/node.py` & `vantage6-3.9.0rc4/vantage6/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/__init__.py` & `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/definitions.py` & `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-3.9.0rc4/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,19 @@
     """
     Manages the RabbitMQ docker container
 
     Parameters
     ----------
     ctx: ServerContext
         Configuration object
-    queue_uri: str
-        URI where the RabbitMQ instance should be running
     network_mgr: NetworkManager
         Network manager for network in which server container resides
+    image: str
+        Docker image to use for RabbitMQ container. By default, the image
+        harbor2.vantage6.ai/infrastructure/rabbitmq is used.
     """
     def __init__(self, ctx: ServerContext, network_mgr: NetworkManager,
                  image: str = None) -> None:
         self.ctx = ctx
         self.queue_uri = self.ctx.config.get('rabbitmq_uri')
         rabbit_splitted = split_rabbitmq_uri(self.queue_uri)
         self.rabbit_user = rabbit_splitted['user']
```

### Comparing `vantage6-3.9.0rc2/vantage6/cli/server.py` & `vantage6-3.9.0rc4/vantage6/cli/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         error(e)
         exit(1)
 
     # Check that we can write in this folder
     if not check_config_writeable(system_folders):
         error("Your user does not have write access to all folders. Exiting")
         info(f"Create a new server using '{Fore.GREEN}vserver new "
-             "--user{Style.RESET_ALL}' instead!")
+             f"--user{Style.RESET_ALL}' instead!")
         exit(1)
 
     # create config in ctx location
     cfg_file = configuration_wizard("server", name, environment=environment,
                                     system_folders=system_folders)
     info(f"New configuration created: {Fore.GREEN}{cfg_file}{Style.RESET_ALL}")
```

### Comparing `vantage6-3.9.0rc2/vantage6/cli/utils.py` & `vantage6-3.9.0rc4/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.9.0rc2/vantage6.egg-info/PKG-INFO` & `vantage6-3.9.0rc4/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc2 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 3.9.0rc4 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-3.9.0rc2/vantage6.egg-info/SOURCES.txt` & `vantage6-3.9.0rc4/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

