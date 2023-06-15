# Comparing `tmp/yplib-1.2.8.tar.gz` & `tmp/yplib-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.2.8.tar", last modified: Thu Jun 15 01:21:27 2023, max compression
+gzip compressed data, was "dist\yplib-1.2.9.tar", last modified: Thu Jun 15 01:46:33 2023, max compression
```

## Comparing `yplib-1.2.8.tar` & `yplib-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:21:27.886358 yplib-1.2.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-15 01:21:27.886358 yplib-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 01:21:27.886358 yplib-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-15 01:21:10.000000 yplib-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:21:27.882619 yplib-1.2.8/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.8/yplib/__init__.py
--rw-rw-rw-   0        0        0     8736 2023-06-15 01:20:54.000000 yplib-1.2.8/yplib/chart.py
--rw-rw-rw-   0        0        0     7978 2023-06-14 08:42:03.000000 yplib-1.2.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.8/yplib/file.py
--rw-rw-rw-   0        0        0    14411 2023-06-15 01:19:19.000000 yplib-1.2.8/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:21:27.885260 yplib-1.2.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-15 01:21:27.000000 yplib-1.2.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-15 01:21:27.000000 yplib-1.2.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:21:27.000000 yplib-1.2.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 01:21:27.000000 yplib-1.2.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:33.123633 yplib-1.2.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 01:46:33.123466 yplib-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:46:33.123633 yplib-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 01:46:01.000000 yplib-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:33.120062 yplib-1.2.9/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0     9213 2023-06-15 01:45:52.000000 yplib-1.2.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8020 2023-06-15 01:43:09.000000 yplib-1.2.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.9/yplib/file.py
+-rw-rw-rw-   0        0        0    14411 2023-06-15 01:19:19.000000 yplib-1.2.9/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:46:33.122644 yplib-1.2.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 01:46:33.000000 yplib-1.2.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 01:46:33.000000 yplib-1.2.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:46:33.000000 yplib-1.2.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 01:46:33.000000 yplib-1.2.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.2.8/LICENSE` & `yplib-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.2.8/setup.py` & `yplib-1.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.2.8",
+  version="1.2.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.2.8/yplib/chart.py` & `yplib-1.2.9/yplib/chart.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 # 将 html 中的占位符 替换成数据
 # 并且 导出 生成后的 html 文件
 def insert_data_to_chart(html_data='',
                          chart_name=None,
                          x_list=None,
                          y_list=None,
                          legend=None,
-                         series=None):
+                         series=None,
+                         smooth=0):
     p_list = [
-        'chart_name', 'x_list', 'y_list', 'legend', 'series'
+        'chart_name', 'x_list', 'y_list', 'legend', 'series', 'smooth'
     ]
     p_data_list = [
-        chart_name, x_list, y_list, legend, series
+        chart_name, x_list, y_list, legend, series, smooth
     ]
     for index in range(len(p_list)):
         one_p = p_list[index]
         one_data = p_data_list[index]
         if one_data is None:
             continue
         one_p = f'-{one_p}-'
@@ -58,15 +59,15 @@
 #                 data: [320, 332, 301, 334, 390, 330, 320],
 #             },
 #             {
 #                 name: 'Search Engine',
 #                 data: [820, 932, 901, 934, 1290, 1330, 1320],
 #             },
 #         ]
-def to_chart(x_list, y_list, chart_name=''):
+def to_chart(x_list, y_list, chart_name=None, chart_name_raw=False):
     # data: ['Email', 'Union Ads', 'Video Ads', 'Direct', 'Search Engine']
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
         if 'hide' in y_one:
             legend_selected[y_one['name']] = 0
@@ -80,19 +81,16 @@
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         if 'smooth' in y_one:
             y_one['name'] = 1
         series.append(y_one)
-
-    if chart_name == '':
-        chart_name = 'line_stack'
-    else:
-        chart_name += '_line_stack'
+    if chart_name_raw is False:
+        chart_name = 'line_stack' if chart_name is None else chart_name + '_line_stack'
     insert_data_to_chart(html_data=line_stack_html(),
                          chart_name=chart_name,
                          x_list=x_list,
                          legend=legend,
                          series=series)
 
 
@@ -102,35 +100,37 @@
 #             ['2020-01-01', 132],
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
 # x_index : x 轴数据的下标
 # y_index : y 轴数据的下标
 # smooth : 曲线是否平滑
-def to_chart_one(list_data, chart_name='', is_area=False, x_index=0, y_index=1, smooth=False):
+def to_chart_one(list_data, chart_name=None, is_area=False, x_index=0, y_index=1, smooth=False):
     x_list = []
     y_list = []
-    if chart_name == '':
-        chart_name = 'line'
-    else:
-        chart_name += '_line'
+    chart_name = 'line' if chart_name is None else chart_name + '_line'
     for d_one in list_data:
         x_list.append(d_one[x_index])
         y_list.append(d_one[y_index])
     if is_area:
