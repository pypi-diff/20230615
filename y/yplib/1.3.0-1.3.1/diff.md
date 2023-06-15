# Comparing `tmp/yplib-1.3.0.tar.gz` & `tmp/yplib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.0.tar", last modified: Thu Jun 15 01:51:27 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.1.tar", last modified: Thu Jun 15 01:55:35 2023, max compression
```

## Comparing `yplib-1.3.0.tar` & `yplib-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:51:27.196656 yplib-1.3.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 01:51:27.196189 yplib-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 01:51:27.197141 yplib-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 01:50:36.000000 yplib-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:51:27.192997 yplib-1.3.0/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.0/yplib/__init__.py
--rw-rw-rw-   0        0        0     9046 2023-06-15 01:51:14.000000 yplib-1.3.0/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.0/yplib/file.py
--rw-rw-rw-   0        0        0    14411 2023-06-15 01:19:19.000000 yplib-1.3.0/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:51:27.195624 yplib-1.3.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 01:51:27.000000 yplib-1.3.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 01:51:27.000000 yplib-1.3.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:51:27.000000 yplib-1.3.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 01:51:27.000000 yplib-1.3.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 01:55:35.518029 yplib-1.3.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 01:55:35.517571 yplib-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:55:35.518708 yplib-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 01:55:07.000000 yplib-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:55:35.514971 yplib-1.3.1/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0     9046 2023-06-15 01:51:14.000000 yplib-1.3.1/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.1/yplib/file.py
+-rw-rw-rw-   0        0        0    14414 2023-06-15 01:54:26.000000 yplib-1.3.1/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:55:35.517135 yplib-1.3.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 01:55:35.000000 yplib-1.3.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 01:55:35.000000 yplib-1.3.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:55:35.000000 yplib-1.3.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 01:55:35.000000 yplib-1.3.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.0/LICENSE` & `yplib-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.0/setup.py` & `yplib-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.0",
+  version="1.3.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.0/yplib/chart.py` & `yplib-1.3.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.0/yplib/chart_html.py` & `yplib-1.3.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.0/yplib/file.py` & `yplib-1.3.1/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.0/yplib/index.py` & `yplib-1.3.1/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         os.mkdir(file_name)
 
 
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
     return str(file_name) \
         + '_' + datetime.today().strftime('%m%d_%H%M') \
-        + '_' + random_str(4) \
+        + '_' + random_letter(4) \
         + suffix
 
 
 def do_md5(data='do_md5'):
     return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
```

