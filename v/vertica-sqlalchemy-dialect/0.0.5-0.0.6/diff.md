# Comparing `tmp/vertica-sqlalchemy-dialect-0.0.5.tar.gz` & `tmp/vertica-sqlalchemy-dialect-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.5.tar", last modified: Fri Jun  9 14:25:23 2023, max compression
+gzip compressed data, was "vertica-sqlalchemy-dialect-0.0.6.tar", last modified: Thu Jun 15 15:09:03 2023, max compression
```

## Comparing `vertica-sqlalchemy-dialect-0.0.5.tar` & `vertica-sqlalchemy-dialect-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.873414 vertica-sqlalchemy-dialect-0.0.5/
--rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5749 2023-06-09 14:25:23.875414 vertica-sqlalchemy-dialect-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5402 2023-06-06 16:57:33.000000 vertica-sqlalchemy-dialect-0.0.5/README.rst
--rw-rw-rw-   0        0        0      211 2023-06-09 14:25:23.880445 vertica-sqlalchemy-dialect-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1922 2023-06-09 13:48:02.000000 vertica-sqlalchemy-dialect-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.698413 vertica-sqlalchemy-dialect-0.0.5/test/
--rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_core.py
--rw-rw-rw-   0        0        0    14580 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_integration.py
--rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/test/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.818415 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/
--rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/__init__.py
--rw-rw-rw-   0        0        0    68765 2023-06-09 14:23:32.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/base.py
--rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_pyodbc.py
--rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_vertica_python.py
--rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/requirements.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:25:23.866415 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/
--rw-rw-rw-   0        0        0     5749 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-09 14:25:22.000000 vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 15:09:03.414387 vertica-sqlalchemy-dialect-0.0.6/
+-rw-rw-rw-   0        0        0    12947 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5749 2023-06-15 15:09:03.416414 vertica-sqlalchemy-dialect-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2023-06-06 16:57:33.000000 vertica-sqlalchemy-dialect-0.0.6/README.rst
+-rw-rw-rw-   0        0        0      211 2023-06-15 15:09:03.419385 vertica-sqlalchemy-dialect-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1922 2023-06-15 15:08:42.000000 vertica-sqlalchemy-dialect-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:09:03.280384 vertica-sqlalchemy-dialect-0.0.6/test/
+-rw-rw-rw-   0        0        0     7941 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/test/test_core.py
+-rw-rw-rw-   0        0        0    14819 2023-06-15 15:08:17.000000 vertica-sqlalchemy-dialect-0.0.6/test/test_integration.py
+-rw-rw-rw-   0        0        0     2624 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:09:03.376389 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/
+-rw-rw-rw-   0        0        0        0 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/__init__.py
+-rw-rw-rw-   0        0        0    69000 2023-06-15 15:08:17.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/base.py
+-rw-rw-rw-   0        0        0     1362 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/dialect_pyodbc.py
+-rw-rw-rw-   0        0        0     1417 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/dialect_vertica_python.py
+-rw-rw-rw-   0        0        0     1500 2023-06-05 10:03:57.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/requirements.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:09:03.409385 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/
+-rw-rw-rw-   0        0        0     5749 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-15 15:09:02.000000 vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/top_level.txt
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/LICENSE` & `vertica-sqlalchemy-dialect-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.5
+Version: 0.0.6
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/README.rst` & `vertica-sqlalchemy-dialect-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/setup.py` & `vertica-sqlalchemy-dialect-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from setuptools import setup
 
 with open("README.rst", "r") as f:
     description = f.read()
 
 
