# Comparing `tmp/siridb-connector-2.1.2.tar.gz` & `tmp/siridb-connector-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siridb-connector-2.1.2.tar", last modified: Fri Feb 10 16:00:24 2023, max compression
+gzip compressed data, was "siridb-connector-2.1.3.tar", last modified: Thu Jun 15 13:29:21 2023, max compression
```

## Comparing `siridb-connector-2.1.2.tar` & `siridb-connector-2.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/
--rw-rw-r--   0 joente    (1000) joente    (1000)      139 2023-02-10 12:43:44.000000 siridb-connector-2.1.2/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)     1078 2022-11-30 07:39:47.000000 siridb-connector-2.1.2/LICENSE.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)     9890 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     7238 2021-03-15 14:25:50.000000 siridb-connector-2.1.2/README.md
--rw-rw-r--   0 joente    (1000) joente    (1000)       79 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1656 2023-02-10 12:47:42.000000 siridb-connector-2.1.2/setup.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb/
--rw-rw-r--   0 joente    (1000) joente    (1000)      154 2023-02-10 15:58:39.000000 siridb-connector-2.1.2/siridb/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb/connector/
--rw-rw-r--   0 joente    (1000) joente    (1000)     2356 2023-02-10 12:43:44.000000 siridb-connector-2.1.2/siridb/connector/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb/connector/lib/
--rw-rw-r--   0 joente    (1000) joente    (1000)      121 2022-11-30 07:40:21.000000 siridb-connector-2.1.2/siridb/connector/lib/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    17408 2023-02-10 15:58:27.000000 siridb-connector-2.1.2/siridb/connector/lib/client.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     6467 2021-03-17 12:08:00.000000 siridb-connector-2.1.2/siridb/connector/lib/connection.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       58 2021-03-15 14:25:50.000000 siridb-connector-2.1.2/siridb/connector/lib/constants.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      980 2022-11-30 07:40:57.000000 siridb-connector-2.1.2/siridb/connector/lib/datapackage.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       57 2021-03-15 14:25:50.000000 siridb-connector-2.1.2/siridb/connector/lib/defaults.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      359 2022-11-30 07:41:10.000000 siridb-connector-2.1.2/siridb/connector/lib/exceptions.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       63 2021-03-30 17:58:49.000000 siridb-connector-2.1.2/siridb/connector/lib/logging.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8847 2023-02-10 12:43:44.000000 siridb-connector-2.1.2/siridb/connector/lib/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     3919 2022-11-30 07:41:32.000000 siridb-connector-2.1.2/siridb/connector/lib/protomap.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     9890 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      633 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        6 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        7 2023-02-10 16:00:24.000000 siridb-connector-2.1.2/siridb_connector.egg-info/top_level.txt
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      139 2023-02-10 12:43:44.000000 siridb-connector-2.1.3/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1078 2022-11-30 07:39:47.000000 siridb-connector-2.1.3/LICENSE.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8265 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     7238 2021-03-15 14:25:50.000000 siridb-connector-2.1.3/README.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)       79 2023-06-15 13:29:21.021011 siridb-connector-2.1.3/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1656 2023-02-10 12:47:42.000000 siridb-connector-2.1.3/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/siridb/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      154 2023-06-15 13:28:15.000000 siridb-connector-2.1.3/siridb/__init__.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/siridb/connector/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2356 2023-02-10 12:43:44.000000 siridb-connector-2.1.3/siridb/connector/__init__.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/siridb/connector/lib/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      121 2022-11-30 07:40:21.000000 siridb-connector-2.1.3/siridb/connector/lib/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    17470 2023-06-15 13:27:56.000000 siridb-connector-2.1.3/siridb/connector/lib/client.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     6467 2021-03-17 12:08:00.000000 siridb-connector-2.1.3/siridb/connector/lib/connection.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       58 2021-03-15 14:25:50.000000 siridb-connector-2.1.3/siridb/connector/lib/constants.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      980 2022-11-30 07:40:57.000000 siridb-connector-2.1.3/siridb/connector/lib/datapackage.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       57 2021-03-15 14:25:50.000000 siridb-connector-2.1.3/siridb/connector/lib/defaults.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      359 2022-11-30 07:41:10.000000 siridb-connector-2.1.3/siridb/connector/lib/exceptions.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       63 2021-03-30 17:58:49.000000 siridb-connector-2.1.3/siridb/connector/lib/logging.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8847 2023-02-10 12:43:44.000000 siridb-connector-2.1.3/siridb/connector/lib/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3919 2022-11-30 07:41:32.000000 siridb-connector-2.1.3/siridb/connector/lib/protomap.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-06-15 13:29:21.017011 siridb-connector-2.1.3/siridb_connector.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8265 2023-06-15 13:29:20.000000 siridb-connector-2.1.3/siridb_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      633 2023-06-15 13:29:20.000000 siridb-connector-2.1.3/siridb_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-06-15 13:29:20.000000 siridb-connector-2.1.3/siridb_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        6 2023-06-15 13:29:20.000000 siridb-connector-2.1.3/siridb_connector.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        7 2023-06-15 13:29:20.000000 siridb-connector-2.1.3/siridb_connector.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `siridb-connector-2.1.2/LICENSE.txt` & `siridb-connector-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/PKG-INFO` & `siridb-connector-2.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,222 +1,16 @@
 Metadata-Version: 2.1
 Name: siridb-connector
-Version: 2.1.2
+Version: 2.1.3
 Summary: SiriDB Connector
 Home-page: https://github.com/SiriDB/siridb-connector
+Download-URL: https://github.com/SiriDB/siridb-connector/tarball/2.1.3
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: UNKNOWN
-Download-URL: https://github.com/SiriDB/siridb-connector/tarball/2.1.2
-Description: SiriDB - Connector
-        ==================
-        
-        The SiriDB Connector is a self-contained Python driver for communicating with SiriDB servers.
-        This manual describes how to install and configure SiriDB Connector for Python 3, and how to use it to develop database applications.
-        
-        
-        ---------------------------------------
-          * [Installation](#installation)
-          * [Quick usage](#quick-usage)
-          * [SiriDBClient](#siridbclient)
-            * [connect](#siridbclientconnect)
-            * [insert](#siridbclientinsert)
-            * [query](#siridbclientquery)
-            * [close](#siridbclientclose)
-          * [Exception codes](#exception-codes)
-          * [Version info](#version-info)
-        
-        ---------------------------------------
-        
-        ## Installation
-        ------------
-        
-        From PyPI (recommended)
-        
-        ```
-        pip install siridb-connector
-        ```
-        
-        From source code
-        
-        ```
-        python setup.py install
-        ```
-        
-        
-        ## Quick usage
-        -------
-        
-        ```python
-        import asyncio
-        import time
-        import random
-        from siridb.connector import SiriDBClient
-        
-        async def example(siri):
-            # Start connecting to SiriDB.
-            # .connect() returns a list of all connections referring to the supplied
-            # hostlist. The list can contain exceptions in case a connection could not
-            # be made.
-            await siri.connect()
-        
-            try:
-                # insert
-                ts = int(time.time())
-                value = random.random()
-                await siri.insert({'some_measurement': [[ts, value]]})
-        
-                # query
-                resp = await siri.query('select * from "some_measurement"')
-                print(resp)
-        
-            finally:
-                # Close all SiriDB connections.
-                siri.close()
-        
-        
-        siri = SiriDBClient(
-            username='iris',
-            password='siri',
-            dbname='dbtest',
-            hostlist=[('localhost', 9000)],  # Multiple connections are supported
-            keepalive=True)
-        
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(example(siri))
-        ```
-        
-        
-        ## SiriDBClient
-        Create a new SiriDB Client. This creates a new client but `.connect()` must be used to connect.
-        
-        ```python
-        siri = SiriDBClient(
-            username=<username>,
-            password=<password>,
-            dbname=<dbname>,
-            hostlist=[(<host>, <port>, {weight: 1}, {backup: False})],
-            loop=None,
-            keepalive=True,
-            timeout=10,
-            inactive_time=30,
-            max_wait_retry=90)
-        ```
-        
-        Arguments:
-        * __username__: User with permissions to use the database.
-        * __password__: Password for the given username.
-        * __dbname__: Name of the database.
-        * __hostlist__: List with SiriDB servers (all servers or a subset of
-        servers can be in this list).
-        
-        
-            *Example:*
-            ```python
-            hostlist=[ ('server1.local', 9000, {'weight': 3}),
-                       ('server2.local', 9001),
-                       ('backup1.local', 9002, {'backup': True}) ]
-            ```
-            Each server should at least have a hostname and port
-            number. Optionally you can provide a dictionary with
-            extra options.
-        
-            Available Options:
-            - __weight__ : Should be a value between 1 and 9. A higher
-                        value gives the server more weight so it will
-                        be more likely chosen. (default 1)
-            - __backup__ : Should be either True or False. When True the
-                        server will be marked as backup server and
-                        will only be chosen if no other server is
-                        available. (default: False)
-        
-        
-        Keyword arguments:
-        * __loop__: Asyncio loop. When 'None' the default event loop will be used.
-        * __keepalive__: When 'True' keep-alive packages are send every 45 seconds.
-        * __timeout__: Maximum time to complete a process, otherwise it will be cancelled.
-        * __inactive_time__: When a server is temporary unavailable, for
-        example the server could be paused, we mark the server as inactive after x seconds.
-        * __max_wait_retry__: When the reconnect loop starts, we try to reconnect in 1 second, then 2 seconds, 4, 8 and so on until max_wait_retry is reached and then use this value to retry again.
-        ******************************************************************************
-        
-        ### SiriDBClient.connect
-        
-        Start connecting to SiriDB. `.connect()` returns a list of all connections referring to the supplied hostlist. The list can contain exceptions in case a connection could not be made.
-        
-        Optionally the keyword argument `timeout` can be set. This will constrain the search time for a connection. Exceeding the timeout will raise an `.TimeoutError`.
-        
-        ```python
-        siri.connect(timeout=None)
-        ```
-        
-        ### SiriDBClient.insert
-        
-        Insert time series data into SiriDB. Requires a 'dictionary' with at least one series.
-        Optionally the `timeout` can be adjusted (default: 300).
-        
-        ```python
-        siri.insert(data, timeout=300)
-        ```
-        
-        ### SiriDBClient.query
-        
-        Query data out of the database. Requires a string containing the query. More about the query language can be found [here](https://siridb.net/documentation/). The documentation about the query language will inform you about a number of useful aggregation and filter functions, different ways of visualizing and grouping the requested data, and how to make changes to the set up of the database. Optionally a `time_precision` (`SECOND`, `MICROSECOND`, `MILLISECOND`, `NANOSECOND`) can be set. The default `None` sets the precision to seconds. Futhermore the `timeout` can be adjusted (default: 60).
-        
-        ```python
-        from siridb.connector import (SECOND,
-                                      MICROSECOND,
-                                      MILLISECOND,
-                                      NANOSECOND)
-        
-        siri.query(query, time_precision=None, timeout=60)
-        ```
-        
-        ### SiriDBClient.close
-        
-        Close the connection.
-        
-        ```python
-        siri.close()
-        ```
-        
-        Check if the connection is closed.
-        
-        ```python
-        siri.is_closed
-        ```
-        
-        ## Exception codes
-        
-        The following exceptions can be returned:
-        
-        - `AuthenticationError`:
-         *Raised when credentials are invalid or insufficient.*
-        - `IndexError`:
-        *Raised when the database does not exist (anymore).*
-        - `InsertError` (can only be raised when using the `.insert()` method):
-         *Make sure the data is correct because this only happens when SiriDB could not process the request.*
-        - `OverflowError` (can only be raised when using the `.insert()` method):
-         *Raised when integer values cannot not be packed due to an overflow error (integer values should be signed and not more than 63 bits).*
-        - `PoolError`:
-         *SiriDB has no online server for at least one required pool. Try again later after some reasonable delay.*
-        - `QueryError` (can only be raised when using the `.query()` method):
-         *Make sure the query is correct because this only happens when SiriDB could not process the query. Consult the [documentation](https://siridb.net/documentation/#help_select) about the query language can be found.*
-        - `RuntimeError`:
-         *Raised when a general error message is received. This should no happen unless a new bug is discovered.*
-        - `ServerError`:
-         *Raised when a server could not perform the request, you could try another server if one is available. Consult the [documentation](https://siridb.net/documentation/#help_list_servers) how to get additional status information about the servers.*
-        - `TimeoutError`:
-         *Raised when a process lasts longer than the `timeout` period*
-        - `TypeError`:
-         *Raised when an unknown package is received (might be caused by running a different SiriDB version).*
-        - `UserAuthError`:
-         *The user as no rights to perform the insert or query. Consult the [documentation](https://siridb.net/documentation/#help_access) how to change the access rights.*
-        
-        
 Keywords: siridb,connector,database,client
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -225,7 +19,216 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+SiriDB - Connector
+==================
+
+The SiriDB Connector is a self-contained Python driver for communicating with SiriDB servers.
+This manual describes how to install and configure SiriDB Connector for Python 3, and how to use it to develop database applications.
+
+
+---------------------------------------
+  * [Installation](#installation)
+  * [Quick usage](#quick-usage)
+  * [SiriDBClient](#siridbclient)
+    * [connect](#siridbclientconnect)
+    * [insert](#siridbclientinsert)
+    * [query](#siridbclientquery)
+    * [close](#siridbclientclose)
+  * [Exception codes](#exception-codes)
+  * [Version info](#version-info)
+
+---------------------------------------
+
+## Installation
+------------
+
+From PyPI (recommended)
+
+```
+pip install siridb-connector
+```
+
+From source code
+
+```
+python setup.py install
+```
+
+
+## Quick usage
+-------
+
+```python
+import asyncio
+import time
+import random
+from siridb.connector import SiriDBClient
+
+async def example(siri):
+    # Start connecting to SiriDB.
+    # .connect() returns a list of all connections referring to the supplied
+    # hostlist. The list can contain exceptions in case a connection could not
+    # be made.
+    await siri.connect()
+
+    try:
+        # insert
+        ts = int(time.time())
+        value = random.random()
+        await siri.insert({'some_measurement': [[ts, value]]})
+
+        # query
+        resp = await siri.query('select * from "some_measurement"')
+        print(resp)
+
+    finally:
+        # Close all SiriDB connections.
+        siri.close()
+
+
+siri = SiriDBClient(
+    username='iris',
+    password='siri',
+    dbname='dbtest',
+    hostlist=[('localhost', 9000)],  # Multiple connections are supported
+    keepalive=True)
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(example(siri))
+```
+
+
+## SiriDBClient
+Create a new SiriDB Client. This creates a new client but `.connect()` must be used to connect.
+
+```python
+siri = SiriDBClient(
+    username=<username>,
+    password=<password>,
+    dbname=<dbname>,
+    hostlist=[(<host>, <port>, {weight: 1}, {backup: False})],
+    loop=None,
+    keepalive=True,
+    timeout=10,
+    inactive_time=30,
+    max_wait_retry=90)
+```
+
+Arguments:
+* __username__: User with permissions to use the database.
+* __password__: Password for the given username.
+* __dbname__: Name of the database.
+* __hostlist__: List with SiriDB servers (all servers or a subset of
+servers can be in this list).
+
+
+    *Example:*
+    ```python
+    hostlist=[ ('server1.local', 9000, {'weight': 3}),
+               ('server2.local', 9001),
+               ('backup1.local', 9002, {'backup': True}) ]
+    ```
+    Each server should at least have a hostname and port
+    number. Optionally you can provide a dictionary with
+    extra options.
+
+    Available Options:
+    - __weight__ : Should be a value between 1 and 9. A higher
+                value gives the server more weight so it will
+                be more likely chosen. (default 1)
+    - __backup__ : Should be either True or False. When True the
+                server will be marked as backup server and
+                will only be chosen if no other server is
+                available. (default: False)
+
+
+Keyword arguments:
+* __loop__: Asyncio loop. When 'None' the default event loop will be used.
+* __keepalive__: When 'True' keep-alive packages are send every 45 seconds.
+* __timeout__: Maximum time to complete a process, otherwise it will be cancelled.
+* __inactive_time__: When a server is temporary unavailable, for
+example the server could be paused, we mark the server as inactive after x seconds.
+* __max_wait_retry__: When the reconnect loop starts, we try to reconnect in 1 second, then 2 seconds, 4, 8 and so on until max_wait_retry is reached and then use this value to retry again.
+******************************************************************************
+
+### SiriDBClient.connect
+
+Start connecting to SiriDB. `.connect()` returns a list of all connections referring to the supplied hostlist. The list can contain exceptions in case a connection could not be made.
+
+Optionally the keyword argument `timeout` can be set. This will constrain the search time for a connection. Exceeding the timeout will raise an `.TimeoutError`.
+
+```python
+siri.connect(timeout=None)
+```
+
+### SiriDBClient.insert
+
+Insert time series data into SiriDB. Requires a 'dictionary' with at least one series.
+Optionally the `timeout` can be adjusted (default: 300).
+
+```python
+siri.insert(data, timeout=300)
+```
+
+### SiriDBClient.query
+
+Query data out of the database. Requires a string containing the query. More about the query language can be found [here](https://siridb.net/documentation/). The documentation about the query language will inform you about a number of useful aggregation and filter functions, different ways of visualizing and grouping the requested data, and how to make changes to the set up of the database. Optionally a `time_precision` (`SECOND`, `MICROSECOND`, `MILLISECOND`, `NANOSECOND`) can be set. The default `None` sets the precision to seconds. Futhermore the `timeout` can be adjusted (default: 60).
+
+```python
+from siridb.connector import (SECOND,
+                              MICROSECOND,
+                              MILLISECOND,
+                              NANOSECOND)
+
+siri.query(query, time_precision=None, timeout=60)
+```
+
+### SiriDBClient.close
+
+Close the connection.
+
+```python
+siri.close()
+```
+
+Check if the connection is closed.
+
+```python
+siri.is_closed
+```
+
+## Exception codes
+
+The following exceptions can be returned:
+
+- `AuthenticationError`:
+ *Raised when credentials are invalid or insufficient.*
+- `IndexError`:
+*Raised when the database does not exist (anymore).*
+- `InsertError` (can only be raised when using the `.insert()` method):
+ *Make sure the data is correct because this only happens when SiriDB could not process the request.*
+- `OverflowError` (can only be raised when using the `.insert()` method):
+ *Raised when integer values cannot not be packed due to an overflow error (integer values should be signed and not more than 63 bits).*
+- `PoolError`:
+ *SiriDB has no online server for at least one required pool. Try again later after some reasonable delay.*
+- `QueryError` (can only be raised when using the `.query()` method):
+ *Make sure the query is correct because this only happens when SiriDB could not process the query. Consult the [documentation](https://siridb.net/documentation/#help_select) about the query language can be found.*
+- `RuntimeError`:
+ *Raised when a general error message is received. This should no happen unless a new bug is discovered.*
+- `ServerError`:
+ *Raised when a server could not perform the request, you could try another server if one is available. Consult the [documentation](https://siridb.net/documentation/#help_list_servers) how to get additional status information about the servers.*
+- `TimeoutError`:
+ *Raised when a process lasts longer than the `timeout` period*
+- `TypeError`:
+ *Raised when an unknown package is received (might be caused by running a different SiriDB version).*
+- `UserAuthError`:
+ *The user as no rights to perform the insert or query. Consult the [documentation](https://siridb.net/documentation/#help_access) how to change the access rights.*
+
+
+
```

