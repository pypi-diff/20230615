# Comparing `tmp/xknxproject-3.1.1.tar.gz` & `tmp/xknxproject-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknxproject-3.1.1.tar", last modified: Fri Jun  9 21:16:56 2023, max compression
+gzip compressed data, was "xknxproject-3.2.0.tar", last modified: Thu Jun 15 21:45:37 2023, max compression
```

## Comparing `xknxproject-3.1.1.tar` & `xknxproject-3.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-09 21:16:39.000000 xknxproject-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-09 21:16:39.000000 xknxproject-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-09 21:16:56.981818 xknxproject-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-09 21:16:39.000000 xknxproject-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-09 21:16:39.000000 xknxproject-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 21:16:56.981818 xknxproject-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 21:16:39.000000 xknxproject-3.1.1/test/test_knxproj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 21:16:39.000000 xknxproject-3.1.1/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/combination/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/combination/combination.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/application_program_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/hardware_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/knx_master_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/project_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/models/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/knxproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xknxproj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/xml/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/zip/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/zip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 21:45:18.000000 xknxproject-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 21:45:18.000000 xknxproject-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-15 21:45:37.069826 xknxproject-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-15 21:45:18.000000 xknxproject-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-15 21:45:18.000000 xknxproject-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-15 21:45:37.069826 xknxproject-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-15 21:45:18.000000 xknxproject-3.2.0/test/test_knxproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-15 21:45:18.000000 xknxproject-3.2.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/combination/combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/loader/application_program_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/loader/hardware_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/loader/knx_master_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/loader/project_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/models/knxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/xknxproj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/xml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-15 21:45:18.000000 xknxproject-3.2.0/xknxproject/zip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:45:37.069826 xknxproject-3.2.0/xknxproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-15 21:45:36.000000 xknxproject-3.2.0/xknxproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 21:45:37.000000 xknxproject-3.2.0/xknxproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:45:36.000000 xknxproject-3.2.0/xknxproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 21:45:36.000000 xknxproject-3.2.0/xknxproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 21:45:36.000000 xknxproject-3.2.0/xknxproject.egg-info/top_level.txt
```

### Comparing `xknxproject-3.1.1/LICENSE` & `xknxproject-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/PKG-INFO` & `xknxproject-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.1.1
+Version: 3.2.0
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.1.1/README.md` & `xknxproject-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/pyproject.toml` & `xknxproject-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/test/test_knxproj.py` & `xknxproject-3.2.0/test/test_knxproj.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 def test_parse_project_ets5():
     """Test parsing of ETS5 project."""
     knxproj = XKNXProj(RESOURCES_PATH / "xknx_test_project.knxproj", "test")
     project = knxproj.parse()
     assert_stub(project, "xknx_test_project.json")
 
 
+def test_parse_project_ets4():
+    """Test parsing of ETS4 project."""
+    knxproj = XKNXProj(
+        RESOURCES_PATH / "test_project-ets4.knxproj", "test", language="de-DE"
+    )
+    project = knxproj.parse()
+    assert_stub(project, "test_project-ets4.json")
+
+
 def test_parse_project_modules():
     """Test parsing of ETS5 project including 2 identical devices with module definitions."""
     knxproj = XKNXProj(
         RESOURCES_PATH / "module-definition-test.knxproj",
         language="De",  # resolves to "de-DE" in parser for knx_master.xml
     )
     project = knxproj.parse()
```

### Comparing `xknxproject-3.1.1/test/test_util.py` & `xknxproject-3.2.0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/combination/combination.py` & `xknxproject-3.2.0/xknxproject/combination/combination.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/loader/application_program_loader.py` & `xknxproject-3.2.0/xknxproject/loader/application_program_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/loader/hardware_loader.py` & `xknxproject-3.2.0/xknxproject/loader/hardware_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/loader/knx_master_loader.py` & `xknxproject-3.2.0/xknxproject/loader/knx_master_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """KNX Master Data Loader."""
 from __future__ import annotations
 
 import logging
 from xml.etree import ElementTree
 from zipfile import Path
 
+from xknxproject.const import ETS4_PRODUCT_LANGUAGES
+from xknxproject.zip import KNXProjContents
+
 _LOGGER = logging.getLogger("xknxproject.log")
 
 
 class KNXMasterLoader:
     """Load KNX master XML."""
 
     @staticmethod
     def load(
+        knx_proj_contents: KNXProjContents,
         knx_master_file: Path,
         language: str | None,
     ) -> tuple[dict[str, str], dict[str, str], str | None]:
         """Load KNX master data."""
         manufacturer_mapping: dict[str, str] = {}
         space_usage_mapping: dict[str, str] = {}
         product_languages: list[str] = []  # eg. "en-US", "de-DE", "fr-FR"
