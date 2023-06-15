# Comparing `tmp/finops-0.0.3.tar.gz` & `tmp/finops-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.0.3.tar", last modified: Thu Jun 15 19:32:18 2023, max compression
+gzip compressed data, was "finops-0.0.4.tar", last modified: Thu Jun 15 19:36:42 2023, max compression
```

## Comparing `finops-0.0.3.tar` & `finops-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)     1544 2023-06-15 19:06:45.000000 finops-0.0.3/LICENSE
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      637 2023-06-15 19:32:18.519399 finops-0.0.3/PKG-INFO
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:08:19.000000 finops-0.0.3/README.md
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-05 14:53:44.000000 finops-0.0.3/finops/__init__.py
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops/data/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:36.000000 finops-0.0.3/finops/data/__init__.py
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:22.000000 finops-0.0.3/finops/data/shareholders.py
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops.egg-info/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      637 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/PKG-INFO
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      291 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/SOURCES.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        1 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/dependency_links.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       13 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/requires.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       13 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/top_level.txt
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       38 2023-06-15 19:32:18.519399 finops-0.0.3/setup.cfg
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      798 2023-06-15 19:27:54.000000 finops-0.0.3/setup.py
-drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/tests/
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:45.000000 finops-0.0.3/tests/__init__.py
--rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:24:10.000000 finops-0.0.3/tests/test_shareholders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.714764 finops-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-15 19:36:31.000000 finops-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 19:36:42.714764 finops-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/finops/data/shareholders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.710764 finops-0.0.4/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 19:36:42.000000 finops-0.0.4/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:36:42.714764 finops-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 19:36:31.000000 finops-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:42.714764 finops-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:36:31.000000 finops-0.0.4/tests/test_shareholders.py
```

### Comparing `finops-0.0.3/LICENSE` & `finops-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.0.3/PKG-INFO` & `finops-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.0.3/finops.egg-info/PKG-INFO` & `finops-0.0.4/finops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.0.3/setup.py` & `finops-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='finops',
-    version='0.0.3',
+    version='0.0.4',
     description='Financial tools for the rest of us.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

