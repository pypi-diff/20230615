# Comparing `tmp/hugegraph-python-1.0.0.5.tar.gz` & `tmp/hugegraph-python-1.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.5.tar", last modified: Tue Apr 18 04:57:59 2023, max compression
+gzip compressed data, was "dist/hugegraph-python-1.0.0.6.tar", last modified: Thu Jun 15 08:07:07 2023, max compression
```

## Comparing `hugegraph-python-1.0.0.5.tar` & `hugegraph-python-1.0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.532528 hugegraph-python-1.0.0.5/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.5/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-04-18 04:57:59.532228 hugegraph-python-1.0.0.5/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-04-18 04:57:38.000000 hugegraph-python-1.0.0.5/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.531256 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      199 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/top_level.txt
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-04-18 04:57:59.532669 hugegraph-python-1.0.0.5/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-04-18 04:57:46.000000 hugegraph-python-1.0.0.5/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.531598 hugegraph-python-1.0.0.5/test/
--rw-r--r--   0 zsm        (501) staff       (20)      740 2023-04-18 04:56:40.000000 hugegraph-python-1.0.0.5/test/test.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.199756 hugegraph-python-1.0.0.6/
+-rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.6/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:07:07.199341 hugegraph-python-1.0.0.6/PKG-INFO
+-rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-04-18 04:57:38.000000 hugegraph-python-1.0.0.6/README.md
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.197877 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      199 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-06-15 08:07:07.000000 hugegraph-python-1.0.0.6/hugegraph_python.egg-info/top_level.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2023-06-15 08:07:07.199876 hugegraph-python-1.0.0.6/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-06-15 08:05:26.000000 hugegraph-python-1.0.0.6/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-06-15 08:07:07.198428 hugegraph-python-1.0.0.6/test/
+-rw-r--r--   0 zsm        (501) staff       (20)      613 2023-06-15 08:01:51.000000 hugegraph-python-1.0.0.6/test/test.py
```

### Comparing `hugegraph-python-1.0.0.5/LICENSE` & `hugegraph-python-1.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.5/PKG-INFO` & `hugegraph-python-1.0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.5
+Version: 1.0.0.6
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hugegraph-python-1.0.0.5/README.md` & `hugegraph-python-1.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.5/hugegraph_python.egg-info/PKG-INFO` & `hugegraph-python-1.0.0.6/hugegraph_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugegraph-python
-Version: 1.0.0.5
+Version: 1.0.0.6
 Summary: A Python SDK for Apache HugeGraph
 Home-page: https://github.com/cvte-research-datamining/hugegraph-python
 Author: cvte-research-datamining
 Author-email: ming@apache.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hugegraph-python-1.0.0.5/setup.py` & `hugegraph-python-1.0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hugegraph-python",
-    version="1.0.0.5",
+    version="1.0.0.6",
     author="cvte-research-datamining",
     author_email="ming@apache.org",
     description="A Python SDK for Apache HugeGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cvte-research-datamining/hugegraph-python",
     packages=setuptools.find_packages(),
```

