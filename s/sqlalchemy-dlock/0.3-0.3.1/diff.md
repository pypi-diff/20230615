# Comparing `tmp/sqlalchemy-dlock-0.3.tar.gz` & `tmp/sqlalchemy-dlock-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-dlock-0.3.tar", last modified: Tue Jun 13 08:15:10 2023, max compression
+gzip compressed data, was "sqlalchemy-dlock-0.3.1.tar", last modified: Thu Jun 15 02:24:29 2023, max compression
```

## Comparing `sqlalchemy-dlock-0.3.tar` & `sqlalchemy-dlock-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.073943 sqlalchemy-dlock-0.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/wait-for-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/scripts/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.073943 sqlalchemy-dlock-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 08:14:56.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 08:15:09.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:15:10.077943 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 08:15:10.000000 sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.925449 sqlalchemy-dlock-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.929449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.929449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/top_level.txt
```

### Comparing `sqlalchemy-dlock-0.3/CHANGELOG.md` & `sqlalchemy-dlock-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## v0.3.1
+
+Date: 2023-06-13
+
+- A hotfix for project's dependencies setup error.
+
 ## v0.3
 
 Date: 2023-06-13
 
 - Remove:
   - Python 3.6 support
```

### Comparing `sqlalchemy-dlock-0.3/LICENSE` & `sqlalchemy-dlock-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3/PKG-INFO` & `sqlalchemy-dlock-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.3
+Version: 0.3.1
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, liu xue yan
         All rights reserved.
         
@@ -217,14 +217,13 @@
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
      ```bash
      cd tests
-     docker compose up --abort-on-container-exit
-     docker compose rm -fsv
+     docker compose up
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
 [asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
```

### Comparing `sqlalchemy-dlock-0.3/README.md` & `sqlalchemy-dlock-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,13 @@
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
      ```bash
      cd tests
-     docker compose up --abort-on-container-exit
-     docker compose rm -fsv
+     docker compose up
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
 [asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
```

### Comparing `sqlalchemy-dlock-0.3/pyproject.toml` & `sqlalchemy-dlock-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 ]
 description = "A distributed lock implementation based on SQLAlchemy"
 keywords = ["SQLAlchemy", "lock", "distributed", "distributed lock", "SQL", "database", "DBMS"]
 license = {file = 'LICENSE'}
 name = "sqlalchemy-dlock"
 readme = {file = 'README.md', content-type = 'text/markdown'}
 requires-python = ">=3.7"
-
+dependencies = [
+  "SQLAlchemy>=1.4.3,<3.0",
+]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/tanbro/sqlalchemy-dlock"
 repository = "https://github.com/tanbro/sqlalchemy-dlock.git"
 
 [tool.setuptools_scm]
@@ -30,16 +32,12 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 127
 
-dependencies = [
-  "SQLAlchemy>=1.4,<3.0",
-]
-
 [options.packages.find]
 where = "src"
 
 [project.optional-dependencies]
 asyncio = ["SQLAlchemy[asyncio]"]
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/functions.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/functions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/mysql.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,31 +39,29 @@
 
 class AsyncSadLock(BaseAsyncSadLock):
     def __init__(
         self,
         connection_or_session: TAsyncConnectionOrSession,
         key,
         convert: Optional[TConvertFunction] = None,
-        *args,
-        **kwargs,
     ):
         if convert:
             key = convert(key)
         elif not isinstance(key, str):
             key = default_convert(key)
         if not isinstance(key, str):
             raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
             raise ValueError(
                 "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
             )
         #
         super().__init__(connection_or_session, key)
 
-    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
+    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
@@ -81,15 +79,15 @@
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
             raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
         else:  # pragma: no cover
             raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
         return self._acquired
 
-    async def release(self, *args, **kwargs):
+    async def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
         stmt = RELEASE_LOCK.params(str=self._key)
         r = await self.connection_or_session.stream(stmt)
         ret_val = (await r.one())[0]
         if ret_val == 1:
             self._acquired = False
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/impl/postgresql.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,14 @@
     def __init__(
         self,
         connection_or_session: TAsyncConnectionOrSession,
         key,
         level: Optional[str] = None,
         interval: Union[float, int, None] = None,
         convert: Optional[TConvertFunction] = None,
-        *args,
-        **kwargs,
     ):
         if convert:
             key = ensure_int64(convert(key))
         elif isinstance(key, int):
             key = ensure_int64(key)
         else:
             key = to_int64_key(key)
@@ -113,16 +111,14 @@
         super().__init__(connection_or_session, key)
 
     async def acquire(
         self,
         block: bool = True,
         timeout: Union[float, int, None] = None,
         interval: Union[float, int, None] = None,
-        *args,
-        **kwargs,
     ) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             if timeout is None:
                 # None: set the timeout period to infinite.
                 stmt = self._stmt_dict["lock"].params(key=self._key)
