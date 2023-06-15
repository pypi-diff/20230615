# Comparing `tmp/pgqmini-0.0.2.tar.gz` & `tmp/pgqmini-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqmini-0.0.2.tar", last modified: Thu Jun 15 17:50:58 2023, max compression
+gzip compressed data, was "pgqmini-0.0.3.tar", last modified: Thu Jun 15 18:08:07 2023, max compression
```

## Comparing `pgqmini-0.0.2.tar` & `pgqmini-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.2/LICENSE
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:50:58.737378 pgqmini-0.0.2/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1990 2023-06-15 17:48:41.000000 pgqmini-0.0.2/README.md
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/pgqmini/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       60 2023-06-15 17:48:41.000000 pgqmini-0.0.2/pgqmini/__init__.py
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     8629 2023-06-15 17:48:41.000000 pgqmini-0.0.2/pgqmini/pgq.py
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/pgqmini.egg-info/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/SOURCES.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/dependency_links.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/not-zip-safe
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/requires.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/top_level.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-15 17:50:58.737378 pgqmini-0.0.2/setup.cfg
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      413 2023-06-15 17:50:36.000000 pgqmini-0.0.2/setup.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.3/LICENSE
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2474 2023-06-15 18:08:07.994202 pgqmini-0.0.3/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2143 2023-06-15 18:07:07.000000 pgqmini-0.0.3/README.md
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/pgqmini/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       60 2023-06-15 17:48:41.000000 pgqmini-0.0.3/pgqmini/__init__.py
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     8629 2023-06-15 17:48:41.000000 pgqmini-0.0.3/pgqmini/pgq.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 18:08:07.994202 pgqmini-0.0.3/pgqmini.egg-info/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     2474 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/SOURCES.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/dependency_links.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/not-zip-safe
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/requires.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-15 18:08:07.000000 pgqmini-0.0.3/pgqmini.egg-info/top_level.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-15 18:08:07.994202 pgqmini-0.0.3/setup.cfg
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      582 2023-06-15 18:04:44.000000 pgqmini-0.0.3/setup.py
```

### Comparing `pgqmini-0.0.2/LICENSE` & `pgqmini-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqmini-0.0.2/README.md` & `pgqmini-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **pgqmini**
 
-![version](https://img.shields.io/badge/version-0.0.1-blue)
+![version](https://img.shields.io/badge/version-0.0.3-blue)
 ![license](https://img.shields.io/badge/license-MIT-green)
 
 pgqmini is a lightweight, easy-to-use Python library for managing PostgreSQL message queues. It provides a simple interface for adding and retrieving messages from a PostgreSQL-based queue, as well as handling timeouts and managing message processing.
 
 ## **Table of Contents**
 
 1. **[Installation](#installation)**
@@ -69,14 +69,15 @@
         pgq.complete_message(msg)
     except Exception as e:
         pgq.rollback_message(msg)
 ```
 
 In this code, we first create a **`PGQ`** object with the necessary database connection parameters. We then connect to the database and enter a loop where we process messages from the queue.
 
+For a more detailed usage guide, please check out the [Usage Guide](https://github.com/over-engineers/pgqmini/wiki/PGQ-Class-Documentation) in our wiki.
 
 
 ## **License**
 
 pgqmini is released under the MIT License. See the `LICENSE` file for more details.
 
 ## **Contact**
```

### Comparing `pgqmini-0.0.2/pgqmini/pgq.py` & `pgqmini-0.0.3/pgqmini/pgq.py`

 * *Files identical despite different names*

