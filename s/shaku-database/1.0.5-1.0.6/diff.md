# Comparing `tmp/shaku-database-1.0.5.tar.gz` & `tmp/shaku-database-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.0.5.tar", last modified: Thu Jun 15 09:45:47 2023, max compression
+gzip compressed data, was "shaku-database-1.0.6.tar", last modified: Thu Jun 15 09:50:50 2023, max compression
```

## Comparing `shaku-database-1.0.5.tar` & `shaku-database-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.521473 shaku-database-1.0.5/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.5/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:45:47.521350 shaku-database-1.0.5/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.5/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.520365 shaku-database-1.0.5/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.5/database/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 09:45:47.521516 shaku-database-1.0.5/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1015 2023-06-15 09:45:45.000000 shaku-database-1.0.5/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.521166 shaku-database-1.0.5/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      236 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.491097 shaku-database-1.0.6/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.6/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:50:50.490950 shaku-database-1.0.6/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.6/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.488894 shaku-database-1.0.6/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489122 shaku-database-1.0.6/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-15 08:42:39.000000 shaku-database-1.0.6/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489383 shaku-database-1.0.6/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      689 2023-06-08 02:35:46.000000 shaku-database-1.0.6/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.489658 shaku-database-1.0.6/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.6/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-06-08 02:35:46.000000 shaku-database-1.0.6/database/cloud_storage/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 09:50:50.491140 shaku-database-1.0.6/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1056 2023-06-15 09:50:44.000000 shaku-database-1.0.6/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:50:50.490732 shaku-database-1.0.6/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      416 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 09:50:50.000000 shaku-database-1.0.6/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.0.5/LICENSE` & `shaku-database-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.5/PKG-INFO` & `shaku-database-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.5
+Version: 1.0.6
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.0.5/README.md` & `shaku-database-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.5/setup.py` & `shaku-database-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import setuptools
+from setuptools import find_packages, setup
 import pathlib
 
 # 若Discription.md中有中文 須加上 encoding="utf-8"
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
-INSTALL_REQUIRES = {s.strip().split('==')[0]:s.strip().split('==')[1] if len(s.strip().split('=='))>1 else "" for s in requirements.split("\n")}
-setuptools.setup(
+INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else "" for s
+                    in requirements.split("\n")}
+setup(
     name="shaku-database",
-    version="1.0.5",
+    version="1.0.6",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
-    packages=['database'],
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     extras_require=INSTALL_REQUIRES
```

### Comparing `shaku-database-1.0.5/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.0.6/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.5
+Version: 1.0.6
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