-version_info = (0, 0, 5)
+version_info = (0, 0, 6)
 
 version = '.'.join(map(str, version_info))
 
 setup(
     name='vertica-sqlalchemy-dialect',
     version=version,
     description='Official Vertica dialect for SQLalchemy',
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/test/test_core.py` & `vertica-sqlalchemy-dialect-0.0.6/test/test_core.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/test/test_integration.py` & `vertica-sqlalchemy-dialect-0.0.6/test/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,22 +244,24 @@
     assert ps>0
 
 def test_get_ifcachedproj(vconn):
     cp = vconn[0].dialect._get_ifcachedproj(vconn[1], projection_name=sample.sample_projections[1], schema="store")
     assert cp in [True,False]
 
 def test_get_projection_comment(vconn):
-    pc = vconn[0].dialect.get_projection_comment(vconn[1],  schema="store")
+    pc = vconn[0].dialect.get_projection_comment(vconn[1], projection_name = sample.sample_projections[1], schema="store")
     projection_name=sample.sample_projections[1]
     projection_comments = sample.sample_projection_properties
     properties = []
     for data in pc['properties']:
         if data["projection_name"] == projection_name:
             properties.append(data)
             
+    print(properties[0])
+            
     assert properties[0] == projection_comments
 
 
 def test_get_model_comment(vconn):
     mc = vconn[0].dialect.get_model_comment(vconn[1], model_name=sample.sample_ml_model, schema="public")
     assert mc["properties"]["used_by"] == "dbadmin"
     assert len(mc["properties"]["Model Attributes"])>0
@@ -279,37 +281,37 @@
     
 def test_get_all_owners(vconn):
     owner = vconn[0].dialect.get_table_owner(vconn[1],schema='public')
     table_owner = owner[0][1]
     assert table_owner == "dbadmin"
     
 def test_get_all_columns(vconn):
-    res = vconn[0].dialect.get_all_columns(connection=vconn[1], schema="public")
+    res = vconn[0].dialect.get_all_columns(connection=vconn[1], table = sample.sample_table_list["public"][2] ,  schema="public")
     table_name=sample.sample_table_list["public"][2]
   
     columns = []
     for data in res:
         if data['tablename'] == table_name:
             columns.append(data)
     # Assert the no. of columns
     assert len(columns)>0
     # # Assert sample columns
     assert all(value["name"] in sample.sample_columns for value in columns)
     
     
 def test_get_all_view_columns(vconn):
-    res = vconn[0].dialect.get_all_view_columns(connection=vconn[1], schema="public")
+    res = vconn[0].dialect.get_all_view_columns(connection=vconn[1],view_name = sample.sample_view,  schema="public")
     # Assert the no. of columns
     assert len(res)>0
     # Assert sample columns
     assert all(value["name"] in sample.sample_view_columns for value in res)
 
 
 def test_get_view_comment(vconn):
-    res = vconn[0].dialect.get_view_comment(connection=vconn[1], schema="public")
+    res = vconn[0].dialect.get_view_comment(connection=vconn[1],view_name = sample.sample_view, schema="public")
     if res['properties'] is not None:
         has_comment = True
     else:
         has_comment = False
         
     assert has_comment == True
     
@@ -321,15 +323,15 @@
     
 def test_get_projection_owner(vconn):
     owner = vconn[0].dialect.get_projection_owner(vconn[1],schema='public')
     table_owner = owner[0][1]
     assert table_owner == "dbadmin"
     
 def test_get_all_projection_columns(vconn):
-    res = vconn[0].dialect.get_all_projection_columns(connection=vconn[1], schema="public")
+    res = vconn[0].dialect.get_all_projection_columns(connection=vconn[1], projection_name='inventory_fact_super', schema="public")
     projection_name = 'inventory_fact_super'
     columns = []
     for data in res:
         if data['tablename'] == projection_name:
             columns.append(data)
 
     # Assert the no. of columns
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/test/test_suite.py` & `vertica-sqlalchemy-dialect-0.0.6/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/base.py` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     def get_table_owner(self, schema: Optional[str] = None, **kw: Any):
         r"""Return primary key columns names within a particular schema. """
 
         return self.dialect.get_table_owner(
             self.bind, schema, info_cache=self.info_cache, **kw
         )
         
-    def get_all_columns(self, schema: Optional[str] = None, **kw: Any):
+    def get_all_columns(self,schema: Optional[str] = None, **kw: Any):
         r"""Return all table columns names within a particular schema. """
 
         return self.dialect.get_all_columns(
             self.bind, schema, info_cache=self.info_cache, **kw
         )
 
     def get_pk_constraint(self, schema=None, **kw):
@@ -277,22 +277,22 @@
             self.bind,table , schema, info_cache=self.info_cache, **kw
         )
         
     def get_all_view_columns(self, schema: Optional[str] = None, **kw: Any):
         r"""Return all view columns names within a particular schema. """
 
         return self.dialect.get_all_view_columns(
-            self.bind, schema, info_cache=self.info_cache, **kw
+            self.bind , schema, info_cache=self.info_cache, **kw
         )
 
-    def get_view_comment(self,  schema: Optional[str] = None, **kw: Any):
+    def get_view_comment(self,schema: Optional[str] = None,**kw):
         r"""Return view comments within a particular schema. """
 
         return self.dialect.get_view_comment(
-            self.bind, schema, info_cache=self.info_cache, **kw
+            self.bind,schema, info_cache=self.info_cache, **kw
         )
         
         
     def get_view_owner(self, schema: Optional[str] = None, **kw: Any):
         r"""Return primary key columns names within a particular schema. """
 
         return self.dialect.get_view_owner(
@@ -302,19 +302,19 @@
     def _populate_view_lineage(self, schema: Optional[str] = None, **kw: Any):
         r"""Return primary key columns names within a particular schema. """
 
         return self.dialect._populate_view_lineage(
             self.bind, schema , **kw
         )  
         
-    def get_all_projection_columns(self, schema: Optional[str] = None, **kw: Any):
+    def get_all_projection_columns(self,schema: Optional[str] = None, **kw: Any):
         r"""Return all projection columns names within a particular schema. """
 
         return self.dialect.get_all_projection_columns(
-            self.bind, schema, info_cache=self.info_cache, **kw
+            self.bind,schema, info_cache=self.info_cache, **kw
         )
         
     def get_projection_owner(self, schema: Optional[str] = None, **kw: Any):
         r"""Return all projection columns names within a particular schema. """
 
         return self.dialect.get_projection_owner(
             self.bind, schema, info_cache=self.info_cache, **kw
@@ -414,16 +414,20 @@
             WHERE lower(type_name) = '%(type)s')
         """ % {'type': type_name.lower()}))
 
         c = connection.execute(has_type_sql)
         return bool(c.scalar())
 
     def _get_database_properties(self, connection, database):
+        
+        
+        
         try:
-
+        
+            
             cluster_type_qry = sql.text(dedent(
                 """SELECT CASE COUNT(*) WHEN 0 THEN 'Enterprise' ELSE 'Eon' END AS database_mode FROM v_catalog.shards """))
 
             communal_storage_path = sql.text(dedent(
                 """SELECT location_path from storage_locations WHERE sharing_type = 'COMMUNAL' """))
             cluster_type = ""
             communal_path = ""
@@ -519,14 +523,16 @@
     def get_table_comment(self, connection,table_name, schema=None, **kw):
         if schema is not None:
             schema_condition = "lower(table_schema) = '%(schema)s'" % {
                 'schema': schema.lower()}
         else:
             schema_condition = "1"
 
+        
+        tables = table_name
         sct = sql.text(dedent("""
                 SELECT create_time , table_name
                 FROM v_catalog.tables
                 where lower(table_schema) = '%(schema)s'
             """ % {'schema': schema.lower()}))
 
         sts = sql.text(dedent(""" 
@@ -534,24 +540,26 @@
                 FROM v_monitor.column_storage
                 where lower(anchor_table_schema) = '%(schema)s'
                         """ % {'schema': schema.lower()}))
         
         columns = []
         
         for row in connection.execute(sct):
+            
 
             columns.append({'create_time': str(row[0]), 'table_name': row[1]})
+                
         table_size_dict={}
         for table_size in connection.execute(sts):
-        
-            if table_size[1] not in table_size_dict:
-                table_size_dict[table_size[1]] = table_size[0] / 1024
+            if row[1] in tables:
+                if table_size[1] not in table_size_dict:
+                    table_size_dict[table_size[1]] = table_size[0] / 1024
 
-            else:
-                table_size_dict[table_size[1]] += table_size[0] / 1024
+                else:
+                    table_size_dict[table_size[1]] += table_size[0] / 1024
                         
         for a in columns:
             if a['table_name'] in table_size_dict:
                 a['table_size'] = str(int(table_size_dict[a['table_name']])) + " KB"
             
             else:
                 a['table_size'] = "0 KB"
@@ -940,15 +948,14 @@
             """ % {'schema': schema.lower()}))
 
         pk_columns = []
        
         for row in connection.execute(spk):
             columns = row['column_name']
             table_name = row['table_name'].lower()
-            # print(row)
             pk_columns.append({'constrained_columns': [columns], 'name': [columns],"tablename":table_name})
 
         return pk_columns
 
     # @reflection.cache
     def _get_extra_tags(
         self, connection, name, schema=None
@@ -1143,15 +1150,15 @@
             if data[0] > 0:
                 cached_projection = True
             else:
                 cached_projection = False
         return cached_projection
 
     @reflection.cache
-    def get_projection_comment(self, connection, schema=None, **kw):
+    def get_projection_comment(self, connection,  schema=None, **kw):
         
         src = sql.text(dedent("""
                 SELECT ros_count , LOWER(projection_name)
                 FROM v_monitor.projection_storage
                 WHERE projection_schema = '%(schema)s'
 
             """ % {'schema': schema}))
@@ -1174,15 +1181,15 @@
                 SELECT  DISTINCT LOWER(projection_name) ,  partition_key 
                 FROM v_monitor.partitions
                 WHERE table_schema = '%(schema)s'
               
             """ % {'schema': schema}))
         
         partition_num = sql.text(dedent("""
-                SELECT  COUNT(ros_id) , LOWER(projection_name)
+                SELECT  COUNT(ros_id) as Partition_Size , LOWER(projection_name)
                 FROM v_monitor.partitions
                 WHERE table_schema = '%(schema)s'
                 GROUP BY projection_name
             """ % {'schema': schema}))
         
         projection_size = sql.text(dedent("""
             SELECT used_bytes , LOWER(projection_name) 
@@ -1198,42 +1205,44 @@
             """ % {'schema': schema}))
         
         projection_comment = []
       
         ros_count = {}
         for data in connection.execute(src):
             # ros_count = data['ros_count']
+
             ros_count = {"ROS_Count": data[0] , "projection_name" : data[1]}
             projection_comment.append(ros_count)
-        
+    
         
      
         lst = ["is_super_projection", "is_key_constraint_projection",
                    "is_aggregate_projection", "has_expressions"]
         
-        for ptype in connection.execute(projection_type):    
+        for ptype in connection.execute(projection_type):  
+           
             for i, value in enumerate(ptype):
                 if value is True:
                     for a in projection_comment:
                         if a['projection_name'] == ptype[4]:
                             if "Projection_Type" in a:
                                 a["Projection_Type"] = a["Projection_Type"] + ", "+str(lst[i])
                             else:
                                 a["Projection_Type"] = str(lst[i])
                                  
         for projection_segment in connection.execute(is_segmented):
-            
+
             for a in projection_comment:
                 if a['projection_name'] == projection_segment[2]:
                     a["is_segmented"] = str(projection_segment[0])
                     a["Segmentation_key"] = str(projection_segment[1])
          
         for partion_keys in connection.execute(partition_key):
+           
             for a in projection_comment:
-                
                 if a['projection_name'] == partion_keys[0]:
                     a["Partition_Key"] = str(partion_keys[1])
               
 
      
         projection_size_dict={}
         for projection_sizes in connection.execute(projection_size):
@@ -1249,32 +1258,31 @@
                     a['projection_size'] = str(int(projection_size_dict[a['projection_name']])) + " KB"
                 
                 else:
                     a['projection_size'] = "0 KB"
              
            
         for partition_number in connection.execute(partition_num):
+            
+            
             for a in projection_comment:
-                if a['projection_name'] == partition_number[0]:
-                    a["Partition_Size"] = str(partition_number[1])
+                if a['projection_name'].lower() == partition_number[1]:
+
+                    a["Partition_Size"] = str(partition_number['Partition_Size'])
                     
         for projection_cached in connection.execute(projection_cache):
+           
+                
             for a in projection_comment:
-                if a['projection_name'] == projection_cached[1]:
-                    if projection_cached[0] > 0:
-                        a["Projection_Cached"] = True
-                    else:
-                        a["Projection_Cached"] = False
+              
+                if projection_cached[0] > 0:
+                    a["Projection_Cached"] = True
+                else:
+                    a["Projection_Cached"] = False
                         
-        
-     
-            
-            
-        # print(projection_comment)
-        # exit()
         return {"text": "Vertica physically stores table data in projections, \
             which are collections of table columns. Projections store data in a format that optimizes query execution \
             For more info on projections and corresponding properties check out the Vertica Docs: https://www.vertica.com/docs",
                 "properties": projection_comment }
 
     @reflection.cache
     def get_model_comment(self, connection, model_name, schema=None, **kw):
@@ -1557,23 +1565,22 @@
             comment=str(default),
             tablename = str(table_name)
         )
         
         return column_info
     
     @reflection.cache
-    def get_all_view_columns(self, connection,schema=None, **kw):
+    def get_all_view_columns(self, connection, schema=None, **kw):
        
         s = sql.text(dedent("""
             SELECT column_name, data_type, '' as column_default, true as is_nullable,lower(table_name) as table_name
             FROM v_catalog.view_columns
             where lower(table_schema) = '%(schema)s'
         """ % {'schema': schema.lower()}))
 
-  
         columns = []
        
         for row in connection.execute(s):
             name = row.column_name
             dtype = row.data_type.lower()
             default = row.column_default
             nullable = row.is_nullable
@@ -1591,29 +1598,34 @@
             # column_info.update({'primary_key': primary_key})
             columns.append(column_info)
             
         
         
         return columns
     
-    @reflection.cache
-    def get_view_comment(self, connection, schema=None, **kw):
+    def get_view_comment(self, connection,schema=None, **kw):
+        
+        if schema is not None:
+            schema_condition = "lower(table_schema) = '%(schema)s'" % {
+                'schema': schema.lower()}
+        else:
+            schema_condition = "1"
+
 
         sct = sql.text(dedent("""
                 SELECT create_time , table_name
                 FROM v_catalog.views
                 where lower(table_schema) = '%(schema)s'
                
                 
             """ % {'schema': schema.lower()}))
 
-       
         columns = []
         for row in connection.execute(sct):
-            columns.append({'create_time': str(row[0]), 'table_name': row[1]})
+                columns.append({'create_time': str(row[0]), 'table_name': row[1]})
 
         return {"text": "References the properties of a native table in Vertica. \
         Vertica physically stores table data in projections, which are collections of table columns. \
         Projections store data in a format that optimizes query execution. \
         In order to query or perform any operation on a Vertica table, the table must have one or more projections associated with it. ",
                 "properties":  columns }
         
@@ -1700,15 +1712,15 @@
             )
 
         logger.info(
             f"A total of {num_edges} View upstream edges found found for {schema}"
         )
         
     @reflection.cache
-    def get_all_projection_columns(self, connection,schema=None, **kw):
+    def get_all_projection_columns(self, connection, schema=None, **kw):
        
         s = sql.text(dedent("""
             SELECT projection_column_name, data_type, '' as column_default, true as is_nullable,lower(projection_name) as projection_name
             FROM PROJECTION_COLUMNS
             where lower(table_schema) = '%(schema)s'
         """ % {'schema': schema.lower()}))
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_pyodbc.py` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/dialect_pyodbc.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/dialect_vertica_python.py` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/dialect_vertica_python.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect/requirements.py` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect/requirements.py`

 * *Files identical despite different names*

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/PKG-INFO` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-sqlalchemy-dialect
-Version: 0.0.5
+Version: 0.0.6
 Summary: Official Vertica dialect for SQLalchemy
 Home-page: https://github.com/vertica/vertica-sqlalchemy-dialect
 Author: Narendra Prabhu
 License: Apache License 2.0
 Platform: UNKNOWN
 Provides-Extra: pyodbc
 Provides-Extra: vertica-python
```

### Comparing `vertica-sqlalchemy-dialect-0.0.5/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt` & `vertica-sqlalchemy-dialect-0.0.6/vertica_sqlalchemy_dialect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

