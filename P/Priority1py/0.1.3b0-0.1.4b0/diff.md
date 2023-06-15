# Comparing `tmp/Priority1py-0.1.3-beta.tar.gz` & `tmp/Priority1py-0.1.4-beta.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Priority1py-0.1.3-beta.tar", last modified: Thu Jun 15 01:23:55 2023, max compression
+gzip compressed data, was "dist\Priority1py-0.1.4-beta.tar", last modified: Thu Jun 15 01:26:53 2023, max compression
```

## Comparing `Priority1py-0.1.3-beta.tar` & `Priority1py-0.1.4-beta.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:23:55.000000 Priority1py-0.1.3-beta/
--rw-rw-rw-   0        0        0      779 2023-06-15 01:23:55.000000 Priority1py-0.1.3-beta/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 01:23:55.000000 Priority1py-0.1.3-beta/Priority1py/
--rw-rw-rw-   0        0        0     2102 2023-06-14 04:27:50.000000 Priority1py-0.1.3-beta/Priority1py/Priority1py.py
--rw-rw-rw-   0        0        0      129 2023-06-15 01:22:15.000000 Priority1py-0.1.3-beta/Priority1py/__init__.py
--rw-rw-rw-   0        0        0       37 2023-06-14 03:02:08.000000 Priority1py-0.1.3-beta/Priority1py/json.py
--rw-rw-rw-   0        0        0     1225 2023-06-14 03:47:26.000000 Priority1py-0.1.3-beta/Priority1py/request.py
--rw-rw-rw-   0        0        0      591 2023-06-14 03:43:47.000000 Priority1py-0.1.3-beta/Priority1py/strings.py
--rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-0.1.3-beta/setup.cfg
--rw-rw-rw-   0        0        0     1656 2023-06-15 01:22:54.000000 Priority1py-0.1.3-beta/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:26:53.000000 Priority1py-0.1.4-beta/
+-rw-rw-rw-   0        0        0      779 2023-06-15 01:26:53.000000 Priority1py-0.1.4-beta/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 01:26:53.000000 Priority1py-0.1.4-beta/Priority1py/
+-rw-rw-rw-   0        0        0     2102 2023-06-14 04:27:50.000000 Priority1py-0.1.4-beta/Priority1py/Priority1py.py
+-rw-rw-rw-   0        0        0      124 2023-06-15 01:25:18.000000 Priority1py-0.1.4-beta/Priority1py/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-06-14 03:02:08.000000 Priority1py-0.1.4-beta/Priority1py/json.py
+-rw-rw-rw-   0        0        0     1225 2023-06-14 03:47:26.000000 Priority1py-0.1.4-beta/Priority1py/request.py
+-rw-rw-rw-   0        0        0      591 2023-06-14 03:43:47.000000 Priority1py-0.1.4-beta/Priority1py/strings.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:31:48.000000 Priority1py-0.1.4-beta/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-06-15 01:25:47.000000 Priority1py-0.1.4-beta/setup.py
```

### Comparing `Priority1py-0.1.3-beta/PKG-INFO` & `Priority1py-0.1.4-beta/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Priority1py
-Version: 0.1.3-beta
+Version: 0.1.4-beta
 Summary: Priority 1 web API python library
 Home-page: https://github.com/reid10305/Priority1py
 Author: Daniel Pifer
 Author-email: UNKNOWN
 License: MIT
-Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.3-beta.tar.gz
+Download-URL: https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.4-beta.tar.gz
 Description: UNKNOWN
 Keywords: API,Priority1
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Priority1py-0.1.3-beta/Priority1py/Priority1py.py` & `Priority1py-0.1.4-beta/Priority1py/Priority1py.py`

 * *Files identical despite different names*

### Comparing `Priority1py-0.1.3-beta/Priority1py/request.py` & `Priority1py-0.1.4-beta/Priority1py/request.py`

 * *Files identical despite different names*

### Comparing `Priority1py-0.1.3-beta/Priority1py/strings.py` & `Priority1py-0.1.4-beta/Priority1py/strings.py`

 * *Files identical despite different names*

### Comparing `Priority1py-0.1.3-beta/setup.py` & `Priority1py-0.1.4-beta/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from distutils.core import setup
 setup(
   name = 'Priority1py',         # How you named your package folder (MyLib)
   packages = ['Priority1py'],   # Chose the same as "name"
-  version = '0.1.3-beta',      # Start with a small number and increase it with every change you make
+  version = '0.1.4-beta',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Priority 1 web API python library',   # Give a short description about your library
   author = 'Daniel Pifer',                   # Type in your name
   author_email = '',      # Type in your E-Mail
   url = 'https://github.com/reid10305/Priority1py',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.3-beta.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/reid10305/Priority1py/archive/refs/tags/v0.1.4-beta.tar.gz',    # I explain this later on
   keywords = ['API', 'Priority1'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

