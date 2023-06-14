# Comparing `tmp/FlyBaseDownloads-1.0.2.tar.gz` & `tmp/FlyBaseDownloads-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.2.tar", last modified: Wed Jun 14 17:19:15 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.2.1.tar", last modified: Wed Jun 14 23:07:12 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.2.tar` & `FlyBaseDownloads-1.0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 17:19:15.216315 FlyBaseDownloads-1.0.2/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 17:19:15.216315 FlyBaseDownloads-1.0.2/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    13544 2023-06-14 17:15:00.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      480 2023-06-13 21:24:44.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 17:19:15.216315 FlyBaseDownloads-1.0.2/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     5271 2023-06-14 17:19:15.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      241 2023-06-14 17:19:15.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-14 17:19:15.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-14 17:19:15.000000 FlyBaseDownloads-1.0.2/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     5271 2023-06-14 17:19:15.216315 FlyBaseDownloads-1.0.2/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)     4709 2023-06-14 01:00:42.000000 FlyBaseDownloads-1.0.2/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-14 17:19:15.216315 FlyBaseDownloads-1.0.2/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      849 2023-06-14 17:03:02.000000 FlyBaseDownloads-1.0.2/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    18483 2023-06-14 22:58:15.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      702 2023-06-14 22:55:23.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26504 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      280 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26504 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.2.1/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      910 2023-06-14 22:00:23.000000 FlyBaseDownloads-1.0.2.1/setup.py
```

### Comparing `FlyBaseDownloads-1.0.2/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/FBD.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import pandas as pd
 import fnmatch
 import gzip
 from ftplib import FTP
 import re
 import csv
+import obonet
+import json
 
 
 
 class FBD():
     
     def __name__(self):
         self.__name__ = 'FlyBase Downloads'
@@ -57,15 +59,15 @@
             else:
                 print('Failed to download the file')
                 return []
             
         
         
         
-        def open_file(self, ruta_archivo, header):
+        def open_file_tsv(self, ruta_archivo, header):
             def df_r(df):
                 if re.search(r"FB\w{9}", df.columns[0]):
                     df_columns = pd.DataFrame(df.columns).T
 
                     df.columns = range(len(df.columns))
                     
                     # Unir la fila de columnas con el resto del DataFrame
@@ -101,15 +103,59 @@
                         df.columns = columns
                         df = df.dropna(axis='columns')
                       
       
                         return df_r(df)
                     except:
                         print('Failed to download the file') 
+                        
+        def open_file_json(self, ruta_archivo):
+            
+            a = []
+
+            if re.search(r'gz', ruta_archivo):
+                
+                try: 
+                    with gzip.open('../' + ruta_archivo, 'rt') as archivo:
+                        d = json.load(archivo)
+                        d_ = d['data']
+                        datos = pd.DataFrame(d_)
+                        a.append(datos)
+                       
+                except:
+                    print('Failed to download the file') 
+                
+                return a[0]
+                        
+        def open_obo(self, ruta_archivo):
+            a = []
+            
+            if re.search(r'gz', ruta_archivo):
+                with gzip.open('../' + ruta_archivo, 'rt') as archivo:
+                   if re.search(r'obo', ruta_archivo):
+                       
+                      graph = obonet.read_obo(archivo)
+                      
+                      a.append(graph)
+
+            return a[0]
+        
+        def get(self, header = None):
+            
+            archivos = self.download_file()
             
+            if len(archivos) > 0:
+                if re.search('.obo', self.url):
+                    return self.open_obo(archivos[0])
+                elif re.search('.json', self.url):
+                    return self.open_file_json(archivos[0])
+                else:
+                    return self.open_file_tsv(archivos[0], header)
+            
+        
                     
     
     class Synonyms():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
@@ -120,27 +166,24 @@
         
         def get(self):
             
             url = self.main_url + self.syn_url
             
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
         
     class Genes():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
             self.main_url = self.db.main_url
             self.gen_url = 'genes/'
+            self.header = None
             
         def Genetic_interaction_table(self):
             self.un_url = 'gene_genetic_interactions_fb_*.tsv.gz'
             self.header = 3
             return self.get()
             
         def RNASeq_values(self):
