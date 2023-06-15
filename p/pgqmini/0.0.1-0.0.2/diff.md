# Comparing `tmp/pgqmini-0.0.1.tar.gz` & `tmp/pgqmini-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqmini-0.0.1.tar", last modified: Thu Jun 15 17:37:59 2023, max compression
+gzip compressed data, was "pgqmini-0.0.2.tar", last modified: Thu Jun 15 17:50:58 2023, max compression
```

## Comparing `pgqmini-0.0.1.tar` & `pgqmini-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:37:59.909449 pgqmini-0.0.1/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.1/LICENSE
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:37:59.909449 pgqmini-0.0.1/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1977 2023-06-15 17:09:52.000000 pgqmini-0.0.1/README.md
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:37:59.909449 pgqmini-0.0.1/pgqmini/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       63 2023-06-15 17:33:28.000000 pgqmini-0.0.1/pgqmini/__init__.py
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     8629 2023-06-14 17:41:00.000000 pgqmini-0.0.1/pgqmini/pgqmini.py
-drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:37:59.909449 pgqmini-0.0.1/pgqmini.egg-info/
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/PKG-INFO
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      249 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/SOURCES.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/dependency_links.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/not-zip-safe
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/requires.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-15 17:37:59.000000 pgqmini-0.0.1/pgqmini.egg-info/top_level.txt
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-15 17:37:59.909449 pgqmini-0.0.1/setup.cfg
--rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      413 2023-06-15 17:28:38.000000 pgqmini-0.0.1/setup.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1070 2023-06-15 16:54:52.000000 pgqmini-0.0.2/LICENSE
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:50:58.737378 pgqmini-0.0.2/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     1990 2023-06-15 17:48:41.000000 pgqmini-0.0.2/README.md
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/pgqmini/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       60 2023-06-15 17:48:41.000000 pgqmini-0.0.2/pgqmini/__init__.py
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)     8629 2023-06-15 17:48:41.000000 pgqmini-0.0.2/pgqmini/pgq.py
+drwxrwxr-x   0 jangsc0000  (1000) jangsc0000  (1000)        0 2023-06-15 17:50:58.737378 pgqmini-0.0.2/pgqmini.egg-info/
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      290 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/PKG-INFO
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      245 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/SOURCES.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/dependency_links.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        1 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/not-zip-safe
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       16 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/requires.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)        8 2023-06-15 17:50:58.000000 pgqmini-0.0.2/pgqmini.egg-info/top_level.txt
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)       38 2023-06-15 17:50:58.737378 pgqmini-0.0.2/setup.cfg
+-rw-rw-r--   0 jangsc0000  (1000) jangsc0000  (1000)      413 2023-06-15 17:50:36.000000 pgqmini-0.0.2/setup.py
```

### Comparing `pgqmini-0.0.1/LICENSE` & `pgqmini-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqmini-0.0.1/README.md` & `pgqmini-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 You also need to have a PostgreSQL server up and running. The library uses the psycopg2 package to connect to the PostgreSQL server.
 
 ## **Usage**
 
 Here is a basic example of how to use pgqmini:
 
 ### **Publisher**
-```
+```python
 from pgqmini import PGQ
 
 pgq = PGQ(
     qname="message_queue",
     dbname="pgq",
     host="127.0.0.1",
     user="username",
@@ -44,15 +44,15 @@
 
 pgq.pub_message('{"key1": "value1", "key2": "value2"}')
 
 pgq.disconnect()
 ```
 
 ### **Subscriber**
-```
+```python
 from pgqmini import PGQ
 
 pgq = PGQ(
     qname="message_queue",
     dbname="pgq",
     host="127.0.0.1",
     user="username",
@@ -77,8 +77,8 @@
 
 ## **License**
 
 pgqmini is released under the MIT License. See the `LICENSE` file for more details.
 
 ## **Contact**
 
-If you have any questions, issues, or suggestions, please open an issue in this repository, or contact the maintainer at **jangsc0000@gmail.com**.
+If you have any questions, issues, or suggestions, please open an issue in this repository, or contact the maintainer at **jangsc0000@gmail.com**.
```

### Comparing `pgqmini-0.0.1/pgqmini/pgqmini.py` & `pgqmini-0.0.2/pgqmini/pgq.py`

 * *Files identical despite different names*

