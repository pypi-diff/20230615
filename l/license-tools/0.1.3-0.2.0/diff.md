# Comparing `tmp/license_tools-0.1.3.tar.gz` & `tmp/license_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_tools-0.1.3.tar", last modified: Wed Jun 14 13:20:12 2023, max compression
+gzip compressed data, was "license_tools-0.2.0.tar", last modified: Thu Jun 15 07:57:33 2023, max compression
```

## Comparing `license_tools-0.1.3.tar` & `license_tools-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 13:20:12.148863 license_tools-0.1.3/
--rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.1.3/LICENSE.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-14 13:20:12.148863 license_tools-0.1.3/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-13 14:23:14.000000 license_tools-0.1.3/README.md
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 13:20:12.144863 license_tools-0.1.3/license_tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.1.3/license_tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2427 2023-06-14 10:37:12.000000 license_tools-0.1.3/license_tools/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     9979 2023-06-14 11:47:29.000000 license_tools-0.1.3/license_tools/scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-14 13:20:12.144863 license_tools-0.1.3/license_tools.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-14 13:20:12.000000 license_tools-0.1.3/license_tools.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-14 13:20:12.000000 license_tools-0.1.3/license_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-14 13:20:12.000000 license_tools-0.1.3/license_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-14 13:20:12.000000 license_tools-0.1.3/license_tools.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-14 13:20:12.000000 license_tools-0.1.3/license_tools.egg-info/top_level.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-14 13:20:12.148863 license_tools-0.1.3/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-14 13:13:11.000000 license_tools-0.1.3/setup.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/
+-rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.2.0/LICENSE.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-15 07:57:33.391027 license_tools-0.2.0/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-15 07:55:19.000000 license_tools-0.2.0/README.md
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/license_tools/
+-rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.2.0/license_tools/__init__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     2427 2023-06-14 10:37:12.000000 license_tools-0.2.0/license_tools/__main__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    16055 2023-06-15 07:53:43.000000 license_tools-0.2.0/license_tools/scancode_tools.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/license_tools.egg-info/
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/requires.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/top_level.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-15 07:57:33.391027 license_tools-0.2.0/setup.cfg
+-rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-15 07:54:48.000000 license_tools-0.2.0/setup.py
```

### Comparing `license_tools-0.1.3/LICENSE.txt` & `license_tools-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.1.3/PKG-INFO` & `license_tools-0.2.0/license_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: license_tools
-Version: 0.1.3
+Name: license-tools
+Version: 0.2.0
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.1.3/README.md` & `license_tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `license_tools-0.1.3/license_tools/__main__.py` & `license_tools-0.2.0/license_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.1.3/license_tools.egg-info/PKG-INFO` & `license_tools-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: license-tools
-Version: 0.1.3
+Name: license_tools
+Version: 0.2.0
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.1.3/setup.py` & `license_tools-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setuptools.setup(
     name='license_tools',
     description='Collection of tools for working with Open Source licenses',
-    version='0.1.3',
+    version='0.2.0',
     license='Apache-2.0',
     long_description=Path(ROOT_DIRECTORY / 'README.md').read_text(encoding='UTF-8'),
     long_description_content_type='text/markdown',
     author='stefan6419846',
     url='https://github.com/stefan6419846/license_tools',
     packages=setuptools.find_packages(),
     include_package_data=True,
```

