# Comparing `tmp/libcoveofds-0.7.0.tar.gz` & `tmp/libcoveofds-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveofds-0.7.0.tar", last modified: Wed Jan 11 15:56:27 2023, max compression
+gzip compressed data, was "libcoveofds-0.8.0.tar", last modified: Thu Jun 15 12:07:14 2023, max compression
```

## Comparing `libcoveofds-0.7.0.tar` & `libcoveofds-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-01-11 15:56:27.433460 libcoveofds-0.7.0/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      900 2022-10-04 14:04:27.000000 libcoveofds-0.7.0/LICENSE
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      627 2023-01-11 15:56:27.433460 libcoveofds-0.7.0/PKG-INFO
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      837 2023-01-11 15:30:07.000000 libcoveofds-0.7.0/README.rst
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-01-11 15:56:27.433460 libcoveofds-0.7.0/libcove2/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)        0 2022-11-03 16:05:58.000000 libcoveofds-0.7.0/libcove2/__init__.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     3742 2022-11-23 10:11:57.000000 libcoveofds-0.7.0/libcove2/common.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-01-11 15:56:27.433460 libcoveofds-0.7.0/libcoveofds/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2022-06-22 14:29:56.000000 libcoveofds-0.7.0/libcoveofds/__init__.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      561 2022-11-23 16:53:07.000000 libcoveofds-0.7.0/libcoveofds/additionalfields.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     5275 2022-12-20 08:46:12.000000 libcoveofds-0.7.0/libcoveofds/cli.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)    20731 2023-01-11 15:56:20.000000 libcoveofds-0.7.0/libcoveofds/geojson.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     2159 2022-12-01 11:25:10.000000 libcoveofds-0.7.0/libcoveofds/jsonschemavalidate.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-01-11 15:56:20.000000 libcoveofds-0.7.0/libcoveofds/python_validate.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     2152 2023-01-11 15:56:20.000000 libcoveofds-0.7.0/libcoveofds/schema.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-01-11 15:56:27.433460 libcoveofds-0.7.0/libcoveofds.egg-info/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      627 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/PKG-INFO
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      474 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/SOURCES.txt
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)        1 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/dependency_links.txt
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)       53 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/entry_points.txt
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      106 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/requires.txt
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)       21 2023-01-11 15:56:27.000000 libcoveofds-0.7.0/libcoveofds.egg-info/top_level.txt
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)       61 2023-01-11 15:56:27.437460 libcoveofds-0.7.0/setup.cfg
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     1114 2023-01-11 15:56:23.000000 libcoveofds-0.7.0/setup.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-06-07 07:23:52.000000 libcoveofds-0.8.0/MANIFEST.in
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      837 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/README.rst
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.536264 libcoveofds-0.8.0/libcove2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-07 07:24:06.000000 libcoveofds-0.8.0/libcove2/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3742 2023-06-07 07:24:06.000000 libcoveofds-0.8.0/libcove2/common.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/additionalfields.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5520 2023-06-13 07:34:18.000000 libcoveofds-0.8.0/libcoveofds/cli.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds/data/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)   215804 2023-06-15 10:03:03.000000 libcoveofds-0.8.0/libcoveofds/data/schema-0-3-0.json
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    21467 2023-06-13 07:34:18.000000 libcoveofds-0.8.0/libcoveofds/geojson.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2159 2023-05-04 15:08:13.000000 libcoveofds-0.8.0/libcoveofds/jsonschemavalidate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/python_validate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1595 2023-06-15 10:03:03.000000 libcoveofds-0.8.0/libcoveofds/schema.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds.egg-info/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      513 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/SOURCES.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/dependency_links.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       52 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/entry_points.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       89 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/requires.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       21 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/top_level.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/setup.cfg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1075 2023-06-15 12:06:39.000000 libcoveofds-0.8.0/setup.py
```

### Comparing `libcoveofds-0.7.0/PKG-INFO` & `libcoveofds-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.7.0
+Version: 0.8.0
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
+License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
 Project-URL: Source, https://github.com/Open-Telecoms-Data/lib-cove-ofds
+Description: A data review library
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Provides-Extra: dev
-License-File: LICENSE
-
-A data review library
```

### Comparing `libcoveofds-0.7.0/README.rst` & `libcoveofds-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.7.0/libcove2/common.py` & `libcoveofds-0.8.0/libcove2/common.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.7.0/libcoveofds/additionalfields.py` & `libcoveofds-0.8.0/libcoveofds/additionalfields.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.7.0/libcoveofds/cli.py` & `libcoveofds-0.8.0/libcoveofds/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,22 @@
         with open(args.inputnodesfilename) as fp:
             nodes_data = json.load(fp)
 
         with open(args.inputspansfilename) as fp:
             spans_data = json.load(fp)
 
         converter = libcoveofds.geojson.GeoJSONToJSONConverter()
