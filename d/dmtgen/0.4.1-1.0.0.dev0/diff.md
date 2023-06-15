# Comparing `tmp/dmtgen-0.4.1.tar.gz` & `tmp/dmtgen-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtgen-0.4.1.tar", last modified: Thu Jun 15 13:42:14 2023, max compression
+gzip compressed data, was "dmtgen-1.0.0.dev0.tar", last modified: Wed Oct 19 05:29:46 2022, max compression
```

## Comparing `dmtgen-0.4.1.tar` & `dmtgen-1.0.0.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.951106 dmtgen-0.4.1/
--rw-rw-rw-   0        0        0     1093 2022-03-22 09:41:00.000000 dmtgen-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      535 2023-06-15 13:42:14.950106 dmtgen-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-09-10 11:08:42.000000 dmtgen-0.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 13:42:14.952105 dmtgen-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-06-15 13:41:51.000000 dmtgen-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.878117 dmtgen-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.901107 dmtgen-0.4.1/src/dmtgen/
--rw-rw-rw-   0        0        0      208 2022-10-19 05:20:30.000000 dmtgen-0.4.1/src/dmtgen/__init__.py
--rw-rw-rw-   0        0        0     3746 2023-04-13 09:17:25.000000 dmtgen-0.4.1/src/dmtgen/base_generator.py
--rw-rw-rw-   0        0        0     1689 2022-10-19 05:18:49.000000 dmtgen-0.4.1/src/dmtgen/basic_template_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.942107 dmtgen-0.4.1/src/dmtgen/common/
--rw-rw-rw-   0        0        0        0 2021-09-10 09:22:37.000000 dmtgen-0.4.1/src/dmtgen/common/__init__.py
--rw-rw-rw-   0        0        0     2873 2022-10-19 05:21:50.000000 dmtgen-0.4.1/src/dmtgen/common/blueprint.py
--rw-rw-rw-   0        0        0     2213 2022-10-19 05:27:29.000000 dmtgen-0.4.1/src/dmtgen/common/blueprint_attribute.py
--rw-rw-rw-   0        0        0     1528 2022-05-30 12:16:28.000000 dmtgen-0.4.1/src/dmtgen/common/enum_description.py
--rw-rw-rw-   0        0        0     6088 2023-06-15 13:38:26.000000 dmtgen-0.4.1/src/dmtgen/common/package.py
--rw-rw-rw-   0        0        0      187 2021-09-10 10:54:56.000000 dmtgen-0.4.1/src/dmtgen/common/system_package.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.880106 dmtgen-0.4.1/src/dmtgen/data/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.881108 dmtgen-0.4.1/src/dmtgen/data/system/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.946106 dmtgen-0.4.1/src/dmtgen/data/system/SIMOS/
--rw-rw-rw-   0        0        0      503 2022-09-29 12:07:04.000000 dmtgen-0.4.1/src/dmtgen/data/system/SIMOS/entity.json
--rw-rw-rw-   0        0        0      585 2022-09-29 12:07:11.000000 dmtgen-0.4.1/src/dmtgen/data/system/SIMOS/named_enity.json
--rw-rw-rw-   0        0        0      445 2022-10-19 05:13:00.000000 dmtgen-0.4.1/src/dmtgen/package_generator.py
--rw-rw-rw-   0        0        0      186 2021-09-10 09:22:09.000000 dmtgen-0.4.1/src/dmtgen/template.py
--rw-rw-rw-   0        0        0      722 2022-08-15 06:50:41.000000 dmtgen-0.4.1/src/dmtgen/template_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:42:14.929106 dmtgen-0.4.1/src/dmtgen.egg-info/
--rw-rw-rw-   0        0        0      535 2023-06-15 13:42:14.000000 dmtgen-0.4.1/src/dmtgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-15 13:42:14.000000 dmtgen-0.4.1/src/dmtgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:42:14.000000 dmtgen-0.4.1/src/dmtgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 13:42:14.000000 dmtgen-0.4.1/src/dmtgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 13:42:14.000000 dmtgen-0.4.1/src/dmtgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.124677 dmtgen-1.0.0.dev0/
+-rw-rw-rw-   0        0        0     1093 2022-03-22 09:41:00.000000 dmtgen-1.0.0.dev0/LICENSE
+-rw-rw-rw-   0        0        0      540 2022-10-19 05:29:46.123677 dmtgen-1.0.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-09-10 11:08:42.000000 dmtgen-1.0.0.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2022-10-19 05:29:46.124677 dmtgen-1.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2022-10-19 05:06:42.000000 dmtgen-1.0.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:45.999678 dmtgen-1.0.0.dev0/src/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.050679 dmtgen-1.0.0.dev0/src/dmtgen/
+-rw-rw-rw-   0        0        0      208 2022-10-19 05:20:30.000000 dmtgen-1.0.0.dev0/src/dmtgen/__init__.py
+-rw-rw-rw-   0        0        0     3725 2022-10-19 05:15:02.000000 dmtgen-1.0.0.dev0/src/dmtgen/base_generator.py
+-rw-rw-rw-   0        0        0     1689 2022-10-19 05:18:49.000000 dmtgen-1.0.0.dev0/src/dmtgen/basic_template_generator.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.110677 dmtgen-1.0.0.dev0/src/dmtgen/common/
+-rw-rw-rw-   0        0        0        0 2021-09-10 09:22:37.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/__init__.py
+-rw-rw-rw-   0        0        0     2873 2022-10-19 05:21:50.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint.py
+-rw-rw-rw-   0        0        0     2213 2022-10-19 05:27:29.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint_attribute.py
+-rw-rw-rw-   0        0        0     1528 2022-05-30 12:16:28.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/enum_description.py
+-rw-rw-rw-   0        0        0     4639 2021-09-10 09:22:37.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/package.py
+-rw-rw-rw-   0        0        0      187 2021-09-10 10:54:56.000000 dmtgen-1.0.0.dev0/src/dmtgen/common/system_package.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.001678 dmtgen-1.0.0.dev0/src/dmtgen/data/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.001678 dmtgen-1.0.0.dev0/src/dmtgen/data/system/
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.122677 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/
+-rw-rw-rw-   0        0        0      503 2022-09-29 12:07:04.000000 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/entity.json
+-rw-rw-rw-   0        0        0      585 2022-09-29 12:07:11.000000 dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/named_enity.json
+-rw-rw-rw-   0        0        0      445 2022-10-19 05:13:00.000000 dmtgen-1.0.0.dev0/src/dmtgen/package_generator.py
+-rw-rw-rw-   0        0        0      186 2021-09-10 09:22:09.000000 dmtgen-1.0.0.dev0/src/dmtgen/template.py
+-rw-rw-rw-   0        0        0      722 2022-08-15 06:50:41.000000 dmtgen-1.0.0.dev0/src/dmtgen/template_generator.py
+drwxrwxrwx   0        0        0        0 2022-10-19 05:29:46.074677 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/
+-rw-rw-rw-   0        0        0      540 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-10-19 05:29:45.000000 dmtgen-1.0.0.dev0/src/dmtgen.egg-info/top_level.txt
```

### Comparing `dmtgen-0.4.1/LICENSE` & `dmtgen-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/PKG-INFO` & `dmtgen-1.0.0.dev0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtgen
-Version: 0.4.1
+Version: 1.0.0.dev0
 Summary: Python generator utilities for DMT
 Home-page: UNKNOWN
 Author: SINTEF Ocean
 License: UNKNOWN
 Description: Python generator utilities for DMT
         =================================================================
