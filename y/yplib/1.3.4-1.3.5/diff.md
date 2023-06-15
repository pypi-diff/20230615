# Comparing `tmp/yplib-1.3.4.tar.gz` & `tmp/yplib-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.4.tar", last modified: Thu Jun 15 07:11:39 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.5.tar", last modified: Thu Jun 15 07:31:30 2023, max compression
```

## Comparing `yplib-1.3.4.tar` & `yplib-1.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.637241 yplib-1.3.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 07:11:39.636662 yplib-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 07:11:39.637658 yplib-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 07:11:23.000000 yplib-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.633890 yplib-1.3.4/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.4/yplib/file.py
--rw-rw-rw-   0        0        0    17251 2023-06-15 07:11:06.000000 yplib-1.3.4/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.635861 yplib-1.3.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.641095 yplib-1.3.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 07:31:30.640931 yplib-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 07:31:30.641593 yplib-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 07:31:14.000000 yplib-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.636771 yplib-1.3.5/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.5/yplib/file.py
+-rw-rw-rw-   0        0        0    17466 2023-06-15 07:30:58.000000 yplib-1.3.5/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.639925 yplib-1.3.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.4/LICENSE` & `yplib-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.4/setup.py` & `yplib-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.4",
+  version="1.3.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.4/yplib/chart.py` & `yplib-1.3.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.4/yplib/chart_html.py` & `yplib-1.3.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.4/yplib/file.py` & `yplib-1.3.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.4/yplib/index.py` & `yplib-1.3.5/yplib/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -301,14 +301,21 @@
                 i_list = one_index.split(',')
                 for i in i_list:
                     list_index_one.append(int(i))
             if isinstance(one_index, list):
                 for i in one_index:
                     list_index_one.append(int(i))
         list_index.append(list_index_one)
+    list_all = []
+    for one_list in list_index:
+        if one_list is not None:
+            for o in one_list:
+                list_all.append(o)
+    if len(list_all) > 0:
+        list_index[0] = list_all
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         # 是否是单 list 类型的数据
         list_only_one = False
         if list_index[0] is not None and len(list_index[0]) == 1:
             list_only_one = True
         book = xlrd.open_workbook(file_name)  # 打开一个excel
```