@@ -24,20 +28,25 @@
 
         with knx_master_file.open(mode="rb") as master_xml:
             tree = ElementTree.parse(master_xml)
             for manufacturer in tree.findall(".//{*}Manufacturers/{*}Manufacturer"):
                 identifier = manufacturer.get("Id", "")
                 manufacturer_mapping[identifier] = manufacturer.get("Name", "")
 
-            for space_usage_node in tree.findall(".//{*}SpaceUsages/{*}SpaceUsage"):
-                identifier = space_usage_node.get("Id", "")
-                space_usage_mapping[identifier] = space_usage_node.get("Text", "")
+            if knx_proj_contents.is_ets4_project():
+                # No SpaceUsage in ETS4, neither ProductLanguages. Therefore, we use an
+                # hardcoded list of common product languages
+                product_languages = ETS4_PRODUCT_LANGUAGES
+            else:
+                for space_usage_node in tree.findall(".//{*}SpaceUsages/{*}SpaceUsage"):
+                    identifier = space_usage_node.get("Id", "")
+                    space_usage_mapping[identifier] = space_usage_node.get("Text", "")
 
-            for language_node in tree.findall(".//{*}ProductLanguages/{*}Language"):
-                product_languages.append(language_node.get("Identifier", ""))
+                for language_node in tree.findall(".//{*}ProductLanguages/{*}Language"):
+                    product_languages.append(language_node.get("Identifier", ""))
 
             if language is not None:
                 language_code = KNXMasterLoader.get_language_code(
                     language, product_languages
                 )
 
             if language_code:
```

### Comparing `xknxproject-3.1.1/xknxproject/loader/project_loader.py` & `xknxproject-3.2.0/xknxproject/loader/project_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,116 +43,120 @@
             for ga_element in tree.findall(
                 # `//` to ignore <GroupRange> tags to support different GA level formats
                 "{*}Project/{*}Installations/{*}Installation/{*}GroupAddresses//{*}GroupAddress"
             ):
                 group_address_list.append(
                     _GroupAddressLoader.load(group_address_element=ga_element),
                 )
+            topology_loader = _TopologyLoader(knx_proj_contents)
             for topology_element in tree.findall(
                 "{*}Project/{*}Installations/{*}Installation/{*}Topology"
             ):
-                areas.extend(
-                    _TopologyLoader.load(topology_element=topology_element),
-                )
+                areas.extend(topology_loader.load(topology_element=topology_element))
             for area in areas:
                 for line in area.lines:
                     devices.extend(line.devices)
+
+            # ETS4 has a different naming for locations than ETS5/6
+            element_name = (
+                "Buildings" if knx_proj_contents.is_ets4_project() else "Locations"
+            )
+
+            location_loader = _LocationLoader(
+                knx_proj_contents, devices, space_usage_names
+            )
             for location_element in tree.findall(
-                "{*}Project/{*}Installations/{*}Installation/{*}Locations"
+                f"{{*}}Project/{{*}}Installations/{{*}}Installation/{{*}}{element_name}"
             ):
-                spaces.extend(
-                    _LocationLoader(devices, space_usage_names).load(
-                        location_element=location_element
-                    ),
-                )
+                spaces.extend(location_loader.load(location_element=location_element))
 
         with knx_proj_contents.open_project_meta() as project_file:
             tree = ElementTree.parse(project_file)
             project_info = load_project_info(tree)
 
         return group_address_list, areas, devices, spaces, project_info
 
 
 class _GroupAddressLoader:
     """Load GroupAddress info from KNX XML."""
 
     @staticmethod
     def load(group_address_element: ElementTree.Element) -> XMLGroupAddress:
         """Load GroupAddress mappings."""
-
+        project_uid = group_address_element.get("Puid")
         return XMLGroupAddress(
             name=group_address_element.get("Name", ""),
             identifier=group_address_element.get("Id", ""),
             address=group_address_element.get("Address", ""),
-            project_uid=int(group_address_element.get("Puid")),  # type: ignore[arg-type]
+            project_uid=int(project_uid) if project_uid else None,
             description=group_address_element.get("Description", ""),
             dpt=get_dpt_type(group_address_element.get("DatapointType")),
         )
 
 
 class _TopologyLoader:
     """Load topology from KNX XML."""
 