```

### Comparing `dmtgen-0.4.1/setup.py` & `dmtgen-1.0.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt',encoding='utf8') as f:
     required = f.read().splitlines()
 
 setup(
     name='dmtgen',
-    version='0.4.1',
+    version='1.0.0.dev0',
     author="SINTEF Ocean",
     description="Python generator utilities for DMT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages= find_packages(where="src"),
     package_data={'dmtgen': ['data/system/SIMOS/*.json']},
```

### Comparing `dmtgen-0.4.1/src/dmtgen/base_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/base_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         self.post_generate(output_dir)
 
     def copy_templates(self, template_root: Path, output_dir: Path):
         """Copy template folder to output folder"""
         # First we copy the entire tree structure
         # Then we have the sceleton to convert the files afterwards
-        shutil.copytree(str(template_root), str(output_dir),  dirs_exist_ok=True)
+        shutil.copytree(str(template_root), str(output_dir))
 
     def pre_generate(self,output_dir: Path):
         """ override in subclass """
 
     def post_generate(self,output_dir: Path):
         """ override in subclass """
```

### Comparing `dmtgen-0.4.1/src/dmtgen/basic_template_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/basic_template_generator.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen/common/blueprint.py` & `dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen/common/blueprint_attribute.py` & `dmtgen-1.0.0.dev0/src/dmtgen/common/blueprint_attribute.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen/common/enum_description.py` & `dmtgen-1.0.0.dev0/src/dmtgen/common/enum_description.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen/data/system/SIMOS/named_enity.json` & `dmtgen-1.0.0.dev0/src/dmtgen/data/system/SIMOS/named_enity.json`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen/template_generator.py` & `dmtgen-1.0.0.dev0/src/dmtgen/template_generator.py`

 * *Files identical despite different names*

### Comparing `dmtgen-0.4.1/src/dmtgen.egg-info/PKG-INFO` & `dmtgen-1.0.0.dev0/src/dmtgen.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtgen
-Version: 0.4.1
+Version: 1.0.0.dev0
 Summary: Python generator utilities for DMT
 Home-page: UNKNOWN
 Author: SINTEF Ocean
 License: UNKNOWN
 Description: Python generator utilities for DMT
         =================================================================
```

### Comparing `dmtgen-0.4.1/src/dmtgen.egg-info/SOURCES.txt` & `dmtgen-1.0.0.dev0/src/dmtgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

