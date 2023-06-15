# Comparing `tmp/betby-0.2.6.tar.gz` & `tmp/betby-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.6.tar", last modified: Sun May 14 17:12:11 2023, max compression
+gzip compressed data, was "betby-0.2.7.tar", last modified: Thu Jun 15 12:34:50 2023, max compression
```

## Comparing `betby-0.2.6.tar` & `betby-0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.106006 betby-0.2.6/
--rw-rw-rw-   0        0        0      539 2023-05-14 17:12:11.104007 betby-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.078008 betby-0.2.6/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.6/betby/__init__.py
--rw-rw-rw-   0        0        0     6864 2023-05-14 17:10:07.000000 betby-0.2.6/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.100007 betby-0.2.6/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-14 17:12:10.000000 betby-0.2.6/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 17:12:11.107008 betby-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-14 17:08:16.000000 betby-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:34:50.013244 betby-0.2.7/
+-rw-rw-rw-   0        0        0      539 2023-06-15 12:34:50.012243 betby-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 12:34:49.989243 betby-0.2.7/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.7/betby/__init__.py
+-rw-rw-rw-   0        0        0     8736 2023-06-15 11:56:52.000000 betby-0.2.7/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:34:50.008243 betby-0.2.7/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-06-15 12:34:49.000000 betby-0.2.7/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:34:50.014243 betby-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-06-15 12:00:01.000000 betby-0.2.7/setup.py
```

### Comparing `betby-0.2.6/PKG-INFO` & `betby-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.6
+Version: 0.2.7
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.6/betby.egg-info/PKG-INFO` & `betby-0.2.7/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.6
+Version: 0.2.7
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.6/setup.py` & `betby-0.2.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.6",
+    version="0.2.7",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

