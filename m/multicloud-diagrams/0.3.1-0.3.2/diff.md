# Comparing `tmp/multicloud_diagrams-0.3.1.tar.gz` & `tmp/multicloud_diagrams-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.3.1.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.3.2.tar", max compression
```

## Comparing `multicloud_diagrams-0.3.1.tar` & `multicloud_diagrams-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.1/LICENSE
--rw-r--r--   0        0        0     8242 2023-05-18 14:59:20.511642 multicloud_diagrams-0.3.1/README.md
--rw-r--r--   0        0        0    14373 2023-05-18 12:36:03.603823 multicloud_diagrams-0.3.1/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0     3683 2023-05-18 15:01:58.100234 multicloud_diagrams-0.3.1/multicloud_diagrams/providers/aws_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.1/multicloud_diagrams/providers/azure_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.1/multicloud_diagrams/providers/gcp_services.json
--rw-r--r--   0        0        0        2 2023-05-17 19:53:33.563770 multicloud_diagrams-0.3.1/multicloud_diagrams/providers/on_prem_services.json
--rw-r--r--   0        0        0      525 2023-05-18 16:56:37.335541 multicloud_diagrams-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8332 2023-05-18 17:11:07.243158 multicloud_diagrams-0.3.2/README.md
+-rw-r--r--   0        0        0    14490 2023-06-15 15:06:17.039471 multicloud_diagrams-0.3.2/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0     3479 2023-05-19 12:11:13.264328 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/aws_services.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.575412 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/azure_services.json
+-rw-r--r--   0        0        0      207 2023-05-19 12:11:15.381235 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/fallback.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.570337 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/gcp_services.json
+-rw-r--r--   0        0        0        2 2023-05-17 19:53:33.563770 multicloud_diagrams-0.3.2/multicloud_diagrams/providers/on_prem_services.json
+-rw-r--r--   0        0        0      525 2023-06-15 15:10:52.562654 multicloud_diagrams-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.2/PKG-INFO
```

### Comparing `multicloud_diagrams-0.3.1/LICENSE` & `multicloud_diagrams-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.3.1/README.md` & `multicloud_diagrams-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             'SSEType': 'KMS',
             'KMSMasterKeyArn': 'string',
           },
           'DeletionProtectionEnabled': True
         }
 ```
 
-- Source [aws_dynamo_boto3_response.py](https://github.com/tsypuk/multicloud-diagrams/samples/samples/aws_dynamo_boto3_response.py)
-- Output compiled [output.prod.dynamo.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.dynamo.drawio):
+- Source [aws_dynamo_boto3_response.py](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_dynamo_boto3_response.py)
+- Output compiled [output.prod.dynamo.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.dynamo.drawio):
 
 ![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/raw/main/samples/output/png/output.prod.dynamo.png?raw=True)
 
 #### 2. Diagrams as a Code. DAG. Generating AWS IAM Graph from the code based on DAG declaration:
 
 ```python
     producer_func_arn = 'arn:aws:lambda:eu-west-1:123456789:function:producer-lambda'
@@ -132,16 +132,16 @@
     mcd.add_link(src_node_id=f'lambda_function:{producer_func_arn}', dst_node_id=f's3:{s3_arn}')
     mcd.add_link(src_node_id=f'sns:{sns_arn}', dst_node_id=f'sqs:{sqs_arn}')
     mcd.add_link(src_node_id=f'sns:{sns_arn}', dst_node_id=f'sqs:{sqs_arn2}')
     mcd.add_link(src_node_id=f'sqs:{sqs_arn}', dst_node_id=f'lambda_function:{consumer_func_arn}')
     mcd.add_link(src_node_id=f'lambda_function:{consumer_func_arn}', dst_node_id=f'dynamo:{dynamo_arn}')
 ```
 
-- Source [aws_service_end_2_end](https://github.com/tsypuk/multicloud-diagrams/samples/samples/aws_service_end_2_end.py)
-- Output compiled [output.prod.end2end.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.end2end.drawio)
+- Source [aws_service_end_2_end](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_service_end_2_end.py)
+- Output compiled [output.prod.end2end.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.end2end.drawio)
 
 ![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.end2end.png?raw=True)
 
 
 #### 3. Generating Diagram from YAML source
 
 ```yaml
@@ -178,17 +178,16 @@
   - {
     src_arn: arn:aws:iam::123456789:role/prod-lambda-name,
     src_type: iam_role,
     dst: prod-dynamodb-policy,
     label: Allow DynamoDB read access,
     link_type: none }
 ```
+- Source [aws_iam_from_yaml.py](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_iam_from_yaml.py)
+- Output compiled [output.prod.iam-roles-from-yaml.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.iam-roles-from-yaml.drawio)
 
-- Source [aws_iam_from_yaml.py](https://github.com/tsypuk/multicloud-diagrams/samples/samples/[aws_iam_from_yaml.py)
-- Output compiled [output.prod.iam-roles-from-yaml.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.iam-roles-from-yaml.drawio)
-
-![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles-from-yaml.png?raw=True)
+- ![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles-from-yaml.png?raw=True)
 
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

### Comparing `multicloud_diagrams-0.3.1/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.3.2/multicloud_diagrams/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         self.mx_cell_id_1 = et.SubElement(self.root, 'mxCell', id="1", parent="0")
 
     prev_coords = {}
 
     supported_vertex = {}
 
     # Load supported vertexes for registered Cloud Providers
