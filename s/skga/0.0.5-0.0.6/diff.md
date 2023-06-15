# Comparing `tmp/skga-0.0.5.tar.gz` & `tmp/skga-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.5.tar", last modified: Thu Jun 15 13:20:19 2023, max compression
+gzip compressed data, was "skga-0.0.6.tar", last modified: Thu Jun 15 13:31:10 2023, max compression
```

## Comparing `skga-0.0.5.tar` & `skga-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:20:19.802753 skga-0.0.5/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.5/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:20:19.802547 skga-0.0.5/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.5/README.md
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.5/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 13:20:19.802829 skga-0.0.5/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2408 2023-06-15 13:20:15.000000 skga-0.0.5/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:20:19.801093 skga-0.0.5/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.5/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8663 2023-06-15 13:13:31.000000 skga-0.0.5/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.5/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:20:19.802258 skga-0.0.5/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:20:19.000000 skga-0.0.5/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-15 13:20:19.000000 skga-0.0.5/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 13:20:19.000000 skga-0.0.5/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      865 2023-06-15 13:20:19.000000 skga-0.0.5/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 13:20:19.000000 skga-0.0.5/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.373540 skga-0.0.6/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.6/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:31:10.373335 skga-0.0.6/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.6/README.md
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.6/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 13:31:10.373613 skga-0.0.6/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2382 2023-06-15 13:31:06.000000 skga-0.0.6/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.371994 skga-0.0.6/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.6/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8663 2023-06-15 13:13:31.000000 skga-0.0.6/skga/adaptee.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.6/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 13:31:10.373048 skga-0.0.6/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 13:31:10.000000 skga-0.0.6/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.5/LICENSE` & `skga-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.5/PKG-INFO` & `skga-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.5
+Version: 0.0.6
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.5/README.md` & `skga-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.5/pyproject.toml` & `skga-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.5/setup.py` & `skga-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.5",
+    version="0.0.6",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
@@ -28,15 +28,14 @@
         "certifi==2023.5.7",
         "charset-normalizer==3.1.0",
         "contourpy==1.0.7",
         "cycler==0.11.0",
         "Cython==0.29.30",
         "docutils==0.19",
         "fonttools==4.39.3",
-        "hbrkga===0.0.1",
         "idna==3.4",
         "importlib-metadata==6.6.0",
         "importlib-resources==5.12.0",
         "jaraco.classes==3.2.3",
         "joblib==1.2.0",
         "keyring==23.13.1",
         "kiwisolver==1.4.4",
```

### Comparing `skga-0.0.5/skga/adaptee.py` & `skga-0.0.6/skga/adaptee.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.5/skga/main.py` & `skga-0.0.6/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.5/skga.egg-info/PKG-INFO` & `skga-0.0.6/skga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.5
+Version: 0.0.6
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.5/skga.egg-info/requires.txt` & `skga-0.0.6/skga.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 certifi==2023.5.7
 charset-normalizer==3.1.0
 contourpy==1.0.7
 cycler==0.11.0
 Cython==0.29.30
 docutils==0.19
 fonttools==4.39.3
-hbrkga===0.0.1
 idna==3.4
 importlib-metadata==6.6.0
 importlib-resources==5.12.0
 jaraco.classes==3.2.3
 joblib==1.2.0
 keyring==23.13.1
 kiwisolver==1.4.4
```

