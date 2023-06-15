# Comparing `tmp/yplib-1.3.2.tar.gz` & `tmp/yplib-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.2.tar", last modified: Thu Jun 15 03:01:51 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.3.tar", last modified: Thu Jun 15 06:32:18 2023, max compression
```

## Comparing `yplib-1.3.2.tar` & `yplib-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 03:01:51.916138 yplib-1.3.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 03:01:51.915279 yplib-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 03:01:51.916138 yplib-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 03:01:39.000000 yplib-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:01:51.908380 yplib-1.3.2/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.2/yplib/file.py
--rw-rw-rw-   0        0        0    14414 2023-06-15 01:54:26.000000 yplib-1.3.2/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:01:51.914712 yplib-1.3.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 03:01:51.000000 yplib-1.3.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 03:01:51.000000 yplib-1.3.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 03:01:51.000000 yplib-1.3.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 03:01:51.000000 yplib-1.3.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.120536 yplib-1.3.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 06:32:18.120536 yplib-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:32:18.121143 yplib-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 06:32:04.000000 yplib-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.117077 yplib-1.3.3/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.3/yplib/file.py
+-rw-rw-rw-   0        0        0    15688 2023-06-15 06:31:43.000000 yplib-1.3.3/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:32:18.119553 yplib-1.3.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 06:32:18.000000 yplib-1.3.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.2/LICENSE` & `yplib-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.2/setup.py` & `yplib-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.2",
+  version="1.3.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.2/yplib/chart.py` & `yplib-1.3.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.2/yplib/chart_html.py` & `yplib-1.3.3/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.2/yplib/file.py` & `yplib-1.3.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.2/yplib/index.py` & `yplib-1.3.3/yplib/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -272,28 +272,54 @@
     result = ''
     for one_data in key_list:
         result += one_data + '=' + data[one_data] + '&'
     if len(result) > 0:
         return result[0: -1]
 
 
-# 将 txt 文件读取到 list 中, 每一行自动过滤掉行前,行后的空格
-def to_list(file_name='a.txt', sheet_index=0):
+# 当读取 txt 之类的文件的时候
+# 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
+# 当读取 excel 之类的文件的时候
+# 将 excel 文件读取到 list 中, 可以指定 sheet, 也可以指定列 column_index(列) ,自动过滤掉每个单元格前后的特殊字符
+# sheet : 从 1 开始编号,
+# column_index : 从 1 开始编号, 指定列
+# column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
+# column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
+def to_list(file_name='a.txt', sheet_index=1, column_index=None):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
         return []
     data_list = list()
+    list_index = None
+    if column_index is not None:
+        list_index = []
+        if isinstance(column_index, int):
+            list_index.append(column_index)
+        if isinstance(column_index, str):
+            i_list = column_index.split(',')
+            for i in i_list:
+                list_index.append(int(i))
+        if isinstance(column_index, list):
+            for i in column_index:
+                list_index.append(int(i))
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         book = xlrd.open_workbook(file_name)  # 打开一个excel
-        sheet = book.sheet_by_index(sheet_index)  # 根据顺序获取sheet
+        sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
         for i in range(sheet.nrows):  # 0 1 2 3 4 5
             rows = sheet.row_values(i)
             row_data = []
             for j in range(len(rows)):
-                row_data.append(str(rows[j]).strip())
+                cell_data = str(rows[j]).strip()
+                if list_index is None:
+                    row_data.append(cell_data)
+                else:
+                    if len(list_index) == 1:
+                        row_data = cell_data
+                    elif j + 1 in list_index:
+                        row_data.append(cell_data)
             data_list.append(row_data)
         return data_list
     # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
     for line in file.readlines():
         line = line.strip()
         data_list.append(line)
```