### Comparing `siridb-connector-2.1.2/README.md` & `siridb-connector-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/setup.py` & `siridb-connector-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb/connector/__init__.py` & `siridb-connector-2.1.3/siridb/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb/connector/lib/client.py` & `siridb-connector-2.1.3/siridb/connector/lib/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 :copyright: 2022, Jeroen van der Heijden (Cesbit.com)
 '''
 import asyncio
 import functools
 import random
 from .protocol import _SiriDBProtocol, _SiriDBConnProtocol
 from .connection import SiriDBAsyncConnection
-from .exceptions import AuthenticationError
 from .exceptions import ServerError
 from .exceptions import PoolError
 from .constants import SECOND
 from .constants import MICROSECOND
 from .constants import MILLISECOND
 from .constants import NANOSECOND
 from .protomap import CPROTO_REQ_QUERY
@@ -327,15 +326,15 @@
         raise PoolError('No available connections found')
 
 
 class SiriDBConn:
 
     MAX_RECONNECT_WAIT_TIME = 60
     MAX_RECONNECT_TIMEOUT = 10
-    MAX_WRITE_RETRY = 600
+    MAX_WRITE_RETRY = 120
     RECONNECT_ATTEMPT = 3
 
     def __init__(self,
                  username,
                  password,
                  dbname,
                  server,
@@ -456,15 +455,18 @@
                     logging.info('Wait for a connection')
                 await self._reconnect()  # ensure the re-connect loop
                 continue
 
             try:
                 res = await self._protocol.send_package(
                     tipe, data, is_binary, timeout)
-            except Exception as e:
+            except (ServerError,
+                    PoolError,
+                    OSError,
+                    asyncio.TimeoutError) as e:
                 if retry > self.MAX_WRITE_RETRY:
                     raise e
                 if retry % self.RECONNECT_ATTEMPT == 0:
                     await self._reconnect()
                 else:
                     await asyncio.sleep(1.0)
                 continue
```

### Comparing `siridb-connector-2.1.2/siridb/connector/lib/connection.py` & `siridb-connector-2.1.3/siridb/connector/lib/connection.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb/connector/lib/datapackage.py` & `siridb-connector-2.1.3/siridb/connector/lib/datapackage.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb/connector/lib/protocol.py` & `siridb-connector-2.1.3/siridb/connector/lib/protocol.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb/connector/lib/protomap.py` & `siridb-connector-2.1.3/siridb/connector/lib/protomap.py`

 * *Files identical despite different names*

### Comparing `siridb-connector-2.1.2/siridb_connector.egg-info/PKG-INFO` & `siridb-connector-2.1.3/siridb_connector.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,222 +1,16 @@
 Metadata-Version: 2.1
 Name: siridb-connector
-Version: 2.1.2
+Version: 2.1.3
 Summary: SiriDB Connector
 Home-page: https://github.com/SiriDB/siridb-connector
+Download-URL: https://github.com/SiriDB/siridb-connector/tarball/2.1.3
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: UNKNOWN
-Download-URL: https://github.com/SiriDB/siridb-connector/tarball/2.1.2
-Description: SiriDB - Connector
-        ==================
-        
-        The SiriDB Connector is a self-contained Python driver for communicating with SiriDB servers.
-        This manual describes how to install and configure SiriDB Connector for Python 3, and how to use it to develop database applications.
-        
-        
-        ---------------------------------------
-          * [Installation](#installation)
-          * [Quick usage](#quick-usage)
-          * [SiriDBClient](#siridbclient)
-            * [connect](#siridbclientconnect)
-            * [insert](#siridbclientinsert)
-            * [query](#siridbclientquery)
-            * [close](#siridbclientclose)
-          * [Exception codes](#exception-codes)
-          * [Version info](#version-info)
-        
-        ---------------------------------------
-        
-        ## Installation
-        ------------
-        
-        From PyPI (recommended)
-        
-        ```
-        pip install siridb-connector
-        ```
-        
-        From source code
-        
-        ```
-        python setup.py install
-        ```
-        
-        
-        ## Quick usage
-        -------
-        
-        ```python
-        import asyncio
-        import time
-        import random
-        from siridb.connector import SiriDBClient
-        
-        async def example(siri):
-            # Start connecting to SiriDB.
-            # .connect() returns a list of all connections referring to the supplied
-            # hostlist. The list can contain exceptions in case a connection could not
-            # be made.
-            await siri.connect()
-        
-            try:
-                # insert
-                ts = int(time.time())
-                value = random.random()
-                await siri.insert({'some_measurement': [[ts, value]]})
-        
-                # query
-                resp = await siri.query('select * from "some_measurement"')
-                print(resp)
-        
-            finally:
-                # Close all SiriDB connections.
-                siri.close()
-        
-        
-        siri = SiriDBClient(
-            username='iris',
-            password='siri',
-            dbname='dbtest',
-            hostlist=[('localhost', 9000)],  # Multiple connections are supported
-            keepalive=True)
-        
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(example(siri))
-        ```
-        
-        
-        ## SiriDBClient
-        Create a new SiriDB Client. This creates a new client but `.connect()` must be used to connect.
-        
-        ```python
-        siri = SiriDBClient(
-            username=<username>,
-            password=<password>,
-            dbname=<dbname>,
-            hostlist=[(<host>, <port>, {weight: 1}, {backup: False})],
-            loop=None,
-            keepalive=True,
-            timeout=10,
-            inactive_time=30,
-            max_wait_retry=90)
-        ```
-        
-        Arguments:
-        * __username__: User with permissions to use the database.
-        * __password__: Password for the given username.
-        * __dbname__: Name of the database.
-        * __hostlist__: List with SiriDB servers (all servers or a subset of
-        servers can be in this list).
-        
-        
-            *Example:*
-            ```python
-            hostlist=[ ('server1.local', 9000, {'weight': 3}),
-                       ('server2.local', 9001),
-                       ('backup1.local', 9002, {'backup': True}) ]
-            ```
-            Each server should at least have a hostname and port
-            number. Optionally you can provide a dictionary with
-            extra options.
-        
-            Available Options:
-            - __weight__ : Should be a value between 1 and 9. A higher
-                        value gives the server more weight so it will
-                        be more likely chosen. (default 1)
-            - __backup__ : Should be either True or False. When True the
-                        server will be marked as backup server and
-                        will only be chosen if no other server is
-                        available. (default: False)
-        
-        
-        Keyword arguments:
-        * __loop__: Asyncio loop. When 'None' the default event loop will be used.
-        * __keepalive__: When 'True' keep-alive packages are send every 45 seconds.
-        * __timeout__: Maximum time to complete a process, otherwise it will be cancelled.
-        * __inactive_time__: When a server is temporary unavailable, for
-        example the server could be paused, we mark the server as inactive after x seconds.
-        * __max_wait_retry__: When the reconnect loop starts, we try to reconnect in 1 second, then 2 seconds, 4, 8 and so on until max_wait_retry is reached and then use this value to retry again.
-        ******************************************************************************
-        
-        ### SiriDBClient.connect
-        
-        Start connecting to SiriDB. `.connect()` returns a list of all connections referring to the supplied hostlist. The list can contain exceptions in case a connection could not be made.
-        
-        Optionally the keyword argument `timeout` can be set. This will constrain the search time for a connection. Exceeding the timeout will raise an `.TimeoutError`.
-        
-        ```python
-        siri.connect(timeout=None)
-        ```
-        
-        ### SiriDBClient.insert
-        
-        Insert time series data into SiriDB. Requires a 'dictionary' with at least one series.
-        Optionally the `timeout` can be adjusted (default: 300).
-        
-        ```python
-        siri.insert(data, timeout=300)
-        ```
-        
-        ### SiriDBClient.query
-        
-        Query data out of the database. Requires a string containing the query. More about the query language can be found [here](https://siridb.net/documentation/). The documentation about the query language will inform you about a number of useful aggregation and filter functions, different ways of visualizing and grouping the requested data, and how to make changes to the set up of the database. Optionally a `time_precision` (`SECOND`, `MICROSECOND`, `MILLISECOND`, `NANOSECOND`) can be set. The default `None` sets the precision to seconds. Futhermore the `timeout` can be adjusted (default: 60).
-        
-        ```python
-        from siridb.connector import (SECOND,
-                                      MICROSECOND,
-                                      MILLISECOND,
-                                      NANOSECOND)
-        
-        siri.query(query, time_precision=None, timeout=60)
-        ```
-        
-        ### SiriDBClient.close
-        
-        Close the connection.
-        
-        ```python
-        siri.close()
-        ```
-        
-        Check if the connection is closed.
-        
-        ```python
-        siri.is_closed
-        ```
-        
-        ## Exception codes
-        
-        The following exceptions can be returned:
-        
-        - `AuthenticationError`:
-         *Raised when credentials are invalid or insufficient.*
-        - `IndexError`:
-        *Raised when the database does not exist (anymore).*
-        - `InsertError` (can only be raised when using the `.insert()` method):
-         *Make sure the data is correct because this only happens when SiriDB could not process the request.*
-        - `OverflowError` (can only be raised when using the `.insert()` method):
-         *Raised when integer values cannot not be packed due to an overflow error (integer values should be signed and not more than 63 bits).*
-        - `PoolError`:
-         *SiriDB has no online server for at least one required pool. Try again later after some reasonable delay.*
-        - `QueryError` (can only be raised when using the `.query()` method):
-         *Make sure the query is correct because this only happens when SiriDB could not process the query. Consult the [documentation](https://siridb.net/documentation/#help_select) about the query language can be found.*
-        - `RuntimeError`:
-         *Raised when a general error message is received. This should no happen unless a new bug is discovered.*
-        - `ServerError`:
-         *Raised when a server could not perform the request, you could try another server if one is available. Consult the [documentation](https://siridb.net/documentation/#help_list_servers) how to get additional status information about the servers.*
-        - `TimeoutError`:
-         *Raised when a process lasts longer than the `timeout` period*
-        - `TypeError`:
-         *Raised when an unknown package is received (might be caused by running a different SiriDB version).*
-        - `UserAuthError`:
-         *The user as no rights to perform the insert or query. Consult the [documentation](https://siridb.net/documentation/#help_access) how to change the access rights.*
-        
-        
 Keywords: siridb,connector,database,client
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -225,7 +19,216 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+SiriDB - Connector
+==================
+
+The SiriDB Connector is a self-contained Python driver for communicating with SiriDB servers.
+This manual describes how to install and configure SiriDB Connector for Python 3, and how to use it to develop database applications.
+
+
+---------------------------------------
+  * [Installation](#installation)
+  * [Quick usage](#quick-usage)
+  * [SiriDBClient](#siridbclient)
+    * [connect](#siridbclientconnect)
+    * [insert](#siridbclientinsert)
+    * [query](#siridbclientquery)
+    * [close](#siridbclientclose)
+  * [Exception codes](#exception-codes)
+  * [Version info](#version-info)
+
+---------------------------------------
+
+## Installation
+------------
+
+From PyPI (recommended)
+
+```
+pip install siridb-connector
+```
+
+From source code
+
+```
+python setup.py install
+```
+
+
+## Quick usage
+-------
+
+```python
+import asyncio
+import time
+import random
+from siridb.connector import SiriDBClient
+
+async def example(siri):
+    # Start connecting to SiriDB.
+    # .connect() returns a list of all connections referring to the supplied
+    # hostlist. The list can contain exceptions in case a connection could not
+    # be made.
+    await siri.connect()
+
+    try:
+        # insert
+        ts = int(time.time())
+        value = random.random()
+        await siri.insert({'some_measurement': [[ts, value]]})
+
+        # query
+        resp = await siri.query('select * from "some_measurement"')
+        print(resp)
+
+    finally:
+        # Close all SiriDB connections.
+        siri.close()
+
+
+siri = SiriDBClient(
+    username='iris',
+    password='siri',
+    dbname='dbtest',
+    hostlist=[('localhost', 9000)],  # Multiple connections are supported
+    keepalive=True)
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(example(siri))
+```
+
+
+## SiriDBClient
+Create a new SiriDB Client. This creates a new client but `.connect()` must be used to connect.
+
+```python
+siri = SiriDBClient(
+    username=<username>,
+    password=<password>,
+    dbname=<dbname>,
+    hostlist=[(<host>, <port>, {weight: 1}, {backup: False})],
+    loop=None,
+    keepalive=True,
+    timeout=10,
+    inactive_time=30,
+    max_wait_retry=90)
+```
+
+Arguments:
+* __username__: User with permissions to use the database.
+* __password__: Password for the given username.
+* __dbname__: Name of the database.
+* __hostlist__: List with SiriDB servers (all servers or a subset of
+servers can be in this list).
+
+
+    *Example:*
+    ```python
+    hostlist=[ ('server1.local', 9000, {'weight': 3}),
+               ('server2.local', 9001),
+               ('backup1.local', 9002, {'backup': True}) ]
+    ```
+    Each server should at least have a hostname and port
+    number. Optionally you can provide a dictionary with
+    extra options.
+
+    Available Options:
+    - __weight__ : Should be a value between 1 and 9. A higher
+                value gives the server more weight so it will
+                be more likely chosen. (default 1)
+    - __backup__ : Should be either True or False. When True the
+                server will be marked as backup server and
+                will only be chosen if no other server is
+                available. (default: False)
+
+
+Keyword arguments:
+* __loop__: Asyncio loop. When 'None' the default event loop will be used.
+* __keepalive__: When 'True' keep-alive packages are send every 45 seconds.
+* __timeout__: Maximum time to complete a process, otherwise it will be cancelled.
+* __inactive_time__: When a server is temporary unavailable, for
+example the server could be paused, we mark the server as inactive after x seconds.
+* __max_wait_retry__: When the reconnect loop starts, we try to reconnect in 1 second, then 2 seconds, 4, 8 and so on until max_wait_retry is reached and then use this value to retry again.
+******************************************************************************
+
+### SiriDBClient.connect
+
+Start connecting to SiriDB. `.connect()` returns a list of all connections referring to the supplied hostlist. The list can contain exceptions in case a connection could not be made.
+
+Optionally the keyword argument `timeout` can be set. This will constrain the search time for a connection. Exceeding the timeout will raise an `.TimeoutError`.
+
+```python
+siri.connect(timeout=None)
+```
+
+### SiriDBClient.insert
+
+Insert time series data into SiriDB. Requires a 'dictionary' with at least one series.
+Optionally the `timeout` can be adjusted (default: 300).
+
+```python
+siri.insert(data, timeout=300)
+```
+
+### SiriDBClient.query
+
+Query data out of the database. Requires a string containing the query. More about the query language can be found [here](https://siridb.net/documentation/). The documentation about the query language will inform you about a number of useful aggregation and filter functions, different ways of visualizing and grouping the requested data, and how to make changes to the set up of the database. Optionally a `time_precision` (`SECOND`, `MICROSECOND`, `MILLISECOND`, `NANOSECOND`) can be set. The default `None` sets the precision to seconds. Futhermore the `timeout` can be adjusted (default: 60).
+
+```python
+from siridb.connector import (SECOND,
+                              MICROSECOND,
+                              MILLISECOND,
+                              NANOSECOND)
+
+siri.query(query, time_precision=None, timeout=60)
+```
+
+### SiriDBClient.close
+
+Close the connection.
+
+```python
+siri.close()
+```
+
+Check if the connection is closed.
+
+```python
+siri.is_closed
+```
+
+## Exception codes
+
+The following exceptions can be returned:
+
+- `AuthenticationError`:
+ *Raised when credentials are invalid or insufficient.*
+- `IndexError`:
+*Raised when the database does not exist (anymore).*
+- `InsertError` (can only be raised when using the `.insert()` method):
+ *Make sure the data is correct because this only happens when SiriDB could not process the request.*
+- `OverflowError` (can only be raised when using the `.insert()` method):
+ *Raised when integer values cannot not be packed due to an overflow error (integer values should be signed and not more than 63 bits).*
+- `PoolError`:
+ *SiriDB has no online server for at least one required pool. Try again later after some reasonable delay.*
+- `QueryError` (can only be raised when using the `.query()` method):
+ *Make sure the query is correct because this only happens when SiriDB could not process the query. Consult the [documentation](https://siridb.net/documentation/#help_select) about the query language can be found.*
+- `RuntimeError`:
+ *Raised when a general error message is received. This should no happen unless a new bug is discovered.*
+- `ServerError`:
+ *Raised when a server could not perform the request, you could try another server if one is available. Consult the [documentation](https://siridb.net/documentation/#help_list_servers) how to get additional status information about the servers.*
+- `TimeoutError`:
+ *Raised when a process lasts longer than the `timeout` period*
+- `TypeError`:
+ *Raised when an unknown package is received (might be caused by running a different SiriDB version).*
+- `UserAuthError`:
+ *The user as no rights to perform the insert or query. Consult the [documentation](https://siridb.net/documentation/#help_access) how to change the access rights.*
+
+
+
```

### Comparing `siridb-connector-2.1.2/siridb_connector.egg-info/SOURCES.txt` & `siridb-connector-2.1.3/siridb_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

