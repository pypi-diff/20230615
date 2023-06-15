# Comparing `tmp/ProTaska-GPT-0.0.0.tar.gz` & `tmp/ProTaska-GPT-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.0.tar", last modified: Thu Jun 15 21:26:38 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.1.tar", last modified: Thu Jun 15 21:41:51 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.0.tar` & `ProTaska-GPT-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:26:38.139361 ProTaska-GPT-0.0.0/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      679 2023-06-15 21:26:38.139361 ProTaska-GPT-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 21:26:38.129508 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0      679 2023-06-15 21:26:37.000000 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-15 21:26:38.000000 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:26:37.000000 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-15 21:26:37.000000 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 21:26:37.000000 ProTaska-GPT-0.0.0/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1486 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 21:26:38.138345 ProTaska-GPT-0.0.0/protaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.0/protaska/__init__.py
--rw-rw-rw-   0        0        0     1807 2023-06-15 20:19:34.000000 ProTaska-GPT-0.0.0/protaska/describer.py
--rw-rw-rw-   0        0        0     1878 2023-06-15 21:11:54.000000 ProTaska-GPT-0.0.0/protaska/ideate.py
--rw-rw-rw-   0        0        0       42 2023-06-15 21:26:38.140344 ProTaska-GPT-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      870 2023-06-15 21:25:13.000000 ProTaska-GPT-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:41:51.567404 ProTaska-GPT-0.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2208 2023-06-15 21:41:51.566403 ProTaska-GPT-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 21:41:51.560894 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2208 2023-06-15 21:41:51.000000 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-15 21:41:51.000000 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:41:51.000000 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-15 21:41:51.000000 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 21:41:51.000000 ProTaska-GPT-0.0.1/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1486 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 21:41:51.565404 ProTaska-GPT-0.0.1/protaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.1/protaska/__init__.py
+-rw-rw-rw-   0        0        0     1807 2023-06-15 20:19:34.000000 ProTaska-GPT-0.0.1/protaska/describer.py
+-rw-rw-rw-   0        0        0     1878 2023-06-15 21:11:54.000000 ProTaska-GPT-0.0.1/protaska/ideate.py
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:41:51.567404 ProTaska-GPT-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-06-15 21:41:19.000000 ProTaska-GPT-0.0.1/setup.py
```

### Comparing `ProTaska-GPT-0.0.0/LICENSE` & `ProTaska-GPT-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.0/README.md` & `ProTaska-GPT-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.0/protaska/describer.py` & `ProTaska-GPT-0.0.1/protaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.0/protaska/ideate.py` & `ProTaska-GPT-0.0.1/protaska/ideate.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.0/setup.py` & `ProTaska-GPT-0.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from setuptools import setup
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='ProTaska-GPT',
-    version='0.0.0',
+    version='0.0.1',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=['protaska'],
     url='https://github.com/AmanPriyanshu/protaska-gpt',
     install_requires=[
         'langchain',
         'numpy',
         'pandas',
         'colorama',
+        'gradio',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