-    path = pkgutil.get_data(__package__, 'providers/aws_services.json')
-    supported_vertex.update(json.loads(path.decode("utf-8")))
+    providers = ['aws_services', 'azure_services', 'gcp_services', 'on_prem_services', 'fallback']
+    for provider in providers:
+        path = pkgutil.get_data(__package__, f'providers/{provider}.json')
+        supported_vertex.update(json.loads(path.decode("utf-8")))
 
     def get_vertex_metadata(self, node_type: str) -> object:
         if node_type in self.supported_vertex:
             return self.supported_vertex[node_type]
         else:
             logging.warn(
                 f'No such nodeType: {node_type} in the Library (using default fallback icon Info). Please contact maintainer to add it, or provide MergeRequest')
@@ -39,57 +41,56 @@
     def stringify_dict(metadata: dict) -> str:
         if metadata != '':
             # return '<BR>-----------<BR>' + '<BR>'.join([f'<b>{k.capitalize()}</b>: {v}' for k, v in metadata.items()])
             return '<BR>-----------<BR>' + '<BR>'.join([f'<b>{k}</b>: {v}' for k, v in metadata.items()])
         else:
             return ''
 
-    def add_list(self, table_name='', rows=[]):
-        width = "300"
+    def add_list(self, table_id: str, table_name='', rows=[], width="300"):
 
         mx_cell = et.SubElement(self.root,
                                 'mxCell',
-                                id=f'vertex:{table_name}:list',
+                                id=f'vertex:{table_id}:list',
                                 value=f'<b>{table_name}</b>',
                                 style=("swimlane;fontStyle=0;childLayout=stackLayout;horizontal=1;"
                                        "startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;"
                                        "collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;"),
                                 parent="1",
                                 vertex="1")
 
         mx_geometry = et.SubElement(mx_cell, 'mxGeometry', width=width,
                                     height=str(30 * (1 + len(rows))))
         mx_geometry.set('as', 'geometry')
 
         # Position Vertex based on X,Y cords
-        if f'vertex:{table_name}:list' in self.prev_coords:
-            if 'x' in self.prev_coords[f'vertex:{table_name}:list']:
-                mx_geometry.set('x', self.prev_coords[f'vertex:{table_name}:list']['x'])
-            if 'y' in self.prev_coords[f'vertex:{table_name}:list']:
-                mx_geometry.set('y', self.prev_coords[f'vertex:{table_name}:list']['y'])
+        if f'vertex:{table_id}:list' in self.prev_coords:
+            if 'x' in self.prev_coords[f'vertex:{table_id}:list']:
+                mx_geometry.set('x', self.prev_coords[f'vertex:{table_id}:list']['x'])
+            if 'y' in self.prev_coords[f'vertex:{table_id}:list']:
+                mx_geometry.set('y', self.prev_coords[f'vertex:{table_id}:list']['y'])
 
         for index, item in enumerate(rows):
             mx_cell = et.SubElement(self.root,
                                     'mxCell',
-                                    id=f'vertex:{table_name}:row:{index}',
+                                    id=f'vertex:{table_id}:row:{index}',
                                     value=item,
                                     style=("text;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;"
                                            "spacingLeft=4;spacingRight=4;overflow=hidden;points=[[0,0.5],[1,0.5]];"
                                            "portConstraint=eastwest;rotatable=0;whiteSpace=wrap;html=1;"),
-                                    parent=f'vertex:{table_name}:list',
+                                    parent=f'vertex:{table_id}:list',
                                     vertex="1")
 
             mx_geometry = et.SubElement(mx_cell, 'mxGeometry', width=width, height="30")
             mx_geometry.set('as', 'geometry')
             # Position Vertex based on X,Y cords
-            if f'vertex:{table_name}:row:{index}' in self.prev_coords:
-                if 'x' in self.prev_coords[f'vertex:{table_name}:row:{index}']:
-                    mx_geometry.set('x', self.prev_coords[f'vertex:{table_name}:row:{index}']['x'])
-                if 'y' in self.prev_coords[f'vertex:{table_name}:row:{index}']:
-                    mx_geometry.set('y', self.prev_coords[f'vertex:{table_name}:row:{index}']['y'])
+            if f'vertex:{table_id}:row:{index}' in self.prev_coords:
+                if 'x' in self.prev_coords[f'vertex:{table_id}:row:{index}']:
+                    mx_geometry.set('x', self.prev_coords[f'vertex:{table_id}:row:{index}']['x'])
+                if 'y' in self.prev_coords[f'vertex:{table_id}:row:{index}']:
+                    mx_geometry.set('y', self.prev_coords[f'vertex:{table_id}:row:{index}']['y'])
 
     def add_vertex(self, id: str, node_name: str, arn: str, metadata='', node_type=''):
 
         # check that there is no such vertex already
         exist = False
         for mx_cell in self.root:
             # print(mxCell.attrib['id'])
