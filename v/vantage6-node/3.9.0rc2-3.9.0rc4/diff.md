# Comparing `tmp/vantage6-node-3.9.0rc2.tar.gz` & `tmp/vantage6-node-3.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.9.0rc2.tar", last modified: Tue May  9 13:37:05 2023, max compression
+gzip compressed data, was "vantage6-node-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
```

## Comparing `vantage6-node-3.9.0rc2.tar` & `vantage6-node-3.9.0rc4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    40378 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.854910 vantage6-node-3.9.0rc2/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19478 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-09 13:36:37.000000 vantage6-node-3.9.0rc2/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:05.858910 vantage6-node-3.9.0rc2/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 13:37:05.000000 vantage6-node-3.9.0rc2/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    42264 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24977 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19729 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/server_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-24 09:33:56.000000 vantage6-node-3.9.0rc4/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.957728 vantage6-node-3.9.0rc4/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 09:34:09.000000 vantage6-node-3.9.0rc4/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.9.0rc2/PKG-INFO` & `vantage6-node-3.9.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc2 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc4 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.9.0rc2/setup.py` & `vantage6-node-3.9.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,30 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'click==8.1.3',
-        'docker==6.0.1',
+        'docker==6.1.2',
         'gevent==22.10.2',
         'python-socketio==5.7.2',