-        converter.process_data(nodes_data, spans_data)
+        converter.process_data(
+            nodes_data,
+            assumed_feature_type=libcoveofds.geojson.GeoJSONAssumeFeatureType.NODE,
+        )
+        converter.process_data(
+            spans_data,
+            assumed_feature_type=libcoveofds.geojson.GeoJSONAssumeFeatureType.SPAN,
+        )
 
         with open(args.outputfilename, "w") as fp:
             json.dump(converter.get_json(), fp, indent=4)
 
         if args.outputmetafilename:
             with open(args.outputmetafilename, "w") as fp:
                 json.dump(converter.get_meta_json(), fp, indent=4)
```

### Comparing `libcoveofds-0.7.0/libcoveofds/geojson.py` & `libcoveofds-0.8.0/libcoveofds/geojson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import copy
 from collections import defaultdict
+from enum import Enum
 from typing import Optional
 
 from json_merge_patch import create_patch as json_diff_function
 
 from libcove2.common import fields_present_generator
 
 
+class GeoJSONAssumeFeatureType(Enum):
+    NODE = "node"
+    SPAN = "span"
+
+
 class JSONToGeoJSONConverter:
     """Converts JSON data to GeoJSON."""
 
     def __init__(self):
         self._nodes_geojson_features: list = []
         self._spans_geojson_features: list = []
 
@@ -141,14 +147,15 @@
         if "phase" in reduced_node_data:
             reduced_node_data["phase"] = self._dereference_object(
                 reduced_node_data["phase"], phases
             )
 
         feature["properties"] = reduced_node_data
         feature["properties"]["network"] = reduced_network_data
