# Comparing `tmp/peewee-jsonfield-0.0.2.tar.gz` & `tmp/peewee-jsonfield-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee-jsonfield-0.0.2.tar", last modified: Wed Jun 14 23:27:33 2023, max compression
+gzip compressed data, was "peewee-jsonfield-0.0.3.tar", last modified: Wed Jun 14 23:29:19 2023, max compression
```

## Comparing `peewee-jsonfield-0.0.2.tar` & `peewee-jsonfield-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:27:33.841112 peewee-jsonfield-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-14 22:22:57.000000 peewee-jsonfield-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4017 2023-06-14 23:27:33.840112 peewee-jsonfield-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3514 2023-06-14 23:14:35.000000 peewee-jsonfield-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 23:27:33.834111 peewee-jsonfield-0.0.2/jsonfield/
--rw-rw-rw-   0        0        0     2461 2023-06-14 10:08:18.000000 peewee-jsonfield-0.0.2/jsonfield/jsonfield.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:27:33.839112 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/
--rw-rw-rw-   0        0        0     4017 2023-06-14 23:27:33.000000 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-14 23:27:33.000000 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:27:33.000000 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 23:27:33.000000 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 23:27:33.000000 peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      492 2023-06-14 23:27:09.000000 peewee-jsonfield-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 23:27:33.841112 peewee-jsonfield-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-14 23:27:20.000000 peewee-jsonfield-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:29:19.217145 peewee-jsonfield-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 22:22:57.000000 peewee-jsonfield-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4003 2023-06-14 23:29:19.216147 peewee-jsonfield-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3500 2023-06-14 23:29:03.000000 peewee-jsonfield-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 23:29:19.212143 peewee-jsonfield-0.0.3/jsonfield/
+-rw-rw-rw-   0        0        0     2461 2023-06-14 10:08:18.000000 peewee-jsonfield-0.0.3/jsonfield/jsonfield.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:29:19.216147 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/
+-rw-rw-rw-   0        0        0     4003 2023-06-14 23:29:19.000000 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-14 23:29:19.000000 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:29:19.000000 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 23:29:19.000000 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 23:29:19.000000 peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      492 2023-06-14 23:29:03.000000 peewee-jsonfield-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:29:19.217145 peewee-jsonfield-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-14 23:29:03.000000 peewee-jsonfield-0.0.3/setup.py
```

### Comparing `peewee-jsonfield-0.0.2/LICENSE` & `peewee-jsonfield-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peewee-jsonfield-0.0.2/PKG-INFO` & `peewee-jsonfield-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-jsonfield
-Version: 0.0.2
+Version: 0.0.3
 Summary: JSONField for Peewee
 Author: Mark Smirnov
 Author-email: Mark Smirnov <mark@mark99.ru>
 License: MIT License
 Project-URL: Source code, https://github.com/mark99i/jsonfield
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 This package is a JSONField on steroids for use with [ORM Peewee](https://github.com/coleifer/peewee), 
 adding functions for working with NoSQL data (JSON fields)
 
 By default, in Peewee, JSONField is a simple field inherited from TextField without any settings and additional methods, however, 
 in MySQL/MariaDB there are [many methods](https://mariadb.com/kb/en/json-functions/) for working with JSON data that are either not used or 
 need to be implemented yourself. This package is designed to fix this situation.
 
-## Installation (in progress)
+## Installation
 ```pip install peeewee-jsonfield```
 
 ## Using
 
 Suppose you have a table with a JSON type field, for example:
 
 ```
```

### Comparing `peewee-jsonfield-0.0.2/README.md` & `peewee-jsonfield-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package is a JSONField on steroids for use with [ORM Peewee](https://github.com/coleifer/peewee), 
 adding functions for working with NoSQL data (JSON fields)
 
 By default, in Peewee, JSONField is a simple field inherited from TextField without any settings and additional methods, however, 
 in MySQL/MariaDB there are [many methods](https://mariadb.com/kb/en/json-functions/) for working with JSON data that are either not used or 
 need to be implemented yourself. This package is designed to fix this situation.
 
-## Installation (in progress)
+## Installation
 ```pip install peeewee-jsonfield```
 
 ## Using
 
 Suppose you have a table with a JSON type field, for example:
 
 ```
```

### Comparing `peewee-jsonfield-0.0.2/jsonfield/jsonfield.py` & `peewee-jsonfield-0.0.3/jsonfield/jsonfield.py`

 * *Files identical despite different names*

### Comparing `peewee-jsonfield-0.0.2/peewee_jsonfield.egg-info/PKG-INFO` & `peewee-jsonfield-0.0.3/peewee_jsonfield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-jsonfield
-Version: 0.0.2
+Version: 0.0.3
 Summary: JSONField for Peewee
 Author: Mark Smirnov
 Author-email: Mark Smirnov <mark@mark99.ru>
 License: MIT License
 Project-URL: Source code, https://github.com/mark99i/jsonfield
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 This package is a JSONField on steroids for use with [ORM Peewee](https://github.com/coleifer/peewee), 
 adding functions for working with NoSQL data (JSON fields)
 
 By default, in Peewee, JSONField is a simple field inherited from TextField without any settings and additional methods, however, 
 in MySQL/MariaDB there are [many methods](https://mariadb.com/kb/en/json-functions/) for working with JSON data that are either not used or 
 need to be implemented yourself. This package is designed to fix this situation.
 
-## Installation (in progress)
+## Installation
 ```pip install peeewee-jsonfield```
 
 ## Using
 
 Suppose you have a table with a JSON type field, for example:
 
 ```
```