@@ -153,15 +149,15 @@
             stmt = self._stmt_dict["trylock"].params(key=self._key)
             r = await self.connection_or_session.stream(stmt)
             ret_val = (await r.one())[0]
             self._acquired = bool(ret_val)
         #
         return self._acquired
 
-    async def release(self, *args, **kwargs):
+    async def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
         stmt = self._stmt_dict["unlock"].params(key=self._key)
         r = await self.connection_or_session.stream(stmt)
         ret_val = (await r.one())[0]
         if ret_val:
             self._acquired = False
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/asyncio/types.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/functions.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,19 +17,21 @@
         Connection or Session object SQL locking functions will be invoked on it.
 
     key:
         ID or name of the SQL locking function
 
     Returns
     -------
-        New created lock object, whose type is a subclass of :class:`BaseSadLock`.
+    BaseSadLock
+        New created lock object.
 
-        The actual type of the lock object depends on the type of `connection` object.
+        Type of the lock object is sub-class of :class:`.BaseSadLock`,
+        which depends on the passed-in SQLAlchemy `connection` or `session`.
 
-        MySQL and PostgreSQL are supported til now.
+        MySQL and PostgreSQL connection/session are supported til now.
     """
     if isinstance(connection_or_session, Connection):
         name = safe_name(connection_or_session.engine.name)
     else:
         name = safe_name(connection_or_session.get_bind().name)
     try:
         mod = import_module("..impl.{}".format(name), __name__)
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/mysql.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 
 class SadLock(BaseSadLock):
     """MySQL named-lock
 
     .. seealso:: https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html
     """
 
-    def __init__(
-        self, connection_or_session: TConnectionOrSession, key, convert: Optional[TConvertFunction] = None, *args, **kwargs
-    ):
+    def __init__(self, connection_or_session: TConnectionOrSession, key, convert: Optional[TConvertFunction] = None):
         """
         MySQL named lock requires the key given by string.
 
         If `key` is not a :class:`str`:
 
         - When :class:`int` or :class:`float`,
           the constructor will force convert it to :class:`str`::
@@ -78,15 +76,15 @@
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
             raise ValueError(
                 "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
             )
         #
         super().__init__(connection_or_session, key)
 
-    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
+    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
@@ -102,15 +100,15 @@
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
             raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
         else:  # pragma: no cover
             raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
         return self._acquired
 
-    def release(self, **kwargs):
+    def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
         stmt = RELEASE_LOCK.params(str=self._key)
         ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val == 1:
             self._acquired = False
         elif ret_val == 0:  # pragma: no cover
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/impl/postgresql.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/postgresql.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,16 +96,14 @@
     def __init__(
         self,
         connection_or_session: TConnectionOrSession,
         key,
         level: Optional[str] = None,
         interval: Union[float, int, None] = None,
         convert: Optional[TConvertFunction] = None,
-        *args,
-        **kwargs,
     ):
         """
         PostgreSQL advisory lock requires the key given by ``INT64``.
 
         - When `key` is :class:`int`, the constructor ensures it to be ``INT64``.
           :class:`OverflowError` is raised if too big or too small for an ``INT64``.
 
@@ -149,16 +147,14 @@
         super().__init__(connection_or_session, key)
 
     def acquire(
         self,
         block: bool = True,
         timeout: Union[float, int, None] = None,
         interval: Union[float, int, None] = None,
-        *args,
-        **kwargs,
     ) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             if timeout is None:
                 # None: set the timeout period to infinite.
                 stmt = self._stmt_dict["lock"].params(key=self._key)
@@ -187,15 +183,15 @@
             # or return false without waiting if the lock cannot be acquired immediately.
             stmt = self._stmt_dict["trylock"].params(key=self._key)
             ret_val = self.connection_or_session.execute(stmt).scalar_one()
             self._acquired = bool(ret_val)
         #
         return self._acquired
 
-    def release(self, **kwargs):
+    def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
         stmt = self._stmt_dict["unlock"].params(key=self._key)
         ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val:
             self._acquired = False
         else:
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/types.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock/utils.py` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/PKG-INFO` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.3
+Version: 0.3.1
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, liu xue yan
         All rights reserved.
         
@@ -217,14 +217,13 @@
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
      ```bash
      cd tests
-     docker compose up --abort-on-container-exit
-     docker compose rm -fsv
+     docker compose up
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
 [asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
```

### Comparing `sqlalchemy-dlock-0.3/src/sqlalchemy_dlock.egg-info/SOURCES.txt` & `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-.coveragerc
-.readthedocs.yaml
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-codecov.yml
 pyproject.toml
-scripts/run-test.sh
-scripts/wait-for-mysql.sh
-scripts/wait-for-postgres.sh
 src/sqlalchemy_dlock/__init__.py
 src/sqlalchemy_dlock/exceptions.py
 src/sqlalchemy_dlock/functions.py
 src/sqlalchemy_dlock/types.py
 src/sqlalchemy_dlock/utils.py
 src/sqlalchemy_dlock/version.py
 src/sqlalchemy_dlock.egg-info/PKG-INFO
```

