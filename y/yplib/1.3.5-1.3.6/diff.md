# Comparing `tmp/yplib-1.3.5.tar.gz` & `tmp/yplib-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.5.tar", last modified: Thu Jun 15 07:31:30 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.6.tar", last modified: Thu Jun 15 08:13:24 2023, max compression
```

## Comparing `yplib-1.3.5.tar` & `yplib-1.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.641095 yplib-1.3.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 07:31:30.640931 yplib-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 07:31:30.641593 yplib-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 07:31:14.000000 yplib-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.636771 yplib-1.3.5/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.5/yplib/file.py
--rw-rw-rw-   0        0        0    17466 2023-06-15 07:30:58.000000 yplib-1.3.5/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:30.639925 yplib-1.3.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 07:31:30.000000 yplib-1.3.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:24.581071 yplib-1.3.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:13:24.580589 yplib-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:13:24.581071 yplib-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 08:12:50.000000 yplib-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:24.577226 yplib-1.3.6/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.6/yplib/file.py
+-rw-rw-rw-   0        0        0    17740 2023-06-15 08:11:52.000000 yplib-1.3.6/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:24.579609 yplib-1.3.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:13:24.000000 yplib-1.3.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 08:13:24.000000 yplib-1.3.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:13:24.000000 yplib-1.3.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 08:13:24.000000 yplib-1.3.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.5/LICENSE` & `yplib-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.5/setup.py` & `yplib-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.5",
+  version="1.3.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.5/yplib/chart.py` & `yplib-1.3.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.5/yplib/chart_html.py` & `yplib-1.3.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.5/yplib/file.py` & `yplib-1.3.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.5/yplib/index.py` & `yplib-1.3.6/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,23 +274,29 @@
         result += one_data + '=' + data[one_data] + '&'
     if len(result) > 0:
         return result[0: -1]
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
+# separator : 是否对每一行进行分割,如果存在这个字段,就分割
 # 当读取 excel 之类的文件的时候
 # 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
 # sheet : 从 1 开始编号,
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
 # column_date : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
-def to_list(file_name='a.txt', sheet_index=1, column_index=None, column_date=None, column_datetime=None):
+def to_list(file_name='a.txt',
+            sheet_index=1,
+            separator=None,
+            column_index=None,
+            column_date=None,
+            column_datetime=None):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
         return []
     data_list = list()
     list_index = []
     for one_index in [column_index, column_date, column_datetime]:
         list_index_one = None
         if one_index is not None:
@@ -353,15 +359,18 @@
                                 row_data = cell_data
             data_list.append(row_data)
         return data_list
     # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
     for line in file.readlines():
         line = line.strip()
-        data_list.append(line)
+        if separator is not None:
+            data_list.append(line.split(str(separator)))
+        else:
+            data_list.append(line)
     return data_list
 
 
 def to_excel(list_data, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
```

