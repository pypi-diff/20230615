# Comparing `tmp/pydatawork-0.0.2.tar.gz` & `tmp/pydatawork-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.2.tar", last modified: Thu Jun 15 10:32:21 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.3.tar", last modified: Thu Jun 15 10:40:13 2023, max compression
```

## Comparing `pydatawork-0.0.2.tar` & `pydatawork-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:32:21.000000 pydatawork-0.0.2/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:32:21.000000 pydatawork-0.0.2/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       74 2023-06-15 10:00:20.000000 pydatawork-0.0.2/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:32:21.000000 pydatawork-0.0.2/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:32:21.000000 pydatawork-0.0.2/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-15 10:32:21.000000 pydatawork-0.0.2/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 10:32:21.000000 pydatawork-0.0.2/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-15 10:32:21.000000 pydatawork-0.0.2/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1052 2023-06-15 10:29:59.000000 pydatawork-0.0.2/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 10:32:21.000000 pydatawork-0.0.2/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-15 10:32:15.000000 pydatawork-0.0.2/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:40:13.000000 pydatawork-0.0.3/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:40:13.000000 pydatawork-0.0.3/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       74 2023-06-15 10:00:20.000000 pydatawork-0.0.3/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1052 2023-06-15 10:29:59.000000 pydatawork-0.0.3/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 10:40:13.000000 pydatawork-0.0.3/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-15 10:39:40.000000 pydatawork-0.0.3/setup.py
```

### Comparing `pydatawork-0.0.2/PKG-INFO` & `pydatawork-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.2
+Version: 0.0.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.2/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.3/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.2
+Version: 0.0.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.2/pydatawork.py` & `pydatawork-0.0.3/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.0.2/setup.py` & `pydatawork-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.2',
+    version='0.0.3',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

