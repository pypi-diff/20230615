# Comparing `tmp/docker-run-docker-ros-1.0.3.tar.gz` & `tmp/docker-run-docker-ros-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-run-docker-ros-1.0.3.tar", last modified: Tue Jun 13 17:07:34 2023, max compression
+gzip compressed data, was "docker-run-docker-ros-1.0.4.tar", last modified: Thu Jun 15 16:44:10 2023, max compression
```

## Comparing `docker-run-docker-ros-1.0.3.tar` & `docker-run-docker-ros-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:34.608324 docker-run-docker-ros-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-13 17:07:05.000000 docker-run-docker-ros-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-13 17:07:34.608324 docker-run-docker-ros-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-13 17:07:05.000000 docker-run-docker-ros-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 17:07:05.000000 docker-run-docker-ros-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:07:34.608324 docker-run-docker-ros-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:34.604324 docker-run-docker-ros-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:34.604324 docker-run-docker-ros-1.0.3/src/docker_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:34.608324 docker-run-docker-ros-1.0.3/src/docker_run/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 17:07:05.000000 docker-run-docker-ros-1.0.3/src/docker_run/plugins/docker_ros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:07:34.608324 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-13 17:07:34.000000 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 17:07:34.000000 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:07:34.000000 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 17:07:34.000000 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 17:07:34.000000 docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/src/docker_run/plugins/docker_ros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/top_level.txt
```

### Comparing `docker-run-docker-ros-1.0.3/LICENSE` & `docker-run-docker-ros-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.3/PKG-INFO` & `docker-run-docker-ros-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.3
+Version: 1.0.4
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

### Comparing `docker-run-docker-ros-1.0.3/README.md` & `docker-run-docker-ros-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.3/pyproject.toml` & `docker-run-docker-ros-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-docker-ros"
-version = "1.0.3"
+version = "1.0.4"
 description = "docker-run plugin for Docker images built by docker-ros"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
```

### Comparing `docker-run-docker-ros-1.0.3/src/docker_run/plugins/docker_ros.py` & `docker-run-docker-ros-1.0.4/src/docker_run/plugins/docker_ros.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import os
 from typing import Any, Dict, List
 
 from docker_run.utils import runCommand
 from docker_run.plugins.plugin import Plugin
 
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 
 class DockerRosPlugin(Plugin):
 
-    TARGET_MOUNT = "/docker-ros/ws/src/target"
+    WORKSPACE = "/docker-ros/ws"
+    TARGET_MOUNT = f"{WORKSPACE}/src/target"
 
     @classmethod
     def addArguments(cls, parser: argparse.ArgumentParser):
 
         prefix = "[docker-ros]"
 
         parser.add_argument("--no-user", action="store_true", help=f"{prefix} disable passing local UID/GID into container")
@@ -47,8 +48,8 @@
 
     @classmethod
     def userExecFlags(cls, user: str) -> List[str]:
         return [f"--user {user}"]
 
     @classmethod
     def currentDirMountWorkspaceFlags(cls) -> List[str]:
-        return [f"--volume {os.getcwd()}:{cls.TARGET_MOUNT}"]
+        return [f"--volume {os.getcwd()}:{cls.TARGET_MOUNT}", f"--workdir {cls.WORKSPACE}"]
```

### Comparing `docker-run-docker-ros-1.0.3/src/docker_run_docker_ros.egg-info/PKG-INFO` & `docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.3
+Version: 1.0.4
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

