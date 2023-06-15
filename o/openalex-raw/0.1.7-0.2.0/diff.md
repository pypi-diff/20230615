# Comparing `tmp/openalex-raw-0.1.7.tar.gz` & `tmp/openalex-raw-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openalex-raw-0.1.7.tar", last modified: Wed May 11 23:06:50 2022, max compression
+gzip compressed data, was "openalex-raw-0.2.0.tar", last modified: Thu Jun 15 16:38:33 2023, max compression
```

## Comparing `openalex-raw-0.1.7.tar` & `openalex-raw-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwx------   0 filsilva (1642435) research  (3000)        0 2022-05-11 23:06:50.258804 openalex-raw-0.1.7/
--rw-------   0 filsilva (1642435) research  (3000)     1531 2022-02-23 01:17:42.000000 openalex-raw-0.1.7/LICENSE
--rw-------   0 filsilva (1642435) research  (3000)       43 2022-02-23 01:17:43.000000 openalex-raw-0.1.7/MANIFEST.in
--rw-------   0 filsilva (1642435) research  (3000)     5885 2022-05-11 23:06:50.258804 openalex-raw-0.1.7/PKG-INFO
--rw-------   0 filsilva (1642435) research  (3000)     5390 2022-05-11 23:02:18.000000 openalex-raw-0.1.7/README.md
-drwx------   0 filsilva (1642435) research  (3000)        0 2022-05-11 23:06:50.254804 openalex-raw-0.1.7/openalex_raw.egg-info/
--rw-------   0 filsilva (1642435) research  (3000)     5885 2022-05-11 23:06:50.000000 openalex-raw-0.1.7/openalex_raw.egg-info/PKG-INFO
--rw-------   0 filsilva (1642435) research  (3000)      282 2022-05-11 23:06:50.000000 openalex-raw-0.1.7/openalex_raw.egg-info/SOURCES.txt
--rw-------   0 filsilva (1642435) research  (3000)        1 2022-05-11 23:06:50.000000 openalex-raw-0.1.7/openalex_raw.egg-info/dependency_links.txt
--rw-------   0 filsilva (1642435) research  (3000)       11 2022-05-11 23:06:50.000000 openalex-raw-0.1.7/openalex_raw.egg-info/requires.txt
--rw-------   0 filsilva (1642435) research  (3000)       12 2022-05-11 23:06:50.000000 openalex-raw-0.1.7/openalex_raw.egg-info/top_level.txt
-drwx------   0 filsilva (1642435) research  (3000)        0 2022-05-11 23:06:50.254804 openalex-raw-0.1.7/openalexraw/
--rw-------   0 filsilva (1642435) research  (3000)      112 2022-05-11 22:54:20.000000 openalex-raw-0.1.7/openalexraw/__init__.py
--rw-------   0 filsilva (1642435) research  (3000)    12622 2022-05-11 05:10:37.000000 openalex-raw-0.1.7/openalexraw/openalex.py
--rw-------   0 filsilva (1642435) research  (3000)       11 2022-05-08 08:24:42.000000 openalex-raw-0.1.7/requirements.txt
--rw-------   0 filsilva (1642435) research  (3000)       38 2022-05-11 23:06:50.258804 openalex-raw-0.1.7/setup.cfg
--rw-------   0 filsilva (1642435) research  (3000)      820 2022-05-11 23:02:20.000000 openalex-raw-0.1.7/setup.py
+drwx------   0 filsilva (1642435) research  (3000)        0 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/
+-rw-------   0 filsilva (1642435) research  (3000)     1531 2022-02-23 01:17:42.000000 openalex-raw-0.2.0/LICENSE
+-rw-------   0 filsilva (1642435) research  (3000)      119 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/MANIFEST.in
+-rw-------   0 filsilva (1642435) research  (3000)     5727 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/PKG-INFO
+-rw-------   0 filsilva (1642435) research  (3000)     5232 2022-05-11 23:33:24.000000 openalex-raw-0.2.0/README.md
+drwx------   0 filsilva (1642435) research  (3000)        0 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/Schema/
+-rw-------   0 filsilva (1642435) research  (3000)     5827 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_authors.json
+-rw-------   0 filsilva (1642435) research  (3000)   115508 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_concepts.json
+-rw-------   0 filsilva (1642435) research  (3000)     5474 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_funders.json
+-rw-------   0 filsilva (1642435) research  (3000)    64610 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_institutions.json
+-rw-------   0 filsilva (1642435) research  (3000)     6081 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_publishers.json
+-rw-------   0 filsilva (1642435) research  (3000)     7313 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_sources.json
+-rw-------   0 filsilva (1642435) research  (3000)    20467 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/Schema/schema_works.json
+drwx------   0 filsilva (1642435) research  (3000)        0 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/openalex_raw.egg-info/
+-rw-------   0 filsilva (1642435) research  (3000)     5727 2023-06-15 16:38:33.000000 openalex-raw-0.2.0/openalex_raw.egg-info/PKG-INFO
+-rw-------   0 filsilva (1642435) research  (3000)      515 2023-06-15 16:38:33.000000 openalex-raw-0.2.0/openalex_raw.egg-info/SOURCES.txt
+-rw-------   0 filsilva (1642435) research  (3000)        1 2023-06-15 16:38:33.000000 openalex-raw-0.2.0/openalex_raw.egg-info/dependency_links.txt
+-rw-------   0 filsilva (1642435) research  (3000)       29 2023-06-15 16:38:33.000000 openalex-raw-0.2.0/openalex_raw.egg-info/requires.txt
+-rw-------   0 filsilva (1642435) research  (3000)       12 2023-06-15 16:38:33.000000 openalex-raw-0.2.0/openalex_raw.egg-info/top_level.txt
+drwx------   0 filsilva (1642435) research  (3000)        0 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/openalexraw/
+-rw-------   0 filsilva (1642435) research  (3000)      150 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/openalexraw/__init__.py
+-rw-------   0 filsilva (1642435) research  (3000)    27193 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/openalexraw/archive.py
+-rw-------   0 filsilva (1642435) research  (3000)    13123 2023-06-15 16:15:56.000000 openalex-raw-0.2.0/openalexraw/openalex.py
+-rw-------   0 filsilva (1642435) research  (3000)       29 2023-06-15 16:18:24.000000 openalex-raw-0.2.0/requirements.txt
+-rw-------   0 filsilva (1642435) research  (3000)       38 2023-06-15 16:38:33.278006 openalex-raw-0.2.0/setup.cfg
+-rw-------   0 filsilva (1642435) research  (3000)      820 2023-06-15 16:16:48.000000 openalex-raw-0.2.0/setup.py
```

### Comparing `openalex-raw-0.1.7/LICENSE` & `openalex-raw-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openalex-raw-0.1.7/PKG-INFO` & `openalex-raw-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openalex-raw
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python library to access OpenAlex Snapshot files
 Home-page: https://github.com/filipinascimento/openalex-raw
 Author: Filipi N. Silva
 Author-email: filipi@iu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -70,39 +70,33 @@
 from tqdm.auto import tqdm
 
 import openalexraw as oaraw
 
 # Path to the OpenAlex snapshot
 openAlexPath = Path("<Location of the OpenAlex Snapshot>")
 
