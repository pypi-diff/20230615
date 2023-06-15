# Comparing `tmp/pytest-rabbitmq-2.2.1.tar.gz` & `tmp/pytest-rabbitmq-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-rabbitmq-2.2.1.tar", last modified: Fri Feb 11 15:19:23 2022, max compression
+gzip compressed data, was "pytest-rabbitmq-3.0.0.tar", last modified: Thu Jun 15 13:37:27 2023, max compression
```

## Comparing `pytest-rabbitmq-2.2.1.tar` & `pytest-rabbitmq-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35146 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7650 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 15:19:23.448536 pytest-rabbitmq-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4509 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-02-11 15:19:18.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 15:19:23.452536 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-11 15:19:23.000000 pytest-rabbitmq-2.2.1/src/pytest_rabbitmq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:14.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:37:27.000000 pytest-rabbitmq-3.0.0/pytest_rabbitmq.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:37:27.441022 pytest-rabbitmq-3.0.0/setup.cfg
```

### Comparing `pytest-rabbitmq-2.2.1/CONTRIBUTING.rst` & `pytest-rabbitmq-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-2.2.1/COPYING` & `pytest-rabbitmq-3.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-2.2.1/COPYING.lesser` & `pytest-rabbitmq-3.0.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-2.2.1/README.rst` & `pytest-rabbitmq-3.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -82,19 +82,24 @@
      - pytest.ini option
      - Default
    * - host
      - host
      - --rabbitmq-host
      - rabbitmq_host
      - 127.0.0.1
-   * - port
+   * - RABBITMQ_NODE_PORT
      - port
      - --rabbitmq-port
      - rabbitmq_port
      - random
+   * - RABBITMQ_DIST_PORT
+     - distribution_port
+     - --rabbitmq-distribution-port
+     - rabbitmq_distribution_port
+     - random
    * - rabbitmqctl path
      - ctl
      - --rabbitmq-ctl
      - rabbitmq_ctl
      - /usr/lib/rabbitmq/bin/rabbitmqctl
    * - rabbitmq server path
      - server
```

### Comparing `pytest-rabbitmq-2.2.1/setup.py` & `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2016 by Clearcode <http://clearcode.cc>
 # and associates (see AUTHORS).
 
 # This file is part of pytest-rabbitmq.
 
 # pytest-rabbitmq is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
@@ -11,13 +10,13 @@
 
 # pytest-rabbitmq is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
-# along with pytest-rabbitmq. If not, see <http://www.gnu.org/licenses/>.
-"""Installation module of pytest-rabbitmq."""
-from setuptools import setup
+# along with pytest-rabbitmq.  If not, see <http://www.gnu.org/licenses/>.
+"""RabbitMQ factory package."""
+from pytest_rabbitmq.factories.client import rabbitmq
+from pytest_rabbitmq.factories.process import rabbitmq_proc
 
-
-setup()
+__all__ = ("rabbitmq", "rabbitmq_proc")
```

### Comparing `pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/__init__.py` & `pytest-rabbitmq-3.0.0/pytest_rabbitmq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq. If not, see <http://www.gnu.org/licenses/>.
 """Main pytest-rabbitmq module."""
-__version__ = "2.2.1"
+__version__ = "3.0.0"
```

### Comparing `pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/client.py` & `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,32 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq.  If not, see <http://www.gnu.org/licenses/>.
 """RabbitMQ client fixture factory."""
 import logging
+from typing import Callable, Generator
 
 import pytest
+from pika import BlockingConnection, ConnectionParameters
+from pika.credentials import PlainCredentials
+from pika.exceptions import ChannelClosed
+from pytest import FixtureRequest
 
-from rabbitpy import Exchange, Queue, Connection
-from rabbitpy.exceptions import ChannelClosedException
+from pytest_rabbitmq.factories.executor import RabbitMqExecutor
 
 logger = logging.getLogger("pytest-rabbitmq")
 
 
-def clear_rabbitmq(process, rabbitmq_connection):
-    """
-    Clear queues and exchanges from given rabbitmq process.
+def clear_rabbitmq(process: RabbitMqExecutor, rabbitmq_connection: BlockingConnection) -> None:
+    """Clear queues and exchanges from given rabbitmq process.
 
     :param RabbitMqExecutor process: rabbitmq process
