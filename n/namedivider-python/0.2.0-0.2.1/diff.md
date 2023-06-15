# Comparing `tmp/namedivider-python-0.2.0.tar.gz` & `tmp/namedivider-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namedivider-python-0.2.0.tar", last modified: Sun May 29 08:59:14 2022, max compression
+gzip compressed data, was "namedivider-python-0.2.1.tar", last modified: Thu Jun 15 06:37:19 2023, max compression
```

## Comparing `namedivider-python-0.2.0.tar` & `namedivider-python-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/
--rw-rw-r--   0 ml        (1001) ml        (1001)     1063 2022-04-29 07:01:55.000000 namedivider-python-0.2.0/LICENSE
--rw-rw-r--   0 ml        (1001) ml        (1001)       66 2022-04-29 07:01:55.000000 namedivider-python-0.2.0/MANIFEST.in
--rw-rw-r--   0 ml        (1001) ml        (1001)      566 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/PKG-INFO
--rw-rw-r--   0 ml        (1001) ml        (1001)     4408 2022-05-29 08:05:55.000000 namedivider-python-0.2.0/README.md
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider/
--rw-rw-r--   0 ml        (1001) ml        (1001)      585 2022-05-29 08:58:46.000000 namedivider-python-0.2.0/namedivider/__init__.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider/assets/
--rwxrwxr-x   0 ml        (1001) ml        (1001)    30784 2022-04-29 07:01:55.000000 namedivider-python-0.2.0/namedivider/assets/kanji.csv
--rwxrwxr-x   0 ml        (1001) ml        (1001)     5323 2022-05-29 08:58:46.000000 namedivider-python-0.2.0/namedivider/cli.py
--rwxrwxr-x   0 ml        (1001) ml        (1001)     1092 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/divided_name.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider/divider/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2022-05-29 08:54:05.000000 namedivider-python-0.2.0/namedivider/divider/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     1572 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/divider/basic_name_divider.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     3488 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/divider/config.py
--rw-rw-r--   0 ml        (1001) ml        (1001)      819 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/divider/divided_name.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     2131 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/divider/gbdt_name_divider.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     8291 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/divider/name_divider_base.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider/feature/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2022-05-29 08:54:05.000000 namedivider-python-0.2.0/namedivider/feature/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4474 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/feature/extractor.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     1247 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/feature/family_name.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     7623 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/feature/functional.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     5406 2022-05-29 07:13:49.000000 namedivider-python-0.2.0/namedivider/feature/kanji.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4604 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/kanji_statistics.py
--rwxrwxr-x   0 ml        (1001) ml        (1001)    15296 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/name_divider.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider/training/
--rw-rw-r--   0 ml        (1001) ml        (1001)        0 2022-05-29 08:54:05.000000 namedivider-python-0.2.0/namedivider/training/__init__.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     4549 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/training/kanji_statistics_taker.py
--rw-rw-r--   0 ml        (1001) ml        (1001)     1973 2022-05-29 08:57:22.000000 namedivider-python-0.2.0/namedivider/util.py
--rw-rw-r--   0 ml        (1001) ml        (1001)       22 2022-05-29 05:02:25.000000 namedivider-python-0.2.0/namedivider/version.py
-drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/namedivider_python.egg-info/
--rw-rw-r--   0 ml        (1001) ml        (1001)      566 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/PKG-INFO
--rw-rw-r--   0 ml        (1001) ml        (1001)      960 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/SOURCES.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)        1 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/dependency_links.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       47 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/entry_points.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       43 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/requires.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       12 2022-05-29 08:59:14.000000 namedivider-python-0.2.0/namedivider_python.egg-info/top_level.txt
--rw-rw-r--   0 ml        (1001) ml        (1001)       38 2022-05-29 08:59:14.590711 namedivider-python-0.2.0/setup.cfg
--rw-rw-r--   0 ml        (1001) ml        (1001)      970 2022-05-29 08:40:43.000000 namedivider-python-0.2.0/setup.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/
+-rw-rw-r--   0 ml        (1001) ml        (1001)     1063 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/LICENSE
+-rw-rw-r--   0 ml        (1001) ml        (1001)       66 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/MANIFEST.in
+-rw-rw-r--   0 ml        (1001) ml        (1001)      567 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/PKG-INFO
+-rw-rw-r--   0 ml        (1001) ml        (1001)     4480 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/README.md
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/
+-rw-rw-r--   0 ml        (1001) ml        (1001)      585 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/__init__.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/assets/
+-rwxrwxr-x   0 ml        (1001) ml        (1001)    30784 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/assets/kanji.csv
+-rwxrwxr-x   0 ml        (1001) ml        (1001)     5323 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/cli.py
+-rwxrwxr-x   0 ml        (1001) ml        (1001)     1092 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divided_name.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/divider/
+-rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/__init__.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     1572 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/basic_name_divider.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     3488 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/config.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)      819 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/divided_name.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     2131 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/gbdt_name_divider.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     8291 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/divider/name_divider_base.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/feature/
+-rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/__init__.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     4474 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/extractor.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     1263 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/namedivider/feature/family_name.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     7623 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/functional.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     5406 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/feature/kanji.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     4604 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/kanji_statistics.py
+-rwxrwxr-x   0 ml        (1001) ml        (1001)    15296 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/name_divider.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider/training/
+-rw-rw-r--   0 ml        (1001) ml        (1001)        0 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/training/__init__.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     4549 2023-06-15 03:50:44.000000 namedivider-python-0.2.1/namedivider/training/kanji_statistics_taker.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)     2001 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/namedivider/util.py
+-rw-rw-r--   0 ml        (1001) ml        (1001)       22 2023-06-15 06:36:27.000000 namedivider-python-0.2.1/namedivider/version.py
+drwxrwxr-x   0 ml        (1001) ml        (1001)        0 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/namedivider_python.egg-info/
+-rw-rw-r--   0 ml        (1001) ml        (1001)      567 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/PKG-INFO
+-rw-rw-r--   0 ml        (1001) ml        (1001)      960 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 ml        (1001) ml        (1001)        1 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 ml        (1001) ml        (1001)       47 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/entry_points.txt
+-rw-rw-r--   0 ml        (1001) ml        (1001)       60 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/requires.txt
+-rw-rw-r--   0 ml        (1001) ml        (1001)       12 2023-06-15 06:37:19.000000 namedivider-python-0.2.1/namedivider_python.egg-info/top_level.txt
+-rw-rw-r--   0 ml        (1001) ml        (1001)       38 2023-06-15 06:37:19.605939 namedivider-python-0.2.1/setup.cfg
+-rw-rw-r--   0 ml        (1001) ml        (1001)      990 2023-06-15 06:09:48.000000 namedivider-python-0.2.1/setup.py
```

### Comparing `namedivider-python-0.2.0/LICENSE` & `namedivider-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/README.md` & `namedivider-python-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 input: 菅義偉 -> output: 菅 義偉
 ```
 
 NameDivider divides the name using statistical information of the kanji used in the names.
 
 Measuring the accuracy using a privately held data set, the accuracy is 99.91%.
 
-You can see how it works with [this demo](https://share.streamlit.io/rskmoi/namedivider-python/feature/add_demo/examples/demo/example_streamlit.py "Demo").
+You can see how it works with [this demo](https://share.streamlit.io/rskmoi/namedivider-python/examples/demo/example_streamlit.py "Demo").
 
 ## Documents
 
 [NameDivider(日本語)](https://dune-fifth-da7.notion.site/NameDivider-9118f1a74ca545629dbbfa606a39ba0a "NameDivider")
 
 ## Installation
 ```
