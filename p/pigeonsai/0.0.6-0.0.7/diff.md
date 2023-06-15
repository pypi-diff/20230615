# Comparing `tmp/pigeonsai-0.0.6.tar.gz` & `tmp/pigeonsai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.6.tar", last modified: Mon Jun  5 03:53:45 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.7.tar", last modified: Thu Jun 15 18:29:27 2023, max compression
```

## Comparing `pigeonsai-0.0.6.tar` & `pigeonsai-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-05 03:53:45.485007 pigeonsai-0.0.6/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-05 03:53:45.484855 pigeonsai-0.0.6/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.6/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-05 03:53:45.485055 pigeonsai-0.0.6/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-05 03:53:35.000000 pigeonsai-0.0.6/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-05 03:53:45.482927 pigeonsai-0.0.6/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-05 03:53:45.483707 pigeonsai-0.0.6/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.6/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     2492 2023-06-05 03:53:01.000000 pigeonsai-0.0.6/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-05 03:53:45.484421 pigeonsai-0.0.6/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-05 03:53:45.000000 pigeonsai-0.0.6/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-05 03:53:45.000000 pigeonsai-0.0.6/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-05 03:53:45.000000 pigeonsai-0.0.6/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-05 03:53:45.000000 pigeonsai-0.0.6/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-05 03:53:45.000000 pigeonsai-0.0.6/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-05 03:53:45.484543 pigeonsai-0.0.6/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.6/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739722 pigeonsai-0.0.7/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:29:27.739528 pigeonsai-0.0.7/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.7/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-15 18:29:27.739783 pigeonsai-0.0.7/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-15 18:29:07.000000 pigeonsai-0.0.7/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.737229 pigeonsai-0.0.7/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.738095 pigeonsai-0.0.7/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.7/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     8086 2023-06-15 17:37:51.000000 pigeonsai-0.0.7/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739010 pigeonsai-0.0.7/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739147 pigeonsai-0.0.7/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.7/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.6/PKG-INFO` & `pigeonsai-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.6
+Version: 0.0.7
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.6/README.md` & `pigeonsai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.6/setup.py` & `pigeonsai-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.6",
+    version="0.0.7",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.6/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.7/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.6
+Version: 0.0.7
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.6/tests/test_pigeonsdb.py` & `pigeonsai-0.0.7/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