+        feature["properties"]["featureType"] = "node"
 
         return feature
 
     def _convert_span_to_feature(
         self,
         span_data: dict,
         reduced_network_data: dict,
@@ -191,14 +198,15 @@
             if endpoint in reduced_span_data:
                 for node in nodes:
                     if "id" in node and node["id"] == reduced_span_data[endpoint]:
                         reduced_span_data[endpoint] = node
 
         feature["properties"] = reduced_span_data
         feature["properties"]["network"] = reduced_network_data
+        feature["properties"]["featureType"] = "span"
 
         return feature
 
 
 class GeoJSONToJSONConverter:
     """Converts GeoJSON data to JSON."""
 
@@ -206,29 +214,41 @@
         self._networks: dict = {}
         self._inconsistent_phase_ids_by_network_id: defaultdict = defaultdict(set)
         self._inconsistent_organisation_ids_by_network_id: defaultdict = defaultdict(
             set
         )
         self._inconsistent_network_ids_seen: set = set()
 
-    def process_data(self, nodes_data: dict, spans_data: dict) -> None:
-        """Process data. Results are stored on object to get with other methods."""
+    def process_data(
+        self,
+        data: dict,
+        assumed_feature_type: GeoJSONAssumeFeatureType = GeoJSONAssumeFeatureType.NODE,
+    ) -> None:
+        """Process data. Results are stored on object to get with other methods.
+
+        Can be called multiple times with as many GeoJSON files as needed.
+        """
         # Network
-        for geojson_feature in nodes_data.get("features", []):
-            self._process_network(geojson_feature)
-        for geojson_feature in spans_data.get("features", []):
+        for geojson_feature in data.get("features", []):
             self._process_network(geojson_feature)
 
-        # Nodes
-        for geojson_feature in nodes_data.get("features", []):
-            self._process_node(geojson_feature)
-
-        # Spans
-        for geojson_feature in spans_data.get("features", []):
-            self._process_span(geojson_feature)
+        # Nodes/Spans
+        for geojson_feature in data.get("features", []):
+            type = assumed_feature_type.value
+            if isinstance(geojson_feature.get("properties"), dict) and isinstance(
+                geojson_feature["properties"].get("featureType"), str
+            ):
+                type = geojson_feature["properties"]["featureType"]
+            if type.lower() == "node":
+                self._process_node(geojson_feature)
+            elif type.lower() == "span":
+                self._process_span(geojson_feature)
+            else:
+                # TODO log error
+                pass
 
     def _process_network(self, geojson_feature_node_or_span: dict) -> None:
         if (
             "properties" in geojson_feature_node_or_span
             and "network" in geojson_feature_node_or_span["properties"]
         ):
             network = geojson_feature_node_or_span["properties"]["network"]
@@ -311,15 +331,15 @@
                                             out.append(phase_data)
                                         else:
                                             out.append(phase_reference)
                                     contract["relatedPhases"] = out
 
     def _process_node(self, geojson_feature_node: dict) -> None:
         node = copy.deepcopy(geojson_feature_node.get("properties", {}))
-        for key_to_remove in ["network"]:
+        for key_to_remove in ["network", "featureType"]:
             if key_to_remove in node:
                 del node[key_to_remove]
         network_id = (
             geojson_feature_node.get("properties", {}).get("network", {}).get("id")
         )
         if network_id not in self._networks.keys():
             # TODO log error
@@ -346,15 +366,15 @@
         if geojson_feature_node.get("geometry"):
             node["location"] = geojson_feature_node["geometry"]
 
         self._networks[network_id]["nodes"].append(node)
 
     def _process_span(self, geojson_feature_span: dict) -> None:
         span = copy.deepcopy(geojson_feature_span.get("properties", {}))
-        for key_to_remove in ["network"]:
+        for key_to_remove in ["network", "featureType"]:
             if key_to_remove in span:
                 del span[key_to_remove]
         network_id = (
             geojson_feature_span.get("properties", {}).get("network", {}).get("id")
         )
         if network_id not in self._networks.keys():
             # TODO log error
@@ -377,16 +397,18 @@
             phase_data = self._process_phase(network_id, span["phase"])
             if phase_data:
                 span["phase"] = phase_data
 
         if geojson_feature_span.get("geometry"):
             span["route"] = geojson_feature_span["geometry"]
 
-        span["start"] = span.get("start", {}).get("id")
-        span["end"] = span.get("end", {}).get("id")
+        if isinstance(span.get("start"), dict):
+            span["start"] = span["start"].get("id")
+        if isinstance(span.get("end"), dict):
+            span["end"] = span["end"].get("id")
 
         self._networks[network_id]["spans"].append(span)
 
     def _process_phase(self, network_id: str, phase: dict) -> Optional[dict]:
         phase_id = phase.get("id")
         # If no id, can't do anything. TODO log somewhere?
         if not phase_id or not isinstance(phase_id, str):
```

### Comparing `libcoveofds-0.7.0/libcoveofds/jsonschemavalidate.py` & `libcoveofds-0.8.0/libcoveofds/jsonschemavalidate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.7.0/libcoveofds/python_validate.py` & `libcoveofds-0.8.0/libcoveofds/python_validate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.7.0/libcoveofds/schema.py` & `libcoveofds-0.8.0/libcoveofds/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-import jsonref
-import requests
+import json
+import os
 
 from libcove2.common import schema_dict_fields_generator
 
+_schema_folder = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
+
 
 class OFDSSchema:
     """Represents and provides information about the schema."""
 
-    # Please lock to a specific tag or commit hash - never a branch name!
-    # This prevents changes to the standard suddenly breaking previously working software/tests etc.
-    package_schema_url: str = "https://raw.githubusercontent.com/Open-Telecoms-Data/open-fibre-data-standard/0__2__0/schema/network-package-schema.json"
-    data_schema_url: str = "https://raw.githubusercontent.com/Open-Telecoms-Data/open-fibre-data-standard/0__2__0/schema/network-schema.json"
+    package_schema_url: str = os.path.join(_schema_folder, "schema-0-3-0.json")
 
     def get_package_schema(self):
-        r = requests.get(self.package_schema_url)
-        return r.json()
-
-    def get_package_schema_dereferenced(self):
-        r = requests.get(self.package_schema_url)
-        return jsonref.loads(r.text)
-
-    def get_data_schema(self):
-        r = requests.get(self.data_schema_url)
-        return r.json()
+        with open(self.package_schema_url) as fp:
+            return json.load(fp)
 
     def get_link_rels_for_external_nodes(self) -> list:
         return [
             "tag:opentelecomdata.net,2022:nodesAPI",
             "tag:opentelecomdata.net,2022:nodesFile",
         ]
 
     def get_link_rels_for_external_spans(self) -> list:
         return [
             "tag:opentelecomdata.net,2022:spansAPI",
             "tag:opentelecomdata.net,2022:spansFile",
         ]
 
     def get_package_schema_fields(self) -> set:
-        return set(schema_dict_fields_generator(self.get_package_schema_dereferenced()))
+        return set(schema_dict_fields_generator(self.get_package_schema()))
 
     def extract_data_ids_from_data_and_path(self, data: dict, path: list) -> dict:
         out: dict = {}
         # network_id
         if len(path) >= 2 and path[0] == "networks":
             network_id = data["networks"][path[1]].get("id")
             if network_id:
```

### Comparing `libcoveofds-0.7.0/libcoveofds.egg-info/PKG-INFO` & `libcoveofds-0.8.0/libcoveofds.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.7.0
+Version: 0.8.0
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
+License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
 Project-URL: Source, https://github.com/Open-Telecoms-Data/lib-cove-ofds
+Description: A data review library
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Provides-Extra: dev
-License-File: LICENSE
-
-A data review library
```

### Comparing `libcoveofds-0.7.0/setup.py` & `libcoveofds-0.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name="libcoveofds",
-    version="0.7.0",
+    version="0.8.0",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     url="https://github.com/Open-Telecoms-Data/lib-cove-ofds",
     project_urls={
         "Documentation": "https://libcoveofds.readthedocs.io/en/latest/",
         "Issues": "https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues",
         "Source": "https://github.com/Open-Telecoms-Data/lib-cove-ofds",
     },
     description="A data review library",
     packages=find_packages(),
     long_description="A data review library",
     python_requires=">=3.8",
     install_requires=[
         "jsonschema",
-        "requests",
-        "jsonref",
         "json-merge-patch",
         "rfc3987",
     ],
     extras_require={
         "dev": ["pytest", "flake8", "black==22.3.0", "isort", "mypy", "Sphinx"]
     },
     classifiers=[
```

