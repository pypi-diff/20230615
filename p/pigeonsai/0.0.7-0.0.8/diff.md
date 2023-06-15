# Comparing `tmp/pigeonsai-0.0.7.tar.gz` & `tmp/pigeonsai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-0.0.7.tar", last modified: Thu Jun 15 18:29:27 2023, max compression
+gzip compressed data, was "pigeonsai-0.0.8.tar", last modified: Thu Jun 15 18:41:30 2023, max compression
```

## Comparing `pigeonsai-0.0.7.tar` & `pigeonsai-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739722 pigeonsai-0.0.7/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:29:27.739528 pigeonsai-0.0.7/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.7/README.md
--rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-15 18:29:27.739783 pigeonsai-0.0.7/setup.cfg
--rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-15 18:29:07.000000 pigeonsai-0.0.7/setup.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.737229 pigeonsai-0.0.7/src/
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.738095 pigeonsai-0.0.7/src/pigeonsai/
--rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.7/src/pigeonsai/__init__.py
--rw-r--r--   0 ariaattar   (501) staff       (20)     8086 2023-06-15 17:37:51.000000 pigeonsai-0.0.7/src/pigeonsai/pigeonsdb.py
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739010 pigeonsai-0.0.7/src/pigeonsai.egg-info/
--rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       17 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-15 18:29:27.000000 pigeonsai-0.0.7/src/pigeonsai.egg-info/top_level.txt
-drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:29:27.739147 pigeonsai-0.0.7/tests/
--rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.7/tests/test_pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:41:30.383155 pigeonsai-0.0.8/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:41:30.382993 pigeonsai-0.0.8/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)     1508 2023-06-03 00:14:17.000000 pigeonsai-0.0.8/README.md
+-rw-r--r--   0 ariaattar   (501) staff       (20)       38 2023-06-15 18:41:30.383203 pigeonsai-0.0.8/setup.cfg
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2064 2023-06-15 18:41:18.000000 pigeonsai-0.0.8/setup.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:41:30.380933 pigeonsai-0.0.8/src/
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:41:30.381737 pigeonsai-0.0.8/src/pigeonsai/
+-rw-r--r--   0 ariaattar   (501) staff       (20)       32 2023-06-03 00:01:24.000000 pigeonsai-0.0.8/src/pigeonsai/__init__.py
+-rw-r--r--   0 ariaattar   (501) staff       (20)     7830 2023-06-15 18:39:56.000000 pigeonsai-0.0.8/src/pigeonsai/pigeonsdb.py
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:41:30.382561 pigeonsai-0.0.8/src/pigeonsai.egg-info/
+-rw-r--r--   0 ariaattar   (501) staff       (20)     2921 2023-06-15 18:41:30.000000 pigeonsai-0.0.8/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 ariaattar   (501) staff       (20)      279 2023-06-15 18:41:30.000000 pigeonsai-0.0.8/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)        1 2023-06-15 18:41:30.000000 pigeonsai-0.0.8/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       90 2023-06-15 18:41:30.000000 pigeonsai-0.0.8/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 ariaattar   (501) staff       (20)       10 2023-06-15 18:41:30.000000 pigeonsai-0.0.8/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 ariaattar   (501) staff       (20)        0 2023-06-15 18:41:30.382689 pigeonsai-0.0.8/tests/
+-rw-r--r--   0 ariaattar   (501) staff       (20)      609 2023-06-02 23:54:25.000000 pigeonsai-0.0.8/tests/test_pigeonsdb.py
```

### Comparing `pigeonsai-0.0.7/PKG-INFO` & `pigeonsai-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.7
+Version: 0.0.8
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.7/README.md` & `pigeonsai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-0.0.7/setup.py` & `pigeonsai-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="0.0.7",
+    version="0.0.8",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-0.0.7/src/pigeonsai/pigeonsdb.py` & `pigeonsai-0.0.8/src/pigeonsai/pigeonsdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -208,21 +208,7 @@
                     chunk = []
                     tokens_in_chunk = 0
             if chunk:
                 chunks.append(' '.join(chunk))
 
         return chunks
     
-
-
-
-
-
-api_key = "psk-a64360f51474feb264542e6a4a8865c9"
-db_name = "Magic"
-
-PigeonsDB.init(API=api_key, DB_Name=db_name)
-
-# PigeonsDB.add(["This is a good reply", "This is a bad reply"], metadata_list=None)
-
-res = PigeonsDB.search("Bad review", 5)
-print(res)
```

### Comparing `pigeonsai-0.0.7/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-0.0.8/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 0.0.7
+Version: 0.0.8
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://pigeonsai.com/docs
```

### Comparing `pigeonsai-0.0.7/tests/test_pigeonsdb.py` & `pigeonsai-0.0.8/tests/test_pigeonsdb.py`

 * *Files identical despite different names*