@@ -231,75 +274,80 @@
 
             
         def Unique_protein_isoforms(self):
             self.un_url = 'dmel_unique_protein_isoforms_fb_*.tsv.gz'
             self.header = 3
             return self.get()
         
-        #FALTA JSON NON-CODING
+        def Noncoding_RNAs(self):
+            self.un_url = 'ncRNA_genes_fb_*.json.gz'
+            return self.get()
+        
+        #FALTA JSON NON-CODI
         
         def Enzyme(self):
             self.un_url = 'Dmel_enzyme_data_fb_*.tsv.gz'
             self.header = 4
             return self.get()
     
             
         
         def get(self):
             
             url = self.main_url + self.gen_url + self.un_url
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
             
     class Gene_Ontology_annotation():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
             self.main_url = self.db.main_url
             self.go_url = 'go/gene_association.fb.gz'
+            self.header = 5
+            self.df_columns = ['DB', 'DB_Object_ID', 'DB_Object_Symbol',
+                               'Qualifier', 'GO ID', 'DB:Reference',
+                               'Evidence', 'With (or) From', 'Aspect',
+                               'DB_Object_Name', 'DB_Object_Synonym', 'DB_Object_Type',
+                               'taxon', 'Date', 'Assigned_by']
             
         def get(self):
             
             url = self.main_url + self.go_url
             descargas = self.db.Downloads(url)
             
             archivos = []
             
             archivos = descargas.download_file()
             
             if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+                df = descargas.open_file_tsv(archivos[0], self.header)
+                df = df.iloc[:, :-2]
+                df_ = pd.DataFrame(df.columns).T
+                df_.columns = self.df_columns
+                df.columns = self.df_columns
+                return pd.concat([df_, df])
+            
                 
-           
     class Gene_groups():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
             self.main_url = self.db.main_url
             self.gen_url = 'genes/'
             
         def get(self):
             
             url = self.main_url + self.gen_url + self.un_url
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
             
         def Gene_group(self):
             self.un_url = 'gene_group_data_fb_*.tsv.gz'
             self.header = 6
             return self.get()
         
         def Gene_groups_HGNC(self):
@@ -321,20 +369,15 @@
             self.gen_url = ''
             
         def get(self):
             
             url = self.main_url + self.gen_url + self.un_url
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
             
         def Stock(self):
             self.gen_url = 'stocks/'
             self.un_url = 'stocks_*.tsv.gz'
             self.header = 0
             return self.get()
             
@@ -365,20 +408,15 @@
             self.gen_url = 'orthologs/'
             
         def get(self):
             
             url = self.main_url + self.gen_url + self.un_url
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
             
         def Drosophila_Paralogs(self):
             self.un_url = 'dmel_paralogs_fb_*.tsv.gz'
             self.header = 4
             return self.get()
         
         def Human_Orthologs(self):
@@ -395,33 +433,71 @@
             self.gen_url = 'human_disease/'
             
         def get(self):
             
             url = self.main_url + self.gen_url + self.un_url
             descargas = self.db.Downloads(url)
             
-            archivos = []
-            
-            archivos = descargas.download_file()
-            
-            if len(archivos) > 0:
-                return descargas.open_file(archivos[0], self.header)
+            return descargas.get(self.header)
             
         def Disease_model_annotations(self):
             self.gen_url = 'human_disease/'
             self.un_url = 'disease_model_annotations_fb_*.tsv.gz'
             self.header = 4
             return self.get()
         
         def Human_Orthologs(self):
             self.gen_url = 'orthologs/'
             self.un_url = 'dmel_human_orthologs_disease_fb_*.tsv.gz'
             self.header = 3
             return self.get()
+    
+    class Ontology_Terms():
+        
+        def __init__(self, fbd_instance):
+            self.db = fbd_instance
         
