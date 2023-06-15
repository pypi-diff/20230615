# Comparing `tmp/yplib-1.3.9.tar.gz` & `tmp/yplib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.9.tar", last modified: Thu Jun 15 08:47:49 2023, max compression
+gzip compressed data, was "dist\yplib-1.4.0.tar", last modified: Thu Jun 15 08:53:54 2023, max compression
```

## Comparing `yplib-1.3.9.tar` & `yplib-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:47:49.710810 yplib-1.3.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 08:47:49.710098 yplib-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 08:47:49.710810 yplib-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 08:47:29.000000 yplib-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:47:49.707093 yplib-1.3.9/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    10727 2023-06-15 08:38:10.000000 yplib-1.3.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.9/yplib/file.py
--rw-rw-rw-   0        0        0    18056 2023-06-15 08:47:23.000000 yplib-1.3.9/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:47:49.709421 yplib-1.3.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 08:47:49.000000 yplib-1.3.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 08:47:49.000000 yplib-1.3.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:47:49.000000 yplib-1.3.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 08:47:49.000000 yplib-1.3.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.032299 yplib-1.4.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:53:54.031659 yplib-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:53:54.032299 yplib-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 08:53:49.000000 yplib-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.028377 yplib-1.4.0/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.4.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11227 2023-06-15 08:53:38.000000 yplib-1.4.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.4.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.4.0/yplib/file.py
+-rw-rw-rw-   0        0        0    18056 2023-06-15 08:47:23.000000 yplib-1.4.0/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:53:54.030727 yplib-1.4.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 08:53:53.000000 yplib-1.4.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.9/LICENSE` & `yplib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.9/setup.py` & `yplib-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.9",
+  version="1.4.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.9/yplib/chart.py` & `yplib-1.4.0/yplib/chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,15 +74,18 @@
 #             {
 #                 name: 'Search Engine',
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
 #  name : 文件名称,折线图的名称
 #  name_raw : 用原始的名字,不用带上属性 line_stack
-def to_chart(x_list, y_list=None, name=None, name_raw=False):
+def to_chart(x_list,
+             y_list=None,
+             name=None,
+             name_raw=False):
     if y_list is None:
         data_list = x_list
         x_list = []
         y_list = []
         index = 0
         for line_one in data_list:
             if index > 0:
@@ -133,25 +136,32 @@
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
 # x_index : x 轴数据的下标
 # y_index : y 轴数据的下标
 # 或者
 # 数据 : data = [
-#        {x: "Search Engine", y: 1048 },
-#        {x: "Direct", y: 735 },
-#        {x: "Email", y:580 },
-#        {x: "Union Ads", y:484 },
-#        {x: "Video Ads", y:300 }
+#        {name: "Search Engine", value: 1048 },
+#        {name: "Direct", value: 735 },
+#        {name: "Email", value:580 },
+#        {name: "Union Ads", value:484 },
+#        {name: "Video Ads", value:300 }
 #       }]
 #  x_key : 当元素为对象的时候, x 的 key
 #  y_key : 当元素为对象的时候, y 的 key
 # is_area : 是否使用 area 图
 # smooth : 曲线是否平滑
-def to_chart_one(data_list, name=None, is_area=False, x_index=0, x_key='x', y_index=1, y_key='y', smooth=False):
+def to_chart_one(data_list,
+                 name=None,
+                 is_area=False,
+                 x_index=0,
+                 x_key='name',
+                 y_index=1,
+                 y_key='value',
+                 smooth=False):
     x_list = []
     y_list = []
     name = 'line' if name is None else name + '_line'
     for d_one in data_list:
         if isinstance(d_one, list):
             x_list.append(d_one[x_index])
             y_list.append(d_one[y_index])
@@ -169,15 +179,18 @@
                              y_list=y_list,
                              smooth=sm)
     else:
         sm = 0
         if smooth:
             sm = 1
             name += '_smooth'
-        to_chart(x_list, [{'name': name, 'data': y_list, 'smooth': sm}], name=name, name_raw=True)
+        to_chart(x_list=x_list,
+                 y_list=[{'name': name, 'data': y_list, 'smooth': sm}],
+                 name=name,
+                 name_raw=True)
 
 
 # 将数据整理成饼状图
 # 数据 : data = [
 #         { value: 1048, name: "Search Engine" },
 #         { value: 735, name: "Direct" },
 #         { value: 580, name: "Email" },
@@ -192,15 +205,20 @@
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
 #  name_index : 当元素为数组的时候, name 的下标
 #  value_index : 当元素为数组的时候, value 的下标
-def to_chart_pie(data_list, name=None, name_index=0, name_key='name', value_index=1, value_key='value'):
+def to_chart_pie(data_list,
+                 name=None,
+                 name_index=0,
+                 name_key='name',
+                 value_index=1,
+                 value_key='value'):
     x_list = []
     name = 'pie' if name is None else name + '_pie'
     if isinstance(data_list[0], list):
         for one_data in data_list:
             x_list.append({'name': one_data[name_index], 'value': one_data[value_index]})
     else:
         for one_data in data_list:
@@ -219,23 +237,28 @@
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
 #  x_index : 当元素为数组的时候, x 的下标
 #  y_index : 当元素为数组的时候, y 的下标
 # 或者
 # 数据 : data = [
-#        {x: "Search Engine", y: 1048 },
-#        {x: "Direct", y: 735 },
-#        {x: "Email", y:580 },
-#        {x: "Union Ads", y:484 },
-#        {x: "Video Ads", y:300 }
+#        {name: "Search Engine", value: 1048 },
+#        {name: "Direct", value: 735 },
+#        {name: "Email", value:580 },
+#        {name: "Union Ads", value:484 },
+#        {name: "Video Ads", value:300 }
 #       }]
 #  x_key : 当元素为对象的时候, x 的 key
 #  y_key : 当元素为对象的时候, y 的 key
-def to_chart_bar(data_list, name=None, x_index=0, x_key='x', y_index=1, y_key='y'):
+def to_chart_bar(data_list,
+                 name=None,
+                 x_index=0,
+                 x_key='name',
+                 y_index=1,
+                 y_key='value'):
     x_list = []
     y_list = []
     name = 'bar' if name is None else name + '_bar'
     for one in data_list:
         if isinstance(one, list):
             x_list.append(one[x_index])
             y_list.append(one[y_index])
```

### Comparing `yplib-1.3.9/yplib/chart_html.py` & `yplib-1.4.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.9/yplib/file.py` & `yplib-1.4.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.9/yplib/index.py` & `yplib-1.4.0/yplib/index.py`

 * *Files identical despite different names*

