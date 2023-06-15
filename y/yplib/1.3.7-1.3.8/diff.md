# Comparing `tmp/yplib-1.3.7.tar.gz` & `tmp/yplib-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.3.7.tar", last modified: Thu Jun 15 08:20:03 2023, max compression
+gzip compressed data, was "dist\yplib-1.3.8.tar", last modified: Thu Jun 15 08:38:57 2023, max compression
```

## Comparing `yplib-1.3.7.tar` & `yplib-1.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:20:03.573738 yplib-1.3.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 08:20:03.573738 yplib-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 08:20:03.574509 yplib-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 08:19:49.000000 yplib-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:20:03.570246 yplib-1.3.7/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    10365 2023-06-15 03:00:45.000000 yplib-1.3.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.7/yplib/file.py
--rw-rw-rw-   0        0        0    18005 2023-06-15 08:19:40.000000 yplib-1.3.7/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:20:03.572622 yplib-1.3.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 08:20:03.000000 yplib-1.3.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 08:20:03.000000 yplib-1.3.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:20:03.000000 yplib-1.3.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 08:20:03.000000 yplib-1.3.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:38:57.624544 yplib-1.3.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:38:57.624043 yplib-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:38:57.624544 yplib-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 08:38:53.000000 yplib-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:38:57.620965 yplib-1.3.8/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.3.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10727 2023-06-15 08:38:10.000000 yplib-1.3.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.3.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.3.8/yplib/file.py
+-rw-rw-rw-   0        0        0    18005 2023-06-15 08:35:31.000000 yplib-1.3.8/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:38:57.623281 yplib-1.3.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 08:38:57.000000 yplib-1.3.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 08:38:57.000000 yplib-1.3.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:38:57.000000 yplib-1.3.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 08:38:57.000000 yplib-1.3.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.3.7/LICENSE` & `yplib-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.3.7/setup.py` & `yplib-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.3.7",
+  version="1.3.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.3.7/yplib/chart.py` & `yplib-1.3.8/yplib/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         one_p = p_list[index]
         one_data = p_data_list[index]
         if one_data is None:
             continue
         one_p = f'-{one_p}-'
         if one_p in html_data:
             html_data = html_data.replace(one_p, str(one_data))