+        sm = 1 if smooth else 0
+        chart_name += '_area'
+        if smooth:
+            chart_name += '_smooth'
         insert_data_to_chart(html_data=line_area_html(),
-                             chart_name=chart_name + '_area',
+                             chart_name=chart_name,
                              x_list=x_list,
-                             y_list=y_list)
+                             y_list=y_list,
+                             smooth=sm)
     else:
         sm = 0
         if smooth:
             sm = 1
             chart_name += '_smooth'
-        to_chart(x_list, [{'name': chart_name, 'data': y_list, 'smooth': sm}], chart_name=chart_name)
+        to_chart(x_list, [{'name': chart_name, 'data': y_list, 'smooth': sm}], chart_name=chart_name, chart_name_raw=True)
 
 
 # legend_data.append(y_one['name'])
 #     if 'hide' in y_one:
 #         legend_selected[y_one['name']] = 0
 # legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
 # # {
@@ -164,22 +164,24 @@
 # 数据 : data = [
 #         [ "Search Engine", 1048 ],
 #         [ "Direct", 735 ],
 #         [ "Email",580 ],
 #         [ "Union Ads",484 ],
 #         [ "Video Ads",300 ]
 #       ]
-def to_chart_pie(data_list, chart_name=None):
+def to_chart_pie(data_list, chart_name=None, name_index=0, value_index=1):
     x_list = []
     chart_name = 'pie' if chart_name is None else chart_name + '_pie'
     if isinstance(data_list[0], list):
-        for one in data_list:
-            x_list.append({'name': one[0], 'value': one[1]})
+        for one_data in data_list:
+            x_list.append({'name': one_data[name_index], 'value': one_data[value_index]})
     else:
-        x_list = data_list
+        for one_data in data_list:
+            # 有多余的属性,就只保留这两个
+            x_list.append({'name': one_data['name'], 'value': one_data['value']})
     insert_data_to_chart(html_data=pie_html(),
                          chart_name=chart_name,
                          x_list=x_list)
 
 
 # 将数据整理成柱状图
 # 数据 : data = [
@@ -193,21 +195,18 @@
 # 数据 : data = [
 #        {x: "Search Engine", y: 1048 },
 #        {x: "Direct", y: 735 },
 #        {x: "Email", y:580 },
 #        {x: "Union Ads", y:484 },
 #        {x: "Video Ads", y:300 }
 #       }]
-def to_chart_bar(data_list, chart_name='', x_index=0, y_index=1):
+def to_chart_bar(data_list, chart_name=None, x_index=0, y_index=1):
     x_list = []
     y_list = []
-    if chart_name == '':
-        chart_name = 'bar'
-    else:
-        chart_name += '_bar'
+    chart_name = 'bar' if chart_name is None else chart_name + '_bar'
     for one in data_list:
         if isinstance(one, list):
             x_list.append(one[x_index])
             y_list.append(one[y_index])
         else:
             x_list.append(one['x'])
             y_list.append(one['y'])
@@ -230,20 +229,18 @@
 
 #
 #
 # data = []
 # # for i in range(10):
 # #     data.append([uuid_random(), int(random.uniform(0, 1000))])
 # for i in range(10):
-#     one = {}
-#     one['name'] = uuid_random()
-#     one['value'] = int(random.uniform(0, 1000))
-#     data.append(one)
+#     data.append([random_uuid(), int(random.uniform(0, 1000))])
 #
 # to_chart_pie(data)
+# to_chart_pie(data, 'yp')
 
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
 # # # 将 list 转化成 图表的例子
@@ -266,14 +263,16 @@
 #     # n['hide'] = '1'
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
 #
 # data_list = []
-# for i in range(10000):
+# for i in range(100):
 #     data_list.append([i, int(random.uniform(0, 1000))])
-#
+
 # to_chart_one(data_list)
-# to_chart_one(list_data=data_list, is_area=True)
+# to_chart_one(data_list, smooth=True)
+# to_chart_one(data_list, is_area=True)
+# to_chart_one(data_list, is_area=True, smooth=True)
 
 # print('end')
```

### Comparing `yplib-1.2.8/yplib/chart_html.py` & `yplib-1.2.9/yplib/chart_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
              '            realtime: true,' \
              '        },' \
              '    ],' \
              '  series: [' \
              '    {' \
              '      type: "line",' \
              '      symbol: "none",' \
+             '      smooth: -smooth-,' \
              '      sampling: "lttb",' \
              '      itemStyle: {' \
              '        color: "rgb(255, 70, 131)"' \
              '      },' \
              '      areaStyle: {' \
              '        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [' \
              '          {' \
```

### Comparing `yplib-1.2.8/yplib/file.py` & `yplib-1.2.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.8/yplib/index.py` & `yplib-1.2.9/yplib/index.py`

 * *Files identical despite different names*