+            self.main_url = self.db.main_url
+            self.go_url = 'ontologies/'
+            
+        def get(self):
+            
+            url = self.main_url + self.go_url + self.un_url
+            descargas = self.db.Downloads(url)
+            
+            return descargas.get(self.header)
+            
+        def Fly_anatomy(self):
+            self.un_url = 'fly_anatomy.obo.gz'
+            return self.get()
+        
+        def Fly_development(self):
+            self.un_url = 'fly_development.obo.gz'
+            return self.get()
+        
+        def Flybase_controlled_vocabulary(self):
+            self.un_url = 'flybase_controlled_vocabulary.obo.gz'
+            return self.get()
+        
+        def Flybase_stock_vocabulary(self):
+            self.un_url = 'flybase_stock_vocabulary.obo.gz'
+            return self.get()
+        
+        def GO_ontology(self):
+            self.un_url = 'go-basic.obo.gz'
+            return self.get()
+        
+        def Image_ontology(self):
+            self.un_url = 'image.obo.gz'
+            return self.get()
+        
+        def DO_ontology(self):
+            self.un_url = 'so-simple.obo.gz'
+            return self.get()
+    
     class Organisms():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
             self.main_url = self.db.main_url
             self.org_url = 'species/organism_list_fb*.tsv.gz'
@@ -430,15 +506,90 @@
         
         def Species_list(self):
             
             url = self.main_url + self.org_url
             
             descargas = self.db.Downloads(url)
             
-            archivos = []
+            return descargas.get(self.header)
+        
+    class Insertions():
+        
+        def __init__(self, fbd_instance):
+            self.db = fbd_instance
+        
+            self.main_url = self.db.main_url
+            self.in_url = 'insertions/'
+            self.header = 0
             
-            archivos = descargas.download_file()
+        def GAL4_drivers(self):
+            self.un_url = 'fu_gal4_table_fb_2023_03.json.gz'
+            df = self.get()
+            df = pd.concat([df.drop(['driver'], axis=1), df['driver'].apply(pd.Series)], axis=1)
+
+            # Reemplazar los valores None por NaN
+            df = df.replace({None: pd.NA})
             
-            return descargas.open_file(archivos[0], self.header)
+            # Mostrar el dataframe
+            return (df)
             
-
+            
+        
+        def Map_insertions(self):
+            self.un_url = 'insertion_mapping_fb_*.tsv.gz'
+            self.header = 3
+            return self.get()
+            
+        def get(self):
+            url = self.main_url + self.in_url + self.un_url
+            
+            descargas = self.db.Downloads(url)
+            
+            return descargas.get(self.header)
+        
+    class Clones():
+        
+        def __init__(self, fbd_instance):
+            self.db = fbd_instance
+        
+            self.main_url = self.db.main_url
+            self.cl_url = 'clones/'
+            self.header = None
+            
+        def cDNA_clone_data(self):
+            self.un_url = 'cDNA_clone_data_fb_*.tsv.gz'
+            self.header = 3
+            return self.get()
+        
+        def genomic_clone_data(self):
+            self.un_url = 'genomic_clone_data_fb_*.tsv.gz'
+            self.header = 3
+            return self.get()
+        
+        
+        def get(self):    
+            url = self.main_url + self.cl_url + self.un_url
+            
+            descargas = self.db.Downloads(url)
+            
+            return descargas.get(self.header)
+        
+            
+    class References():
+        
+        def __init__(self, fbd_instance):
+            self.db = fbd_instance
+        
+            self.main_url = self.db.main_url
+            self.org_url = 'references/fbrf_pmid_pmcid_doi_fb*.tsv.gz'
+            self.header = 2
+            
+        
+        def FBrf_PMid_PMCid_doi(self):
+            
+            url = self.main_url + self.org_url
+            
+            descargas = self.db.Downloads(url)
+            
+            df = descargas.get(self.header)
+            return df.iloc[1:, :]
```

### Comparing `FlyBaseDownloads-1.0.2/setup.py` & `FlyBaseDownloads-1.0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.2',
+    version='1.0.2.1',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
+    install_requires=open('requirements.txt').readlines(),
     description='Package to download Flybase data in Python, easily and quickly.',
     packages=['FlyBaseDownloads'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

