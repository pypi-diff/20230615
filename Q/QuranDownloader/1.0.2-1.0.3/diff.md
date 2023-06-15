# Comparing `tmp/QuranDownloader-1.0.2.tar.gz` & `tmp/QuranDownloader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuranDownloader-1.0.2.tar", last modified: Thu Jun 15 14:29:26 2023, max compression
+gzip compressed data, was "QuranDownloader-1.0.3.tar", last modified: Thu Jun 15 14:31:18 2023, max compression
```

## Comparing `QuranDownloader-1.0.2.tar` & `QuranDownloader-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:29:26.353409 QuranDownloader-1.0.2/
--rwxrwxrwx   0 shark     (1000) shark     (1000)     2022 2023-06-15 14:29:26.349427 QuranDownloader-1.0.2/PKG-INFO
-drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:29:26.204411 QuranDownloader-1.0.2/QuranDownloader/
--rwxrwxrwx   0 shark     (1000) shark     (1000)      271 2023-06-08 13:31:10.000000 QuranDownloader-1.0.2/QuranDownloader/__init__.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)      215 2023-06-08 13:19:03.000000 QuranDownloader-1.0.2/QuranDownloader/concurrent_req.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)      417 2023-06-08 13:21:56.000000 QuranDownloader-1.0.2/QuranDownloader/consts.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)     4652 2023-06-05 18:06:50.000000 QuranDownloader-1.0.2/QuranDownloader/download_org.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)     2815 2023-06-08 14:20:12.000000 QuranDownloader-1.0.2/QuranDownloader/download_verse.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)     1509 2023-06-08 13:30:37.000000 QuranDownloader-1.0.2/QuranDownloader/download_word.py
--rwxrwxrwx   0 shark     (1000) shark     (1000)      342 2023-06-05 18:08:56.000000 QuranDownloader-1.0.2/QuranDownloader/verse_key_converters.py
-drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:29:26.325386 QuranDownloader-1.0.2/QuranDownloader.egg-info/
--rwxrwxrwx   0 shark     (1000) shark     (1000)     2022 2023-06-15 14:29:25.000000 QuranDownloader-1.0.2/QuranDownloader.egg-info/PKG-INFO
--rwxrwxrwx   0 shark     (1000) shark     (1000)      439 2023-06-15 14:29:25.000000 QuranDownloader-1.0.2/QuranDownloader.egg-info/SOURCES.txt
--rwxrwxrwx   0 shark     (1000) shark     (1000)        1 2023-06-15 14:29:25.000000 QuranDownloader-1.0.2/QuranDownloader.egg-info/dependency_links.txt
--rwxrwxrwx   0 shark     (1000) shark     (1000)       25 2023-06-15 14:29:25.000000 QuranDownloader-1.0.2/QuranDownloader.egg-info/requires.txt
--rwxrwxrwx   0 shark     (1000) shark     (1000)       16 2023-06-15 14:29:25.000000 QuranDownloader-1.0.2/QuranDownloader.egg-info/top_level.txt
--rwxrwxrwx   0 shark     (1000) shark     (1000)     1047 2023-06-15 14:27:08.000000 QuranDownloader-1.0.2/README.md
--rwxrwxrwx   0 shark     (1000) shark     (1000)       38 2023-06-15 14:29:26.354410 QuranDownloader-1.0.2/setup.cfg
--rwxrwxrwx   0 shark     (1000) shark     (1000)     1310 2023-06-15 14:28:44.000000 QuranDownloader-1.0.2/setup.py
+drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:31:18.460538 QuranDownloader-1.0.3/
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     2034 2023-06-15 14:31:18.456529 QuranDownloader-1.0.3/PKG-INFO
+drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:31:18.322780 QuranDownloader-1.0.3/QuranDownloader/
+-rwxrwxrwx   0 shark     (1000) shark     (1000)      271 2023-06-08 13:31:10.000000 QuranDownloader-1.0.3/QuranDownloader/__init__.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)      215 2023-06-08 13:19:03.000000 QuranDownloader-1.0.3/QuranDownloader/concurrent_req.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)      417 2023-06-08 13:21:56.000000 QuranDownloader-1.0.3/QuranDownloader/consts.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     4652 2023-06-05 18:06:50.000000 QuranDownloader-1.0.3/QuranDownloader/download_org.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     2815 2023-06-08 14:20:12.000000 QuranDownloader-1.0.3/QuranDownloader/download_verse.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     1509 2023-06-08 13:30:37.000000 QuranDownloader-1.0.3/QuranDownloader/download_word.py
+-rwxrwxrwx   0 shark     (1000) shark     (1000)      342 2023-06-05 18:08:56.000000 QuranDownloader-1.0.3/QuranDownloader/verse_key_converters.py
+drwxrwxrwx   0 shark     (1000) shark     (1000)        0 2023-06-15 14:31:18.432779 QuranDownloader-1.0.3/QuranDownloader.egg-info/
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     2034 2023-06-15 14:31:17.000000 QuranDownloader-1.0.3/QuranDownloader.egg-info/PKG-INFO
+-rwxrwxrwx   0 shark     (1000) shark     (1000)      439 2023-06-15 14:31:17.000000 QuranDownloader-1.0.3/QuranDownloader.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shark     (1000) shark     (1000)        1 2023-06-15 14:31:17.000000 QuranDownloader-1.0.3/QuranDownloader.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shark     (1000) shark     (1000)       25 2023-06-15 14:31:17.000000 QuranDownloader-1.0.3/QuranDownloader.egg-info/requires.txt
+-rwxrwxrwx   0 shark     (1000) shark     (1000)       16 2023-06-15 14:31:17.000000 QuranDownloader-1.0.3/QuranDownloader.egg-info/top_level.txt
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     1058 2023-06-15 14:30:47.000000 QuranDownloader-1.0.3/README.md
+-rwxrwxrwx   0 shark     (1000) shark     (1000)       38 2023-06-15 14:31:18.461560 QuranDownloader-1.0.3/setup.cfg
+-rwxrwxrwx   0 shark     (1000) shark     (1000)     1311 2023-06-15 14:31:01.000000 QuranDownloader-1.0.3/setup.py
```

### Comparing `QuranDownloader-1.0.2/PKG-INFO` & `QuranDownloader-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: QuranDownloader
-Version: 1.0.2
-Summary: download quran audio easly
+Version: 1.0.3
+Summary: download quran audio easily
 Home-page: UNKNOWN
 Author: Malik
 Author-email: myemail46926213@gmail.com
 License: UNKNOWN