```

### Comparing `multicloud_diagrams-0.3.1/multicloud_diagrams/providers/aws_services.json` & `multicloud_diagrams-0.3.2/multicloud_diagrams/providers/aws_services.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {'delete': "['fallback_vertex']"}*

```diff
@@ -13,20 +13,14 @@
     },
     "dynamo_stream": {
         "height": "78",
         "nodeLevel": "1",
         "style": "sketch=0;outlineConnect=0;fontColor=#232F3E;gradientColor=none;fillColor=#2E27AD;strokeColor=none;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=left;html=1;fontSize=12;fontStyle=0;aspect=fixed;pointerEvents=1;shape=mxgraph.aws4.dynamodb_stream",
         "width": "78"
     },
-    "fallback_vertex": {
-        "height": "78",
-        "nodeLevel": "1",
-        "style": "sketch=0;aspect=fixed;html=1;points=[];align=center;image;fontSize=12;image=img/lib/mscae/Info.svg;",
-        "width": "78"
-    },
     "iam_permission": {
         "height": "63",
         "nodeLevel": "2",
         "style": "outlineConnect=0;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=left;html=1;shape=mxgraph.aws3.permissions_2;fillColor=#D2D3D3;gradientColor=none;",
         "width": "46.5"
     },
     "iam_policy": {
```

### Comparing `multicloud_diagrams-0.3.1/pyproject.toml` & `multicloud_diagrams-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicloud-diagrams"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported."
 authors = ["Roman Tsypuk <tsypuk.conf@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "multicloud_diagrams"}]
 
 [tool.poetry.dependencies]
```

### Comparing `multicloud_diagrams-0.3.1/PKG-INFO` & `multicloud_diagrams-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -86,16 +86,16 @@
             'SSEType': 'KMS',
             'KMSMasterKeyArn': 'string',
           },
           'DeletionProtectionEnabled': True
         }
 ```
 
-- Source [aws_dynamo_boto3_response.py](https://github.com/tsypuk/multicloud-diagrams/samples/samples/aws_dynamo_boto3_response.py)
-- Output compiled [output.prod.dynamo.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.dynamo.drawio):
+- Source [aws_dynamo_boto3_response.py](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_dynamo_boto3_response.py)
+- Output compiled [output.prod.dynamo.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.dynamo.drawio):
 
 ![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/raw/main/samples/output/png/output.prod.dynamo.png?raw=True)
 
 #### 2. Diagrams as a Code. DAG. Generating AWS IAM Graph from the code based on DAG declaration:
 
 ```python
     producer_func_arn = 'arn:aws:lambda:eu-west-1:123456789:function:producer-lambda'
@@ -146,16 +146,16 @@
     mcd.add_link(src_node_id=f'lambda_function:{producer_func_arn}', dst_node_id=f's3:{s3_arn}')
     mcd.add_link(src_node_id=f'sns:{sns_arn}', dst_node_id=f'sqs:{sqs_arn}')
     mcd.add_link(src_node_id=f'sns:{sns_arn}', dst_node_id=f'sqs:{sqs_arn2}')
     mcd.add_link(src_node_id=f'sqs:{sqs_arn}', dst_node_id=f'lambda_function:{consumer_func_arn}')
     mcd.add_link(src_node_id=f'lambda_function:{consumer_func_arn}', dst_node_id=f'dynamo:{dynamo_arn}')
 ```
 
-- Source [aws_service_end_2_end](https://github.com/tsypuk/multicloud-diagrams/samples/samples/aws_service_end_2_end.py)
-- Output compiled [output.prod.end2end.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.end2end.drawio)
+- Source [aws_service_end_2_end](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_service_end_2_end.py)
+- Output compiled [output.prod.end2end.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.end2end.drawio)
 
 ![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.end2end.png?raw=True)
 
 
 #### 3. Generating Diagram from YAML source
 
 ```yaml
@@ -192,17 +192,16 @@
   - {
     src_arn: arn:aws:iam::123456789:role/prod-lambda-name,
     src_type: iam_role,
     dst: prod-dynamodb-policy,
     label: Allow DynamoDB read access,
     link_type: none }
 ```
+- Source [aws_iam_from_yaml.py](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/samples/aws_iam_from_yaml.py)
+- Output compiled [output.prod.iam-roles-from-yaml.drawio](https://raw.githubusercontent.com/tsypuk/multicloud-diagrams/main/samples/output/output.prod.iam-roles-from-yaml.drawio)
 
-- Source [aws_iam_from_yaml.py](https://github.com/tsypuk/multicloud-diagrams/samples/samples/[aws_iam_from_yaml.py)
-- Output compiled [output.prod.iam-roles-from-yaml.drawio](https://github.com/tsypuk/multicloud-diagrams/samples/output/output.prod.iam-roles-from-yaml.drawio)
-
-![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles-from-yaml.png?raw=True)
+- ![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles-from-yaml.png?raw=True)
 
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

