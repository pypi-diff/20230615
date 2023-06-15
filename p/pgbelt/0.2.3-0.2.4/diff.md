# Comparing `tmp/pgbelt-0.2.3.tar.gz` & `tmp/pgbelt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.2.3.tar", max compression
+gzip compressed data, was "pgbelt-0.2.4.tar", max compression
```

## Comparing `pgbelt-0.2.3.tar` & `pgbelt-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10758 2023-05-04 19:18:44.104060 pgbelt-0.2.3/LICENSE
--rw-r--r--   0        0        0     2047 2023-05-04 19:18:44.104060 pgbelt-0.2.3/README.md
--rw-r--r--   0        0        0      137 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     2275 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5292 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3043 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/login.py
--rw-r--r--   0        0        0     8215 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     3148 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     5082 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     3190 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     8080 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3754 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3817 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/config/config.py
--rw-r--r--   0        0        0     5421 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/config/models.py
--rw-r--r--   0        0        0     5247 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/config/remote.py
--rw-r--r--   0        0        0      186 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/main.py
--rw-r--r--   0        0        0       40 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0     9698 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1424 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/logs.py
--rw-r--r--   0        0        0    12313 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    13669 2023-05-04 19:18:44.108060 pgbelt-0.2.3/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1202 2023-05-04 19:18:44.112060 pgbelt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pgbelt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-06-15 21:23:29.672229 pgbelt-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2047 2023-06-15 21:23:29.672229 pgbelt-0.2.4/README.md
+-rw-r--r--   0        0        0      137 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     2275 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5292 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0     8215 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     3148 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     5082 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     3190 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     8080 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3754 2023-06-15 21:23:29.672229 pgbelt-0.2.4/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3817 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/config/config.py
+-rw-r--r--   0        0        0     5421 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5247 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0     9698 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1424 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    12313 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    13669 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1202 2023-06-15 21:23:29.676229 pgbelt-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 pgbelt-0.2.4/PKG-INFO
```

### Comparing `pgbelt-0.2.3/LICENSE` & `pgbelt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/README.md` & `pgbelt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/convenience.py` & `pgbelt-0.2.4/pgbelt/cmd/convenience.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/helpers.py` & `pgbelt-0.2.4/pgbelt/cmd/helpers.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/login.py` & `pgbelt-0.2.4/pgbelt/cmd/login.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/preflight.py` & `pgbelt-0.2.4/pgbelt/cmd/preflight.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/schema.py` & `pgbelt-0.2.4/pgbelt/cmd/schema.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/setup.py` & `pgbelt-0.2.4/pgbelt/cmd/setup.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/status.py` & `pgbelt-0.2.4/pgbelt/cmd/status.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/sync.py` & `pgbelt-0.2.4/pgbelt/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/cmd/teardown.py` & `pgbelt-0.2.4/pgbelt/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/config/config.py` & `pgbelt-0.2.4/pgbelt/config/config.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/config/models.py` & `pgbelt-0.2.4/pgbelt/config/models.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/config/remote.py` & `pgbelt-0.2.4/pgbelt/config/remote.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/util/asyncfuncs.py` & `pgbelt-0.2.4/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/util/dump.py` & `pgbelt-0.2.4/pgbelt/util/dump.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/util/logs.py` & `pgbelt-0.2.4/pgbelt/util/logs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/util/pglogical.py` & `pgbelt-0.2.4/pgbelt/util/pglogical.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pgbelt/util/postgres.py` & `pgbelt-0.2.4/pgbelt/util/postgres.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.2.3/pyproject.toml` & `pgbelt-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.2.3"
+version = "0.2.4"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.9"
 aiofiles = ">=0.8,<23.2"
 asyncpg = "^0.27.0"
 pydantic = "^1.10.0"
 tabulate = "^0.9.0"
 typer = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pgbelt-0.2.3/PKG-INFO` & `pgbelt-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pgbelt
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
 Author: Varjitt Jeeva
 Author-email: varjitt.jeeva@autodesk.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.8,<23.2)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: pgbelt Version: 0.2.3 Summary: A CLI tool used to
+Metadata-Version: 2.1 Name: pgbelt Version: 0.2.4 Summary: A CLI tool used to
 manage Postgres data migrations from beginning to end, for a single database or
 a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
-varjitt.jeeva@autodesk.com Requires-Python: >=3.11,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (>=0.8,<23.2) Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tabulate
-(>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-
-Type: text/markdown # Pgbelt
+varjitt.jeeva@autodesk.com Requires-Python: >=3.9 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: aiofiles (>=0.8,<23.2) Requires-Dist:
+asyncpg (>=0.27.0,<0.28.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-
+Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown # Pgbelt
       [https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true]
  [Latest_Commit] [https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/
       badge.svg] [https://img.shields.io/github/license/Autodesk/pgbelt]
 PgBelt is a CLI tool used to manage Postgres data migrations from beginning to
 end, for a single database or a fleet, leveraging pglogical replication. It was
 built to assist in migrating data between postgres databases with as little
 application downtime as possible. It works in databases running different
```

