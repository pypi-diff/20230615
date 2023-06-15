# Comparing `tmp/tybase-0.1.3.tar.gz` & `tmp/tybase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.1.3.tar", last modified: Thu Jun 15 03:31:58 2023, max compression
+gzip compressed data, was "tybase-0.1.4.tar", last modified: Thu Jun 15 03:35:34 2023, max compression
```

## Comparing `tybase-0.1.3.tar` & `tybase-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.781574 tybase-0.1.3/
--rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.1.3/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      602 2023-06-15 03:31:58.781432 tybase-0.1.3/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.1.3/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-06-15 03:31:58.781625 tybase-0.1.3/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)      938 2023-06-15 03:31:27.000000 tybase-0.1.3/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.778358 tybase-0.1.3/tybase/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.1.3/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.779604 tybase-0.1.3/tybase/baidu/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.1.3/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.1.3/tybase/baidu/kw_tool.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.1.3/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.780378 tybase-0.1.3/tybase/dbtool/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.1.3/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.1.3/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2206 2023-05-13 03:56:34.000000 tybase-0.1.3/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.780803 tybase-0.1.3/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.1.3/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.1.3/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.781236 tybase-0.1.3/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.1.3/tybase/tools/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1632 2023-06-15 03:30:59.000000 tybase-0.1.3/tybase/tools/riqit_ools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.1.3/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:31:58.779373 tybase-0.1.3/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      602 2023-06-15 03:31:58.000000 tybase-0.1.3/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      453 2023-06-15 03:31:58.000000 tybase-0.1.3/tybase.egg-info/SOURCES.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-06-15 03:31:58.000000 tybase-0.1.3/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)       86 2023-06-15 03:31:58.000000 tybase-0.1.3/tybase.egg-info/requires.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-06-15 03:31:58.000000 tybase-0.1.3/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.961342 tybase-0.1.4/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.1.4/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      575 2023-06-15 03:35:34.961190 tybase-0.1.4/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.1.4/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-06-15 03:35:34.961382 tybase-0.1.4/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      911 2023-06-15 03:35:28.000000 tybase-0.1.4/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.958195 tybase-0.1.4/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.1.4/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.959388 tybase-0.1.4/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.1.4/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.1.4/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.1.4/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.960064 tybase-0.1.4/tybase/dbtool/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.1.4/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.1.4/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2206 2023-05-13 03:56:34.000000 tybase-0.1.4/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.960491 tybase-0.1.4/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.1.4/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.1.4/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.960915 tybase-0.1.4/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.1.4/tybase/tools/__init__.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1632 2023-06-15 03:30:59.000000 tybase-0.1.4/tybase/tools/riqit_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.1.4/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-15 03:35:34.959109 tybase-0.1.4/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      575 2023-06-15 03:35:34.000000 tybase-0.1.4/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      454 2023-06-15 03:35:34.000000 tybase-0.1.4/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-06-15 03:35:34.000000 tybase-0.1.4/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       86 2023-06-15 03:35:34.000000 tybase-0.1.4/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-06-15 03:35:34.000000 tybase-0.1.4/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.1.3/PKG-INFO` & `tybase-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.1.3
-Summary: 新增了一个日期tools的方法,用于分割日期
+Version: 0.1.4
+Summary: 修改了日期的文件名
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.1.3/setup.py` & `tybase-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.1.3',
+    version='0.1.4',
     include_package_data=True,
-    description='新增了一个日期tools的方法,用于分割日期',
+    description='修改了日期的文件名',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.1.3/tybase/baidu/kw_tool.py` & `tybase-0.1.4/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.3/tybase/dbtool/data_import.py` & `tybase-0.1.4/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.3/tybase/dbtool/mysql.py` & `tybase-0.1.4/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.3/tybase/lc/eg1.py` & `tybase-0.1.4/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.3/tybase/tools/riqit_ools.py` & `tybase-0.1.4/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.3/tybase.egg-info/PKG-INFO` & `tybase-0.1.4/tybase.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.1.3
-Summary: 新增了一个日期tools的方法,用于分割日期
+Version: 0.1.4
+Summary: 修改了日期的文件名
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

