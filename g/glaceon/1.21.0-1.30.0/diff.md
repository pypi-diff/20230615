# Comparing `tmp/glaceon-1.21.0.tar.gz` & `tmp/glaceon-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glaceon-1.21.0.tar", last modified: Wed Jun 14 22:46:35 2023, max compression
+gzip compressed data, was "glaceon-1.30.0.tar", last modified: Wed Jun 14 22:41:52 2023, max compression
```

## Comparing `glaceon-1.21.0.tar` & `glaceon-1.30.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:46:35.142461 glaceon-1.21.0/
-drwxrwxrwx   0        0        0        0 2023-06-14 22:46:35.138473 glaceon-1.21.0/GLACEON/
--rw-rw-rw-   0        0        0      323 2023-06-14 22:46:23.000000 glaceon-1.21.0/GLACEON/__init__.py
--rw-rw-rw-   0        0        0     2421 2023-05-20 18:37:28.000000 glaceon-1.21.0/GLACEON/cli.py
--rw-rw-rw-   0        0        0      581 2023-06-14 22:45:19.000000 glaceon-1.21.0/GLACEON/gflask.py
--rw-rw-rw-   0        0        0     3137 2023-06-14 22:46:35.142461 glaceon-1.21.0/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-05-20 18:14:31.000000 glaceon-1.21.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 22:46:35.141464 glaceon-1.21.0/glaceon.egg-info/
--rw-rw-rw-   0        0        0     3137 2023-06-14 22:46:35.000000 glaceon-1.21.0/glaceon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-14 22:46:35.000000 glaceon-1.21.0/glaceon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:46:35.000000 glaceon-1.21.0/glaceon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 22:46:35.000000 glaceon-1.21.0/glaceon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 22:46:35.142461 glaceon-1.21.0/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-06-14 22:46:28.000000 glaceon-1.21.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.859710 glaceon-1.30.0/
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.850513 glaceon-1.30.0/GLACEON/
+-rw-rw-rw-   0        0        0      325 2023-06-14 22:40:02.000000 glaceon-1.30.0/GLACEON/__init__.py
+-rw-rw-rw-   0        0        0     2421 2023-05-20 18:37:28.000000 glaceon-1.30.0/GLACEON/cli.py
+-rw-rw-rw-   0        0        0      573 2023-05-20 18:41:33.000000 glaceon-1.30.0/GLACEON/gflask.py
+-rw-rw-rw-   0        0        0     3137 2023-06-14 22:41:52.859710 glaceon-1.30.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-05-20 18:14:31.000000 glaceon-1.30.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 22:41:52.858713 glaceon-1.30.0/glaceon.egg-info/
+-rw-rw-rw-   0        0        0     3137 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 22:41:52.000000 glaceon-1.30.0/glaceon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:41:52.860704 glaceon-1.30.0/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-06-14 22:40:40.000000 glaceon-1.30.0/setup.py
```

### Comparing `glaceon-1.21.0/GLACEON/cli.py` & `glaceon-1.30.0/GLACEON/cli.py`

 * *Files identical despite different names*

### Comparing `glaceon-1.21.0/GLACEON/gflask.py` & `glaceon-1.30.0/GLACEON/gflask.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 import time
-from GLACEON.cli import cli
+from cli import cli
 
 g = cli(debug=True, speed=2)
 
 class FlaskGlaceon:
 
     def __init__(self, glaceon_instance):
         self.g = glaceon_instance
```

### Comparing `glaceon-1.21.0/PKG-INFO` & `glaceon-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaceon
-Version: 1.21.0
+Version: 1.30.0
 Summary: A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.
 Home-page: https://pypi.python.org/pypi/glaceon
 Author: Zappy
 Author-email: monkey@monk.com
 License: MIT
 Project-URL: Homepage, https://github.com/BornPaster/Glaceon
 Project-URL: Suggestions, https://github.com/BornPaster/Glaceon/issues
```

### Comparing `glaceon-1.21.0/README.md` & `glaceon-1.30.0/README.md`

 * *Files identical despite different names*

### Comparing `glaceon-1.21.0/glaceon.egg-info/PKG-INFO` & `glaceon-1.30.0/glaceon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaceon
-Version: 1.21.0
+Version: 1.30.0
 Summary: A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.
 Home-page: https://pypi.python.org/pypi/glaceon
 Author: Zappy
 Author-email: monkey@monk.com
 License: MIT
 Project-URL: Homepage, https://github.com/BornPaster/Glaceon
 Project-URL: Suggestions, https://github.com/BornPaster/Glaceon/issues
```

### Comparing `glaceon-1.21.0/setup.py` & `glaceon-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
     
 setup(name="glaceon",
-      version="1.21.0",
+      version="1.30.0",
       description="A Simple And Clean Logging Library That Can Be Used For Any Type Of Application.",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
       author="Zappy",
       url="https://pypi.python.org/pypi/glaceon",
       author_email="monkey@monk.com",
```