-    :param rabbitpy.Connection rabbitmq_connection: connection to rabbitmq
+    :param pika.connection.Connection rabbitmq_connection: connection to rabbitmq
 
     """
     channel = rabbitmq_connection.channel()
 
     for exchange in process.list_exchanges():
         if exchange.startswith("amq."):
             # ----------------------------------------------------------------
@@ -44,36 +47,36 @@
             # ----------------------------------------------------------------
             # Exchange names starting with "amq." are reserved for pre-declared
             # and standardised exchanges. The client MAY declare an exchange
             # starting with "amq." if the passive option is set, or the
             # exchange already exists. Error code: access-refused
             # ----------------------------------------------------------------
             continue
-        ex = Exchange(channel, exchange)
-        ex.delete()
+        channel.exchange_delete(exchange)
 
     for queue_name in process.list_queues():
         if queue_name.startswith("amq."):
             # ----------------------------------------------------------------
             # From rabbit docs:
             # https://www.rabbitmq.com/amqp-0-9-1-reference.html
             # ----------------------------------------------------------------
             # Queue names starting with "amq." are reserved for pre-declared
             # and standardised queues. The client MAY declare a queue starting
             # with "amq." if the passive option is set, or the queue already
             # exists. Error code: access-refused
             # ----------------------------------------------------------------
             continue
-        queue = Queue(channel, queue_name)
-        queue.delete()
+        channel.queue_delete(queue_name)
 
 
-def rabbitmq(process_fixture_name, teardown=clear_rabbitmq):
-    """
-    Client fixture factory for RabbitMQ.
+def rabbitmq(
+    process_fixture_name: str,
+    teardown: Callable[[RabbitMqExecutor, BlockingConnection], None] = clear_rabbitmq,
+) -> Callable[[FixtureRequest], Generator[BlockingConnection, None, None]]:
+    """Client fixture factory for RabbitMQ.
 
     :param str process_fixture_name: name of RabbitMQ process variable
         returned by rabbitmq_proc
     :param callable teardown: custom callable that clears rabbitmq
 
     .. note::
 
@@ -82,33 +85,36 @@
         to remove queues and exchanges of your choosing, without querying
         rabbitmqctl underneath.
 
     :returns RabbitMQ connection
     """
 
     @pytest.fixture
-    def rabbitmq_factory(request):
-        """
-        Client fixture for RabbitMQ.
+    def rabbitmq_factory(request: FixtureRequest) -> Generator[BlockingConnection, None, None]:
+        """Client fixture for RabbitMQ.
 
         #. Get module and config.
         #. Connect to RabbitMQ using the parameters from config.
 
         :param TCPExecutor rabbitmq_proc: tcp executor
         :param FixtureRequest request: fixture request object
-        :rtype: rabbitpy.adapters.blocking_connection.BlockingConnection
+        :rtype: pika.adapters.blocking_connection.BlockingConnection
         :returns: instance of :class:`BlockingConnection`
         """
         # load required process fixture
         process = request.getfixturevalue(process_fixture_name)
 
-        connection = Connection(f"amqp://guest:guest@{process.host}:{process.port}/%2F")
+        credentials = PlainCredentials("guest", "guest")
+        parameters = ConnectionParameters(
+            host=process.host, port=process.port, virtual_host="/", credentials=credentials
+        )
+        connection = BlockingConnection(parameters)
 
         yield connection
         teardown(process, connection)
         try:
             connection.close()
-        except ChannelClosedException as e:
+        except ChannelClosed as e:
             # at this stage this exception occurs when connection is being closed
             logger.warning(f"ChannelClosedException occured while closing connection {e}")
 
     return rabbitmq_factory
```

### Comparing `pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/factories/executor.py` & `pytest-rabbitmq-3.0.0/pytest_rabbitmq/factories/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 """RabbitMQ Executor."""
 import re
 import subprocess
+from pathlib import Path
+from typing import List, Optional
 
 from mirakuru import TCPExecutor
 
 
 class RabbitMqExecutor(TCPExecutor):
     """RabbitMQ executor to start specific rabbitmq instances."""
 
     _UNWANTED_QUEUE_PATTERN = re.compile("(done|timeout:|listing queues)")
 
     def __init__(
         self,
-        command,
-        host,
-        port,
-        rabbit_ctl,
-        logpath,
-        path,
-        plugin_path,
-        node_name=None,
-        **kwargs,
-    ):  # pylint:disable=too-many-arguments
-        """
-        Initialize RabbitMQ executor.
-
-        :param str command: rabbitmq-server location
-        :param str host: host where rabbitmq will be accessible
-        :param int port: port under which rabbitmq runs
-        :param str rabbit_ctl: rabbitctl location
-        :param str logpath:
-        :param str path: Path containing rabbitmq'a mnesia na plugins
-        :param str node_name: RabbitMQ node name
-        :param kwargs: see TCPExecutor for description
+        command: str,
+        host: str,
+        port: int,
+        distribution_port: int,
+        rabbit_ctl: str,
+        logpath: Path,
+        path: Path,
+        plugin_path: Path,
+        node_name: Optional[str] = None,
+    ) -> None:  # pylint:disable=too-many-arguments
+        """Initialize RabbitMQ executor.
+
+        :param command: rabbitmq-server location
+        :param host: host where rabbitmq will be accessible
+        :param port: port under which rabbitmq runs
+        :param rabbit_ctl: rabbitctl location
+        :param logpath:
+        :param path: Path containing rabbitmq'a mnesia na plugins
+        :param node_name: RabbitMQ node name
         """
         envvars = {
-            "RABBITMQ_LOG_BASE": logpath + f"/rabbit-server.{port}.log",
-            "RABBITMQ_MNESIA_BASE": path + "mnesia",
-            "RABBITMQ_ENABLED_PLUGINS_FILE": plugin_path + "/plugins",
+            "RABBITMQ_LOG_BASE": str(logpath / f"rabbit-server.{port}.log"),
+            "RABBITMQ_MNESIA_BASE": str(path / "mnesia"),
+            "RABBITMQ_ENABLED_PLUGINS_FILE": str(plugin_path / "plugins"),
             "RABBITMQ_NODE_PORT": str(port),
+            "RABBITMQ_DIST_PORT": str(distribution_port),
             # Use the port number in node name, so multiple instances started
             # at different ports will work separately instead of clustering.
             "RABBITMQ_NODENAME": node_name or f"rabbitmq-test-{port}",
         }
