# Comparing `tmp/ProTaska-GPT-0.0.2.tar.gz` & `tmp/ProTaska-GPT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.2.tar", last modified: Thu Jun 15 21:47:59 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.3.tar", last modified: Thu Jun 15 21:52:05 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.2.tar` & `ProTaska-GPT-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:47:59.152198 ProTaska-GPT-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2208 2023-06-15 21:47:59.150207 ProTaska-GPT-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 21:47:59.090052 ProTaska-GPT-0.0.2/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.2/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:47:59.124218 ProTaska-GPT-0.0.2/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.2/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.2/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.2/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5317 2023-06-15 20:26:22.000000 ProTaska-GPT-0.0.2/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     1807 2023-06-15 20:19:34.000000 ProTaska-GPT-0.0.2/ProTaska/describer.py
--rw-rw-rw-   0        0        0     1878 2023-06-15 21:11:54.000000 ProTaska-GPT-0.0.2/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:47:59.148200 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2208 2023-06-15 21:47:58.000000 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-15 21:47:59.000000 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:47:58.000000 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-15 21:47:58.000000 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 21:47:58.000000 ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1486 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 21:47:59.152198 ProTaska-GPT-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-06-15 21:47:51.000000 ProTaska-GPT-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.892230 ProTaska-GPT-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2208 2023-06-15 21:52:05.891220 ProTaska-GPT-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.859976 ProTaska-GPT-0.0.3/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.3/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.867178 ProTaska-GPT-0.0.3/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.3/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.3/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.3/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5317 2023-06-15 20:26:22.000000 ProTaska-GPT-0.0.3/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     1807 2023-06-15 20:19:34.000000 ProTaska-GPT-0.0.3/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     1878 2023-06-15 21:11:54.000000 ProTaska-GPT-0.0.3/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:52:05.889220 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2208 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 21:52:05.000000 ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1486 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:52:05.892230 ProTaska-GPT-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-06-15 21:51:53.000000 ProTaska-GPT-0.0.3/setup.py
```

### Comparing `ProTaska-GPT-0.0.2/LICENSE` & `ProTaska-GPT-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/PKG-INFO` & `ProTaska-GPT-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.2/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.3/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.3/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.3/ProTaska/data/loader.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/ProTaska/describer.py` & `ProTaska-GPT-0.0.3/ProTaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/ProTaska/ideate.py` & `ProTaska-GPT-0.0.3/ProTaska/ideate.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.3/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.2/README.md` & `ProTaska-GPT-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.2/setup.py` & `ProTaska-GPT-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.2',
+    version='0.0.3',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
     install_requires=[
         'langchain',
         'numpy',
         'pandas',
         'colorama',
         'gradio',
+        'openai',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

