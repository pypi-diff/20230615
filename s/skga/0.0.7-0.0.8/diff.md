# Comparing `tmp/skga-0.0.7.tar.gz` & `tmp/skga-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.7.tar", last modified: Thu Jun 15 16:12:26 2023, max compression
+gzip compressed data, was "skga-0.0.8.tar", last modified: Thu Jun 15 16:27:13 2023, max compression
```

## Comparing `skga-0.0.7.tar` & `skga-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.978668 skga-0.0.7/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.7/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:12:26.978490 skga-0.0.7/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.7/README.md
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.7/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 16:12:26.978750 skga-0.0.7/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2382 2023-06-15 16:12:09.000000 skga-0.0.7/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.977173 skga-0.0.7/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.7/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8659 2023-06-15 16:10:12.000000 skga-0.0.7/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.7/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:12:26.978217 skga-0.0.7/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 16:12:26.000000 skga-0.0.7/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:27:13.613741 skga-0.0.8/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.8/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:27:13.613562 skga-0.0.8/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.8/README.md
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.8/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-15 16:27:13.613818 skga-0.0.8/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2397 2023-06-15 16:27:11.000000 skga-0.0.8/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:27:13.609900 skga-0.0.8/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       39 2023-06-15 12:11:54.000000 skga-0.0.8/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8659 2023-06-15 16:10:12.000000 skga-0.0.8/skga/adaptee.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:27:13.613263 skga-0.0.8/skga/hbrkga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)      308 2023-06-15 13:16:50.000000 skga-0.0.8/skga/hbrkga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.8/skga/hbrkga/data_utils.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7539 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/exploitation_method_BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7785 2023-06-15 13:19:37.000000 skga-0.0.8/skga/hbrkga/exploitation_method_BO_only_elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3899 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/exploitation_method_random_search.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2873 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/main-BO-only-elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2575 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/main-BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2585 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/main-randomwalk.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1316 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/nn_decoder_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5042 2023-06-15 13:13:31.000000 skga-0.0.8/skga/hbrkga/nn_instance_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)       62 2023-06-01 19:48:13.000000 skga-0.0.8/skga/hbrkga/test.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.8/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-15 16:27:13.611107 skga-0.0.8/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-15 16:27:13.000000 skga-0.0.8/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      581 2023-06-15 16:27:13.000000 skga-0.0.8/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-15 16:27:13.000000 skga-0.0.8/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-15 16:27:13.000000 skga-0.0.8/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-15 16:27:13.000000 skga-0.0.8/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.7/LICENSE` & `skga-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.7/PKG-INFO` & `skga-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.7
+Version: 0.0.8
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.7/README.md` & `skga-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.7/pyproject.toml` & `skga-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.7/setup.py` & `skga-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.7",
+    version="0.0.8",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    packages=["skga"],
+    packages=["skga", "skga.hbrkga"],
     include_package_data=True,
     install_requires=[
         "bayesian-optimization==1.2.0",
         "bleach==6.0.0",
         "build==0.10.0",
         "certifi==2023.5.7",
         "charset-normalizer==3.1.0",
```

### Comparing `skga-0.0.7/skga/adaptee.py` & `skga-0.0.8/skga/adaptee.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.7/skga/main.py` & `skga-0.0.8/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.7/skga.egg-info/PKG-INFO` & `skga-0.0.8/skga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.7
+Version: 0.0.8
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.7/skga.egg-info/requires.txt` & `skga-0.0.8/skga.egg-info/requires.txt`

 * *Files identical despite different names*