-        super().__init__(command, host, port, timeout=60, envvars=envvars, **kwargs)
+        super().__init__(command, host, port, timeout=60, envvars=envvars)
         self.rabbit_ctl = rabbit_ctl
 
-    def rabbitctl_output(self, *args):
-        """
-        Query rabbitctl with args.
+    def rabbitctl_output(self, *args: str) -> str:
+        """Query rabbitctl with args.
 
         :param list args: list of additional args to query
         """
-        ctl_command = [self.rabbit_ctl]
+        ctl_command: List[str] = [self.rabbit_ctl]
         ctl_command.extend(args)
         return subprocess.check_output(ctl_command, env=self._popen_kwargs["env"]).decode("utf-8")
 
-    def list_exchanges(self):
+    def list_exchanges(self) -> List[str]:
         """Get exchanges defined on given rabbitmq."""
-        exchanges = []
+        exchanges: List[str] = []
         output = self.rabbitctl_output("list_exchanges", "name")
-        unwanted_exchanges = ["Listing exchanges ...", "...done."]
+        unwanted_exchanges = ["Listing exchanges for vhost / ...", "...done."]
 
         for exchange in output.split("\n"):
             if exchange and exchange not in unwanted_exchanges:
                 exchanges.append(str(exchange))
 
         return exchanges
 
-    def list_queues(self):
+    def list_queues(self) -> List[str]:
         """Get queues defined on given rabbitmq."""
-        queues = []
+        queues: List[str] = []
         output = self.rabbitctl_output("list_queues", "name")
 
         for queue in output.split("\n"):
             if queue and not self._UNWANTED_QUEUE_PATTERN.search(queue.strip(". ").lower()):
                 queues.append(str(queue))
 
         return queues
```

### Comparing `pytest-rabbitmq-2.2.1/src/pytest_rabbitmq/plugin.py` & `pytest-rabbitmq-3.0.0/pytest_rabbitmq/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,49 +14,56 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq.  If not, see <http://www.gnu.org/licenses/>.
 """Plugin definition for pytest-rabbitmq."""
 from tempfile import gettempdir
 
-from pytest_rabbitmq import factories
+from pytest import Parser
 
+from pytest_rabbitmq import factories
 
 # pylint:disable=invalid-name
 _help_ctl = "RabbitMQ ctl path"
 _help_server = "RabbitMQ server path"
 _help_logsdir = "Logs directory location"
 _help_plugindir = "Directory where 'plugin' file is located"
 _help_host = "Host at which RabbitMQ will accept connections"
 _help_port = "Port at which RabbitMQ will accept connections"
+_help_distribution_port = "Port at which RabbitMQ nodes will communicate with each other"
 _help_node = "Node name for rabbitmq instance"
 
 
-def pytest_addoption(parser):
+def pytest_addoption(parser: Parser) -> None:
     """Confioguration option."""
     parser.addini(name="rabbitmq_host", help=_help_host, default="127.0.0.1")
     parser.addini(
         name="rabbitmq_port",
         help=_help_port,
         default=None,
     )
     parser.addini(
+        name="rabbitmq_distribution_port",
+        help=_help_distribution_port,
+        default=None,
+    )
+    parser.addini(
         name="rabbitmq_ctl",
         help=_help_ctl,
         default="/usr/lib/rabbitmq/bin/rabbitmqctl",
     )
     parser.addini(
         name="rabbitmq_server",
         help=_help_server,
         default="/usr/lib/rabbitmq/bin/rabbitmq-server",
     )
     parser.addini(
         name="rabbitmq_logsdir",
         help=_help_logsdir,
-        default=gettempdir(),
+        default=None,
     )
     parser.addini(
         name="rabbitmq_plugindir",
         help=_help_logsdir,
         default=gettempdir(),
     )
     parser.addini(
@@ -68,14 +75,20 @@
     parser.addoption(
         "--rabbitmq-host",
         action="store",
         dest="rabbitmq_host",
         help=_help_host,
     )
     parser.addoption("--rabbitmq-port", action="store", dest="rabbitmq_port", help=_help_port)
+    parser.addoption(
+        "--rabbitmq-distribution-port",
+        action="store",
+        dest="rabbitmq_distribution_port",
+        help=_help_distribution_port,
+    )
     parser.addoption("--rabbitmq-ctl", action="store", dest="rabbitmq_ctl", help=_help_ctl)
     parser.addoption("--rabbitmq-server", action="store", dest="rabbitmq_server", help=_help_server)
     parser.addoption(
         "--rabbitmq-logsdir",
         action="store",
         metavar="path",
         dest="rabbitmq_logsdir",
```