-# Path to where to save the schema files
-schemasPath = Path("Schema")
-
 # Initializing the OpenAlex object with the OpenAlex snapshot path
 oa = oaraw.OpenAlex(
     openAlexPath = openAlexPath
 )
 
-# Creating any necessary directories
-schemasPath.mkdir(parents=True, exist_ok=True)
-
 # Which entity to process
 # "works" | "authors" | "institutions" | "venues" | "concepts"
 entityType = "works"
 
 # Getting the number of entries
 entitiesCount = oa.getRawEntityCount(entityType)
 
 # Iterating over all the entities of a certain type
 for entity in tqdm(oa.rawEntities(entityType),total=entitiesCount):
     openAlexID = entity["id"]
     # do something with the entity
 ```
 
-On fast storage, it may take a couple of hours to iterate over all the entities for `works` or ```authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
+On fast storage, it may take a couple of hours to iterate over all the entities for `works` or `authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
 
 
 ## Generating Schema and Report
 Schemas and reports for each entity type can be found respectively in the folders `Schema` and `Reports` of this repository. Schema files are in machine-readable JSON format and contain all the fields and non-null counts, nested structures and lists are included. The reports show the number and percentage of the coverage of the fields in the dataset. Both Schema and Report files are named according to the OpenAlex entity type. Schema files also include the most common values (samples) for each field. Two schema files are provided: one with samples (e.g., `Schema/schema_works_samples.json`) and another without (e.g., `Schema/schema_works.json`).
 
 To generate/update all the reports and schema, check the file `Examples/create_report.py`. Building the report can take a long time. You can use the provided schema files when generating `dbgz` archives.
```

### Comparing `openalex-raw-0.1.7/README.md` & `openalex-raw-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,39 +54,33 @@
 from tqdm.auto import tqdm
 
 import openalexraw as oaraw
 
 # Path to the OpenAlex snapshot
 openAlexPath = Path("<Location of the OpenAlex Snapshot>")
 
-# Path to where to save the schema files
-schemasPath = Path("Schema")
-
 # Initializing the OpenAlex object with the OpenAlex snapshot path
 oa = oaraw.OpenAlex(
     openAlexPath = openAlexPath
 )
 
-# Creating any necessary directories
-schemasPath.mkdir(parents=True, exist_ok=True)
-
 # Which entity to process
 # "works" | "authors" | "institutions" | "venues" | "concepts"
 entityType = "works"
 
 # Getting the number of entries
 entitiesCount = oa.getRawEntityCount(entityType)
 
 # Iterating over all the entities of a certain type
 for entity in tqdm(oa.rawEntities(entityType),total=entitiesCount):
     openAlexID = entity["id"]
     # do something with the entity
 ```
 
-On fast storage, it may take a couple of hours to iterate over all the entities for `works` or ```authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
+On fast storage, it may take a couple of hours to iterate over all the entities for `works` or `authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
 
 
 ## Generating Schema and Report
 Schemas and reports for each entity type can be found respectively in the folders `Schema` and `Reports` of this repository. Schema files are in machine-readable JSON format and contain all the fields and non-null counts, nested structures and lists are included. The reports show the number and percentage of the coverage of the fields in the dataset. Both Schema and Report files are named according to the OpenAlex entity type. Schema files also include the most common values (samples) for each field. Two schema files are provided: one with samples (e.g., `Schema/schema_works_samples.json`) and another without (e.g., `Schema/schema_works.json`).
 
 To generate/update all the reports and schema, check the file `Examples/create_report.py`. Building the report can take a long time. You can use the provided schema files when generating `dbgz` archives.
```

