# Comparing `tmp/facekiapiclientv2-1.0.tar.gz` & `tmp/facekiapiclientv2-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facekiapiclientv2-1.0.tar", last modified: Thu Jun 15 13:27:48 2023, max compression
+gzip compressed data, was "facekiapiclientv2-1.1.tar", last modified: Thu Jun 15 13:34:09 2023, max compression
```

## Comparing `facekiapiclientv2-1.0.tar` & `facekiapiclientv2-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:27:48.851752 facekiapiclientv2-1.0/
--rw-rw-rw-   0        0        0      587 2023-06-15 13:27:48.851752 facekiapiclientv2-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2023-06-15 13:26:07.000000 facekiapiclientv2-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 13:27:48.845219 facekiapiclientv2-1.0/faceki-kyc-python/
--rw-rw-rw-   0        0        0       72 2023-06-15 13:23:35.000000 facekiapiclientv2-1.0/faceki-kyc-python/__init__.py
--rw-rw-rw-   0        0        0     4534 2023-06-15 13:23:00.000000 facekiapiclientv2-1.0/faceki-kyc-python/client.py
--rw-rw-rw-   0        0        0      198 2023-06-14 13:21:15.000000 facekiapiclientv2-1.0/faceki-kyc-python/test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:27:48.850379 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/
--rw-rw-rw-   0        0        0      587 2023-06-15 13:27:48.000000 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-15 13:27:48.000000 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:27:48.000000 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 13:27:48.000000 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 13:27:48.000000 facekiapiclientv2-1.0/facekiapiclientv2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 13:27:48.852759 facekiapiclientv2-1.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-15 13:27:33.000000 facekiapiclientv2-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.342960 facekiapiclientv2-1.1/
+-rw-rw-rw-   0        0        0     3068 2023-06-15 13:34:09.339773 facekiapiclientv2-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2447 2023-06-15 13:26:07.000000 facekiapiclientv2-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.333724 facekiapiclientv2-1.1/faceki-kyc-python/
+-rw-rw-rw-   0        0        0       72 2023-06-15 13:23:35.000000 facekiapiclientv2-1.1/faceki-kyc-python/__init__.py
+-rw-rw-rw-   0        0        0     4534 2023-06-15 13:23:00.000000 facekiapiclientv2-1.1/faceki-kyc-python/client.py
+-rw-rw-rw-   0        0        0      198 2023-06-14 13:21:15.000000 facekiapiclientv2-1.1/faceki-kyc-python/test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:34:09.338765 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/
+-rw-rw-rw-   0        0        0     3068 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 13:34:09.000000 facekiapiclientv2-1.1/facekiapiclientv2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:34:09.342960 facekiapiclientv2-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-06-15 13:33:59.000000 facekiapiclientv2-1.1/setup.py
```

### Comparing `facekiapiclientv2-1.0/README.md` & `facekiapiclientv2-1.1/README.md`

 * *Files identical despite different names*

### Comparing `facekiapiclientv2-1.0/faceki-kyc-python/client.py` & `facekiapiclientv2-1.1/faceki-kyc-python/client.py`

 * *Files identical despite different names*

### Comparing `facekiapiclientv2-1.0/setup.py` & `facekiapiclientv2-1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='facekiapiclientv2',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     install_requires=['requests'],
     description='FACEKI KYC Api Library',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Faceki',
     author_email='haziq@faceki.com',
     keywords=['api', 'client', 'library'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

