# Comparing `tmp/multicloud_diagrams-0.3.2.tar.gz` & `tmp/multicloud_diagrams-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.3.2.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.3.3.tar", max compression
```

## Comparing `multicloud_diagrams-0.3.2.tar` & `multicloud_diagrams-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.2/LICENSE
--rw-r--r--   0        0        0     8332 2023-05-18 17:11:07.243158 multicloud_diagrams-0.3.2/README.md
--rw-r--r--   0        0        0    14490 2023-06-15 15:06:17.039471 multicloud_diagrams-0.3.2/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0     3479 2023-05-19 12:11:13.264328 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/aws_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/azure_services.json
--rw-r--r--   0        0        0      207 2023-05-19 12:11:15.381235 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/fallback.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/gcp_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.563770 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/on_prem_services.json
--rw-r--r--   0        0        0      525 2023-06-15 15:10:52.562654 multicloud_diagrams-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8332 2023-05-18 17:11:07.243158 multicloud_diagrams-0.3.3/README.md
+-rw-r--r--   0        0        0    14627 2023-06-15 15:55:14.082468 multicloud_diagrams-0.3.3/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0     3479 2023-05-19 12:11:13.264328 multicloud_diagrams-0.3.3/multicloud_diagrams/providers/aws_services.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.3/multicloud_diagrams/providers/azure_services.json
+-rw-r--r--   0        0        0      207 2023-05-19 12:11:15.381235 multicloud_diagrams-0.3.3/multicloud_diagrams/providers/fallback.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.3/multicloud_diagrams/providers/gcp_services.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.563770 multicloud_diagrams-0.3.3/multicloud_diagrams/providers/on_prem_services.json
+-rw-r--r--   0        0        0      525 2023-06-15 15:57:49.497018 multicloud_diagrams-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.3/PKG-INFO
```

### Comparing `multicloud_diagrams-0.3.2/LICENSE` & `multicloud_diagrams-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.2/README.md` & `multicloud_diagrams-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.2/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.3.3/multicloud_diagrams/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,23 +41,30 @@
     def stringify_dict(metadata: dict) -> str:
         if metadata != '':
             # return '<BR>-----------<BR>' + '<BR>'.join([f'<b>{k.capitalize()}</b>: {v}' for k, v in metadata.items()])
             return '<BR>-----------<BR>' + '<BR>'.join([f'<b>{k}</b>: {v}' for k, v in metadata.items()])
         else:
             return ''
 
-    def add_list(self, table_id: str, table_name='', rows=[], width="300"):
+    # green fillColor=#d5e8d4
+    # red fillColor=#f8cecc;"
+    def add_list(self, table_id='', table_name='', fillColor='', rows=[], width="300"):
+        if not table_id:
+            table_id = table_name
+
+        style="swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;"
+
+        if fillColor:
+            style += f"fillColor={fillColor}"
 
         mx_cell = et.SubElement(self.root,
                                 'mxCell',
                                 id=f'vertex:{table_id}:list',
                                 value=f'<b>{table_name}</b>',
-                                style=("swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;"
-                                       "startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;"
-                                       "collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;"),
+                                style=(style),
                                 parent="1",
                                 vertex="1")
 
         mx_geometry = et.SubElement(mx_cell, 'mxGeometry', width=width,
                                     height=str(30 * (1 + len(rows))))
         mx_geometry.set('as', 'geometry')
```

### Comparing `multicloud_diagrams-0.3.2/multicloud_diagrams/providers/aws_services.json` & `multicloud_diagrams-0.3.3/multicloud_diagrams/providers/aws_services.json`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.2/pyproject.toml` & `multicloud_diagrams-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicloud-diagrams"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported."
 authors = ["Roman Tsypuk <tsypuk.conf@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "multicloud_diagrams"}]
 
 [tool.poetry.dependencies]
```

### Comparing `multicloud_diagrams-0.3.2/PKG-INFO` & `multicloud_diagrams-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

