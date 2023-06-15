# Comparing `tmp/Telexception-0.1.2.tar.gz` & `tmp/Telexception-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telexception-0.1.2.tar", last modified: Thu Jun 15 13:41:15 2023, max compression
+gzip compressed data, was "Telexception-0.1.4.tar", last modified: Thu Jun 15 13:43:58 2023, max compression
```

## Comparing `Telexception-0.1.2.tar` & `Telexception-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:41:15.319989 Telexception-0.1.2/
--rw-r--r--   0 unn        (501) staff       (20)       18 2023-06-15 13:40:19.000000 Telexception-0.1.2/MANIFEST.in
--rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:41:15.319870 Telexception-0.1.2/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)     1486 2023-06-15 13:24:38.000000 Telexception-0.1.2/README.md
-drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:41:15.319536 Telexception-0.1.2/Telexception.egg-info/
--rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:41:15.000000 Telexception-0.1.2/Telexception.egg-info/PKG-INFO
--rw-r--r--   0 unn        (501) staff       (20)      388 2023-06-15 13:41:15.000000 Telexception-0.1.2/Telexception.egg-info/SOURCES.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:41:15.000000 Telexception-0.1.2/Telexception.egg-info/dependency_links.txt
--rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:41:15.000000 Telexception-0.1.2/Telexception.egg-info/requires.txt
--rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:41:15.000000 Telexception-0.1.2/Telexception.egg-info/top_level.txt
--rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:41:15.320028 Telexception-0.1.2/setup.cfg
--rw-r--r--   0 unn        (501) staff       (20)      650 2023-06-15 13:41:11.000000 Telexception-0.1.2/setup.py
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:43:58.525680 Telexception-0.1.4/
+-rw-r--r--   0 unn        (501) staff       (20)       18 2023-06-15 13:40:19.000000 Telexception-0.1.4/MANIFEST.in
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:43:58.525553 Telexception-0.1.4/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)     1486 2023-06-15 13:42:16.000000 Telexception-0.1.4/README.md
+drwxr-xr-x   0 unn        (501) staff       (20)        0 2023-06-15 13:43:58.525203 Telexception-0.1.4/Telexception.egg-info/
+-rw-r--r--   0 unn        (501) staff       (20)     1729 2023-06-15 13:43:58.000000 Telexception-0.1.4/Telexception.egg-info/PKG-INFO
+-rw-r--r--   0 unn        (501) staff       (20)      388 2023-06-15 13:43:58.000000 Telexception-0.1.4/Telexception.egg-info/SOURCES.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:43:58.000000 Telexception-0.1.4/Telexception.egg-info/dependency_links.txt
+-rw-r--r--   0 unn        (501) staff       (20)       26 2023-06-15 13:43:58.000000 Telexception-0.1.4/Telexception.egg-info/requires.txt
+-rw-r--r--   0 unn        (501) staff       (20)        1 2023-06-15 13:43:58.000000 Telexception-0.1.4/Telexception.egg-info/top_level.txt
+-rw-r--r--   0 unn        (501) staff       (20)       38 2023-06-15 13:43:58.525726 Telexception-0.1.4/setup.cfg
+-rw-r--r--   0 unn        (501) staff       (20)      650 2023-06-15 13:42:29.000000 Telexception-0.1.4/setup.py
```

### Comparing `Telexception-0.1.2/PKG-INFO` & `Telexception-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telexception
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python module that sends exception messages to Telegram
 Home-page: https://github.com/UrNickName16/Telexception/
 Author: Andrey Zotov
 Description-Content-Type: text/markdown
 
 # Telexception
```

### Comparing `Telexception-0.1.2/README.md` & `Telexception-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Telexception-0.1.2/Telexception.egg-info/PKG-INFO` & `Telexception-0.1.4/Telexception.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Telexception
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python module that sends exception messages to Telegram
 Home-page: https://github.com/UrNickName16/Telexception/
 Author: Andrey Zotov
 Description-Content-Type: text/markdown
 
 # Telexception
```

### Comparing `Telexception-0.1.2/setup.py` & `Telexception-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Telexception',
-    version='0.1.2',
+    version='0.1.4',
     author='Andrey Zotov',
     description='A Python module that sends exception messages to Telegram',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/UrNickName16/Telexception/',
     packages=find_packages(),
     install_requires=[
```

