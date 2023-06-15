# Comparing `tmp/datawork000-0.1.tar.gz` & `tmp/datawork000-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datawork000-0.1.tar", last modified: Thu Jun 15 07:43:47 2023, max compression
+gzip compressed data, was "dist/datawork000-0.2.0.tar", last modified: Thu Jun 15 08:27:13 2023, max compression
```

## Comparing `datawork000-0.1.tar` & `datawork000-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 07:43:47.000000 datawork000-0.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      730 2023-06-15 07:43:47.000000 datawork000-0.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      113 2023-06-15 05:51:30.000000 datawork000-0.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 07:43:47.000000 datawork000-0.1/datawork000.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      730 2023-06-15 07:43:47.000000 datawork000-0.1/datawork000.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      173 2023-06-15 07:43:47.000000 datawork000-0.1/datawork000.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 07:43:47.000000 datawork000-0.1/datawork000.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       12 2023-06-15 07:43:47.000000 datawork000-0.1/datawork000.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1050 2023-06-15 04:57:24.000000 datawork000-0.1/datawork000.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 07:43:47.000000 datawork000-0.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      981 2023-06-15 07:43:41.000000 datawork000-0.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:27:13.000000 datawork000-0.2.0/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      731 2023-06-15 08:27:13.000000 datawork000-0.2.0/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      113 2023-06-15 05:51:30.000000 datawork000-0.2.0/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      731 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      173 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       12 2023-06-15 08:27:13.000000 datawork000-0.2.0/datawork000.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1050 2023-06-15 04:57:24.000000 datawork000-0.2.0/datawork000.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 08:27:13.000000 datawork000-0.2.0/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      983 2023-06-15 08:27:08.000000 datawork000-0.2.0/setup.py
```

### Comparing `datawork000-0.1/PKG-INFO` & `datawork000-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: datawork000
-Version: 0.1
-Summary: jkzhou's datawork
+Version: 0.2.0
+Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: 1406584456@qq.com
 License: MIT
-Description: README
+Description: README.md
 Keywords: datawork
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
+Description-Content-Type: markdown
```

### Comparing `datawork000-0.1/datawork000.egg-info/PKG-INFO` & `datawork000-0.2.0/datawork000.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: datawork000
-Version: 0.1
-Summary: jkzhou's datawork
+Version: 0.2.0
+Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: 1406584456@qq.com
 License: MIT
-Description: README
+Description: README.md
 Keywords: datawork
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
+Description-Content-Type: markdown
```

### Comparing `datawork000-0.1/datawork000.py` & `datawork000-0.2.0/datawork000.py`

 * *Files identical despite different names*

### Comparing `datawork000-0.1/setup.py` & `datawork000-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 ###### Thu Jun 15 13:20:21 CST 2023
 # 制作完成，后续更新时，需要维护此处的信息。版本更新。入口不变。
 
 from setuptools import setup
 
 setup(
     name='datawork000',
-    version='0.1',
+    version='0.2.0',
     py_modules=['datawork000'],
     author='jk.zhou',
     author_email='1406584456@qq.com',
-    description="jkzhou's datawork",
-    long_description_content_type="text/markdown",
-    long_description="README",
+    description="jk.zhou's datawork",
+    long_description_content_type="markdown",
+    long_description= "README.md",
     license='MIT',
     keywords='datawork',
     url='https://github.com/jkjoker/datawork',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

