# Comparing `tmp/evatr-client-0.0.1.tar.gz` & `tmp/evatr-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evatr-client-0.0.1.tar", last modified: Thu Jun 15 16:28:51 2023, max compression
+gzip compressed data, was "evatr-client-0.0.2.tar", last modified: Thu Jun 15 17:02:03 2023, max compression
```

## Comparing `evatr-client-0.0.1.tar` & `evatr-client-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:28:51.811005 evatr-client-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-06-15 16:27:48.000000 evatr-client-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      825 2023-06-15 16:28:51.812005 evatr-client-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 16:26:44.000000 evatr-client-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 16:28:51.784006 evatr-client-0.0.1/evatr-client/
--rw-rw-rw-   0        0        0       36 2023-06-15 16:06:16.000000 evatr-client-0.0.1/evatr-client/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-06-15 16:20:36.000000 evatr-client-0.0.1/evatr-client/evatr_client.py
--rw-rw-rw-   0        0        0     4612 2023-06-15 15:56:16.000000 evatr-client-0.0.1/evatr-client/status_codes.py
--rw-rw-rw-   0        0        0     2113 2023-06-15 15:57:13.000000 evatr-client-0.0.1/evatr-client/util.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:28:51.810005 evatr-client-0.0.1/evatr_client.egg-info/
--rw-rw-rw-   0        0        0      825 2023-06-15 16:28:51.000000 evatr-client-0.0.1/evatr_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-15 16:28:51.000000 evatr-client-0.0.1/evatr_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:28:51.000000 evatr-client-0.0.1/evatr_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-15 16:28:51.000000 evatr-client-0.0.1/evatr_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 16:28:51.000000 evatr-client-0.0.1/evatr_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 16:28:51.813004 evatr-client-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-15 16:28:50.000000 evatr-client-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.300916 evatr-client-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-15 16:27:48.000000 evatr-client-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      825 2023-06-15 17:02:03.300916 evatr-client-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1751 2023-06-15 16:53:34.000000 evatr-client-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.291906 evatr-client-0.0.2/evatr_client/
+-rw-rw-rw-   0        0        0      119 2023-06-15 16:57:51.000000 evatr-client-0.0.2/evatr_client/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-06-15 16:20:36.000000 evatr-client-0.0.2/evatr_client/evatr_client.py
+-rw-rw-rw-   0        0        0     4612 2023-06-15 15:56:16.000000 evatr-client-0.0.2/evatr_client/status_codes.py
+-rw-rw-rw-   0        0        0     2113 2023-06-15 15:57:13.000000 evatr-client-0.0.2/evatr_client/util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.299905 evatr-client-0.0.2/evatr_client.egg-info/
+-rw-rw-rw-   0        0        0      825 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 17:02:03.301904 evatr-client-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-15 17:00:13.000000 evatr-client-0.0.2/setup.py
```

### Comparing `evatr-client-0.0.1/LICENSE.txt` & `evatr-client-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.1/PKG-INFO` & `evatr-client-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz
 Author: CeeDiii
 License: MIT
 Keywords: python,uid,vat,uid prüfung,vat validation,evatr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `evatr-client-0.0.1/evatr-client/evatr_client.py` & `evatr-client-0.0.2/evatr_client/evatr_client.py`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.1/evatr-client/status_codes.py` & `evatr-client-0.0.2/evatr_client/status_codes.py`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.1/evatr-client/util.py` & `evatr-client-0.0.2/evatr_client/util.py`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.1/evatr_client.egg-info/PKG-INFO` & `evatr-client-0.0.2/evatr_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz
 Author: CeeDiii
 License: MIT
 Keywords: python,uid,vat,uid prüfung,vat validation,evatr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `evatr-client-0.0.1/setup.py` & `evatr-client-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A client for: https://evatr.bff-online.de/eVatR/'
 LONG_DESCRIPTION = 'A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/'
 
 # Setting up
 setup(
     name="evatr-client",
     version=VERSION,
     author="CeeDiii",
     description=DESCRIPTION,
     license='MIT',
     url='https://github.com/CeeDiii/evatr-client',
-    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.1.tar.gz',
+    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr'],
     install_requires=[
           'requests',
           'urllib3',
```