-    @staticmethod
-    def load(topology_element: ElementTree.Element) -> list[XMLArea]:
+    def __init__(self, knx_proj_contents: KNXProjContents) -> None:
+        self.__knx_proj_contents = knx_proj_contents
+
+    def load(self, topology_element: ElementTree.Element) -> list[XMLArea]:
         """Load topology mappings."""
         areas: list[XMLArea] = []
 
         for area in topology_element.findall("{*}Area"):
-            areas.append(_TopologyLoader._create_area(area))
+            areas.append(self._create_area(area))
 
         return areas
 
-    @staticmethod
-    def _create_area(area_element: ElementTree.Element) -> XMLArea:
+    def _create_area(self, area_element: ElementTree.Element) -> XMLArea:
         """Create an Area."""
         address: int = int(area_element.get("Address", ""))
         name: str = area_element.get("Name", "")
         description: str | None = area_element.get("Description")
         area: XMLArea = XMLArea(address, name, description, [])
 
         for line_element in area_element:
-            area.lines.append(_TopologyLoader._create_line(line_element, area))
+            area.lines.append(self._create_line(line_element, area))
 
         return area
 
-    @staticmethod
-    def _create_line(line_element: ElementTree.Element, area: XMLArea) -> XMLLine:
+    def _create_line(self, line_element: ElementTree.Element, area: XMLArea) -> XMLLine:
         """Create a Line."""
         address: int = int(line_element.get("Address", ""))
         name: str = line_element.get("Name", "")
         description: str | None = line_element.get("Description")
         if (segment := line_element.find("{*}Segment")) is not None:
             #  ETS-6 (21) adds "Segment" tags between "Line" and "DeviceInstance" tags
             medium_type = segment.get("MediumTypeRefId", "")
         else:
             medium_type = line_element.get("MediumTypeRefId", "")
         line: XMLLine = XMLLine(address, description, name, medium_type, [], area)
 
         for device_element in line_element.findall(".//{*}DeviceInstance"):
-            if device := _TopologyLoader._create_device(device_element, line):
+            if device := self._create_device(device_element, line):
                 line.devices.append(device)
 
         return line
 
-    @staticmethod
     def _create_device(
-        device_element: ElementTree.Element, line: XMLLine
+        self, device_element: ElementTree.Element, line: XMLLine
     ) -> DeviceInstance | None:
         """Create device."""
         address: str | None = device_element.get("Address")
         #  devices like power supplies do usually not have an IA.
         if address is None:
             return None
 
