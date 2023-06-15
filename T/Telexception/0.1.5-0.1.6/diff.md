# Comparing `tmp/Telexception-0.1.5.tar.gz` & `tmp/Telexception-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telexception-0.1.5.tar", last modified: Thu Jun 15 13:51:24 2023, max compression
+gzip compressed data, was "Telexception-0.1.6.tar", last modified: Thu Jun 15 13:54:30 2023, max compression
```

## Comparing `Telexception-0.1.5.tar` & `Telexception-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:51:24.562168 Telexception-0.1.5/
--rw-r--r--   0 unn        (501) staff       (20)       18 2023-06-15 13:44:54.000000 Telexception-0.1.5/MANIFEST.in
--rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:51:24.562027 Telexception-0.1.5/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)     1486 2023-06-15 13:42:16.000000 Telexception-0.1.5/README.md
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:51:24.561690 Telexception-0.1.5/Telexception.egg-info/
--rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)      388 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/SOURCES.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/dependency_links.txt
--rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/requires.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:51:24.000000 Telexception-0.1.5/Telexception.egg-info/top_level.txt
--rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:51:24.562213 Telexception-0.1.5/setup.cfg
--rw-r--r--   0 unn        (501) staff       (20)      650 2023-06-15 13:51:16.000000 Telexception-0.1.5/setup.py
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:54:30.091549 Telexception-0.1.6/
+-rw-r--r--   0 unn        (501) staff       (20)       18 2023-06-15 13:44:54.000000 Telexception-0.1.6/MANIFEST.in
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:54:30.091432 Telexception-0.1.6/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)     1486 2023-06-15 13:42:16.000000 Telexception-0.1.6/README.md
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:54:30.091092 Telexception-0.1.6/Telexception.egg-info/
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:54:30.000000 Telexception-0.1.6/Telexception.egg-info/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)      318 2023-06-15 13:54:30.000000 Telexception-0.1.6/Telexception.egg-info/SOURCES.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:54:30.000000 Telexception-0.1.6/Telexception.egg-info/dependency_links.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:54:30.000000 Telexception-0.1.6/Telexception.egg-info/top_level.txt
+-rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:54:30.091609 Telexception-0.1.6/setup.cfg
+-rw-r--r--   0 unn        (501) staff       (20)      562 2023-06-15 13:54:25.000000 Telexception-0.1.6/setup.py
```

### Comparing `Telexception-0.1.5/PKG-INFO` & `Telexception-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telexception
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python module that sends exception messages to Telegram
 Home-page: https://github.com/UrNickName16/Telexception/
 Author: Andrey Zotov
 Description-Content-Type: text/markdown
 
 # Telexception
```

### Comparing `Telexception-0.1.5/README.md` & `Telexception-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `Telexception-0.1.5/Telexception.egg-info/PKG-INFO` & `Telexception-0.1.6/Telexception.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telexception
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python module that sends exception messages to Telegram
 Home-page: https://github.com/UrNickName16/Telexception/
 Author: Andrey Zotov
 Description-Content-Type: text/markdown
 
 # Telexception
```

### Comparing `Telexception-0.1.5/setup.py` & `Telexception-0.1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Telexception',
-    version='0.1.5',
+    version='0.1.6',
     author='Andrey Zotov',
     description='A Python module that sends exception messages to Telegram',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/UrNickName16/Telexception/',
     packages=find_packages(),
-    install_requires=[
-        'requests',
-        'urllib',
-        'traceback'
-    ],
 )
```

