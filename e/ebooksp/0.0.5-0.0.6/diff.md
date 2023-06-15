# Comparing `tmp/ebooksp-0.0.5.tar.gz` & `tmp/ebooksp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebooksp-0.0.5.tar", last modified: Wed Jun 14 02:35:48 2023, max compression
+gzip compressed data, was "ebooksp-0.0.6.tar", last modified: Thu Jun 15 07:04:13 2023, max compression
```

## Comparing `ebooksp-0.0.5.tar` & `ebooksp-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.288675 ebooksp-0.0.5/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.5/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:35:48.288555 ebooksp-0.0.5/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      567 2023-06-13 11:19:50.000000 ebooksp-0.0.5/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.287886 ebooksp-0.0.5/ebooksp/
--rw-r--r--   0 bo         (501) staff       (20)      667 2023-06-13 11:19:50.000000 ebooksp-0.0.5/ebooksp/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2023 2023-06-14 01:56:52.000000 ebooksp-0.0.5/ebooksp/ebook_convert_format.py
--rw-r--r--   0 bo         (501) staff       (20)     1308 2023-06-14 02:35:36.000000 ebooksp-0.0.5/ebooksp/ebook_to_text.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-14 02:35:48.288403 ebooksp-0.0.5/ebooksp.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     1025 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-14 02:35:48.000000 ebooksp-0.0.5/ebooksp.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-14 02:35:48.288710 ebooksp-0.0.5/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-14 02:35:36.000000 ebooksp-0.0.5/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-15 07:04:13.946402 ebooksp-0.0.6/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-13 11:17:27.000000 ebooksp-0.0.6/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     1105 2023-06-15 07:04:13.946271 ebooksp-0.0.6/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      647 2023-06-14 07:39:17.000000 ebooksp-0.0.6/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-15 07:04:13.945438 ebooksp-0.0.6/ebooksp/
+-rw-r--r--   0 bo         (501) staff       (20)      684 2023-06-15 07:03:56.000000 ebooksp-0.0.6/ebooksp/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2023 2023-06-14 01:56:52.000000 ebooksp-0.0.6/ebooksp/ebook_convert_format.py
+-rw-r--r--   0 bo         (501) staff       (20)     1308 2023-06-14 02:35:36.000000 ebooksp-0.0.6/ebooksp/ebook_to_text.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-15 07:04:13.946103 ebooksp-0.0.6/ebooksp.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     1105 2023-06-15 07:04:13.000000 ebooksp-0.0.6/ebooksp.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      257 2023-06-15 07:04:13.000000 ebooksp-0.0.6/ebooksp.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-15 07:04:13.000000 ebooksp-0.0.6/ebooksp.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       13 2023-06-15 07:04:13.000000 ebooksp-0.0.6/ebooksp.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)        8 2023-06-15 07:04:13.000000 ebooksp-0.0.6/ebooksp.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-15 07:04:13.946437 ebooksp-0.0.6/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      791 2023-06-15 07:03:56.000000 ebooksp-0.0.6/setup.py
```

### Comparing `ebooksp-0.0.5/LICENSE` & `ebooksp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.5/PKG-INFO` & `ebooksp-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ebook
 
 ## 介绍
-处理电子书的工具
+- 处理电子书的工具
+- 首次使用需安装calibre, 地址是 https://calibre-ebook.com/download
+
 
 ## 安装
 
 
     pip install ebooksp
 
 ## 功能
```

### Comparing `ebooksp-0.0.5/README.md` & `ebooksp-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # ebook
 
 ## 介绍
-处理电子书的工具
+- 处理电子书的工具
+- 首次使用需安装calibre, 地址是 https://calibre-ebook.com/download
+
 
 ## 安装
 
 
     pip install ebooksp
 
 ## 功能
```

### Comparing `ebooksp-0.0.5/ebooksp/__init__.py` & `ebooksp-0.0.6/ebooksp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 
 
 def convert_format_many(ebooks_input: list, ebooks_output: list, timeout=60):
     from ebooksp.ebook_convert_format import ebook_convert_format_many
     return ebook_convert_format_many(ebooks_input, ebooks_output, timeout)
 
 
-def to_text(ebook_input: str, delete=True, timeout=60):
+def to_text(ebook_input: str, delete=True, timeout=60, func=None):
     from ebooksp.ebook_to_text import ebook_to_text
-    return ebook_to_text(ebook_input, delete, timeout)
+    return ebook_to_text(ebook_input, delete, timeout, func)
```

### Comparing `ebooksp-0.0.5/ebooksp/ebook_convert_format.py` & `ebooksp-0.0.6/ebooksp/ebook_convert_format.py`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.5/ebooksp/ebook_to_text.py` & `ebooksp-0.0.6/ebooksp/ebook_to_text.py`

 * *Files identical despite different names*

### Comparing `ebooksp-0.0.5/ebooksp.egg-info/PKG-INFO` & `ebooksp-0.0.6/ebooksp.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebooksp
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Conversion Tool for e-book
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ebook
 
 ## 介绍
-处理电子书的工具
+- 处理电子书的工具
+- 首次使用需安装calibre, 地址是 https://calibre-ebook.com/download
+
 
 ## 安装
 
 
     pip install ebooksp
 
 ## 功能
```

### Comparing `ebooksp-0.0.5/setup.py` & `ebooksp-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ebooksp',
-    version='0.0.5',
+    version='0.0.6',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A Conversion Tool for e-book',
     long_description=long_description,
```

