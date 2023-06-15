# Comparing `tmp/handpose_x-0.0.1.tar.gz` & `tmp/handpose_x-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handpose_x-0.0.1.tar", last modified: Thu Jun 15 08:44:13 2023, max compression
+gzip compressed data, was "handpose_x-0.0.2.tar", last modified: Thu Jun 15 09:00:12 2023, max compression
```

## Comparing `handpose_x-0.0.1.tar` & `handpose_x-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:44:13.804134 handpose_x-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 handpose_x-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     9425 2023-06-15 08:44:13.803142 handpose_x-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 handpose_x-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 08:44:13.799147 handpose_x-0.0.1/handpose_x.egg-info/
--rw-rw-rw-   0        0        0     9425 2023-06-15 08:44:13.000000 handpose_x-0.0.1/handpose_x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-06-15 08:44:13.000000 handpose_x-0.0.1/handpose_x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:44:13.000000 handpose_x-0.0.1/handpose_x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:44:13.000000 handpose_x-0.0.1/handpose_x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 08:44:13.804134 handpose_x-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1129 2023-06-15 08:43:11.000000 handpose_x-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:00:12.663123 handpose_x-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-10 13:07:48.000000 handpose_x-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9425 2023-06-15 09:00:12.662349 handpose_x-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8990 2023-06-10 13:11:14.000000 handpose_x-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 09:00:12.658117 handpose_x-0.0.2/handpose_x.egg-info/
+-rw-rw-rw-   0        0        0     9425 2023-06-15 09:00:12.000000 handpose_x-0.0.2/handpose_x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-06-15 09:00:12.000000 handpose_x-0.0.2/handpose_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:00:12.000000 handpose_x-0.0.2/handpose_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:00:12.000000 handpose_x-0.0.2/handpose_x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:00:12.663123 handpose_x-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-06-15 08:59:02.000000 handpose_x-0.0.2/setup.py
```

### Comparing `handpose_x-0.0.1/LICENSE` & `handpose_x-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `handpose_x-0.0.1/PKG-INFO` & `handpose_x-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handpose_x
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `handpose_x-0.0.1/README.md` & `handpose_x-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `handpose_x-0.0.1/handpose_x.egg-info/PKG-INFO` & `handpose_x-0.0.2/handpose_x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handpose-x
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/EricLee2021-72324/handpose_x
 Author: Eric
 Author-email: koke8756@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `handpose_x-0.0.1/setup.py` & `handpose_x-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="handpose_x", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",    #包版本号，便于维护版本
+    version="0.0.2",    #包版本号，便于维护版本
     author="Eric",    #作者，可以写自己的姓名
     author_email="koke8756@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/EricLee2021-72324/handpose_x",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

