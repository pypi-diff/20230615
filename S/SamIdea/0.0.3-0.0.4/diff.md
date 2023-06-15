# Comparing `tmp/samidea-0.0.3.tar.gz` & `tmp/samidea-0.0.4.tar.gz`

## Comparing `samidea-0.0.3.tar` & `samidea-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 samidea-0.0.3/.pypirc
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 samidea-0.0.3/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 samidea-0.0.3/sun_config/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 samidea-0.0.3/sun_config/sun_idea_config.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 samidea-0.0.3/sun_module/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 samidea-0.0.3/sun_module/multi_task.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 samidea-0.0.3/sun_utils/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 samidea-0.0.3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 samidea-0.0.3/LICENSE
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 samidea-0.0.3/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 samidea-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 samidea-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 samidea-0.0.4/.pypirc
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 samidea-0.0.4/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 samidea-0.0.4/sun_config/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 samidea-0.0.4/sun_config/sun_idea_config.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 samidea-0.0.4/sun_module/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 samidea-0.0.4/sun_module/multi_task.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 samidea-0.0.4/sun_utils/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 samidea-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 samidea-0.0.4/LICENSE
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 samidea-0.0.4/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 samidea-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 samidea-0.0.4/PKG-INFO
```

### Comparing `samidea-0.0.3/sun_module/multi_task.py` & `samidea-0.0.4/sun_module/multi_task.py`

 * *Files identical despite different names*

### Comparing `samidea-0.0.3/.gitignore` & `samidea-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `samidea-0.0.3/LICENSE` & `samidea-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `samidea-0.0.3/pyproject.toml` & `samidea-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 5361 6d49 6465 6122 0d0a 7665 7273   "SamIdea"..vers
-00000070: 696f 6e20 3d20 2230 2e30 2e33 220d 0a61  ion = "0.0.3"..a
+00000070: 696f 6e20 3d20 2230 2e30 2e34 220d 0a61  ion = "0.0.4"..a
 00000080: 7574 686f 7273 203d 205b 0d0a 2020 7b20  uthors = [..  { 
 00000090: 6e61 6d65 3d22 e5ad 99e5 b08f e4ba 9422  name="........."
 000000a0: 2c20 656d 6169 6c3d 2273 756e 7368 7561  , email="sunshua
 000000b0: 6e67 6c6f 6e67 6466 4067 6d61 696c 2e63  nglongdf@gmail.c
 000000c0: 6f6d 227d 2c0d 0a5d 0d0a 6465 7363 7269  om"},..]..descri
 000000d0: 7074 696f 6e20 3d20 2273 756e 5f69 6465  ption = "sun_ide
 000000e0: 6120 6973 2061 2070 6163 6b61 6765 2066  a is a package f
```

### Comparing `samidea-0.0.3/PKG-INFO` & `samidea-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SamIdea
-Version: 0.0.3
+Version: 0.0.4
 Summary: sun_idea is a package for multiprocess
 Project-URL: Homepage, https://github.com/sunxiaowu?tab=projects
 Author-email: 孙小五 <sunshuanglongdf@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Othneil Drew
```

