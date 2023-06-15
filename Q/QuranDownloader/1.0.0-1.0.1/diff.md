# Comparing `tmp/QuranDownloader-1.0.0.tar.gz` & `tmp/QuranDownloader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuranDownloader-1.0.0.tar", last modified: Thu Jun  8 14:15:10 2023, max compression
+gzip compressed data, was "QuranDownloader-1.0.1.tar", last modified: Thu Jun 15 11:19:19 2023, max compression
```

## Comparing `QuranDownloader-1.0.0.tar` & `QuranDownloader-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:15:10.778801 QuranDownloader-1.0.0/
--rw-rw-rw-   0        0        0      545 2023-06-08 14:15:10.778801 QuranDownloader-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 14:15:10.764800 QuranDownloader-1.0.0/QuranDownloader/
--rw-rw-rw-   0        0        0      271 2023-06-08 13:31:10.000000 QuranDownloader-1.0.0/QuranDownloader/__init__.py
--rw-rw-rw-   0        0        0      215 2023-06-08 13:19:03.000000 QuranDownloader-1.0.0/QuranDownloader/concurrent_req.py
--rw-rw-rw-   0        0        0      417 2023-06-08 13:21:56.000000 QuranDownloader-1.0.0/QuranDownloader/consts.py
--rw-rw-rw-   0        0        0     4652 2023-06-05 18:06:50.000000 QuranDownloader-1.0.0/QuranDownloader/download_org.py
--rw-rw-rw-   0        0        0     2758 2023-06-08 13:30:45.000000 QuranDownloader-1.0.0/QuranDownloader/download_verse.py
--rw-rw-rw-   0        0        0     1509 2023-06-08 13:30:37.000000 QuranDownloader-1.0.0/QuranDownloader/download_word.py
--rw-rw-rw-   0        0        0      342 2023-06-05 18:08:56.000000 QuranDownloader-1.0.0/QuranDownloader/verse_key_converters.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:15:10.777800 QuranDownloader-1.0.0/QuranDownloader.egg-info/
--rw-rw-rw-   0        0        0      545 2023-06-08 14:15:10.000000 QuranDownloader-1.0.0/QuranDownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-06-08 14:15:10.000000 QuranDownloader-1.0.0/QuranDownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:15:10.000000 QuranDownloader-1.0.0/QuranDownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 14:15:10.000000 QuranDownloader-1.0.0/QuranDownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 14:15:10.779800 QuranDownloader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-06-08 14:15:01.000000 QuranDownloader-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:19:19.580633 QuranDownloader-1.0.1/
+-rw-rw-rw-   0        0        0      623 2023-06-15 11:19:19.579632 QuranDownloader-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 11:19:19.536865 QuranDownloader-1.0.1/QuranDownloader/
+-rw-rw-rw-   0        0        0      271 2023-06-08 13:31:10.000000 QuranDownloader-1.0.1/QuranDownloader/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-08 13:19:03.000000 QuranDownloader-1.0.1/QuranDownloader/concurrent_req.py
+-rw-rw-rw-   0        0        0      417 2023-06-08 13:21:56.000000 QuranDownloader-1.0.1/QuranDownloader/consts.py
+-rw-rw-rw-   0        0        0     4652 2023-06-05 18:06:50.000000 QuranDownloader-1.0.1/QuranDownloader/download_org.py
+-rw-rw-rw-   0        0        0     2815 2023-06-08 14:20:12.000000 QuranDownloader-1.0.1/QuranDownloader/download_verse.py
+-rw-rw-rw-   0        0        0     1509 2023-06-08 13:30:37.000000 QuranDownloader-1.0.1/QuranDownloader/download_word.py
+-rw-rw-rw-   0        0        0      342 2023-06-05 18:08:56.000000 QuranDownloader-1.0.1/QuranDownloader/verse_key_converters.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:19:19.577640 QuranDownloader-1.0.1/QuranDownloader.egg-info/
+-rw-rw-rw-   0        0        0      623 2023-06-15 11:19:19.000000 QuranDownloader-1.0.1/QuranDownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-06-15 11:19:19.000000 QuranDownloader-1.0.1/QuranDownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 11:19:19.000000 QuranDownloader-1.0.1/QuranDownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-15 11:19:19.000000 QuranDownloader-1.0.1/QuranDownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 11:19:19.000000 QuranDownloader-1.0.1/QuranDownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 11:19:19.580633 QuranDownloader-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1171 2023-06-15 11:18:06.000000 QuranDownloader-1.0.1/setup.py
```

### Comparing `QuranDownloader-1.0.0/QuranDownloader/download_org.py` & `QuranDownloader-1.0.1/QuranDownloader/download_org.py`

 * *Files identical despite different names*

### Comparing `QuranDownloader-1.0.0/QuranDownloader/download_verse.py` & `QuranDownloader-1.0.1/QuranDownloader/download_verse.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     export_dir='./export',
     chapter_number=None,
     juz_number=None,
     page_number=None,
 ):
     # eval reciter id
     if reciter_name != 'all':
-        try:
-            reciter_id = RECITERS.index(reciter_name) + 1
-            if not reciter_id in range(SHIKS_LIMITS[0], SHIKS_LIMITS[1]):
-                raise Exception('invalid parameters')
-        except:
-            return print(f'{reciter_name} is not a valid reciter name\ncheck the all list from "RECITERS"')
+        # try:
+        reciter_id = RECITERS.index(reciter_name) + 1
+        if not reciter_id in range(SHIKS_LIMITS[0], SHIKS_LIMITS[1]):
+            raise Exception('{reciter_name} is not a valid reciter name\ncheck the all list from "RECITERS"')
+        # except:
+        #     raise Exception(f'{reciter_name} is not a valid reciter name\ncheck the all list from "RECITERS"')
     #
     queries = ''
     # prepare url filters
     for filter in FILTERS:
         filter_value = eval(filter)
         if (filter_value):
             queries += '?' if queries.find('?') == -1 else '&'
```

### Comparing `QuranDownloader-1.0.0/QuranDownloader/download_word.py` & `QuranDownloader-1.0.1/QuranDownloader/download_word.py`

 * *Files identical despite different names*

### Comparing `QuranDownloader-1.0.0/setup.py` & `QuranDownloader-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,39 +3,37 @@
 # import os
 
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'download quran verses'
-LONG_DESCRIPTION = 'download quran verses'
+LONG_DESCRIPTION = '''
+# Quran Downloader
+
+A brief description of what this project does and who it's for
+
+'''
 
 # Setting up
 setup(
     name="QuranDownloader",
     version=VERSION,
     author="Malik",
     author_email="myemail46926213@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
-    keywords=['python', 'quran', 'audio', 'reciter', 'verses'],
+    install_requires=['os', 're', 'requests', 'grequests'],
+    keywords=['python', 'quran', 'audio', 'reciter', 'verses', 'concurrent'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
-
-
-"""
-python setup.py sdist
-twine upload dist/*
-
-"""
+)
```