+        project_uid = device_element.get("Puid")
         product_ref = device_element.get("ProductRefId", "")
         device: DeviceInstance = DeviceInstance(
             identifier=device_element.get("Id", ""),
             address=address,
-            project_uid=int(device_element.get("Puid")),  # type: ignore[arg-type]
+            project_uid=int(project_uid) if project_uid else None,
             name=device_element.get("Name", ""),
             description=device_element.get("Description", ""),
             last_modified=device_element.get("LastModified", ""),
             product_ref=product_ref,
             hardware_program_ref=device_element.get("Hardware2ProgramRefId", ""),
             line=line,
             manufacturer=product_ref.split("_", 1)[0],
@@ -161,27 +165,53 @@
         for sub_node in device_element:
             if sub_node.tag.endswith("AdditionalAddresses"):
                 for address_node in sub_node:
                     if _address := address_node.get("Address"):
                         device.additional_addresses.append(_address)
             if sub_node.tag.endswith("ComObjectInstanceRefs"):
                 for com_object in sub_node:
-                    if instance := _TopologyLoader._create_com_object_instance(
-                        com_object
-                    ):
+                    if instance := self._create_com_object_instance(com_object):
                         device.com_object_instance_refs.append(instance)
 
         return device
 
     @staticmethod
+    def __get_links_from_ets4(com_object: ElementTree.Element) -> list[str]:
+        # Check if "Connectors" is available. This will always fail for ETS5/6
+        if (connectors := com_object.find("{*}Connectors")) is None:
+            return []
+
+        # Send GA is the primary GA, Receive GA are additional group addresses
+        ga_list = connectors.findall("{*}Send") + connectors.findall("{*}Receive")
+
+        # Remove the project ID from GA
+        return [ga.get("GroupAddressRefId", "").split("_")[1] for ga in ga_list]
+
+    @staticmethod
+    def __get_links_from_ets5(com_object: ElementTree.Element) -> list[str]:
+        # ETS5/6 uses a space-separated string of GA
+        links = com_object.get("Links")
+
+        if links is None:
+            return []
+
+        return links.split(" ")
+
     def _create_com_object_instance(
+        self,
         com_object: ElementTree.Element,
     ) -> ComObjectInstanceRef | None:
         """Create ComObjectInstanceRef."""
-        if not (links := com_object.get("Links")):
+
+        if self.__knx_proj_contents.is_ets4_project():
+            links = self.__get_links_from_ets4(com_object)
+        else:
+            links = self.__get_links_from_ets5(com_object)
+
+        if not links:
             return None
 
         return ComObjectInstanceRef(
             identifier=com_object.get("Id"),
             ref_id=com_object.get("RefId"),  # type: ignore[arg-type]
             text=com_object.get("Text"),
             function_text=com_object.get("FunctionText"),
@@ -189,57 +219,63 @@
             write_flag=parse_xml_flag(com_object.get("WriteFlag")),
             communication_flag=parse_xml_flag(com_object.get("CommunicationFlag")),
             transmit_flag=parse_xml_flag(com_object.get("TransmitFlag")),
             update_flag=parse_xml_flag(com_object.get("UpdateFlag")),
             read_on_init_flag=parse_xml_flag(com_object.get("ReadOnInitFlag")),
             datapoint_types=parse_dpt_types(com_object.get("DatapointType")),
             description=com_object.get("Description"),
-            links=links.split(" "),
+            links=links,
         )
 
 
 class _LocationLoader:
     """Load location infos from KNX XML."""
 
     def __init__(
         self,
+        knx_proj_contents: KNXProjContents,
         devices: list[DeviceInstance],
         space_usage_names: dict[str, str],
     ):
         """Initialize the LocationLoader."""
+        self._element_name = (
+            "BuildingPart" if knx_proj_contents.is_ets4_project() else "Space"
+        )
         self.devices: dict[str, str] = {
             device.identifier: device.individual_address for device in devices
         }
         self.space_usage_names = space_usage_names
 
     def load(self, location_element: ElementTree.Element) -> list[XMLSpace]:
         """Load Location mappings."""
         return [
-            self.parse_space(space) for space in location_element.findall("{*}Space")
+            self.parse_space(space)
+            for space in location_element.findall(f"{{*}}{self._element_name}")
         ]
 
     def parse_space(self, node: ElementTree.Element) -> XMLSpace:
         """Parse a space from the document."""
         usage_id = node.get("Usage")
         usage_text = self.space_usage_names.get(usage_id, "") if usage_id else ""
+        project_uid = node.get("Puid")
         space: XMLSpace = XMLSpace(
             identifier=node.get("Id"),  # type: ignore[arg-type]
             name=node.get("Name"),  # type: ignore[arg-type]
             space_type=SpaceType(node.get("Type")),
             usage_id=usage_id,
             usage_text=usage_text,
             number=node.get("Number", ""),
             description=node.get("Description", ""),
-            project_uid=int(node.get("Puid")),  # type: ignore[arg-type]
+            project_uid=int(project_uid) if project_uid else None,
             spaces=[],
             devices=[],
         )
 
         for sub_node in node:
-            if sub_node.tag.endswith("Space"):
+            if sub_node.tag.endswith(self._element_name):
                 # recursively call parse space since this can be nested for an unbound time in the XSD
                 space.spaces.append(self.parse_space(sub_node))
             elif sub_node.tag.endswith("DeviceInstanceRef"):
                 if individual_address := self.devices.get(sub_node.get("RefId", "")):
                     space.devices.append(individual_address)
 
         return space
```

### Comparing `xknxproject-3.1.1/xknxproject/models/__init__.py` & `xknxproject-3.2.0/xknxproject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/models/knxproject.py` & `xknxproject-3.2.0/xknxproject/models/knxproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     """Devices dictionary."""
 
     name: str
     hardware_name: str
     description: str
     manufacturer_name: str
     individual_address: str
-    project_uid: int
+    project_uid: int | None
     communication_object_ids: list[str]
 
 
 class Line(TypedDict):
     """Line typed dict."""
 
     name: str
@@ -69,15 +69,15 @@
 class GroupAddress(TypedDict):
     """GroupAddress typed dict."""
 
     name: str
     identifier: str
     raw_address: int
     address: str
-    project_uid: int
+    project_uid: int | None
     dpt: DPTType | None
     communication_object_ids: list[str]
     description: str
 
 
 class Space(TypedDict):
     """Space typed dict."""
@@ -85,15 +85,15 @@
     type: str
     identifier: str
     name: str
     usage_id: str | None
     usage_text: str
     number: str
     description: str
-    project_uid: int
+    project_uid: int | None
     devices: list[str]
     spaces: dict[str, Space]
 
 
 class ProjectInfo(TypedDict):
     """Information about the project."""
```

### Comparing `xknxproject-3.1.1/xknxproject/models/models.py` & `xknxproject-3.2.0/xknxproject/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 import re
 
 from xknxproject.models.knxproject import DPTType
 from xknxproject.models.static import SpaceType
+from xknxproject.zip import KNXProjContents
 
 
 class XMLGroupAddress:
     """Class that represents a group address."""
 
     def __init__(
         self,
         name: str,
         identifier: str,
         address: str,
-        project_uid: int,
+        project_uid: int | None,
         description: str,
         dpt: DPTType | None,
     ):
         """Initialize a group address."""
         self.name = name
         self.identifier = identifier.split("_")[1]
         self.raw_address = int(address)
@@ -70,15 +71,15 @@
     """Class that represents a device instance."""
 
     def __init__(
         self,
         *,
         identifier: str,
         address: str,
-        project_uid: int,
+        project_uid: int | None,
         name: str,
         description: str,
         last_modified: str,
         product_ref: str,
         hardware_program_ref: str,
         line: XMLLine,
         manufacturer: str,
@@ -144,19 +145,24 @@
     com_object_ref_id: str | None = None
 
     # only available form ComObject and ComObjectRef
     name: str | None = None
     number: int | None = None
     object_size: str | None = None
 
-    def resolve_com_object_ref_id(self, application_program_ref: str) -> None:
+    def resolve_com_object_ref_id(
+        self, application_program_ref: str, knx_proj_contents: KNXProjContents
+    ) -> None:
         """Prepend the ref_id with the application program ref."""
         # Remove module and ModuleInstance occurrence as they will not be in the application program directly
         ref_id = re.sub(r"(M-\d+?_MI-\d+?_)", "", self.ref_id)
-        self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
+        if knx_proj_contents.is_ets4_project():
+            self.com_object_ref_id = ref_id
+        else:
+            self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
 
     def merge_from_application(self, com_object: ComObject | ComObjectRef) -> None:
         """Fill missing information with information parsed from the application program."""
         if self.name is None:
             self.name = com_object.name
         if self.text is None:
             self.text = com_object.text
@@ -260,15 +266,15 @@
     identifier: str
     name: str
     space_type: SpaceType
     usage_id: str | None  # SU-<int> resolved from knx_master.xml (with translation)
     usage_text: str  # default to "" - translated
     number: str  # default to ""
     description: str  # default to ""
-    project_uid: int
+    project_uid: int | None
     spaces: list[XMLSpace]
     devices: list[str]  # [DeviceInstance.individual_address]
 
 
 @dataclass
 class Product:
     """Model a Product instance."""
```

### Comparing `xknxproject-3.1.1/xknxproject/models/static.py` & `xknxproject-3.2.0/xknxproject/models/static.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/util.py` & `xknxproject-3.2.0/xknxproject/util.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/xknxproj.py` & `xknxproject-3.2.0/xknxproject/xknxproj.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.1/xknxproject/xml/parser.py` & `xknxproject-3.2.0/xknxproject/xml/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,15 @@
     def load(self, language: str | None) -> None:
         """Load XML files."""
         (
             manufacturer_names,
             space_usage_names,
             self.language_code,
         ) = KNXMasterLoader.load(
+            knx_proj_contents=self.knx_proj_contents,
             knx_master_file=self.knx_proj_contents.root_path / "knx_master.xml",
             language=language,
         )
         (
             self.group_addresses,
             self.areas,
             self.devices,
@@ -240,15 +241,17 @@
                     "Could not find application_program_ref for device %s with hardware_program_ref %s",
                     device.individual_address,
                     device.hardware_program_ref,
                 )
                 continue
             device.application_program_ref = application_program_ref
             for com_object in device.com_object_instance_refs:
-                com_object.resolve_com_object_ref_id(application_program_ref)
+                com_object.resolve_com_object_ref_id(
+                    application_program_ref, self.knx_proj_contents
+                )
 
         application_programs = (
             ApplicationProgramLoader.get_application_program_files_for_devices(
                 project_root_path=self.knx_proj_contents.root_path,
                 devices=self.devices,
             )
         )
```

### Comparing `xknxproject-3.1.1/xknxproject/zip/extractor.py` & `xknxproject-3.2.0/xknxproject/zip/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import IO
 from zipfile import Path as ZipPath, ZipFile, ZipInfo
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 import pyzipper
 
-from xknxproject.const import ETS_6_SCHEMA_VERSION
+from xknxproject.const import ETS_4_2_SCHEMA_VERSION, ETS_6_SCHEMA_VERSION
 from xknxproject.exceptions import (
     InvalidPasswordException,
     ProjectNotFoundException,
     UnexpectedFileContent,
 )
 
 _LOGGER = logging.getLogger("xknxproject.log")
@@ -36,26 +36,32 @@
     ):
         """Initialize a KNXProjContents."""
         self._project_archive = project_archive
         self._project_relative_path = project_relative_path
         self.root = root_zip
         self.root_path = ZipPath(root_zip)
         self.xml_namespace = xml_namespace
+        self.schema_version = _get_schema_version(xml_namespace)
+
+    def is_ets4_project(self) -> bool:
+        """Check if the project is an ETS4 project."""
+        return self.schema_version <= ETS_4_2_SCHEMA_VERSION
 
     def open_project_0(self) -> IO[bytes]:
         """Open the project 0.xml file."""
         return self._project_archive.open(
             f"{self._project_relative_path}0.xml",
             mode="r",
         )
 
     def open_project_meta(self) -> IO[bytes]:
         """Open the project.xml file."""
+        project_filename = "Project.xml" if self.is_ets4_project() else "project.xml"
         return self._project_archive.open(
-            f"{self._project_relative_path}project.xml",
+            f"{self._project_relative_path}{project_filename}",
             mode="r",
         )
 
 
 @contextmanager
 def extract(
     archive_path: Path, password: str | None = None
@@ -113,31 +119,29 @@
 def _extract_protected_project_file(
     archive_zip: ZipFile, info: ZipInfo, password: str | None, schema_version: int
 ) -> Iterator[ZipFile]:
     """Unzip a protected ETS5/6 project file."""
     if not password:
         raise InvalidPasswordException("Password required.")
 
-    project_archive: ZipFile
-    if not _is_ets6_project(schema_version):
-        try:
+    try:
+        project_archive: ZipFile
+        # Password protection is different for ETS4/5 and ETS6
+        if schema_version < ETS_6_SCHEMA_VERSION:
             project_archive = ZipFile(archive_zip.open(info, mode="r"), mode="r")
             project_archive.setpassword(password.encode("utf-8"))
             yield project_archive
-        except RuntimeError as exception:
-            raise InvalidPasswordException("Invalid password.") from exception
-    else:
-        try:
+        else:
             project_archive = pyzipper.AESZipFile(
                 archive_zip.open(info, mode="r"), mode="r"
             )
             project_archive.setpassword(_generate_ets6_zip_password(password))
             yield project_archive
-        except RuntimeError as exception:
-            raise InvalidPasswordException("Invalid password.") from exception
+    except RuntimeError as exception:
+        raise InvalidPasswordException("Invalid password.") from exception
 
 
 def _get_xml_namespace(project_zip: ZipFile) -> str:
     """Get the XML namespace of the project."""
     with project_zip.open("knx_master.xml", mode="r") as master:
         for line_number, line in enumerate(master, start=1):
             if line_number == 2:
@@ -163,19 +167,14 @@
         _LOGGER.error("Could not parse schema version from %s", namespace)
         raise UnexpectedFileContent("Could not parse schema version.")
 
     _LOGGER.debug("Schema version: %s", schema_version)
     return schema_version
 
 
-def _is_ets6_project(schema_version: int) -> bool:
-    """Check if the project is an ETS6 project."""
-    return schema_version >= ETS_6_SCHEMA_VERSION
-
-
 def _generate_ets6_zip_password(password: str) -> bytes:
     """Generate ZIP archive password."""
     return base64.b64encode(
         PBKDF2HMAC(
             algorithm=hashes.SHA256(),
             length=32,
             salt=b"21.project.ets.knx.org",
```

### Comparing `xknxproject-3.1.1/xknxproject.egg-info/PKG-INFO` & `xknxproject-3.2.0/xknxproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.1.1
+Version: 3.2.0
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.1.1/xknxproject.egg-info/SOURCES.txt` & `xknxproject-3.2.0/xknxproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

