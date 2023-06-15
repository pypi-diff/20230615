# Comparing `tmp/SydneyGPT-0.10.13.tar.gz` & `tmp/SydneyGPT-0.10.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SydneyGPT-0.10.13.tar", last modified: Tue Jun 13 14:29:10 2023, max compression
+gzip compressed data, was "SydneyGPT-0.10.16.tar", last modified: Thu Jun 15 10:05:10 2023, max compression
```

## Comparing `SydneyGPT-0.10.13.tar` & `SydneyGPT-0.10.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:10.890389 SydneyGPT-0.10.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-13 14:29:10.890389 SydneyGPT-0.10.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 14:29:10.890389 SydneyGPT-0.10.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:10.886388 SydneyGPT-0.10.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:10.890389 SydneyGPT-0.10.13/src/SydneyGPT/
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/src/SydneyGPT/SydneyGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/src/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/src/SydneyGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/src/SydneyGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 14:28:44.000000 SydneyGPT-0.10.13/src/SydneyGPT/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:29:10.890389 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 14:29:10.000000 SydneyGPT-0.10.13/src/SydneyGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.009564 SydneyGPT-0.10.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.009564 SydneyGPT-0.10.16/src/SydneyGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/top_level.txt
```

### Comparing `SydneyGPT-0.10.13/LICENSE` & `SydneyGPT-0.10.16/LICENSE`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.13/PKG-INFO` & `SydneyGPT-0.10.16/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.10.13
+Version: 0.10.16
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SydneyGPT 🚀
 
@@ -40,15 +38,15 @@
 - EdgeGPT Requirements
 
 ## Setup
 
 To start using SydneyGPT:
 
 ```yaml
-pip install -r requirements.txt
+python3 -m pip install SydneyGPT --upgrade
 ```
 
 ## Usage Examples
 
 Here are some examples of how to use SydneyGPT:
 
 ```python
```

### Comparing `SydneyGPT-0.10.13/README.md` & `SydneyGPT-0.10.16/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - EdgeGPT Requirements
 
 ## Setup
 
 To start using SydneyGPT:
 
 ```yaml
-pip install -r requirements.txt
+python3 -m pip install SydneyGPT --upgrade
 ```
 
 ## Usage Examples
 
 Here are some examples of how to use SydneyGPT:
 
 ```python
```

### Comparing `SydneyGPT-0.10.13/setup.py` & `SydneyGPT-0.10.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,38 +8,35 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="SydneyGPT",
-    version="0.10.13",
+    version="0.10.16",
     license="GNU General Public License v2.0",
     author="Rafael Calleja",
     author_email="rafaelcalleja@gmail.com",
     description="Reverse engineered Sydney Bing Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/rafaelcalleja/SydneyGPT",
     project_urls={"Bug Report": "https://github.com/rafaelcalleja/SydneyGPT/issues/new"},
     entry_points={
         "console_scripts": [
-            "edge-gpt = EdgeGPT:main",
-            "edge-gpt-image = ImageGen:main",
+            "sydney-gpt = SydneyGPT:main",
         ],
     },
     install_requires=[
         "EdgeGPT>=0.8.2",
     ],
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["SydneyGPT"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `SydneyGPT-0.10.13/src/SydneyGPT/SydneyGPT.py` & `SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.13/src/SydneyGPT/SydneyGPTUtils.py` & `SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.13/src/SydneyGPT/conversation_style.py` & `SydneyGPT-0.10.16/src/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.13/src/SydneyGPT.egg-info/PKG-INFO` & `SydneyGPT-0.10.16/src/SydneyGPT.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.10.13
+Version: 0.10.16
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SydneyGPT 🚀
 
@@ -40,15 +38,15 @@
 - EdgeGPT Requirements
 
 ## Setup
 
 To start using SydneyGPT:
 
 ```yaml
-pip install -r requirements.txt
+python3 -m pip install SydneyGPT --upgrade
 ```
 
 ## Usage Examples
 
 Here are some examples of how to use SydneyGPT:
 
 ```python
```