-        'requests==2.28.2',
+        'requests==2.31.0',
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-client == {version_ns["__version__"]}',
     ],
     extras_require={
         'dev': [
             'coverage==6.4.4',
             'python-coveralls==2.9.3',
             'SQLAlchemy==1.4.46',
             'schema==0.7.5',
             'appdirs==1.4.4',
             'PyJWT==2.6.0',
-            'Flask==1.1.1'
+            'flask==2.2.5'
         ]
     },
     package_data={
         'vantage6.node': [
             '__build__',
             '_data/*.*',
         ],
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/__init__.py` & `vantage6-node-3.9.0rc4/vantage6/node/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class VPNConnectMode(Enum):
     FIRST_TRY = 1
     REFRESH_KEYPAIR = 2
     REFRESH_COMPLETE = 3
 
 
 # ------------------------------------------------------------------------------
-class Node(object):
+class Node:
     """
     Authenticates to the central server, setup encryption, a
     websocket connection, retrieving task that were posted while
     offline, preparing dataset for usage and finally setup a
     local proxy server..
 
     Parameters
@@ -99,14 +99,15 @@
 
     def initialize(self) -> None:
         """Initialization of the node"""
         # check if docker is running, otherwise exit with error
         check_docker_running()
 
         self.config = self.ctx.config
+        self.debug: dict = self.config.get('debug', {})
         self.queue = queue.Queue()
         self._using_encryption = None
 
         # initialize Node connection to the server
         self.server_io = NodeClient(
             host=self.config.get('server_url'),
             port=self.config.get('port'),
@@ -125,18 +126,14 @@
 
         # Thread for proxy server for algorithm containers, so they can
         # communicate with the central server.
         self.log.info("Setting up proxy server")
         t = Thread(target=self.__proxy_server_worker, daemon=True)
         t.start()
 
-        # Create a long-lasting websocket connection.
-        self.log.debug("Creating websocket connection with the server")
-        self.connect_to_socket()
-
         # setup docker isolated network manager
         internal_ = running_in_docker()
         if not internal_:
             self.log.warn(
                 "Algorithms have internet connection! "
                 "This happens because you use 'vnode-local'!"
             )
@@ -163,14 +160,18 @@
             isolated_network_mgr=isolated_network_mgr,
             vpn_manager=self.vpn_manager,
             tasks_dir=self.__tasks_dir,
             client=self.server_io,
             proxy=self.squid
         )
 
+        # Create a long-lasting websocket connection.
+        self.log.debug("Creating websocket connection with the server")
+        self.connect_to_socket()
+
         # Connect the node to the isolated algorithm network *only* if we're
         # running in a docker container.
         if self.ctx.running_in_docker:
             isolated_network_mgr.connect(
                 container_name=self.ctx.docker_container_name,
                 aliases=[NODE_PROXY_SERVER_HOSTNAME]
             )
@@ -213,15 +214,18 @@
         # value.
         proxy_host = os.environ.get("PROXY_SERVER_HOST", default_proxy_host)
         os.environ["PROXY_SERVER_HOST"] = proxy_host
 
         proxy_port = int(os.environ.get("PROXY_SERVER_PORT", 8080))
 
         # 'app' is defined in vantage6.node.proxy_server
-        # app.debug = True
+        debug_mode = self.debug.get("proxy_server", False)
+        if debug_mode:
+            self.log.debug("Debug mode enabled for proxy server")
+            proxy_server.app.debug = True
         proxy_server.app.config["SERVER_IO"] = self.server_io
         proxy_server.server_url = self.server_io.base_path
 
         # set up proxy server logging
         log_level = getattr(logging, self.config["logging"]["level"].upper())
         self.proxy_log = get_file_logger(
             'proxy_server', self.ctx.proxy_log_file, log_level_file=log_level
@@ -255,20 +259,64 @@
                 self.log.error(e)
 
     def sync_task_queue_with_server(self) -> None:
         """ Get all unprocessed tasks from the server for this node."""
         assert self.server_io.cryptor, "Encrpytion has not been setup"
 
         # request open tasks from the server
-        tasks = self.server_io.get_results(state="open", include_task=True)
-        self.log.debug(tasks)
-        for task in tasks:
-            self.queue.put(task)
+        task_results = self.server_io.get_results(state="open",
+                                                  include_task=True)
+        self.log.debug(task_results)
+
+        # add the tasks to the queue
+        self.__add_tasks_to_queue(task_results)
+        self.log.info(f"Received {self.queue._qsize()} tasks")
+
+    def get_task_and_add_to_queue(self, task_id: int) -> None:
+        """
+        Fetches (open) task with task_id from the server. The `task_id` is
+        delivered by the websocket-connection.
+
+        Parameters
+        ----------
+        task_id : int
+            Task identifier
+        """
+        # fetch (open) result for the node with the task_id
+        task_results = self.server_io.get_results(
+            include_task=True,
+            state='open',
+            task_id=task_id
+        )
 
-        self.log.info(f"received {self.queue._qsize()} tasks")
+        # add the tasks to the queue
+        self.__add_tasks_to_queue(task_results)
+
+    def __add_tasks_to_queue(self, task_results: list[dict]) -> None:
+        """
+        Add a task to the queue.
+
+        Parameters
+        ----------
+        taskresult : list[dict]
+            A list of dictionaries with information required to run the
+            algorithm
+        """
+        for task_result in task_results:
+            try:
+                if not self.__docker.is_running(task_result['id']):
+                    self.queue.put(task_result)
+                else:
+                    self.log.info(
+                        f"Not starting task {task_result['task']['id']} - "
+                        f"{task_result['task']['name']} as it is already "
+                        "running"
+                    )
+            except Exception:
+                self.log.exception("Error while syncing task queue")
 
     def __start_task(self, taskresult: dict) -> None:
         """
         Start the docker image and notify the server that the task has been
         started.
 
         Parameters
@@ -317,14 +365,28 @@
             # set finished_at to now, so that the task is not picked up again
             # (as the task is not started at all, unlike other crashes, it will
             # never finish and hence not be set to finished)
             update['finished_at'] = datetime.datetime.now().isoformat()
         self.server_io.patch_results(
             id_=taskresult['id'], result=update
         )
+
+        # ensure that the /tasks namespace is connected. This may take a while
+        # (usually < 5s) when the socket just (re)connected
+        MAX_ATTEMPTS = 30
+        retries = 0
+        while '/tasks' not in self.socketIO.namespaces and \
+                retries < MAX_ATTEMPTS:
+            retries += 1
+            self.log.debug('Waiting for /tasks namespace to connect...')
+            time.sleep(1)
+        self.log.debug('Connected to /tasks namespace')
+        # in case the namespace is still not connected, the socket notification
+        # will not be sent to other nodes, but the task will still be processed
+
         # send socket event to alert everyone of task status change
         self.socketIO.emit(
             'algorithm_status_change',
             data={
                 'node_id': self.server_io.whoami.id_,
                 'status': task_status,
                 'result_id': taskresult['id'],
@@ -836,15 +898,19 @@
             )
 
     def connect_to_socket(self) -> None:
         """
         Create long-lasting websocket connection with the server. The
         connection is used to receive status updates, such as new tasks.
         """
-        self.socketIO = SocketIO(request_timeout=60)
+        debug_mode = self.debug.get('socketio', False)
+        if debug_mode:
+            self.log.debug("Debug mode enabled for socketio")
+        self.socketIO = SocketIO(request_timeout=60, logger=debug_mode,
+                                 engineio_logger=debug_mode)
 
         self.socketIO.register_namespace(NodeTaskNamespace('/tasks'))
         NodeTaskNamespace.node_worker_ref = self
 
         self.socketIO.connect(
             url=f'{self.server_io.host}:{self.server_io.port}',
             headers=self.server_io.headers,
@@ -875,54 +941,35 @@
         connection to notify the server that this node is online
         """
         # Wait for the socket to be connected to the namespaces on startup
         time.sleep(5)
 
         while True:
             try:
-                self.socketIO.emit('ping', namespace='/tasks')
+                if self.socketIO.connected:
+                    self.socketIO.emit('ping', namespace='/tasks')
+                else:
+                    self.log.debug('SocketIO is not connected, skipping ping')
             except Exception:
                 self.log.exception('Ping thread had an exception')
             # Wait before sending next ping
             time.sleep(PING_INTERVAL_SECONDS)
 
-    def get_task_and_add_to_queue(self, task_id: int) -> None:
-        """
-        Fetches (open) task with task_id from the server. The `task_id` is
-        delivered by the websocket-connection.
-
-        Parameters
-        ----------
-        task_id : int
-            Task identifier
-        """
-        # fetch (open) result for the node with the task_id
-        tasks = self.server_io.get_results(
-            include_task=True,
-            state='open',
-            task_id=task_id
-        )
-
-        # in the current setup, only a single result for a single node
-        # in a task exists.
-        for task in tasks:
-            self.queue.put(task)
-
     def run_forever(self) -> None:
         """Keep checking queue for incoming tasks (and execute them)."""
         kill_listener = ContainerKillListener()
         try:
             while True:
                 # blocking untill a task comes available
                 # timeout specified, else Keyboard interupts are ignored
                 self.log.info("Waiting for new tasks....")
 
                 while not kill_listener.kill_now:
                     try:
-                        task = self.queue.get(timeout=1)
+                        taskresult = self.queue.get(timeout=1)
                         # if no item is returned, the Empty exception is
                         # triggered, thus break statement is not reached
                         break
 
                     except queue.Empty:
                         pass
 
@@ -930,15 +977,15 @@
                         self.log.debug(e)
 
                 if kill_listener.kill_now:
                     raise InterruptedError
 
                 # if task comes available, attempt to execute it
                 try:
-                    self.__start_task(task)
+                    self.__start_task(taskresult)
                 except Exception as e:
                     self.log.exception(e)
 
         except (KeyboardInterrupt, InterruptedError):
             self.log.info("Vnode is interrupted, shutting down...")
             self.cleanup()
             sys.exit()
@@ -1039,16 +1086,13 @@
 
         self.log.info("Bye!")
 
 
 # ------------------------------------------------------------------------------
 def run(ctx):
     """ Start the node."""
-    logging.getLogger("urllib3").setLevel(logging.WARNING)
-    logging.getLogger("requests").setLevel(logging.WARNING)
-    logging.getLogger("engineio.client").setLevel(logging.WARNING)
 
     # initialize node, connect to the server using websockets
     node = Node(ctx)
 
     # put the node to work, executing tasks that are in the que
     node.run_forever()
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/_version.py` & `vantage6-node-3.9.0rc4/vantage6/node/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/cli/node.py` & `vantage6-node-3.9.0rc4/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/context.py` & `vantage6-node-3.9.0rc4/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/docker_base.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/docker_manager.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/docker_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,30 +191,30 @@
         # the environment variables for us. This has the added bonus that we
         # can override the URI from the command line as well.
         self.databases = {}
         for label in db_labels:
             label_upper = label.upper()
             db_config = get_database_config(databases, label)
             if running_in_docker():
-                uri_env = os.environ[f'{label_upper}_DATABASE_URI']
-                uri = f'/mnt/{uri_env}'
+                uri = os.environ[f'{label_upper}_DATABASE_URI']
             else:
                 uri = db_config['uri']
 
-            db_type = db_config['type']
-
             db_is_file = Path(uri).exists()
+            if running_in_docker() and db_is_file:
+                uri = f'/mnt/{uri}'
+
             if db_is_file:
                 # We'll copy the file to the folder `data` in our task_dir.
                 self.log.info(f'Copying {uri} to {self.__tasks_dir}')
                 shutil.copy(uri, self.__tasks_dir)
                 uri = self.__tasks_dir / os.path.basename(uri)
 
             self.databases[label] = {'uri': uri, 'is_file': db_is_file,
-                                     'type': db_type}
+                                     'type': db_config['type']}
         self.log.debug(f"Databases: {self.databases}")
 
     def _set_algorithm_device_requests(self, device_requests_config: dict) \
             -> None:
         """
         Configure device access for the algorithm container.
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/exceptions.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/squid.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/squid.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/task_manager.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/task_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 import pickle
 import docker.errors
 import json
 
 from pathlib import Path
 
-from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
     remove_container_if_exists, remove_container, pull_if_newer,
     running_in_docker
 )
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.common.task_status import TaskStatus
@@ -33,15 +32,14 @@
     Manager for running a vantage6 algorithm container within docker.
 
     Ensures that the environment is properly set up (docker volumes,
     directories, environment variables, etc). Then runs the algorithm as a
     docker container. Finally, it monitors the container state and can return
     it's results when the algorithm finished.
     """
-    log = logging.getLogger(logger_name(__name__))
 
     def __init__(self, image: str, vpn_manager: VPNManager, node_name: str,
                  result_id: int, task_info: dict, tasks_dir: Path,
                  isolated_network_mgr: NetworkManager,
                  databases: dict, docker_volume_name: str,
                  alpine_image: str | None = None, proxy: Squid | None = None,
                  device_requests: list | None = None):
@@ -70,19 +68,21 @@
             Name of the docker volume
         alpine_image: str | None
             Name of alternative Alpine image to be used
         device_requests: list | None
             List of DeviceRequest objects to be passed to the algorithm
             container
         """
+        self.task_id = task_info['id']
+        self.log = logging.getLogger(f"task ({self.task_id})")
+
         super().__init__(isolated_network_mgr)
         self.image = image
         self.__vpn_manager = vpn_manager
         self.result_id = result_id
-        self.task_id = task_info['id']
         self.parent_id = get_parent_id(task_info)
         self.__tasks_dir = tasks_dir
         self.databases = databases
         self.data_volume_name = docker_volume_name
         self.node_name = node_name
         self.alpine_image = ALPINE_IMAGE if alpine_image is None \
             else alpine_image
@@ -93,15 +93,15 @@
         self.docker_input = None
 
         self.labels = {
             f"{APPNAME}-type": "algorithm",
             "node": node_name,
             "result_id": str(result_id)
         }
-        self.helper_labels = self.labels
+        self.helper_labels = self.labels.copy()
         self.helper_labels[f"{APPNAME}-type"] = "algorithm-helper"
 
         # FIXME: these values should be retrieved from DockerNodeContext
         #   in some way.
         self.tmp_folder = "/mnt/tmp"
         self.data_folder = "/mnt/data"
 
@@ -183,15 +183,15 @@
         except Exception as e:
             self.log.debug('Failed to pull image')
             self.log.exception(e)
             self.status = TaskStatus.FAILED
             raise PermanentAlgorithmStartFail
 
     def run(self, docker_input: bytes, tmp_vol_name: str, token: str,
-            algorithm_env: dict, database: str) -> list[dict]:
+            algorithm_env: dict, database: str) -> list[dict] | None:
         """
         Runs the docker-image in detached mode.
 
         It will will attach all mounts (input, output and datafile) to the
         docker image. And will supply some environment variables.
 
         Parameters
@@ -250,44 +250,48 @@
         container_name = f'{APPNAME}-{self.node_name}-result-{self.result_id}'
         helper_container_name = container_name + '-helper'
 
         # Try to pull the latest image
         self.pull()
 
         # remove algorithm containers if they were already running
+        self.log.debug("Check if algorithm container is already running")
         remove_container_if_exists(
             docker_client=self.docker, name=container_name
         )
         remove_container_if_exists(
             docker_client=self.docker, name=helper_container_name
         )
 
         if self.__vpn_manager:
             # if VPN is active, network exceptions must be configured
             # First, start a container that runs indefinitely. The algorithm
             # container will run in the same network and network exceptions
             # will therefore also affect the algorithm.
+            self.log.debug("Start helper container to setup VPN network")
             self.helper_container = self.docker.containers.run(
                 command='sleep infinity',
                 image=self.alpine_image,
                 labels=self.helper_labels,
                 network=self.isolated_network_mgr.network_name,
                 name=helper_container_name,
                 detach=True
             )
             # setup forwarding of traffic via VPN client to and from the
             # algorithm container:
+            self.log.debug("Setup port forwarder")
             vpn_ports = self.__vpn_manager.forward_vpn_traffic(
                 helper_container=self.helper_container,
                 algo_image_name=self.image
             )
 
         # try reading docker input
         deserialized_input = None
         if self.docker_input:
+            self.log.debug("Deserialize input")
             try:
                 deserialized_input = pickle.loads(self.docker_input)
             except Exception:
                 pass
 
         # attempt to run the image
         try:
@@ -471,16 +475,16 @@
         if database in self.databases:
             environment_variables["USER_REQUESTED_DATABASE_LABEL"] = database
         else:
             # In this case the algorithm might crash if it tries to access
             # the DATABASE_LABEL environment variable
             self.log.warning("A user specified a database that does not "
                              "exist. Available databases are: "
-                             f"{self.databases.keys()}. This is likely to "
-                             "result in an algorithm crash.")
+                             f"{', '.join(list(self.databases.keys()))}. This "
+                             "is likely to result in an algorithm crash.")
             self.log.debug(f"User specified database: {database}")
 
         # Only prepend the data_folder is it is a file-based database
         # This allows algorithms to access multiple data sources at the
         # same time
         db_labels = []
         for label in self.databases:
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/docker/vpn_manager.py` & `vantage6-node-3.9.0rc4/vantage6/node/docker/vpn_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,18 +227,22 @@
 
         Returns
         -------
         str
             IP address assigned to VPN client container by VPN server
         """
         try:
-            _, vpn_interface = self.vpn_client_container.exec_run(
-                'ip --json addr show dev tun0'
-            )
-            vpn_interface = json.loads(vpn_interface)
+            # use has_connection() to check if VPN is active. This function
+            # also waits for a connection to be established, which is helpful
+            # for unstable connections
+            if self.has_connection():
+                _, vpn_interface = self.vpn_client_container.exec_run(
+                    'ip --json addr show dev tun0'
+                )
+                vpn_interface = json.loads(vpn_interface)
         except (JSONDecodeError, docker.errors.APIError):
             # JSONDecodeError if VPN is not setup yet, APIError if VPN
             # container is restarting (e.g. due to connection errors)
             raise ConnectionError(
                 "Could not get VPN IP: VPN is not connected!")
         return vpn_interface[0]['addr_info'][0]['local']
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/globals.py` & `vantage6-node-3.9.0rc4/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/proxy_server.py` & `vantage6-node-3.9.0rc4/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/server_io.py` & `vantage6-node-3.9.0rc4/vantage6/node/server_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             if time_until_expiry < REFRESH_BEFORE_EXPIRES_SECONDS:
                 self.refresh_token()
             else:
                 time.sleep(
                     int(time_until_expiry - REFRESH_BEFORE_EXPIRES_SECONDS + 1)
                 )
 
-    def request_token_for_container(self, task_id: int, image: str):
+    def request_token_for_container(self, task_id: int, image: str) -> dict:
         """ Request a container-token at the central server.
 
         This token is used by algorithm containers that run on this
         node. These algorithms can then post tasks and retrieve
         child-results (usually refered to as a master container).
         The server performs a few checks (e.g. if the task you
         request the key for is still open) before handing out this
@@ -141,15 +141,15 @@
 
         Returns
         -------
         dict
             The results.
         """
         return super().get_results(
-            id=id_,
+            id_=id_,
             state=state,
             include_task=include_task,
             task_id=task_id,
             node_id=self.whoami.id_
         )
 
     def is_encrypted_collaboration(self) -> bool:
```

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/socket.py` & `vantage6-node-3.9.0rc4/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6/node/util/colorer.py` & `vantage6-node-3.9.0rc4/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.9.0rc2/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-3.9.0rc4/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc2 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.9.0rc4 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.9.0rc2/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-3.9.0rc4/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