### Comparing `openalex-raw-0.1.7/openalex_raw.egg-info/PKG-INFO` & `openalex-raw-0.2.0/openalex_raw.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openalex-raw
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python library to access OpenAlex Snapshot files
 Home-page: https://github.com/filipinascimento/openalex-raw
 Author: Filipi N. Silva
 Author-email: filipi@iu.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -70,39 +70,33 @@
 from tqdm.auto import tqdm
 
 import openalexraw as oaraw
 
 # Path to the OpenAlex snapshot
 openAlexPath = Path("<Location of the OpenAlex Snapshot>")
 
-# Path to where to save the schema files
-schemasPath = Path("Schema")
-
 # Initializing the OpenAlex object with the OpenAlex snapshot path
 oa = oaraw.OpenAlex(
     openAlexPath = openAlexPath
 )
 
-# Creating any necessary directories
-schemasPath.mkdir(parents=True, exist_ok=True)
-
 # Which entity to process
 # "works" | "authors" | "institutions" | "venues" | "concepts"
 entityType = "works"
 
 # Getting the number of entries
 entitiesCount = oa.getRawEntityCount(entityType)
 
 # Iterating over all the entities of a certain type
 for entity in tqdm(oa.rawEntities(entityType),total=entitiesCount):
     openAlexID = entity["id"]
     # do something with the entity
 ```
 
-On fast storage, it may take a couple of hours to iterate over all the entities for `works` or ```authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
+On fast storage, it may take a couple of hours to iterate over all the entities for `works` or `authors` types. For `institutions` and `venues`, and `concepts` types, it may take just a few minutes.
 
 
 ## Generating Schema and Report
 Schemas and reports for each entity type can be found respectively in the folders `Schema` and `Reports` of this repository. Schema files are in machine-readable JSON format and contain all the fields and non-null counts, nested structures and lists are included. The reports show the number and percentage of the coverage of the fields in the dataset. Both Schema and Report files are named according to the OpenAlex entity type. Schema files also include the most common values (samples) for each field. Two schema files are provided: one with samples (e.g., `Schema/schema_works_samples.json`) and another without (e.g., `Schema/schema_works.json`).
 
 To generate/update all the reports and schema, check the file `Examples/create_report.py`. Building the report can take a long time. You can use the provided schema files when generating `dbgz` archives.
```

### Comparing `openalex-raw-0.1.7/openalexraw/openalex.py` & `openalex-raw-0.2.0/openalexraw/openalex.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 class OpenAlex:
     '''
     OpenAlex is a class for accessing the OpenAlex data snapshots
     '''
     # init
 
     def __init__(self,
-                 openAlexPath,
-                 processedPath=None,
+                 openAlexPath = None,
+                 processedPath = None,
                  tempPath=None,
                  tagLabel=None,  # current yyyy-mm-dd-hh-mm-ss will be used instead
                  verbose=False
                  ):
         """
         OpenAlex is a class for accessing the OpenAlex data snapshots.
 
@@ -248,14 +248,24 @@
     elif(isinstance(obj, bool)):
         return "bool"
     elif(isinstance(obj, list)):
         return "list"
     else:
         return type(obj).__name__
 
+# from https://github.com/smierz/openalex-utils/blob/8e423319987a07fc7b5599b1b4f19069510d6e9a/notebooks/inverted_index_to_text.ipynb
+def processInvertedAbstract(entry):
+    invertedAbstract = entry or {}
+    abstract_index = {}
+    for k, vlist in invertedAbstract.items():
+        for v in vlist:
+            abstract_index[v] = k
+    abstract = ' '.join(abstract_index[k] for k in sorted(abstract_index.keys()))
+    return abstract.replace("\n", " ").replace("\r", " ").replace("\t", " ")
+
 def _flatten(d, parent_key=""):
     items = []
     for k, v in d.items():
         if(k == "abstract_inverted_index" and v):
             v = "<ABSTRACT>" # avoid large abstracts in the schema when not null
         k = k.replace(":", "_") # no ":" allowed in keys
         new_key = parent_key+":"+str(k) if parent_key else str(k)
```

### Comparing `openalex-raw-0.1.7/setup.py` & `openalex-raw-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
    requirements = fh.readlines()
 
 setuptools.setup(
     name="openalex-raw",
-    version="0.1.7",
+    version="0.2.0",
     author="Filipi N. Silva",
     author_email="filipi@iu.edu",
     description="Python library to access OpenAlex Snapshot files",
     install_requires=[req for req in requirements if req[:2] != "# "],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipinascimento/openalex-raw",
```

