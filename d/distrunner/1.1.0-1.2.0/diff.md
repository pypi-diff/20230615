# Comparing `tmp/distrunner-1.1.0.tar.gz` & `tmp/distrunner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distrunner-1.1.0.tar", last modified: Thu Jun 15 09:50:18 2023, max compression
+gzip compressed data, was "distrunner-1.2.0.tar", last modified: Thu Jun 15 10:05:38 2023, max compression
```

## Comparing `distrunner-1.1.0.tar` & `distrunner-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 09:50:18.598068 distrunner-1.1.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 distrunner-1.1.0/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     4491 2023-06-15 09:50:18.598068 distrunner-1.1.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2599 2023-06-14 13:47:04.000000 distrunner-1.1.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1069 2023-06-15 09:48:35.000000 distrunner-1.1.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1032 2023-06-15 09:50:18.598068 distrunner-1.1.0/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 09:50:18.590068 distrunner-1.1.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 09:50:18.594068 distrunner-1.1.0/src/distrunner/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-08 11:26:28.000000 distrunner-1.1.0/src/distrunner/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4867 2023-06-15 09:46:26.000000 distrunner-1.1.0/src/distrunner/distrunner.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      337 2023-06-14 13:46:05.000000 distrunner-1.1.0/src/distrunner/dr_test.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 09:50:18.598068 distrunner-1.1.0/src/distrunner.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     4491 2023-06-15 09:50:18.000000 distrunner-1.1.0/src/distrunner.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      342 2023-06-15 09:50:18.000000 distrunner-1.1.0/src/distrunner.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-15 09:50:18.000000 distrunner-1.1.0/src/distrunner.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      135 2023-06-15 09:50:18.000000 distrunner-1.1.0/src/distrunner.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-06-15 09:50:18.000000 distrunner-1.1.0/src/distrunner.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 09:50:18.598068 distrunner-1.1.0/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2496 2023-06-15 09:32:19.000000 distrunner-1.1.0/tests/test_dist_runner.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 10:05:38.247148 distrunner-1.2.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 distrunner-1.2.0/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4491 2023-06-15 10:05:38.247148 distrunner-1.2.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2599 2023-06-14 13:47:04.000000 distrunner-1.2.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1069 2023-06-15 10:04:55.000000 distrunner-1.2.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1032 2023-06-15 10:05:38.247148 distrunner-1.2.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 10:05:38.247148 distrunner-1.2.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 10:05:38.247148 distrunner-1.2.0/src/distrunner/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-08 11:26:28.000000 distrunner-1.2.0/src/distrunner/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5030 2023-06-15 10:04:55.000000 distrunner-1.2.0/src/distrunner/distrunner.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      337 2023-06-14 13:46:05.000000 distrunner-1.2.0/src/distrunner/dr_test.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 10:05:38.247148 distrunner-1.2.0/src/distrunner.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4491 2023-06-15 10:05:38.000000 distrunner-1.2.0/src/distrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      342 2023-06-15 10:05:38.000000 distrunner-1.2.0/src/distrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-15 10:05:38.000000 distrunner-1.2.0/src/distrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      135 2023-06-15 10:05:38.000000 distrunner-1.2.0/src/distrunner.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-06-15 10:05:38.000000 distrunner-1.2.0/src/distrunner.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-15 10:05:38.247148 distrunner-1.2.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2496 2023-06-15 09:32:19.000000 distrunner-1.2.0/tests/test_dist_runner.py
```

### Comparing `distrunner-1.1.0/LICENSE.md` & `distrunner-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `distrunner-1.1.0/PKG-INFO` & `distrunner-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrunner
-Version: 1.1.0
+Version: 1.2.0
 Summary: This library allows for the easy construction and management of Dask clusters.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `distrunner-1.1.0/README.md` & `distrunner-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `distrunner-1.1.0/pyproject.toml` & `distrunner-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "distrunner"
-version = "1.1.0"
+version = "1.2.0"
 description = "This library allows for the easy construction and management of Dask clusters."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `distrunner-1.1.0/setup.cfg` & `distrunner-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = distrunner
-version = 1.1.0
+version = 1.2.0
 description = This library allows for the easy construction and management of Dask clusters.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = martin@eve.gd
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `distrunner-1.1.0/src/distrunner/distrunner.py` & `distrunner-1.2.0/src/distrunner/distrunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,17 @@
             )
 
             # we don't import coiled until this point because it loads
             # the config file on import
             import coiled
 
             if self._requirements:
-                env = coiled.create_software_environment(pip=self._requirements)
+                env = coiled.create_software_environment(
+                    name=self._application_name, pip=self._requirements
+                )
 
                 self._cluster = coiled.Cluster(
                     name=f"distrunner-{uuid.uuid4()}",
                     n_workers=self._workers,
                     worker_memory=self._worker_memory,
                     worker_cpu=self._worker_cpus,
                     software=env,
@@ -118,14 +120,15 @@
         worker_cpus: int = 2,
         local: bool = False,
         region: str = "eu-west-2",
         api_key_secret_name: str = "LabsAPI/coiled-api-key",
         coiled_account: str = "martin-eve",
         coiled_user: str = "martin-eve",
         requirements: list = None,
+        application_name: str = "distrunner",
     ):
         """
         Initialize a Dask cluster with the specified number of workers.
         :param workers: the number of workers required
         :param worker_memory: the memory in MB to use for workers
         :param worker_cpus: the CPU in milli-cpu (1/1024) to use for workers
         :param local: whether to run the cluster locally
@@ -136,14 +139,15 @@
         self._worker_cpus = worker_cpus
         self._local = local
         self._region = region
         self._api_key_secret_name = api_key_secret_name
         self._coiled_account = coiled_account
         self._coiled_user = coiled_user
         self._requirements = requirements
+        self._application_name = application_name
 
         # create the temporary storage directory
         self._temp_dir = tempfile.TemporaryDirectory()
 
         # internal variables
         self._config_file = pathlib.Path(
             pathlib.Path.home() / ".config" / "dask" / "coiled.yaml"
```

### Comparing `distrunner-1.1.0/src/distrunner.egg-info/PKG-INFO` & `distrunner-1.2.0/src/distrunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distrunner
-Version: 1.1.0
+Version: 1.2.0
 Summary: This library allows for the easy construction and management of Dask clusters.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `distrunner-1.1.0/tests/test_dist_runner.py` & `distrunner-1.2.0/tests/test_dist_runner.py`

 * *Files identical despite different names*

