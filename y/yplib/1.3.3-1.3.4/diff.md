# Comparing `tmp/yplib-1.3.3.tar.gz` & `tmp/yplib-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.3.tar", last modified: Thu Jun 15 06:32:18 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.4.tar", last modified: Thu Jun 15 07:11:39 2023, max compression
```

## Comparing `yplib-1.3.3.tar` & `yplib-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.120536 yplib-1.3.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 06:32:18.120536 yplib-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 06:32:18.121143 yplib-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 06:32:04.000000 yplib-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.117077 yplib-1.3.3/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.3/yplib/file.py
--rw-rw-rw-   0        0        0    15688 2023-06-15 06:31:43.000000 yplib-1.3.3/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.119553 yplib-1.3.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.637241 yplib-1.3.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 07:11:39.636662 yplib-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 07:11:39.637658 yplib-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 07:11:23.000000 yplib-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.633890 yplib-1.3.4/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.4/yplib/file.py
+-rw-rw-rw-   0        0        0    17251 2023-06-15 07:11:06.000000 yplib-1.3.4/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:11:39.635861 yplib-1.3.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 07:11:39.000000 yplib-1.3.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.3/LICENSE` & `yplib-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.3/setup.py` & `yplib-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.3",
+  version="1.3.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.3/yplib/chart.py` & `yplib-1.3.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.3/yplib/chart_html.py` & `yplib-1.3.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.3/yplib/file.py` & `yplib-1.3.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.3/yplib/index.py` & `yplib-1.3.4/yplib/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -280,46 +280,74 @@
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # 当读取 excel 之类的文件的时候
 # 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
 # sheet : 从 1 开始编号,
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
-def to_list(file_name='a.txt', sheet_index=1, column_index=None):
+# column_date : 指定日期格式的列,规则与 column_index 一样
+# column_datetime : 指定日期格式的列,规则与 column_index 一样
+def to_list(file_name='a.txt', sheet_index=1, column_index=None, column_date=None, column_datetime=None):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
         return []
     data_list = list()
-    list_index = None
-    if column_index is not None:
-        list_index = []
-        if isinstance(column_index, int):
-            list_index.append(column_index)
-        if isinstance(column_index, str):
-            i_list = column_index.split(',')
-            for i in i_list:
-                list_index.append(int(i))
-        if isinstance(column_index, list):
-            for i in column_index:
-                list_index.append(int(i))
+    list_index = []
+    for one_index in [column_index, column_date, column_datetime]:
+        list_index_one = None
+        if one_index is not None:
+            list_index_one = []
+            if isinstance(one_index, int):
+                list_index_one.append(one_index)
+            if isinstance(one_index, str):
+                i_list = one_index.split(',')
+                for i in i_list:
+                    list_index_one.append(int(i))
+            if isinstance(one_index, list):
+                for i in one_index:
+                    list_index_one.append(int(i))
+        list_index.append(list_index_one)
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
+        # 是否是单 list 类型的数据
+        list_only_one = False
+        if list_index[0] is not None and len(list_index[0]) == 1:
+            list_only_one = True
         book = xlrd.open_workbook(file_name)  # 打开一个excel
         sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
         for i in range(sheet.nrows):  # 0 1 2 3 4 5
             rows = sheet.row_values(i)
             row_data = []
             for j in range(len(rows)):
                 cell_data = str(rows[j]).strip()
-                if list_index is None:
+                is_date = False
+                is_datetime = False
+                # 日期格式的列
+                if list_index[1] is not None and j + 1 in list_index[1]:
+                    cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                    is_date = True
                     row_data.append(cell_data)
-                else:
-                    if len(list_index) == 1:
+                    if list_only_one:
                         row_data = cell_data
-                    elif j + 1 in list_index:
+                # 日期时间格式的列
+                if is_date is False and list_index[2] is not None and j + 1 in list_index[2]:
+                    cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                    is_datetime = True
+                    row_data.append(cell_data)
+                    if list_only_one:
+                        row_data = cell_data
+                # 指定需要的列
+                if is_date is False and is_datetime is False:
+                    if list_index[0] is None:
                         row_data.append(cell_data)
+                    else:
+                        # 指定需要的列
+                        if j + 1 in list_index[0]:
+                            row_data.append(cell_data)
+                            if list_only_one:
+                                row_data = cell_data
             data_list.append(row_data)
         return data_list
     # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
     for line in file.readlines():
         line = line.strip()
         data_list.append(line)
```