@@ -143,7 +143,13 @@
 (2) 責任
 
 作者または著作権者は、family_name_repository.pickleに関して一切の責任を負いません。
 
 The family name data used in family_name_repository.pickle is provided by Myoji-Yurai.net(名字由来net).
 
 ![](https://user-images.githubusercontent.com/26462938/170855242-84ec7418-b288-4b64-bbc2-4927776493bf.png)
+
+## Ongoing Projects
+
+- Porting Python to Rust
+
+https://github.com/rskmoi/namedivider-rs
```

### Comparing `namedivider-python-0.2.0/namedivider/__init__.py` & `namedivider-python-0.2.1/namedivider/__init__.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/assets/kanji.csv` & `namedivider-python-0.2.1/namedivider/assets/kanji.csv`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/cli.py` & `namedivider-python-0.2.1/namedivider/cli.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divided_name.py` & `namedivider-python-0.2.1/namedivider/divided_name.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divider/basic_name_divider.py` & `namedivider-python-0.2.1/namedivider/divider/basic_name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divider/config.py` & `namedivider-python-0.2.1/namedivider/divider/config.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divider/divided_name.py` & `namedivider-python-0.2.1/namedivider/divider/divided_name.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divider/gbdt_name_divider.py` & `namedivider-python-0.2.1/namedivider/divider/gbdt_name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/divider/name_divider_base.py` & `namedivider-python-0.2.1/namedivider/divider/name_divider_base.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/feature/extractor.py` & `namedivider-python-0.2.1/namedivider/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/feature/family_name.py` & `namedivider-python-0.2.1/namedivider/feature/family_name.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import os
 from typing import Union
 from pathlib import Path
 
 
 class FamilyNameRepository:
     def __init__(self, path_txt: Union[str, Path]):
         """
@@ -15,15 +16,15 @@
         高橋
         ...
         ------------
         """
         with open(path_txt, "rb") as f:
             family_text = f.read().decode()
         self.__family_names = {}
-        for rank, _family in enumerate(family_text.split("\n")):
+        for rank, _family in enumerate(family_text.split(os.linesep)):
             self.__family_names[_family] = rank
 
     def exists(self, family: str) -> bool:
         """
         Returns if the family name entered is included in the pre-prepared family names.
         :param family: Family name.
         :return: bool
```

### Comparing `namedivider-python-0.2.0/namedivider/feature/functional.py` & `namedivider-python-0.2.1/namedivider/feature/functional.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/feature/kanji.py` & `namedivider-python-0.2.1/namedivider/feature/kanji.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/kanji_statistics.py` & `namedivider-python-0.2.1/namedivider/kanji_statistics.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/name_divider.py` & `namedivider-python-0.2.1/namedivider/name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/training/kanji_statistics_taker.py` & `namedivider-python-0.2.1/namedivider/training/kanji_statistics_taker.py`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/namedivider/util.py` & `namedivider-python-0.2.1/namedivider/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
     """
     When a default path is provided, download from the Internet if not already downloaded.
     """
     if Path(path) != get_family_name_pkl_default_path():
         return None
     if path.exists():
         return None
-    DEFAULT_CACHE_DIR.mkdir(exist_ok=True)
+    DEFAULT_CACHE_DIR.mkdir(exist_ok=True, parents=True)
     print("Download FamilyNameRepository from GitHub...")
     content = requests.get(FAMILY_NAME_REPOSITORY_URL).content
     with open(path, "wb") as f:
         f.write(content)
 
 
 def download_gbdt_model_v1_if_needed(path: Union[str, Path]):
     """
     When a default path is provided, download from the Internet if not already downloaded.
     """
     if Path(path) != get_gbdt_model_v1_default_path():
         return None
     if path.exists():
         return None
-    DEFAULT_CACHE_DIR.mkdir(exist_ok=True)
+    DEFAULT_CACHE_DIR.mkdir(exist_ok=True, parents=True)
     print("Download GBDT Model from GitHub...")
     content = requests.get(GBDT_MODEL_V1_URL).content
     with open(path, "wb") as f:
         f.write(content)
```

### Comparing `namedivider-python-0.2.0/namedivider_python.egg-info/SOURCES.txt` & `namedivider-python-0.2.1/namedivider_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `namedivider-python-0.2.0/setup.py` & `namedivider-python-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     version=__version__,
     url='https://github.com/rskmoi/namedivider-python',
     author="rskmoi",
     author_email='rei.sakamoto.92@gmail.com',
     description='A tool for dividing the Japanese full name into a family name and a given name.',
     license="MIT",
     packages=find_packages(),
-    install_requires=['numpy', 'pandas', 'tqdm', 'click', 'regex', 'typer>=0.3.2'],
+    install_requires=['numpy', 'pandas', 'tqdm', 'regex', 'requests', 'lightgbm>=3.3', 'typer>=0.3.2'],
     tests_require=["pytest"],
     entry_points={
         'console_scripts': ['nmdiv = namedivider.cli:app']
     },
     package_data={'': ['namedivider/assets/*.csv']},
     include_package_data=True,
     classifiers=[
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ]
-)
+)
```

