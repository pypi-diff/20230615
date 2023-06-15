# Comparing `tmp/shaku-database-1.0.4.tar.gz` & `tmp/shaku-database-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.0.4.tar", last modified: Thu Jun 15 08:51:45 2023, max compression
+gzip compressed data, was "shaku-database-1.0.5.tar", last modified: Thu Jun 15 09:45:47 2023, max compression
```

## Comparing `shaku-database-1.0.4.tar` & `shaku-database-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:51:45.155099 shaku-database-1.0.4/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.4/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7197 2023-06-15 08:51:45.154991 shaku-database-1.0.4/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.4/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:51:45.154254 shaku-database-1.0.4/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.4/database/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 08:51:45.155140 shaku-database-1.0.4/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1015 2023-06-15 08:51:35.000000 shaku-database-1.0.4/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 08:51:45.154817 shaku-database-1.0.4/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7197 2023-06-15 08:51:45.000000 shaku-database-1.0.4/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      236 2023-06-15 08:51:45.000000 shaku-database-1.0.4/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 08:51:45.000000 shaku-database-1.0.4/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 08:51:45.000000 shaku-database-1.0.4/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 08:51:45.000000 shaku-database-1.0.4/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.521473 shaku-database-1.0.5/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.5/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:45:47.521350 shaku-database-1.0.5/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.5/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.520365 shaku-database-1.0.5/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.5/database/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-15 09:45:47.521516 shaku-database-1.0.5/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1015 2023-06-15 09:45:45.000000 shaku-database-1.0.5/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-15 09:45:47.521166 shaku-database-1.0.5/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      236 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-15 09:45:47.000000 shaku-database-1.0.5/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.0.4/LICENSE` & `shaku-database-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.4/PKG-INFO` & `shaku-database-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.4
+Version: 1.0.5
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: db-dtypes
 Provides-Extra: google-api-core
@@ -121,9 +119,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `shaku-database-1.0.4/README.md` & `shaku-database-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.4/setup.py` & `shaku-database-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = {s.strip().split('==')[0]:s.strip().split('==')[1] if len(s.strip().split('=='))>1 else "" for s in requirements.split("\n")}
 setuptools.setup(
     name="shaku-database",
-    version="1.0.4",
+    version="1.0.5",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=['database'],
```

### Comparing `shaku-database-1.0.4/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.0.5/shaku_database.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.4
+Version: 1.0.5
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: db-dtypes
 Provides-Extra: google-api-core
@@ -121,9 +119,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