-    to_txt(list_data=[html_data],
+    to_txt(data_list=[html_data],
            file_name=str(name),
            file_path='html',
            fixed_name=False,
            suffix='.html')
     # current_path = os.path.abspath(__file__)
     # html_list = open(current_path[0:current_path.find('__init__')] + 'line-stack-temp.html', 'r', encoding='utf-8').readlines()
 
@@ -76,19 +76,19 @@
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
 #  name : 文件名称,折线图的名称
 #  name_raw : 用原始的名字,不用带上属性 line_stack
 def to_chart(x_list, y_list=None, name=None, name_raw=False):
     if y_list is None:
-        list_data = x_list
+        data_list = x_list
         x_list = []
         y_list = []
         index = 0
-        for line_one in list_data:
+        for line_one in data_list:
             if index > 0:
                 x_list.append(line_one[0])
             # 第一行数据
             if index == 0:
                 for y in range(len(line_one) - 1):
                     y_list.append({'name': line_one[y + 1], 'data': []})
             # 第二行开始的数据
@@ -131,22 +131,37 @@
 # 数据 : data_list = [
 #             ['2020-01-01', 132],
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
 # x_index : x 轴数据的下标
 # y_index : y 轴数据的下标
+# 或者
+# 数据 : data = [
+#        {x: "Search Engine", y: 1048 },
+#        {x: "Direct", y: 735 },
+#        {x: "Email", y:580 },
+#        {x: "Union Ads", y:484 },
+#        {x: "Video Ads", y:300 }
+#       }]
+#  x_key : 当元素为对象的时候, x 的 key
+#  y_key : 当元素为对象的时候, y 的 key
+# is_area : 是否使用 area 图
 # smooth : 曲线是否平滑
-def to_chart_one(list_data, name=None, is_area=False, x_index=0, y_index=1, smooth=False):
+def to_chart_one(data_list, name=None, is_area=False, x_index=0, x_key='x', y_index=1, y_key='y', smooth=False):
     x_list = []
     y_list = []
     name = 'line' if name is None else name + '_line'
-    for d_one in list_data:
-        x_list.append(d_one[x_index])
-        y_list.append(d_one[y_index])
+    for d_one in data_list:
+        if isinstance(d_one, list):
+            x_list.append(d_one[x_index])
+            y_list.append(d_one[y_index])
+        else:
+            x_list.append(d_one[x_key])
+            y_list.append(d_one[y_key])
     if is_area:
         sm = 1 if smooth else 0
         name += '_area'
         if smooth:
             name += '_smooth'
         insert_data_to_chart(html_data=line_area_html(),
                              name=name,
@@ -157,102 +172,86 @@
         sm = 0
         if smooth:
             sm = 1
             name += '_smooth'
         to_chart(x_list, [{'name': name, 'data': y_list, 'smooth': sm}], name=name, name_raw=True)
 
 
-# legend_data.append(y_one['name'])
-#     if 'hide' in y_one:
-#         legend_selected[y_one['name']] = 0
-# legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
-# # {
-# #     name: 'Email',
-# #     type: 'line',
-# #     stack: 'Total',
-# #     data: [120, 132, 101, 134, 90, 230, 210],
-# # }
-# series = []
-# for y_one in y_list:
-#     y_one['type'] = 'line'
-#     y_one['stack'] = 'Total'
-#     series.append(y_one)
-#
-# insert_data_to_chart(html_data=line_stack_html(),
-#                      name=name,
-#                      x_list=x_list,
-#                      legend=legend,
-#                      series=series)
-
-
 # 将数据整理成饼状图
 # 数据 : data = [
 #         { value: 1048, name: "Search Engine" },
 #         { value: 735, name: "Direct" },
 #         { value: 580, name: "Email" },
 #         { value: 484, name: "Union Ads" },
 #         { value: 300, name: "Video Ads" }
 #       ]
+#  name_key : 当元素为对象的时候, x 的 key
+#  value_key : 当元素为对象的时候, y 的 key
 # 或者
 # 数据 : data = [
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
-def to_chart_pie(list_data, name=None, name_index=0, value_index=1):
+#  name_index : 当元素为数组的时候, name 的下标
+#  value_index : 当元素为数组的时候, value 的下标
+def to_chart_pie(data_list, name=None, name_index=0, name_key='name', value_index=1, value_key='value'):
     x_list = []
     name = 'pie' if name is None else name + '_pie'
-    if isinstance(list_data[0], list):
-        for one_data in list_data:
+    if isinstance(data_list[0], list):
+        for one_data in data_list:
             x_list.append({'name': one_data[name_index], 'value': one_data[value_index]})
     else:
-        for one_data in list_data:
+        for one_data in data_list:
             # 有多余的属性,就只保留这两个
-            x_list.append({'name': one_data['name'], 'value': one_data['value']})
+            x_list.append({'name': one_data[name_key], 'value': one_data[value_key]})
     insert_data_to_chart(html_data=pie_html(),
                          name=name,
                          x_list=x_list)
 
 
 # 将数据整理成柱状图
 # 数据 : data = [
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
+#  x_index : 当元素为数组的时候, x 的下标
+#  y_index : 当元素为数组的时候, y 的下标
 # 或者
 # 数据 : data = [
 #        {x: "Search Engine", y: 1048 },
 #        {x: "Direct", y: 735 },
 #        {x: "Email", y:580 },
 #        {x: "Union Ads", y:484 },
 #        {x: "Video Ads", y:300 }
 #       }]
-def to_chart_bar(list_data, name=None, x_index=0, y_index=1):
+#  x_key : 当元素为对象的时候, x 的 key
+#  y_key : 当元素为对象的时候, y 的 key
+def to_chart_bar(data_list, name=None, x_index=0, x_key='x', y_index=1, y_key='y'):
     x_list = []
     y_list = []
     name = 'bar' if name is None else name + '_bar'
-    for one in list_data:
+    for one in data_list:
         if isinstance(one, list):
             x_list.append(one[x_index])
             y_list.append(one[y_index])
         else:
-            x_list.append(one['x'])
-            y_list.append(one['y'])
+            x_list.append(one[x_key])
+            y_list.append(one[y_key])
 
     insert_data_to_chart(html_data=bar_html(),
                          name=name,
                          x_list=x_list,
                          y_list=y_list)
 
-
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
 # for i in range(10000):
 #     one = {}
 #     one['x'] = uuid_random()
 #     one['y'] = int(random.uniform(0, 1000))
```

### Comparing `yplib-1.3.7/yplib/chart_html.py` & `yplib-1.3.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.7/yplib/file.py` & `yplib-1.3.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.3.7/yplib/index.py` & `yplib-1.3.8/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,43 +220,43 @@
 
 def date_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
     return str(datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds, minutes=minutes, hours=hours,
                             weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
-# list_data : 数组数据, 也可以不是数组
+# data_list : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
-def to_txt(list_data, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
+def to_txt(data_list, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     if fixed_name:
         file_name = file_name + suffix
     else:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
-    if isinstance(list_data, list) is False:
-        text_file.write(to_str(list_data) + '\n')
+    if isinstance(data_list, list) is False:
+        text_file.write(to_str(data_list) + '\n')
     else:
-        for one in list_data:
+        for one in data_list:
             text_file.write(to_str(one) + '\n')
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
-def to_txt_data(list_data, file_name='data'):
-    return to_txt(list_data, file_name, 'data', True)
+def to_txt_data(data_list, file_name='data'):
+    return to_txt(data_list, file_name, 'data', True)
 
 
 def to_str(data):
     if can_use_json(data):
         s = json.dumps(data)
     else:
         s = str(data)
@@ -371,27 +371,27 @@
         else:
             data_list.append(line)
     if separator_all is not None:
         return ''.join(data_list).split(str(separator_all))
     return data_list
 
 
-def to_excel(list_data, file_name, file_path='excel'):
+def to_excel(data_list, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     # 2. 创建Excel工作薄
     w_b = xlwt.Workbook()
     # 3. 添加Excel工作表
     sh = w_b.add_sheet(str(file_name))
     # 4. 写入数据
     # myStyle = xlwt.easyxf('font: name Times New Roman, color-index red, bold on')  # 数据格式
     m = 0
-    for one_data in list_data:
+    for one_data in data_list:
         n = 0
         if isinstance(one_data, list):
             for one in one_data:
                 # mySheet.write(n, m, one)  # 写入A3，数值等于1
                 if isinstance(one, dict) or isinstance(one, list):
                     s = json.dumps(one)
                 else:
```

