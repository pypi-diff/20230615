# Comparing `tmp/docker-run-cli-0.9.4.tar.gz` & `tmp/docker-run-cli-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-run-cli-0.9.4.tar", last modified: Tue Jun 13 17:06:55 2023, max compression
+gzip compressed data, was "docker-run-cli-0.9.5.tar", last modified: Thu Jun 15 16:44:04 2023, max compression
```

## Comparing `docker-run-cli-0.9.4.tar` & `docker-run-cli-0.9.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.721861 docker-run-cli-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 17:06:55.721861 docker-run-cli-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.717861 docker-run-cli-0.9.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/scripts/activate-python-docker-run-shell-completion
--rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/scripts/docker-run
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:06:55.721861 docker-run-cli-0.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.713861 docker-run-cli-0.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.717861 docker-run-cli-0.9.4/src/docker_run/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.717861 docker-run-cli-0.9.4/src/docker_run/bash_completion.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/bash_completion.d/docker-run
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.717861 docker-run-cli-0.9.4/src/docker_run/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 17:06:43.000000 docker-run-cli-0.9.4/src/docker_run/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:55.717861 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 17:06:55.000000 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-13 17:06:55.000000 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:06:55.000000 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 17:06:55.000000 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 17:06:55.000000 docker-run-cli-0.9.4/src/docker_run_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.498108 docker-run-cli-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-15 16:44:04.498108 docker-run-cli-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.494108 docker-run-cli-0.9.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/scripts/activate-python-docker-run-shell-completion
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/scripts/docker-run
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:44:04.498108 docker-run-cli-0.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.494108 docker-run-cli-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.494108 docker-run-cli-0.9.5/src/docker_run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.494108 docker-run-cli-0.9.5/src/docker_run/bash_completion.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/bash_completion.d/docker-run
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.498108 docker-run-cli-0.9.5/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-15 16:43:55.000000 docker-run-cli-0.9.5/src/docker_run/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:04.498108 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-15 16:44:04.000000 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-15 16:44:04.000000 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:04.000000 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 16:44:04.000000 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:44:04.000000 docker-run-cli-0.9.5/src/docker_run_cli.egg-info/top_level.txt
```

### Comparing `docker-run-cli-0.9.4/LICENSE` & `docker-run-cli-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/PKG-INFO` & `docker-run-cli-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.4
+Version: 0.9.5
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.4 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.5 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
```

### Comparing `docker-run-cli-0.9.4/README.md` & `docker-run-cli-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/pyproject.toml` & `docker-run-cli-0.9.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-cli"
-version = "0.9.4"
+version = "0.9.5"
 description = "'docker run' and 'docker exec' with useful defaults"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
```

### Comparing `docker-run-cli-0.9.4/scripts/activate-python-docker-run-shell-completion` & `docker-run-cli-0.9.5/scripts/activate-python-docker-run-shell-completion`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/scripts/docker-run` & `docker-run-cli-0.9.5/scripts/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run/bash_completion.d/docker-run` & `docker-run-cli-0.9.5/src/docker_run/bash_completion.d/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run/core.py` & `docker-run-cli-0.9.5/src/docker_run/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run/plugins/core.py` & `docker-run-cli-0.9.5/src/docker_run/plugins/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run/plugins/plugin.py` & `docker-run-cli-0.9.5/src/docker_run/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run/utils.py` & `docker-run-cli-0.9.5/src/docker_run/utils.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.4/src/docker_run_cli.egg-info/PKG-INFO` & `docker-run-cli-0.9.5/src/docker_run_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.4
+Version: 0.9.5
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.4 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.5 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
```

### Comparing `docker-run-cli-0.9.4/src/docker_run_cli.egg-info/SOURCES.txt` & `docker-run-cli-0.9.5/src/docker_run_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