-Description: # test
+Description: # QuranDownloader
         ## Installation
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install QuranDownloader lib.
         
         ```bash
         pip install QuranDownloader
         ```
```

### Comparing `QuranDownloader-1.0.2/QuranDownloader/download_org.py` & `QuranDownloader-1.0.3/QuranDownloader/download_org.py`

 * *Files identical despite different names*

### Comparing `QuranDownloader-1.0.2/QuranDownloader/download_verse.py` & `QuranDownloader-1.0.3/QuranDownloader/download_verse.py`

 * *Files identical despite different names*

### Comparing `QuranDownloader-1.0.2/QuranDownloader/download_word.py` & `QuranDownloader-1.0.3/QuranDownloader/download_word.py`

 * *Files identical despite different names*

### Comparing `QuranDownloader-1.0.2/QuranDownloader.egg-info/PKG-INFO` & `QuranDownloader-1.0.3/QuranDownloader.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: QuranDownloader
-Version: 1.0.2
-Summary: download quran audio easly
+Version: 1.0.3
+Summary: download quran audio easily
 Home-page: UNKNOWN
 Author: Malik
 Author-email: myemail46926213@gmail.com
 License: UNKNOWN
-Description: # test
+Description: # QuranDownloader
         ## Installation
         Use the package manager [pip](https://pip.pypa.io/en/stable/) to install QuranDownloader lib.
         
         ```bash
         pip install QuranDownloader
         ```
```

### Comparing `QuranDownloader-1.0.2/README.md` & `QuranDownloader-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# test
+# QuranDownloader
 ## Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install QuranDownloader lib.
 
 ```bash
 pip install QuranDownloader
 ```
```

### Comparing `QuranDownloader-1.0.2/setup.py` & `QuranDownloader-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # import os
 
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
-DESCRIPTION = 'download quran audio easly'
+VERSION = '1.0.3'
+DESCRIPTION = 'download quran audio easily'
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
```

