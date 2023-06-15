# Comparing `tmp/yplib-1.2.6.tar.gz` & `tmp/yplib-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.2.6.tar", last modified: Wed Jun 14 09:02:04 2023, max compression
+gzip compressed data, was "dist\yplib-1.2.7.tar", last modified: Thu Jun 15 00:14:50 2023, max compression
```

## Comparing `yplib-1.2.6.tar` & `yplib-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:02:04.930575 yplib-1.2.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-14 09:02:04.930575 yplib-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 09:02:04.931384 yplib-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-14 09:02:01.000000 yplib-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:02:04.927928 yplib-1.2.6/yplib/
--rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.6/yplib/__init__.py
--rw-rw-rw-   0        0        0     8345 2023-06-14 09:01:54.000000 yplib-1.2.6/yplib/chart.py
--rw-rw-rw-   0        0        0     7978 2023-06-14 08:42:03.000000 yplib-1.2.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.6/yplib/file.py
--rw-rw-rw-   0        0        0    13793 2023-06-14 08:33:02.000000 yplib-1.2.6/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:02:04.930016 yplib-1.2.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-14 09:02:04.000000 yplib-1.2.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-14 09:02:04.000000 yplib-1.2.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:02:04.000000 yplib-1.2.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 09:02:04.000000 yplib-1.2.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:50.112655 yplib-1.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-15 00:14:50.112529 yplib-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:14:50.113158 yplib-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-15 00:14:10.000000 yplib-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:50.109403 yplib-1.2.7/yplib/
+-rw-rw-rw-   0        0        0      146 2023-06-14 02:29:06.000000 yplib-1.2.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0     8382 2023-06-15 00:14:03.000000 yplib-1.2.7/yplib/chart.py
+-rw-rw-rw-   0        0        0     7978 2023-06-14 08:42:03.000000 yplib-1.2.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-14 02:27:16.000000 yplib-1.2.7/yplib/file.py
+-rw-rw-rw-   0        0        0    13793 2023-06-14 08:33:02.000000 yplib-1.2.7/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:50.111789 yplib-1.2.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-15 00:14:50.000000 yplib-1.2.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-15 00:14:50.000000 yplib-1.2.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 00:14:50.000000 yplib-1.2.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 00:14:50.000000 yplib-1.2.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.2.6/LICENSE` & `yplib-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.2.6/setup.py` & `yplib-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.2.6",
+  version="1.2.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.2.6/yplib/chart.py` & `yplib-1.2.7/yplib/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                              chart_name=chart_name + '_area',
                              x_list=x_list,
                              y_list=y_list)
     else:
         sm = 0
         if smooth:
             sm = 1
+            chart_name += '_smooth'
         to_chart(x_list, [{'name': chart_name, 'data': y_list, 'smooth': sm}], chart_name=chart_name)
 
 
 # legend_data.append(y_one['name'])
 #     if 'hide' in y_one:
 #         legend_selected[y_one['name']] = 0
 # legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
```

### Comparing `yplib-1.2.6/yplib/chart_html.py` & `yplib-1.2.7/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.6/yplib/file.py` & `yplib-1.2.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.2.6/yplib/index.py` & `yplib-1.2.7/yplib/index.py`

 * *Files identical despite different names*

