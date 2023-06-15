# Comparing `tmp/proxidize_wrapper-0.1.1.tar.gz` & `tmp/proxidize_wrapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxidize_wrapper-0.1.1.tar", last modified: Thu Jun 15 01:02:59 2023, max compression
+gzip compressed data, was "proxidize_wrapper-0.2.0.tar", last modified: Thu Jun 15 19:24:19 2023, max compression
```

## Comparing `proxidize_wrapper-0.1.1.tar` & `proxidize_wrapper-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:02:59.151747 proxidize_wrapper-0.1.1/
--rw-rw-rw-   0        0        0     3766 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0        2 2023-06-15 00:49:27.000000 proxidize_wrapper-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1092 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      252 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1824 2023-06-15 01:02:59.151747 proxidize_wrapper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-06-15 00:46:24.000000 proxidize_wrapper-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-15 01:02:59.132814 proxidize_wrapper-0.1.1/docs/
--rw-rw-rw-   0        0        0      638 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0     5067 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      322 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1237 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      815 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       96 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-15 01:02:59.134840 proxidize_wrapper-0.1.1/proxidize_wrapper/
--rw-rw-rw-   0        0        0      182 2023-06-15 01:02:27.000000 proxidize_wrapper-0.1.1/proxidize_wrapper/__init__.py
--rw-rw-rw-   0        0        0      825 2023-06-15 00:36:01.000000 proxidize_wrapper-0.1.1/proxidize_wrapper/proxidize_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:02:59.148748 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/
--rw-rw-rw-   0        0        0     1824 2023-06-15 01:02:59.000000 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-15 01:02:59.000000 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:02:59.000000 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 00:47:05.000000 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-06-15 01:02:59.000000 proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      412 2023-06-15 01:02:59.153256 proxidize_wrapper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-06-15 01:02:29.000000 proxidize_wrapper-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:02:59.150748 proxidize_wrapper-0.1.1/tests/
--rw-rw-rw-   0        0        0       48 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      458 2023-06-15 00:16:30.000000 proxidize_wrapper-0.1.1/tests/test_proxidize_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:24:19.889335 proxidize_wrapper-0.2.0/
+-rw-rw-rw-   0        0        0     3766 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0        2 2023-06-15 00:49:27.000000 proxidize_wrapper-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1092 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1841 2023-06-15 19:24:19.889335 proxidize_wrapper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2023-06-15 08:52:24.000000 proxidize_wrapper-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 19:24:19.859768 proxidize_wrapper-0.2.0/docs/
+-rw-rw-rw-   0        0        0      638 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0     5067 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      322 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1237 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      815 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       96 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 19:24:19.861769 proxidize_wrapper-0.2.0/proxidize_wrapper/
+-rw-rw-rw-   0        0        0      182 2023-06-15 19:23:24.000000 proxidize_wrapper-0.2.0/proxidize_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-06-15 19:10:08.000000 proxidize_wrapper-0.2.0/proxidize_wrapper/proxidize_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:24:19.885303 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     1841 2023-06-15 19:24:19.000000 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-15 19:24:19.000000 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:24:19.000000 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 00:47:05.000000 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-06-15 19:24:19.000000 proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      412 2023-06-15 19:24:19.891343 proxidize_wrapper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-06-15 19:23:10.000000 proxidize_wrapper-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:24:19.887828 proxidize_wrapper-0.2.0/tests/
+-rw-rw-rw-   0        0        0       48 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-06-15 00:16:30.000000 proxidize_wrapper-0.2.0/tests/test_proxidize_wrapper.py
```

### Comparing `proxidize_wrapper-0.1.1/CONTRIBUTING.rst` & `proxidize_wrapper-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/LICENSE` & `proxidize_wrapper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/PKG-INFO` & `proxidize_wrapper-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxidize_wrapper
-Version: 0.1.1
+Version: 0.2.0
 Summary: Wrapper for proxidize android app.
 Home-page: https://github.com/AG4lyf/proxidize_wrapper
 Author: Suraj Bhari
 Author-email: surajbhari159@gmail.com
 License: MIT license
 Keywords: proxidize_wrapper
 Platform: UNKNOWN
@@ -52,15 +52,15 @@
       pip install ec2_proxy
 
 
 .. code-block:: python
 
       from proxidize_wrapper import Proxy
 
-      p = Proxy("IP:PORT:USERNAME:PASSWORD") #Initialize the class object.
+      p = Proxy("127.0.0.1:34517:USERNAME:PASSWORD", "23412") #Initialize the class object.
 
       print(p.get_ip()) # Print the current ip address.
 
       p.change_ip() # change the ip address.
 
       print(p.get_ip()) # Print the current ip address.
```

### Comparing `proxidize_wrapper-0.1.1/README.rst` & `proxidize_wrapper-0.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       pip install ec2_proxy
 
 
 .. code-block:: python
 
       from proxidize_wrapper import Proxy
 
-      p = Proxy("IP:PORT:USERNAME:PASSWORD") #Initialize the class object.
+      p = Proxy("127.0.0.1:34517:USERNAME:PASSWORD", "23412") #Initialize the class object.
 
       print(p.get_ip()) # Print the current ip address.
 
       p.change_ip() # change the ip address.
 
       print(p.get_ip()) # Print the current ip address.
```

### Comparing `proxidize_wrapper-0.1.1/docs/Makefile` & `proxidize_wrapper-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/docs/conf.py` & `proxidize_wrapper-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/docs/installation.rst` & `proxidize_wrapper-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/docs/make.bat` & `proxidize_wrapper-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/PKG-INFO` & `proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxidize-wrapper
-Version: 0.1.1
+Version: 0.2.0
 Summary: Wrapper for proxidize android app.
 Home-page: https://github.com/AG4lyf/proxidize_wrapper
 Author: Suraj Bhari
 Author-email: surajbhari159@gmail.com
 License: MIT license
 Keywords: proxidize_wrapper
 Platform: UNKNOWN
@@ -52,15 +52,15 @@
       pip install ec2_proxy
 
 
 .. code-block:: python
 
       from proxidize_wrapper import Proxy
 
-      p = Proxy("IP:PORT:USERNAME:PASSWORD") #Initialize the class object.
+      p = Proxy("127.0.0.1:34517:USERNAME:PASSWORD", "23412") #Initialize the class object.
 
       print(p.get_ip()) # Print the current ip address.
 
       p.change_ip() # change the ip address.
 
       print(p.get_ip()) # Print the current ip address.
```

### Comparing `proxidize_wrapper-0.1.1/proxidize_wrapper.egg-info/SOURCES.txt` & `proxidize_wrapper-0.2.0/proxidize_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proxidize_wrapper-0.1.1/setup.py` & `proxidize_wrapper-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='proxidize_wrapper',
     name='proxidize_wrapper',
     packages=find_packages(include=['proxidize_wrapper', 'proxidize_wrapper.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/AG4lyf/proxidize_wrapper',
-    version='0.1.1',
+    version='0.2.0',
     zip_safe=False,
 )
```

