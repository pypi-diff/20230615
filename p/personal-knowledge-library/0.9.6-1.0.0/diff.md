# Comparing `tmp/personal_knowledge_library-0.9.6.tar.gz` & `tmp/personal_knowledge_library-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-0.9.6.tar", last modified: Tue May 23 09:39:46 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.0.tar", last modified: Thu Jun 15 12:20:56 2023, max compression
```

## Comparing `personal_knowledge_library-0.9.6.tar` & `personal_knowledge_library-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    39600 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52179 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29014 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39600 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43992 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43122 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79618 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44888 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53247 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29633 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:20:56.547313 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43992 2023-06-15 12:20:56.000000 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-15 12:20:56.000000 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:20:56.000000 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 12:20:56.000000 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 12:20:56.000000 personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 12:20:56.551313 personal_knowledge_library-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-15 12:20:40.000000 personal_knowledge_library-1.0.0/setup.py
```

### Comparing `personal_knowledge_library-0.9.6/LICENSE` & `personal_knowledge_library-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.6/PKG-INFO` & `personal_knowledge_library-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 0.9.6
+Version: 1.0.0
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
@@ -16,34 +16,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Wacom Personal Knowledge Library
+# Wacom Private Knowledge Library
 
-The library and the cloud services are still under development. 
-The required access tokens are only available for selected partner companies.
-
-> :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
+The required tenant API key is only available for selected partner companies.
+Please contact your Wacom representative for more information.
 
 ## Introduction
 
 In knowledge management there is a distinction between data, information and knowledge.
 In the domain of digital ink this means:
 
 - **Data** - The equivalent would be the ink strokes
 - **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
 - **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
 
 The following illustration shows the different layers of knowledge:
 ![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
 
-For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
+For handling semantics, Wacom introduced the Wacom Private Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
 
 This library provide simplified access to Wacom's personal knowledge cloud service.
 It contains:
 
 - Basic datastructures for Ontology object and entities from the knowledge graph
 - Clients for the REST APIs
 - Connector for Wikidata public knowledge graph
@@ -56,19 +54,45 @@
 
 **Entity service:**
 
 - List all entities
 - Add entities to knowledge graph
 - Access object properties
 
+**Search service:**
+
+- Search for entities for labels and descriptions with a given language
+- Search for literals (data properties) 
+- Search for relations (object properties)
+
+**Group service:**
+
+- List all groups
+- Add groups, modify groups, delete groups
+- Add users and entities to groups
+
+**Ontology service:**
+
+- List all Ontology structures
+- Modify Ontology structures
+
+**Named Entity Linking service:**
+
+- Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
+
+**Wikidata connector:**
+
+- Import entities from Wikidata
+- Mapping Wikidata entities to WPK entities
+
 # Technology stack
 
 ## Domain Knowledge
 
-The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
+The tasks of the ontology within Wacom's private knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
 The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
 
 - Foundation for structured data, knowledge representation as concepts and relations among concepts
 - Being explicit definitions of shared vocabularies for interoperability
 - Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
 - Can be used for problem solving
 
@@ -85,23 +109,45 @@
 - Extract knowledge from various sources (Connectors)
 - Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
 - Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
 
 
 # Functionality
 
+## Import Format
+
+For importing entities into the knowledge graph, the tools/import_entities.py script can be used.
+
+The ThingObject support a NDJSON based import format, where the individual JSON files can contain the following structure.
+
+| Field name             | Subfield name | Data Structure | Description                                                                                    |
+|------------------------|---------------|----------------|------------------------------------------------------------------------------------------------|
+| source_reference_id    |               | str            | A unique identifier for the entity used in the source system                                  |
+| source_system          |               | str            | The source system describes the original source of the entity, such as wikidata, youtube, ... |
+| image                  |               | str            | A string representing the URL of the entity's icon.                                           |
+| labels                 |               | array          | An array of label objects, where each object has the following fields:                       |
+|                        | value         | str            | A string representing the label text in the specified locale.                                |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+|                        | isMain        | bool           | A boolean flag indicating if this label is the main label for the entity (true) or an alias (false). |
+| descriptions           |               | array          | An array of description objects, where each object has the following fields:                 |
+|                        | description   | str            | A string representing the description text in the specified locale.                          |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+| type                   |               | str            | A string representing the IRI of the ontology class for this entity.                         |
+| literals               |               | array[map]     | An array of data property objects, where each object has the following fields:               |
+
+
 ## Access API
 
 The personal knowledge graph backend is implement as a multi-tenancy system.
 Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
 
 ![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
 
 In general, a tenant with their users, groups, and entities are logically separated.
-Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
+Physically the entities are store in the same instance of the Wacom Private Knowledge (WPK) backend database system.
 
 The user management is rather limited, each organisation must provide their own authentication service and user management.
 The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
 
 The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
 While users for each tenant can be created by the owner of the **Tenant API Key**.
 You will receive this token from the system owner after the creation of the tenant.
@@ -169,15 +215,15 @@
 
 ### Entity handling
 
 This samples shows how to work with graph service.
 
 ```python
 import argparse
-from typing import Optional, List, Dict
+from typing import Optional
 
 from knowledge.base.entity import LanguageCode, Description, Label
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.services.graph import WacomKnowledgeService
 
 # ------------------------------- Knowledge entities -------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
@@ -194,69 +240,70 @@
 ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
 IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
 HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
 CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
 HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
 
 
-def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
+def print_entity(display_entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService,
+                 short: bool = False):
     """
     Printing entity details.
 
     Parameters
     ----------
-    entity: ThingObject
+    display_entity: ThingObject
         Entity with properties
     list_idx: int
         Index with a list
     auth_key: str
         Authorization key
     client: WacomKnowledgeService
         Knowledge graph client
     short: bool
         Short summary
     """
-    print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
-    if len(entity.label) > 0:
+    print(f'[{list_idx}] : {display_entity.uri} <{display_entity.concept_type.iri}>')
+    if len(display_entity.label) > 0:
         print('    | [Labels]')
-        for la in entity.label:
+        for la in display_entity.label:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if not short:
-        if len(entity.alias) > 0:
+        if len(display_entity.alias) > 0:
             print('    | [Alias]')
-            for la in entity.alias:
+            for la in display_entity.alias:
                 print(f'    |     |- "{la.content}"@{la.language_code}')
             print('    |')
-        if len(entity.data_properties) > 0:
+        if len(display_entity.data_properties) > 0:
             print('    | [Attributes]')
             for data_property, labels in entity.data_properties.items():
                 print(f'    |    |- {data_property.iri}:')
                 for li in labels:
                     print(f'    |    |-- "{li.value}"@{li.language_code}')
             print('    |')
 
-        relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
+        relations_obj: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
                                                                                           uri=entity.uri)
         if len(relations_obj) > 0:
             print('    | [Relations]')
             for re in relations_obj.values():
                 print(f'    |--- {re.relation.iri}: ')
                 print(f'           |- [Incoming]: {re.incoming_relations} ')
                 print(f'           |- [Outgoing]: {re.outgoing_relations}')
         print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
@@ -268,48 +315,48 @@
     print('-----------------------------------------------------------------------------------------------------------')
     print(' First step: Find Leonardo da Vinci in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     s_idx: int = 1
-    for entity in res_entities:
+    for res_entity in res_entities:
         #  Entity must be a person and the label match with full string
-        if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
-            leo = entity
+        if res_entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [la.content for la in res_entity.label]:
+            leo = res_entity
             break
 
     print('-----------------------------------------------------------------------------------------------------------')
     print(' What artwork exists in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
-    relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
+    relations_dict: dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
                                                                                                  uri=leo.uri)
     print(f' Artwork of {leo.label}')
     print('-----------------------------------------------------------------------------------------------------------')
     idx: int = 1
     if CREATED in relations_dict:
         for e in relations_dict[CREATED].outgoing_relations:
             print(f' [{idx}] {e.uri}: {e.label}')
             idx += 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(' Let us create a new piece of artwork.')
     print('-----------------------------------------------------------------------------------------------------------')
 
     # Main labels for entity
-    artwork_labels: List[Label] = [
+    artwork_labels: list[Label] = [
         Label('Ginevra Gherardini', LanguageCode('en_US')),
         Label('Ginevra Gherardini', LanguageCode('de_DE'))
     ]
     # Alias labels for entity
-    artwork_alias: List[Label] = [
+    artwork_alias: list[Label] = [
         Label("Ginevra", LanguageCode('en_US')),
         Label("Ginevra", LanguageCode('de_DE'))
     ]
     # Topic description
-    artwork_description: List[Description] = [
+    artwork_description: list[Description] = [
         Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
         Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
     ]
     # Topic
     artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
                                               description=artwork_description,
                                               icon=ICON)
@@ -404,36 +451,40 @@
     while True:
         # pull
         entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
                                                                         limit=100)
         pulled_entities: int = len(entities)
         if pulled_entities == 0:
             break
-        delete_uris: List[str] = [e.uri for e in entities]
+        delete_uris: list[str] = [e.uri for e in entities]
         print(f'Cleanup. Delete entities: {delete_uris}')
         knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
         page_number += 1
         page_id = next_page_id
     print('-----------------------------------------------------------------------------------------------------------')
 ```
 
 ### Named Entity Linking 
 
 Performing Named Entity Linking (NEL) on text and Universal Ink Model.
 
 ```python
 import argparse
-from typing import List, Dict
+
+import urllib3
 
 from knowledge.base.entity import LanguageCode
 from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.nel.base import KnowledgeGraphEntity
 from knowledge.nel.engine import WacomEntityLinkingEngine
 from knowledge.services.graph import WacomKnowledgeService
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+
 LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
 TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
 
 
 def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
     """
     Printing entity details.
@@ -457,15 +508,15 @@
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if len(thing.label) > 0:
         print('    | [Alias]')
         for la in thing.alias:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
-    relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
+    relations: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
     if len(thing.data_properties) > 0:
         print('    | [Attributes]')
         for data_property, labels in thing.data_properties.items():
             print(f'    |    |- {data_property.iri}:')
             for li in labels:
                 print(f'    |    |-- "{li.value}"@{li.language_code}')
         print('    |')
@@ -476,34 +527,34 @@
             print(f'           |- [Incoming]: {re.incoming_relations} ')
             print(f'           |- [Outgoing]: {re.outgoing_relations}')
     print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Named Entity Linking Knowledge access",
         service_url=args.instance)
     #  Wacom Named Entity Linking
     nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
         service_url=args.instance,
         service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
     )
     # Use special tenant for testing:  Unit-test tenant
     user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-    entities: List[KnowledgeGraphEntity] = nel_client.\
+    entities: list[KnowledgeGraphEntity] = nel_client.\
         link_personal_entities(auth_key=user_token, text=TEXT,
                                language_code=LANGUAGE_CODE)
     idx: int = 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
     print('-----------------------------------------------------------------------------------------------------------')
     for e in entities:
@@ -514,67 +565,74 @@
 
 ### Access Management
 
 The sample shows, how access to entities can be shared with a group of users or the tenant.
 
 ```python
 import argparse
-from typing import List
+
 from knowledge.base.entity import LanguageCode, Label, Description
 from knowledge.base.ontology import OntologyClassReference, ThingObject
 from knowledge.services.base import WacomServiceException
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.group import GroupManagementServiceAPI, Group
 from knowledge.services.users import UserManagementServiceAPI
 
 # ------------------------------- User credential ----------------------------------------------------------------------
 TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
 
 
 def create_entity() -> ThingObject:
+    """Create a new entity.
+
+    Returns
+    -------
+    entity: ThingObject
+        Entity object
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Hidden', LanguageCode('en_US')),
         Label('Versteckt', LanguageCode('de_DE')),
         Label('隠れた', LanguageCode('ja_JP'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
     # Topic
     topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
     return topic_object
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
     # User Management
     user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
     # Group Management
     group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     # Now, we create a users
-    u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
-    u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
-    u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
+    u1, u1_token, _, _ = user_management.create_user(TENANT_KEY, "u1")
+    u2, u2_token, _, _ = user_management.create_user(TENANT_KEY, "u2")
+    u3, u3_token, _, _ = user_management.create_user(TENANT_KEY, "u3")
 
     # Now, let's create an entity
     thing: ThingObject = create_entity()
     entity_uri: str = knowledge_client.create_entity(u1_token, thing)
     # Only user 1 can access the entity from cloud storage
     my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
     print(f'User is the owner of {my_thing.owner}')
@@ -628,20 +686,34 @@
 ```
 
 ### Ontology Creation
 
 The samples show how the ontology can be extended and new entities can be added using the added classes.
 
 ```python
+# -*- coding: utf-8 -*-
+# Copyright © 2021-2022 Wacom Authors. All Rights Reserved.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language_code governing permissions and
+#  limitations under the License.
 import argparse
-from typing import List, Optional
+from typing import Optional
 
-from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
+from knowledge.base.entity import Label, LanguageCode, Description
 from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
-    DataProperty
+    DataProperty, OntologyContext
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.ontology import OntologyService
 
 # ------------------------------- Constants ----------------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
 CONTEXT_NAME: str = 'core'
 # Wacom Base Ontology Types
@@ -651,21 +723,28 @@
 # Demo Object property
 IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
 # Demo Data property
 STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
 
 
 def create_artist() -> ThingObject:
+    """
+    Create a new artist entity.
+    Returns
+    -------
+    instance: ThingObject
+        Artist entity
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
 
     data_property: DataProperty = DataProperty(content='Salaj',
                                                property_ref=STAGE_NAME,
                                                language_code=LanguageCode('en_US'))
@@ -673,52 +752,50 @@
     artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
     artist.add_data_property(data_property)
     return artist
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom Ontology REST API Client
     ontology_client: OntologyService = OntologyService(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Ontology Creation Demo",
         service_url=args.instance)
-    contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
-    if len(contexts) == 0:
+    context: Optional[OntologyContext] = ontology_client.context(admin_token)
+    if context is None:
         # First, create a context for the ontology
         ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
         context_name: str = CONTEXT_NAME
     else:
-        context_name: str = contexts[0].context
+        context_name: str = context.context
     # Creating a class which is a subclass of a person
-    ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
+    ontology_client.create_concept(admin_token, context_name, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
 
     # Object properties
-    ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
-                                           ranges_cls=[PERSON_TYPE],
-                                           inverse_of=None, subproperty_of=None)
+    ontology_client.create_object_property(auth_key=admin_token, context=context_name,
+                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE],
+                                           ranges_cls=[PERSON_TYPE], inverse_of=None, subproperty_of=None)
     # Data properties
-    ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
+    ontology_client.create_data_property(auth_key=admin_token, context=context_name,
                                          reference=STAGE_NAME,
                                          domains_cls=[ARTIST_TYPE],
                                          ranges_cls=[DataPropertyType.STRING],
                                          subproperty_of=None)
-
     # Commit the changes of the ontology. This is very important to confirm changes.
-    ontology_client.commit(admin_token, CONTEXT_NAME)
+    ontology_client.commit(admin_token, context_name)
     # Trigger graph service. After the update the ontology is available and the new entities can be created
     knowledge_client.ontology_update(admin_token)
 
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     for entity in res_entities:
@@ -726,14 +803,15 @@
         if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
             leo = entity
             break
 
     artist_student: ThingObject = create_artist()
     artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
     knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
+
 ```
 
 ## Tools
 
 The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
 
 ### Listing script
@@ -743,15 +821,15 @@
 ```bash
 >> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
@@ -759,50 +837,56 @@
 >> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 - _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
 - _-p, --images (optional)_ - Include the images in the dump.
 - _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
  
-### Push entities script
+### Import entities script
 
 Pushing entities to knowledge graph.
 
 ```bash
->> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
+>> python import_entities.py [-h] [-u USER] [-t TENANT] [-g GROUP_NAME] [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
-  
-### Reset
+- _-g GROUP_NAME, --group_id GROUP_NAME_ - Group name where the entities will be assigned to. 
+- _-p , --public_ - Group name where the entities will be assigned to.
 
-Resets a tenant by removing entities, groups, and users. 
+### Wikidata scrapper
 
 ```bash
->> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
+usage: wikidata_scrapper.py [-h] -u USER -t TENANT [-i INSTANCE] [-c CACHE]
+                            [-m MAPPING] [-d DEPTH]
+                            [-l LANGUAGES [LANGUAGES ...]]
+wikidata_scrapper.py: error: the following arguments are required: -u/--user, -t/--tenant
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
+- _-c CACHE, --cache CACHE_ - Path to entities that must are exports in import format.
+- _-m MAPPING, --mapping MAPPING_ - Mapping file to configure the wikidata mapping.
+- _-d DEPTH, --depth DEPTH_ - Depth of the graph to be scrapped.
+- _-l LANGUAGES [LANGUAGES ...], --languages LANGUAGES [LANGUAGES ...]_ - Languages to be scrapped.
   
 # Documentation
 
 You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
 API documentation is available [here](./docs/).
 
 ## Contributing
```

### Comparing `personal_knowledge_library-0.9.6/README.md` & `personal_knowledge_library-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Wacom Personal Knowledge Library
+# Wacom Private Knowledge Library
 
-The library and the cloud services are still under development. 
-The required access tokens are only available for selected partner companies.
-
-> :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
+The required tenant API key is only available for selected partner companies.
+Please contact your Wacom representative for more information.
 
 ## Introduction
 
 In knowledge management there is a distinction between data, information and knowledge.
 In the domain of digital ink this means:
 
 - **Data** - The equivalent would be the ink strokes
 - **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
 - **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
 
 The following illustration shows the different layers of knowledge:
 ![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
 
-For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
+For handling semantics, Wacom introduced the Wacom Private Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
 
 This library provide simplified access to Wacom's personal knowledge cloud service.
 It contains:
 
 - Basic datastructures for Ontology object and entities from the knowledge graph
 - Clients for the REST APIs
 - Connector for Wikidata public knowledge graph
@@ -34,19 +32,45 @@
 
 **Entity service:**
 
 - List all entities
 - Add entities to knowledge graph
 - Access object properties
 
+**Search service:**
+
+- Search for entities for labels and descriptions with a given language
+- Search for literals (data properties) 
+- Search for relations (object properties)
+
+**Group service:**
+
+- List all groups
+- Add groups, modify groups, delete groups
+- Add users and entities to groups
+
+**Ontology service:**
+
+- List all Ontology structures
+- Modify Ontology structures
+
+**Named Entity Linking service:**
+
+- Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
+
+**Wikidata connector:**
+
+- Import entities from Wikidata
+- Mapping Wikidata entities to WPK entities
+
 # Technology stack
 
 ## Domain Knowledge
 
-The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
+The tasks of the ontology within Wacom's private knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
 The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
 
 - Foundation for structured data, knowledge representation as concepts and relations among concepts
 - Being explicit definitions of shared vocabularies for interoperability
 - Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
 - Can be used for problem solving
 
@@ -63,23 +87,45 @@
 - Extract knowledge from various sources (Connectors)
 - Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
 - Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
 
 
 # Functionality
 
+## Import Format
+
+For importing entities into the knowledge graph, the tools/import_entities.py script can be used.
+
+The ThingObject support a NDJSON based import format, where the individual JSON files can contain the following structure.
+
+| Field name             | Subfield name | Data Structure | Description                                                                                    |
+|------------------------|---------------|----------------|------------------------------------------------------------------------------------------------|
+| source_reference_id    |               | str            | A unique identifier for the entity used in the source system                                  |
+| source_system          |               | str            | The source system describes the original source of the entity, such as wikidata, youtube, ... |
+| image                  |               | str            | A string representing the URL of the entity's icon.                                           |
+| labels                 |               | array          | An array of label objects, where each object has the following fields:                       |
+|                        | value         | str            | A string representing the label text in the specified locale.                                |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+|                        | isMain        | bool           | A boolean flag indicating if this label is the main label for the entity (true) or an alias (false). |
+| descriptions           |               | array          | An array of description objects, where each object has the following fields:                 |
+|                        | description   | str            | A string representing the description text in the specified locale.                          |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+| type                   |               | str            | A string representing the IRI of the ontology class for this entity.                         |
+| literals               |               | array[map]     | An array of data property objects, where each object has the following fields:               |
+
+
 ## Access API
 
 The personal knowledge graph backend is implement as a multi-tenancy system.
 Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
 
 ![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
 
 In general, a tenant with their users, groups, and entities are logically separated.
-Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
+Physically the entities are store in the same instance of the Wacom Private Knowledge (WPK) backend database system.
 
 The user management is rather limited, each organisation must provide their own authentication service and user management.
 The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
 
 The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
 While users for each tenant can be created by the owner of the **Tenant API Key**.
 You will receive this token from the system owner after the creation of the tenant.
@@ -147,15 +193,15 @@
 
 ### Entity handling
 
 This samples shows how to work with graph service.
 
 ```python
 import argparse
-from typing import Optional, List, Dict
+from typing import Optional
 
 from knowledge.base.entity import LanguageCode, Description, Label
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.services.graph import WacomKnowledgeService
 
 # ------------------------------- Knowledge entities -------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
@@ -172,69 +218,70 @@
 ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
 IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
 HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
 CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
 HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
 
 
-def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
+def print_entity(display_entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService,
+                 short: bool = False):
     """
     Printing entity details.
 
     Parameters
     ----------
-    entity: ThingObject
+    display_entity: ThingObject
         Entity with properties
     list_idx: int
         Index with a list
     auth_key: str
         Authorization key
     client: WacomKnowledgeService
         Knowledge graph client
     short: bool
         Short summary
     """
-    print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
-    if len(entity.label) > 0:
+    print(f'[{list_idx}] : {display_entity.uri} <{display_entity.concept_type.iri}>')
+    if len(display_entity.label) > 0:
         print('    | [Labels]')
-        for la in entity.label:
+        for la in display_entity.label:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if not short:
-        if len(entity.alias) > 0:
+        if len(display_entity.alias) > 0:
             print('    | [Alias]')
-            for la in entity.alias:
+            for la in display_entity.alias:
                 print(f'    |     |- "{la.content}"@{la.language_code}')
             print('    |')
-        if len(entity.data_properties) > 0:
+        if len(display_entity.data_properties) > 0:
             print('    | [Attributes]')
             for data_property, labels in entity.data_properties.items():
                 print(f'    |    |- {data_property.iri}:')
                 for li in labels:
                     print(f'    |    |-- "{li.value}"@{li.language_code}')
             print('    |')
 
-        relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
+        relations_obj: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
                                                                                           uri=entity.uri)
         if len(relations_obj) > 0:
             print('    | [Relations]')
             for re in relations_obj.values():
                 print(f'    |--- {re.relation.iri}: ')
                 print(f'           |- [Incoming]: {re.incoming_relations} ')
                 print(f'           |- [Outgoing]: {re.outgoing_relations}')
         print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
@@ -246,48 +293,48 @@
     print('-----------------------------------------------------------------------------------------------------------')
     print(' First step: Find Leonardo da Vinci in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     s_idx: int = 1
-    for entity in res_entities:
+    for res_entity in res_entities:
         #  Entity must be a person and the label match with full string
-        if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
-            leo = entity
+        if res_entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [la.content for la in res_entity.label]:
+            leo = res_entity
             break
 
     print('-----------------------------------------------------------------------------------------------------------')
     print(' What artwork exists in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
-    relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
+    relations_dict: dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
                                                                                                  uri=leo.uri)
     print(f' Artwork of {leo.label}')
     print('-----------------------------------------------------------------------------------------------------------')
     idx: int = 1
     if CREATED in relations_dict:
         for e in relations_dict[CREATED].outgoing_relations:
             print(f' [{idx}] {e.uri}: {e.label}')
             idx += 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(' Let us create a new piece of artwork.')
     print('-----------------------------------------------------------------------------------------------------------')
 
     # Main labels for entity
-    artwork_labels: List[Label] = [
+    artwork_labels: list[Label] = [
         Label('Ginevra Gherardini', LanguageCode('en_US')),
         Label('Ginevra Gherardini', LanguageCode('de_DE'))
     ]
     # Alias labels for entity
-    artwork_alias: List[Label] = [
+    artwork_alias: list[Label] = [
         Label("Ginevra", LanguageCode('en_US')),
         Label("Ginevra", LanguageCode('de_DE'))
     ]
     # Topic description
-    artwork_description: List[Description] = [
+    artwork_description: list[Description] = [
         Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
         Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
     ]
     # Topic
     artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
                                               description=artwork_description,
                                               icon=ICON)
@@ -382,36 +429,40 @@
     while True:
         # pull
         entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
                                                                         limit=100)
         pulled_entities: int = len(entities)
         if pulled_entities == 0:
             break
-        delete_uris: List[str] = [e.uri for e in entities]
+        delete_uris: list[str] = [e.uri for e in entities]
         print(f'Cleanup. Delete entities: {delete_uris}')
         knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
         page_number += 1
         page_id = next_page_id
     print('-----------------------------------------------------------------------------------------------------------')
 ```
 
 ### Named Entity Linking 
 
 Performing Named Entity Linking (NEL) on text and Universal Ink Model.
 
 ```python
 import argparse
-from typing import List, Dict
+
+import urllib3
 
 from knowledge.base.entity import LanguageCode
 from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.nel.base import KnowledgeGraphEntity
 from knowledge.nel.engine import WacomEntityLinkingEngine
 from knowledge.services.graph import WacomKnowledgeService
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+
 LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
 TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
 
 
 def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
     """
     Printing entity details.
@@ -435,15 +486,15 @@
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if len(thing.label) > 0:
         print('    | [Alias]')
         for la in thing.alias:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
-    relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
+    relations: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
     if len(thing.data_properties) > 0:
         print('    | [Attributes]')
         for data_property, labels in thing.data_properties.items():
             print(f'    |    |- {data_property.iri}:')
             for li in labels:
                 print(f'    |    |-- "{li.value}"@{li.language_code}')
         print('    |')
@@ -454,34 +505,34 @@
             print(f'           |- [Incoming]: {re.incoming_relations} ')
             print(f'           |- [Outgoing]: {re.outgoing_relations}')
     print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Named Entity Linking Knowledge access",
         service_url=args.instance)
     #  Wacom Named Entity Linking
     nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
         service_url=args.instance,
         service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
     )
     # Use special tenant for testing:  Unit-test tenant
     user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-    entities: List[KnowledgeGraphEntity] = nel_client.\
+    entities: list[KnowledgeGraphEntity] = nel_client.\
         link_personal_entities(auth_key=user_token, text=TEXT,
                                language_code=LANGUAGE_CODE)
     idx: int = 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
     print('-----------------------------------------------------------------------------------------------------------')
     for e in entities:
@@ -492,67 +543,74 @@
 
 ### Access Management
 
 The sample shows, how access to entities can be shared with a group of users or the tenant.
 
 ```python
 import argparse
-from typing import List
+
 from knowledge.base.entity import LanguageCode, Label, Description
 from knowledge.base.ontology import OntologyClassReference, ThingObject
 from knowledge.services.base import WacomServiceException
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.group import GroupManagementServiceAPI, Group
 from knowledge.services.users import UserManagementServiceAPI
 
 # ------------------------------- User credential ----------------------------------------------------------------------
 TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
 
 
 def create_entity() -> ThingObject:
+    """Create a new entity.
+
+    Returns
+    -------
+    entity: ThingObject
+        Entity object
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Hidden', LanguageCode('en_US')),
         Label('Versteckt', LanguageCode('de_DE')),
         Label('隠れた', LanguageCode('ja_JP'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
     # Topic
     topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
     return topic_object
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
     # User Management
     user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
     # Group Management
     group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     # Now, we create a users
-    u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
-    u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
-    u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
+    u1, u1_token, _, _ = user_management.create_user(TENANT_KEY, "u1")
+    u2, u2_token, _, _ = user_management.create_user(TENANT_KEY, "u2")
+    u3, u3_token, _, _ = user_management.create_user(TENANT_KEY, "u3")
 
     # Now, let's create an entity
     thing: ThingObject = create_entity()
     entity_uri: str = knowledge_client.create_entity(u1_token, thing)
     # Only user 1 can access the entity from cloud storage
     my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
     print(f'User is the owner of {my_thing.owner}')
@@ -606,20 +664,34 @@
 ```
 
 ### Ontology Creation
 
 The samples show how the ontology can be extended and new entities can be added using the added classes.
 
 ```python
+# -*- coding: utf-8 -*-
+# Copyright © 2021-2022 Wacom Authors. All Rights Reserved.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language_code governing permissions and
+#  limitations under the License.
 import argparse
-from typing import List, Optional
+from typing import Optional
 
-from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
+from knowledge.base.entity import Label, LanguageCode, Description
 from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
-    DataProperty
+    DataProperty, OntologyContext
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.ontology import OntologyService
 
 # ------------------------------- Constants ----------------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
 CONTEXT_NAME: str = 'core'
 # Wacom Base Ontology Types
@@ -629,21 +701,28 @@
 # Demo Object property
 IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
 # Demo Data property
 STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
 
 
 def create_artist() -> ThingObject:
+    """
+    Create a new artist entity.
+    Returns
+    -------
+    instance: ThingObject
+        Artist entity
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
 
     data_property: DataProperty = DataProperty(content='Salaj',
                                                property_ref=STAGE_NAME,
                                                language_code=LanguageCode('en_US'))
@@ -651,52 +730,50 @@
     artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
     artist.add_data_property(data_property)
     return artist
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom Ontology REST API Client
     ontology_client: OntologyService = OntologyService(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Ontology Creation Demo",
         service_url=args.instance)
-    contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
-    if len(contexts) == 0:
+    context: Optional[OntologyContext] = ontology_client.context(admin_token)
+    if context is None:
         # First, create a context for the ontology
         ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
         context_name: str = CONTEXT_NAME
     else:
-        context_name: str = contexts[0].context
+        context_name: str = context.context
     # Creating a class which is a subclass of a person
-    ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
+    ontology_client.create_concept(admin_token, context_name, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
 
     # Object properties
-    ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
-                                           ranges_cls=[PERSON_TYPE],
-                                           inverse_of=None, subproperty_of=None)
+    ontology_client.create_object_property(auth_key=admin_token, context=context_name,
+                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE],
+                                           ranges_cls=[PERSON_TYPE], inverse_of=None, subproperty_of=None)
     # Data properties
-    ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
+    ontology_client.create_data_property(auth_key=admin_token, context=context_name,
                                          reference=STAGE_NAME,
                                          domains_cls=[ARTIST_TYPE],
                                          ranges_cls=[DataPropertyType.STRING],
                                          subproperty_of=None)
-
     # Commit the changes of the ontology. This is very important to confirm changes.
-    ontology_client.commit(admin_token, CONTEXT_NAME)
+    ontology_client.commit(admin_token, context_name)
     # Trigger graph service. After the update the ontology is available and the new entities can be created
     knowledge_client.ontology_update(admin_token)
 
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     for entity in res_entities:
@@ -704,14 +781,15 @@
         if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
             leo = entity
             break
 
     artist_student: ThingObject = create_artist()
     artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
     knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
+
 ```
 
 ## Tools
 
 The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
 
 ### Listing script
@@ -721,15 +799,15 @@
 ```bash
 >> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
@@ -737,50 +815,56 @@
 >> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 - _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
 - _-p, --images (optional)_ - Include the images in the dump.
 - _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
  
-### Push entities script
+### Import entities script
 
 Pushing entities to knowledge graph.
 
 ```bash
->> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
+>> python import_entities.py [-h] [-u USER] [-t TENANT] [-g GROUP_NAME] [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
-  
-### Reset
+- _-g GROUP_NAME, --group_id GROUP_NAME_ - Group name where the entities will be assigned to. 
+- _-p , --public_ - Group name where the entities will be assigned to.
 
-Resets a tenant by removing entities, groups, and users. 
+### Wikidata scrapper
 
 ```bash
->> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
+usage: wikidata_scrapper.py [-h] -u USER -t TENANT [-i INSTANCE] [-c CACHE]
+                            [-m MAPPING] [-d DEPTH]
+                            [-l LANGUAGES [LANGUAGES ...]]
+wikidata_scrapper.py: error: the following arguments are required: -u/--user, -t/--tenant
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
+- _-c CACHE, --cache CACHE_ - Path to entities that must are exports in import format.
+- _-m MAPPING, --mapping MAPPING_ - Mapping file to configure the wikidata mapping.
+- _-d DEPTH, --depth DEPTH_ - Depth of the graph to be scrapped.
+- _-l LANGUAGES [LANGUAGES ...], --languages LANGUAGES [LANGUAGES ...]_ - Languages to be scrapped.
   
 # Documentation
 
 You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
 API documentation is available [here](./docs/).
 
 ## Contributing
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/__init__.py` & `personal_knowledge_library-1.0.0/knowledge/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 """"
 Personal knowledge Library
 --------------------------
 This library provides a set of tools to manage Wacom private knowledge graph API.
 All services are wrapped in a pythonic way to make it easy to use.
 """
 import logging
-from typing import Optional
+from typing import Union
 
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "0.9.6"
+__version__ = "1.0.0"
 
 # Create the Logger
-logger: Optional[logging.Logger] = None
+logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
 
     ch: logging.StreamHandler = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.0/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.6/knowledge/base/access.py` & `personal_knowledge_library-1.0.0/knowledge/base/access.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
-from typing import List
 
 
-class AccessRight(object):
+class AccessRight:
     """
     Access rights for entities within a tenant.
 
     Parameters
     ----------
     read: bool (default := False)
         Read access for entity within tenant.
@@ -61,24 +60,24 @@
         if self.write:
             result += prefix + AccessRight.WRITE
         if self.delete:
             result += AccessRight.DELETE
         result += ']'
         return result
 
-    def to_list(self) -> List[str]:
+    def to_list(self) -> list[str]:
         """
         Converts the access to list of properties.
 
         Returns
         -------
-        access_list: List[str]
+        access_list: list[str]
             List of rights
         """
-        rights: List[str] = []
+        rights: list[str] = []
         if self.read:
             rights.append(TenantAccessRight.READ)
         if self.write:
             rights.append(TenantAccessRight.WRITE)
         if self.delete:
             rights.append(TenantAccessRight.DELETE)
         return rights
@@ -100,21 +99,21 @@
         Delete access for entity within tenant.
     """
 
     def __init__(self, read: bool = False, write: bool = False, delete: bool = False):
         super().__init__(read, write, delete)
 
     @classmethod
-    def parse(cls, param: List[str]) -> 'TenantAccessRight':
+    def parse(cls, param: list[str]) -> 'TenantAccessRight':
         """
         Converts the access to list of properties.
 
         Parameters
         ----------
-        param: List[str]
+        param: list[str]
             List of rights
 
         Returns
         -------
         tenant_rights: TenantAccessRight
             Instantiated rights.
         """
@@ -141,21 +140,21 @@
         Delete access for entity within group.
     """
 
     def __init__(self, read: bool = False, write: bool = False, delete: bool = False):
         super().__init__(read, write, delete)
 
     @classmethod
-    def parse(cls, param: List[str]) -> 'GroupAccessRight':
+    def parse(cls, param: list[str]) -> 'GroupAccessRight':
         """
         Converts the access to list of properties.
 
         Parameters
         ----------
-        param: List[str]
+        param: list[str]
             List of rights
 
         Returns
         -------
         group_rights: GroupAccessRight
             Instantiated rights.
         """
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.0/knowledge/base/ontology.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
+# Copyright © 2021-2023 Wacom. All rights reserved.
+import abc
+import enum
+from datetime import datetime
 from json import JSONEncoder
-from typing import List, Union, Set, Tuple
+from typing import Union, Optional, Any
+
+import dateutil
 
 from knowledge.base.access import TenantAccessRight
-from knowledge.base.entity import *
+from knowledge.base.entity import EntityStatus, Label, LanguageCode, Description, URI_TAG, IMAGE_TAG, DESCRIPTIONS_TAG,\
+    LABELS_TAG, TYPE_TAG, STATUS_FLAG_TAG, DATA_PROPERTIES_TAG, OBJECT_PROPERTIES_TAG, GROUP_IDS, OWNER_TAG, \
+    OWNER_ID_TAG, SOURCE_REFERENCE_ID_TAG, SOURCE_SYSTEM_TAG, TENANT_RIGHTS_TAG, SEND_TO_NEL_TAG, LOCALE_TAG, \
+    IS_MAIN_TAG, USE_NEL_TAG, VALUE_TAG, DATA_PROPERTY_TAG, VISIBILITY_TAG, INFLECTION_CASE_SENSITIVE, \
+    INFLECTION_SETTING, INFLECTION_CONCEPT_CLASS, LANGUAGE_TAG, CONTENT_TAG, DATA_TYPE_TAG, RELATION_TAG, INCOMING_TAG,\
+    OUTGOING_TAG, COMMENT_TAG, LocalizedContent, LOCALIZED_CONTENT_TAG, COMMENTS_TAG
 
 # ---------------------------------------------- Vocabulary base URI ---------------------------------------------------
 PREFIX: str = "xsd"
 BASE_URI: str = "http://www.w3.org/2001/XMLSchema#"
 # ---------------------------------------------------- Constants -------------------------------------------------------
 SUB_CLASS_OF_TAG: str = 'subClassOf'
 TENANT_ID: str = 'tenantId'
 NAME_TAG: str = "name"
-SUPPORTED_LOCALES: List[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'zh_CN']
-SUPPORTED_LANGUAGES: List[str] = ['ja', 'en', 'de', 'bg', 'fr', 'it', 'es', 'zh']
-LANGUAGE_LOCALE_MAPPING: Dict[str, str] = dict([(lang, locale)
+EN_US: str = "en_US"
+EN: str = "en"
+SUPPORTED_LOCALES: list[str] = ['ja_JP', EN_US, 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES']
+SUPPORTED_LANGUAGES: list[str] = ['ja', EN, 'de', 'bg', 'fr', 'it', 'es']
+LANGUAGE_LOCALE_MAPPING: dict[str, str] = dict([(lang, locale)
                                                 for lang, locale in zip(SUPPORTED_LANGUAGES, SUPPORTED_LOCALES)])
-LOCALE_LANGUAGE_MAPPING: Dict[str, str] = dict([(locale, lang)
+LOCALE_LANGUAGE_MAPPING: dict[str, str] = dict([(locale, lang)
                                                 for locale, lang in zip(SUPPORTED_LOCALES, SUPPORTED_LANGUAGES)])
 
 
 # ---------------------------------------------------- Ontology --------------------------------------------------------
 class PropertyType(enum.Enum):
     """
     PropertyType
     -----------
     Within the ontology two different property types are defined. A data- and an object property.
     """
     OBJECT_PROPERTY = "Relation"
     DATA_PROPERTY = "Literal"
 
 
-INVERSE_PROPERTY_TYPE: Dict[str, PropertyType] = dict([(pt.value, pt) for pt in PropertyType])
+INVERSE_PROPERTY_TYPE: dict[str, PropertyType] = dict([(pt.value, pt) for pt in PropertyType])
 
 
 class DataPropertyType(enum.Enum):
     """
     DataPropertyType.
     -----------------
     Data types that are used by Datatype properties.
@@ -117,21 +129,98 @@
     """XML NMTOKENs"""
     NAME = BASE_URI + "Name"
     """XML Names"""
     NC_NAME = BASE_URI + "NCName"
     """XML NCNames"""
 
 
-INVERSE_DATA_PROPERTY_TYPE_MAPPING: Dict[str, DataPropertyType] = dict([(str(lit_type.value), lit_type)
+INVERSE_DATA_PROPERTY_TYPE_MAPPING: dict[str, DataPropertyType] = dict([(str(lit_type.value), lit_type)
                                                                         for lit_type in DataPropertyType])
 """Maps the string representation of the XSD data types to the data types enum constants."""
 
 
 # ------------------------------------------ Ontology References -------------------------------------------------------
 
+class OntologyLabel(LocalizedContent):
+    """
+    Ontology Label
+    --------------
+    Label that is multi-lingual.
+
+    Parameters
+    ----------
+    content: str
+        Content value
+    language_code: LanguageCode (default:= 'en')
+        Language code of content
+    main: bool (default:=False)
+        Main content
+    """
+
+    def __init__(self, content: str, language_code: LanguageCode = 'en', main: bool = False):
+        self.__main: bool = main
+        super().__init__(content, language_code)
+
+    @property
+    def main(self) -> bool:
+        """Flag if the content is the  main content or an alias."""
+        return self.__main
+
+    @staticmethod
+    def create_from_dict(dict_label: dict[str, Any], tag_name: str = CONTENT_TAG, locale_name: str = LOCALE_TAG) \
+            -> 'OntologyLabel':
+        """
+        Create a label from a dictionary.
+
+        Parameters
+        ----------
+        dict_label: dict[str, Any]
+            Dictionary with the label information
+        tag_name: str
+            Tag name of the content
+        locale_name: str
+            Tag name of the language code
+
+        Returns
+        -------
+        instance: OntologyLabel
+            Instance of the label
+        """
+        if tag_name not in dict_label:
+            raise ValueError("Dict is does not contain a localized label.")
+        if locale_name not in dict_label:
+            raise ValueError("Dict is does not contain a language code")
+        if IS_MAIN_TAG in dict_label:
+            return OntologyLabel(dict_label[tag_name], dict_label[locale_name], dict_label[IS_MAIN_TAG])
+        return OntologyLabel(dict_label[tag_name], dict_label[locale_name])
+
+    @staticmethod
+    def create_from_list(param: list[dict]) -> list[LOCALIZED_CONTENT_TAG]:
+        """
+        Create a list of labels from a list of dictionaries.
+        Parameters
+        ----------
+        param: list[dict]
+            List of dictionaries with the label information
+
+        Returns
+        -------
+        instances: list[OntologyLabel]
+            List of label instances
+        """
+        return [Label.create_from_dict(p) for p in param]
+
+    def __dict__(self):
+        return {
+            CONTENT_TAG: self.content,
+            LOCALE_TAG: self.language_code,
+            IS_MAIN_TAG: self.main
+        }
+
+
 class OntologyObjectReference(abc.ABC):
     """
         Ontology class type
         ------------------
         Associated to an entity to link the type of the entity.
 
         Parameters
@@ -169,15 +258,31 @@
         """Internationalized Resource Identifier (IRI) encoded ontology class name."""
         return f'{self.scheme}:{self.context}#{self.name}'
 
     def __repr__(self):
         return self.iri
 
     @classmethod
-    def parse_iri(cls, iri: str) -> Tuple[str, str, str]:
+    def parse_iri(cls, iri: str) -> tuple[str, str, str]:
+        """Parse an IRI into its components.
+
+        Parameters
+        ----------
+        iri: str
+            IRI to parse
+
+        Returns
+        -------
+        tuple[str, str, str]
+            Scheme, context and name of the IRI
+        """
+        if iri is None:
+            raise ValueError('IRI cannot be None')
+        if ":" not in iri or "#" not in iri:
+            raise ValueError(f'Invalid IRI: {iri}')
         colon_idx: int = iri.index(':')
         hash_idx: int = iri.index('#')
         scheme: str = iri[:colon_idx]
         context: str = iri[colon_idx + 1:hash_idx]
         name: str = iri[hash_idx + 1:]
         return scheme, context, name
 
@@ -204,14 +309,26 @@
     @property
     def class_name(self):
         """Class name."""
         return self.name
 
     @classmethod
     def parse(cls, iri: str) -> 'OntologyClassReference':
+        """Parse IRI to create an ontology class reference.
+
+        Parameters
+        ----------
+        iri: str
+            IRI of ontology class reference
+
+        Returns
+        -------
+        instance: OntologyClassReference
+            Instance of ontology class reference
+        """
         scheme, context, name = OntologyObjectReference.parse_iri(iri)
         return OntologyClassReference(scheme, context, name)
 
     def __eq__(self, other):
         if not isinstance(other, OntologyClassReference):
             return False
         return self.iri == other.iri
@@ -242,14 +359,26 @@
     @property
     def property_name(self):
         """Property name."""
         return self.name
 
     @classmethod
     def parse(cls, iri: str) -> 'OntologyPropertyReference':
+        """ Parses an IRI into an OntologyPropertyReference.
+
+        Parameters
+        ----------
+        iri: str
+            IRI to parse
+
+        Returns
+        -------
+        instance: OntologyPropertyReference
+            Instance of OntologyPropertyReference
+        """
         scheme, context, name = OntologyObjectReference.parse_iri(iri)
         return OntologyPropertyReference(scheme, context, name)
 
     def __eq__(self, other):
         if not isinstance(other, OntologyPropertyReference):
             return False
         return self.iri == other.iri
@@ -260,14 +389,346 @@
 
 # ------------------------------------------------- Constants ----------------------------------------------------------
 THING_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Thing')
 SYSTEM_SOURCE_SYSTEM: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'sourceSystem')
 SYSTEM_SOURCE_REFERENCE_ID: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'sourceReferenceId')
 
 
+class Comment(LocalizedContent):
+    """
+    Comment
+    -------
+    Comment that is multi-lingual.
+
+    Parameters
+    ----------
+    text: str
+        Text value
+    language_code: LanguageCode (default:= 'en')
+        Language code of content
+    """
+
+    def __init__(self, text: str, language_code: LanguageCode = 'en'):
+        super().__init__(text, language_code)
+
+    @staticmethod
+    def create_from_dict(dict_description: dict[str, Any]) -> 'Comment':
+        """
+        Create a comment from a dictionary.
+        Parameters
+        ----------
+        dict_description: dict[str, Any]
+            Dictionary containing the comment
+
+        Returns
+        -------
+        instance: Comment
+            Instance of comment
+        """
+        if VALUE_TAG not in dict_description or LANGUAGE_TAG not in dict_description:
+            raise ValueError("Dict is does not contain a localized comment.")
+        return Comment(dict_description[VALUE_TAG], dict_description[LANGUAGE_TAG])
+
+    @staticmethod
+    def create_from_list(param: list[dict[str, Any]]) -> list['Comment']:
+        """
+        Create a list of comments from a list of dictionaries.
+        Parameters
+        ----------
+        param: list[dict[str, Any]]
+            List of dictionaries containing the comments
+
+        Returns
+        -------
+        instances: list[Comment]
+            List of instances of comments
+        """
+        return [Comment.create_from_dict(p) for p in param]
+
+    def __dict__(self):
+        return {
+            COMMENT_TAG: self.content,
+            LOCALE_TAG: self.language_code,
+        }
+
+
+class OntologyObject(abc.ABC):
+    """
+    Generic ontology object
+    -----------------------
+
+    Parameters
+    ----------
+    tenant_id: str
+        Reference id for tenant
+    iri: str
+        IRI of the ontology object
+    icon: str
+        Icon assigned to object, visually representing it
+    labels: list[Label]
+        List of multi-language_code labels
+    comments: list[Label]
+        List of multi-language_code comments
+    context: str
+        Context
+    """
+
+    def __init__(self, tenant_id: str, iri: str, icon: str, labels: list[OntologyLabel],
+                 comments: list[Comment], context: str):
+        self.__tenant_id: str = tenant_id
+        self.__labels: list[OntologyLabel] = labels
+        self.__comments: list[Comment] = comments
+        self.__iri: str = iri
+        self.__icon: str = icon
+        self.__context: str = context
+
+    @property
+    def tenant_id(self) -> str:
+        """Tenant id."""
+        return self.__tenant_id
+
+    @property
+    def iri(self) -> str:
+        """IRI """
+        return self.__iri
+
+    @property
+    def context(self) -> str:
+        """Context."""
+        return self.__context
+
+    @property
+    def icon(self) -> str:
+        """Icon."""
+        return self.__icon
+
+    @icon.setter
+    def icon(self, value: str):
+        self.__icon = value
+
+    @property
+    def labels(self) -> list[OntologyLabel]:
+        """Labels related to ontology object."""
+        return self.__labels
+
+    def label_for_lang(self, language_code: LanguageCode) -> Optional[OntologyLabel]:
+        """
+        Get label for language_code.
+        Parameters
+        ----------
+        language_code: LanguageCode
+            Language code
+
+        Returns
+        -------
+        label: Optional[OntologyLabel]
+            Label for language_code
+        """
+        for label in self.labels:
+            if label.language_code == language_code:
+                return label
+        return None
+
+    @property
+    def comments(self) -> list[Comment]:
+        """Comment related to ontology object."""
+        return self.__comments
+
+    def comment_for_lang(self, language_code: LanguageCode) -> Optional[Comment]:
+        """
+        Get comment for language_code.
+        Parameters
+        ----------
+        language_code: LanguageCode
+            Language code
+
+        Returns
+        -------
+        comment: Optional[Comment]
+            Comment for language_code
+        """
+        for comment in self.comments:
+            if comment.language_code == language_code:
+                return comment
+        return None
+
+
+class OntologyContextSettings:
+    """
+    OntologyContextSettings
+    -----------------------
+    Describes the settings of the context, such as:
+    - prefixes for RDF, RDFS and OWL
+    - Base literal URI
+    - Base class URI
+    - Description literal name
+    - depth
+    """
+
+    def __init__(self, rdf_prefix: str, rdfs_prefix: str, owl_prefix: str, base_literal_uri: str, base_class_uri: str,
+                 description_literal_name: str, depth: int):
+        self.__rdf_prefix: str = rdf_prefix
+        self.__rdfs_prefix: str = rdfs_prefix
+        self.__owl_prefix: str = owl_prefix
+        self.__base_literal_uri: str = base_literal_uri
+        self.__base_class_uri: str = base_class_uri
+        self.__description_literal_name: str = description_literal_name
+        self.__depth: int = depth
+
+    @property
+    def rdf_prefix(self):
+        """RDF prefix"""
+        return self.__rdf_prefix
+
+    @property
+    def rdfs_prefix(self):
+        """RDFS prefix"""
+        return self.__rdfs_prefix
+
+    @property
+    def owl_prefix(self):
+        """OWL prefix"""
+        return self.__owl_prefix
+
+    @property
+    def base_literal_uri(self):
+        """Base literal URI."""
+        return self.__base_literal_uri
+
+    @property
+    def base_class_uri(self):
+        """Base class URI."""
+        return self.__base_class_uri
+
+    @property
+    def description_literal_name(self) -> str:
+        """Literal name of the description."""
+        return self.__description_literal_name
+
+    @property
+    def depth(self) -> int:
+        """Depth."""
+        return self.__depth
+
+
+class OntologyContext(OntologyObject):
+    """
+    OntologyContext
+    ----------------
+    Ontology context representation.
+
+    Parameters
+    ----------
+    cid: str
+        Context id
+    tenant_id: str
+        Tenant id.
+    name: str
+        Name of the ontology context
+    icon: str
+        Icon or Base64 encoded
+    labels: list[Label]
+        List of labels
+    comments: list[Comment]
+        List of comments
+    context: str
+        context name
+    base_uri: str
+        Base URI
+    concepts: list[str]
+        List of classes / concepts
+    properties: list[str]
+        List of properties (data and object properties)
+    """
+
+    def __init__(self, cid: str, tenant_id: str, name: str, icon: str, labels: list[OntologyLabel],
+                 comments: list[Comment], date_added: datetime, date_modified: datetime, context: str, base_uri: str,
+                 version: int, orphaned: bool, concepts: list[str], properties: list[str]):
+        self.__id = cid
+        self.__base_uri: str = base_uri
+        self.__version: int = version
+        self.__date_added: datetime = date_added
+        self.__date_modified: datetime = date_modified
+        self.__orphaned: bool = orphaned
+        self.__concepts: list[str] = concepts
+        self.__properties: list[str] = properties
+        super().__init__(tenant_id, name, icon, labels, comments, context)
+
+    @property
+    def id(self) -> str:
+        """Context id."""
+        return self.__id
+
+    @property
+    def base_uri(self) -> str:
+        """Base URI."""
+        return self.__base_uri
+
+    @property
+    def orphaned(self) -> bool:
+        """Orphaned."""
+        return self.__orphaned
+
+    @property
+    def version(self) -> int:
+        """Version."""
+        return self.__version
+
+    @property
+    def date_added(self) -> datetime:
+        """Date added."""
+        return self.__date_added
+
+    @property
+    def date_modified(self) -> datetime:
+        """Date modified."""
+        return self.__date_modified
+
+    @property
+    def concepts(self) -> list[str]:
+        """List of concepts."""
+        return self.__concepts
+
+    @property
+    def properties(self) -> list[str]:
+        """List of properties."""
+        return self.__properties
+
+    @classmethod
+    def from_dict(cls, context_dict: dict[str, Any]):
+        """
+        Create OntologyContext from dictionary.
+
+        Parameters
+        ----------
+        context_dict: dict[str, Any]
+            Dictionary containing the context data.
+
+        Returns
+        -------
+        instance: OntologyContext
+            Instance of OntologyContext object.
+        """
+        context_data: dict[str, Any] = context_dict['context']
+        labels: list[OntologyLabel] = [] if context_data['labels'] is None else \
+            [Label(content=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in context_data['labels']]
+        comments: list[Comment] = [] if context_data['comments'] is None else \
+            [Comment(text=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in context_data['comments']]
+        added: datetime = dateutil.parser.isoparse(context_data['dateAdded'])
+        modified: datetime = dateutil.parser.isoparse(context_data['dateModified'])
+        return OntologyContext(context_data['id'], context_data['tenantId'], context_data['name'],
+                               context_data['icon'], labels, comments, added, modified,
+                               context_data['context'], context_data['baseURI'],
+                               context_dict['version'], context_data['orphaned'],
+                               context_dict.get('concepts'), context_dict.get('properties'))
+
+    def __repr__(self):
+        return f'<OntologyContext> - [id:={self.id}, iri:={self.iri}]'
+
+
 class OntologyClass(OntologyObject):
     """
     OntologyClass
     ----------------
     Concept for ontology.
 
     Parameters
@@ -276,26 +737,26 @@
         Tenant id for ontology
     context: str
         Context
     reference: OntologyClassReference
         Reference for ontology class
     icon: str
         Icon representing concept
-    labels: List[Label]
+    labels: list[Label]
         List of labels
-    comments: List[Comment]
+    comments: list[Comment]
         List of comments
 
     subclass_of: str (default: None)
         Subclass of ontology class
     """
 
     def __init__(self, tenant_id: str, context: str, reference: OntologyClassReference,
                  subclass_of: OntologyClassReference = None, icon: Optional[str] = None,
-                 labels: Optional[List[OntologyLabel]] = None, comments: Optional[List[Comment]] = None):
+                 labels: Optional[list[OntologyLabel]] = None, comments: Optional[list[Comment]] = None):
         self.__subclass_of: OntologyClassReference = subclass_of
         self.__reference: OntologyClassReference = reference
         super().__init__(tenant_id, reference.iri, icon, labels, comments, context)
 
     @property
     def subclass_of(self) -> Optional[OntologyClassReference]:
         """
@@ -310,26 +771,46 @@
         """
         return self.__reference
 
     def __repr__(self):
         return f'<OntologyClass> - [reference:={self.reference}, subclass_of:={self.subclass_of}]'
 
     @classmethod
-    def from_dict(cls, concept_dict: Dict[str, Any]):
-        labels: List[OntologyLabel] = [] if concept_dict[LABELS_TAG] is None else \
+    def from_dict(cls, concept_dict: dict[str, Any]):
+        """Create OntologyClass from dictionary.
+
+        Parameters
+        ----------
+        concept_dict: dict[str, Any]
+            Dictionary containing the concept data.
+
+        Returns
+        -------
+        instance: OntologyClass
+            Instance of OntologyClass object.
+        """
+        labels: list[OntologyLabel] = [] if concept_dict[LABELS_TAG] is None else \
             [OntologyLabel(content=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in concept_dict[LABELS_TAG]]
-        comments: List[Comment] = [] if concept_dict[COMMENTS_TAG] is None else \
+        comments: list[Comment] = [] if concept_dict[COMMENTS_TAG] is None else \
             [Comment(text=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in concept_dict[COMMENTS_TAG]]
         return OntologyClass(tenant_id=concept_dict[TENANT_ID], context=concept_dict['context'],
                              reference=OntologyClassReference.parse(concept_dict[NAME_TAG]),
                              subclass_of=OntologyClassReference.parse(concept_dict[SUB_CLASS_OF_TAG]),
                              icon=concept_dict['icon'], labels=labels, comments=comments)
 
     @classmethod
     def new(cls) -> 'OntologyClass':
+        """
+        Create new ontology class.
+
+        Returns
+        -------
+        instance: OntologyClass
+            New ontology class.
+        """
         return OntologyClass('', '', THING_CLASS)
 
 
 class OntologyProperty(OntologyObject):
     """
     Ontology Property
     -----------------
@@ -347,43 +828,50 @@
         Name of property object
     icon: str
         Icon describing the property
     property_domain: OntologyClassReference
         Domain for the property
     property_range: OntologyClassReference
         Range for the property
-    labels: List[Label]
+    labels: list[Label]
         List of labels (localized)
-    comments: List[Comment],
+    comments: list[Comment],
         List of comments
-    subproperty_of: str (default: = None)
-        Subproperty
+    sub_property_of: str (default: = None)
+        Sub property of.
     inverse_property_of: str (optional)
         Inverse property
     """
 
     def __init__(self, kind: PropertyType, tenant_id: str, context: str, name: OntologyPropertyReference,
                  icon: str = None,
-                 property_domain: Optional[List[OntologyClassReference]] = None,
-                 property_range: Optional[List[Union[OntologyClassReference, DataPropertyType]]] = None,
-                 labels: Optional[List[OntologyLabel]] = None,
-                 comments: Optional[List[Comment]] = None,
-                 subproperty_of: Optional[OntologyPropertyReference] = None,
+                 property_domain: Optional[list[OntologyClassReference]] = None,
+                 property_range: Optional[list[Union[OntologyClassReference, DataPropertyType]]] = None,
+                 labels: Optional[list[OntologyLabel]] = None,
+                 comments: Optional[list[Comment]] = None,
+                 sub_property_of: Optional[OntologyPropertyReference] = None,
                  inverse_property_of: Optional[OntologyPropertyReference] = None):
         self.__kind: PropertyType = kind
-        self.__subproperty_of: OntologyPropertyReference = subproperty_of
+        self.__subproperty_of: OntologyPropertyReference = sub_property_of
         self.__inverse_property_of: OntologyPropertyReference = inverse_property_of
-        self.__domains: List[OntologyClassReference] = property_domain if property_domain else []
-        self.__ranges: List[Optional[Union[OntologyClassReference, DataPropertyType]]] = property_range \
+        self.__domains: list[OntologyClassReference] = property_domain if property_domain else []
+        self.__ranges: list[Optional[Union[OntologyClassReference, DataPropertyType]]] = property_range \
             if property_range else []
         self.__reference: OntologyPropertyReference = name
         super().__init__(tenant_id, name.iri, icon, labels, comments, context)
 
     @property
     def is_data_property(self) -> bool:
+        """Check if property is data property.
+
+        Returns
+        -------
+        is_data_property: bool
+            True if property is data property, False otherwise.
+        """
         return self.kind != PropertyType.OBJECT_PROPERTY
 
     @property
     def kind(self) -> PropertyType:
         """Kind of the property."""
         return self.__kind
 
@@ -399,58 +887,81 @@
 
     @property
     def inverse_property_of(self) -> OntologyPropertyReference:
         """Reference to the inverse property"""
         return self.__inverse_property_of
 
     @property
-    def domains(self) -> List[OntologyClassReference]:
+    def domains(self) -> list[OntologyClassReference]:
         """Domain of the property."""
         return self.__domains
 
     @property
-    def ranges(self) -> List[Union[OntologyClassReference, DataPropertyType]]:
+    def ranges(self) -> list[Union[OntologyClassReference, DataPropertyType]]:
         """Ranges of the property."""
         return self.__ranges
 
     def __repr__(self):
         return f'<OntologyProperty> - [name:= {self.iri} domain:={self.domains}, range:={self.ranges}, ' \
                f'sub-property_of:={self.subproperty_of}, type:={self.kind}]'
 
     @classmethod
-    def from_dict(cls, property_dict: Dict[str, Any]):
-        labels: List[OntologyLabel] = [] if property_dict[LABELS_TAG] is None else \
+    def from_dict(cls, property_dict: dict[str, Any]):
+        """
+        Create ontology property from dictionary.
+        Parameters
+        ----------
+        property_dict: dict[str, Any]
+            Dictionary containing property information.
+
+        Returns
+        -------
+        instance: OntologyProperty
+            Ontology property instance.
+        """
+        labels: list[OntologyLabel] = [] if property_dict[LABELS_TAG] is None else \
             [OntologyLabel.create_from_dict(la, locale_name=LANGUAGE_TAG) for la in property_dict[LABELS_TAG]]
-        comments: List[Comment] = [] if property_dict['comments'] is None else \
+        comments: list[Comment] = [] if property_dict['comments'] is None else \
             [Comment.create_from_dict(co) for co in property_dict['comments']]
         return OntologyProperty(INVERSE_PROPERTY_TYPE[property_dict['kind']],
                                 property_dict['tenantId'], property_dict['context'],
                                 OntologyPropertyReference.parse(property_dict['name']),
                                 property_dict['icon'],
                                 [OntologyClassReference.parse(domain) for domain in property_dict['domains']],
                                 [OntologyClassReference.parse(domain) for domain in property_dict['ranges']],
                                 labels, comments,
                                 OntologyPropertyReference.parse(property_dict['subPropertyOf'])
-                                if property_dict['subPropertyOf'] is not None else None,
+                                if property_dict.get('subPropertyOf') not in ['', None] else None,
                                 OntologyPropertyReference.parse(property_dict['inverseOf'])
-                                if property_dict['inverseOf'] is not None else None)
+                                if property_dict.get('inverseOf') not in ['', None] else None)
 
     @classmethod
     def new(cls, kind: PropertyType) -> 'OntologyProperty':
+        """
+        Create new ontology property.
+        Parameters
+        ----------
+        kind: PropertyType
+            Kind of property.
+
+        Returns
+        -------
+        instance: OntologyProperty
+            New ontology property.
+        """
         return OntologyProperty(kind, '', '',
                                 OntologyPropertyReference.parse('http://www.w3.org/2002/07/owl#topObjectProperty'))
 
 
 class EntityProperty(abc.ABC):
     """
     EntityProperty
     --------------
     Abstract class for the different types of properties.
     """
-    pass
 
 
 class DataProperty(EntityProperty):
     """
     DataProperty
     ------------
     Data property for entities.
@@ -492,25 +1003,37 @@
     @property
     def language_code(self) -> LanguageCode:
         """Language code of the content."""
         return self.__language_code
 
     @staticmethod
     def create_from_dict(data_property_struct: dict):
+        """
+        Create data property from dictionary.
+
+        Parameters
+        ----------
+        data_property_struct: dict
+            Dictionary containing data property information.
+
+        Returns
+        -------
+        instance: DataProperty
+            Data property instance.
+        """
         if CONTENT_TAG not in data_property_struct or \
                 LOCALE_TAG not in data_property_struct \
                 and DATA_PROPERTY_TAG not in data_property_struct:
             raise ValueError("Dict is does not contain a data_property structure.")
         data_property_type: str = data_property_struct[DATA_PROPERTY_TAG]
         data_type: DataPropertyType = DataPropertyType.STRING
         if DATA_TYPE_TAG in data_property_struct and data_property_struct[DATA_TYPE_TAG] is not None:
             if data_property_struct[DATA_TYPE_TAG] not in INVERSE_DATA_PROPERTY_TYPE_MAPPING:
                 raise ValueError(f"DataProperty data type is not supported. Type: {data_type}")
-            else:
-                data_type = INVERSE_DATA_PROPERTY_TYPE_MAPPING[data_property_struct[DATA_TYPE_TAG]]
+            data_type = INVERSE_DATA_PROPERTY_TYPE_MAPPING[data_property_struct[DATA_TYPE_TAG]]
         return DataProperty(data_property_struct[CONTENT_TAG],
                             OntologyPropertyReference.parse(data_property_type),
                             data_property_struct[LOCALE_TAG], data_type)
 
     def __dict__(self):
         return {
             CONTENT_TAG: self.value,
@@ -519,79 +1042,105 @@
             DATA_TYPE_TAG: None if self.data_type is None else self.data_type.value
         }
 
     def __repr__(self):
         return f'{self.value}@{self.language_code}<{self.data_property_type.name}>'
 
     @staticmethod
-    def create_from_list(param: List[dict]) -> List['DataProperty']:
-        DataProperty.create_from_dict(param[0])
+    def create_from_list(param: list[dict]) -> list['DataProperty']:
+        """
+        Create data property list from dictionary list.
+
+        Parameters
+        ----------
+        param: list[dict]
+            List of dictionaries containing data property information.
+
+        Returns
+        -------
+        instances: list[DataProperty]
+            List of data property instances.
+        """
         return [DataProperty.create_from_dict(p) for p in param]
 
 
 class ObjectProperty(EntityProperty):
     """
     Object Property
     ---------------
     ObjectProperty for entities.
 
     Parameter
     ---------
     relation: OntologyPropertyReference
         OntologyPropertyReference type
-    incoming: List[str] (default:= [])
+    incoming: list[str] (default:= [])
         Incoming relations
-    outgoing: List[str] (default:= [])
+    outgoing: list[str] (default:= [])
         Outgoing relations
     """
 
     def __init__(self, relation: OntologyPropertyReference,
-                 incoming: Optional[List[Union[str, 'ThingObject']]] = None,
-                 outgoing: Optional[List[Union[str, 'ThingObject']]] = None):
+                 incoming: Optional[list[Union[str, 'ThingObject']]] = None,
+                 outgoing: Optional[list[Union[str, 'ThingObject']]] = None):
         self.__relation: OntologyPropertyReference = relation
-        self.__incoming: List[Union[str, 'ThingObject']] = incoming if incoming is not None else []
-        self.__outgoing: List[Union[str, 'ThingObject']] = outgoing if outgoing is not None else []
+        self.__incoming: list[Union[str, 'ThingObject']] = incoming if incoming is not None else []
+        self.__outgoing: list[Union[str, 'ThingObject']] = outgoing if outgoing is not None else []
 
     @property
     def relation(self) -> OntologyPropertyReference:
         """Reference from the ontology."""
         return self.__relation
 
     @property
-    def incoming_relations(self) -> List[Union[str, 'ThingObject']]:
+    def incoming_relations(self) -> list[Union[str, 'ThingObject']]:
         """Incoming relation"""
         return self.__incoming
 
     @property
-    def outgoing_relations(self) -> List[Union[str, 'ThingObject']]:
+    def outgoing_relations(self) -> list[Union[str, 'ThingObject']]:
+        """Outgoing relation"""
         return self.__outgoing
 
     @staticmethod
-    def create_from_dict(relation_struct: Dict[str, Any]) -> Tuple[OntologyPropertyReference, 'ObjectProperty']:
+    def create_from_dict(relation_struct: dict[str, Any]) -> tuple[OntologyPropertyReference, 'ObjectProperty']:
+        """
+        Create object property from dictionary.
+
+        Parameters
+        ----------
+        relation_struct: dict[str, Any]
+            Dictionary containing object property information.
+
+        Returns
+        -------
+        relation_type: OntologyPropertyReference
+            OntologyPropertyReference type
+        """
         relation_type: OntologyPropertyReference = \
             OntologyPropertyReference.parse(relation_struct[RELATION_TAG])
-        incoming: List[Union[str, ThingObject]] = []
+        incoming: list[Union[str, ThingObject]] = []
 
         for incoming_relation in relation_struct[INCOMING_TAG]:
             if isinstance(incoming_relation, dict):
                 incoming.append(ThingObject.from_dict(incoming_relation))
             elif isinstance(incoming_relation, str):
                 incoming.append(incoming_relation)
 
-        outgoing: List[Union[str, ThingObject]] = []
+        outgoing: list[Union[str, ThingObject]] = []
         for outgoing_relation in relation_struct[OUTGOING_TAG]:
             if isinstance(outgoing_relation, dict):
                 outgoing.append(ThingObject.from_dict(outgoing_relation))
             elif isinstance(outgoing_relation, str):
                 outgoing.append(outgoing_relation)
         return relation_type, ObjectProperty(relation_type, incoming, outgoing)
 
     def __dict__(self):
-        outgoing_relations: List[str] = []
-        incoming_relations: List[str] = []
+        outgoing_relations: list[str] = []
+        incoming_relations: list[str] = []
         for e in self.incoming_relations:
 
             if isinstance(e, ThingObject):
                 if e.uri is not None:
                     incoming_relations.append(e.uri)
                 else:
                     incoming_relations.append(e.reference_id)
@@ -611,29 +1160,41 @@
             OUTGOING_TAG: outgoing_relations
         }
 
     def __repr__(self):
         return f'{self.relation.iri}, in:={self.incoming_relations}, out:={self.outgoing_relations}'
 
     @staticmethod
-    def create_from_list(param: List[dict]) -> Dict[OntologyPropertyReference, 'ObjectProperty']:
+    def create_from_list(param: list[dict]) -> dict[OntologyPropertyReference, 'ObjectProperty']:
+        """
+        Create object property list from dictionary list.
+        Parameters
+        ----------
+        param: list[dict]
+            List of dictionaries containing object property information.
+
+        Returns
+        -------
+        instances: dict[OntologyPropertyReference, ObjectProperty]
+            Dictionary of object property instances.
+        """
         return dict([ObjectProperty.create_from_dict(p) for p in param])
 
 
-class Ontology(object):
+class Ontology:
     """
     Ontology
     --------
     The ontology consists of classes and properties.
     """
 
     def __init__(self):
-        self.__classes: Dict[OntologyClassReference, OntologyClass] = {}
-        self.__data_properties: Dict[str, OntologyProperty] = {}
-        self.__object_properties: Dict[str, OntologyProperty] = {}
+        self.__classes: dict[OntologyClassReference, OntologyClass] = {}
+        self.__data_properties: dict[str, OntologyProperty] = {}
+        self.__object_properties: dict[str, OntologyProperty] = {}
 
     def add_class(self, class_obj: OntologyClass):
         """
         Adding class object.
 
         Parameters
         ----------
@@ -652,29 +1213,43 @@
         """
         if prop_obj.is_data_property:
             self.__data_properties[prop_obj.reference.iri] = prop_obj
         else:
             self.__object_properties[prop_obj.reference.iri] = prop_obj
 
     @property
-    def data_properties(self) -> List[OntologyProperty]:
+    def data_properties(self) -> list[OntologyProperty]:
         """All data properties."""
         return list(self.__data_properties.values())
 
     @property
-    def object_properties(self) -> List[OntologyProperty]:
+    def object_properties(self) -> list[OntologyProperty]:
         """All object properties."""
         return list(self.__object_properties.values())
 
     @property
-    def classes(self) -> List[OntologyClass]:
+    def classes(self) -> list[OntologyClass]:
         """All classes."""
         return list(self.__classes.values())
 
     def __check_hierarchy__(self, clz: OntologyClassReference, domain: OntologyClassReference) -> bool:
+        """
+        Check if class is in domain.
+        Parameters
+        ----------
+        clz: OntologyClassReference
+            Class reference
+        domain: OntologyClassReference
+            Domain reference
+
+        Returns
+        -------
+        result: bool
+            True if class is in domain.
+        """
         current_clz: Optional[OntologyClass] = self.get_class(clz)
         while current_clz is not None:
             if current_clz.reference == domain:
                 return True
             current_clz = self.get_class(current_clz.subclass_of)
         return False
 
@@ -722,52 +1297,52 @@
         Returns
         --------
         instance: Optional[OntologyProperty]
             Instance of ontology object property.
         """
         return self.__data_properties.get(property_reference.iri)
 
-    def data_properties_for(self, cls_reference: OntologyClassReference) -> List[OntologyPropertyReference]:
+    def data_properties_for(self, cls_reference: OntologyClassReference) -> list[OntologyPropertyReference]:
         """
         Retrieve a list of data properties.
 
         Parameters
         ----------
         cls_reference: OntologyClassReference
             Class of the ontology
 
         Returns
         -------
-        data_properties: List[OntologyPropertyReference]
+        data_properties: list[OntologyPropertyReference]
             List of data properties, where domain fit for the class of one of its super classes.
         """
-        data_properties: List[OntologyPropertyReference] = []
+        data_properties: list[OntologyPropertyReference] = []
         clz: Optional[OntologyClass] = self.get_class(cls_reference)
         if clz is not None:
             for dp in self.data_properties:
                 for domain in dp.domains:
                     if self.__check_hierarchy__(clz.reference, domain):
                         data_properties.append(dp.reference)
         return data_properties
 
-    def object_properties_for(self, cls_reference: OntologyClassReference) -> List[OntologyPropertyReference]:
+    def object_properties_for(self, cls_reference: OntologyClassReference) -> list[OntologyPropertyReference]:
         """
         Retrieve a list of object properties.
 
         Parameters
         ----------
         cls_reference: OntologyClassReference
             Class of the ontology
 
         Returns
         -------
-        object_properties: List[OntologyPropertyReference]
+        object_properties: list[OntologyPropertyReference]
             List of object properties, where domain fit for the class of one of its super classes.
         """
-        object_properties: List[OntologyPropertyReference] = []
+        object_properties: list[OntologyPropertyReference] = []
         clz: Optional[OntologyClass] = self.get_class(cls_reference)
         if clz is not None:
             for dp in self.object_properties:
                 for domain in dp.domains:
                     if self.__check_hierarchy__(clz.reference, domain):
                         object_properties.append(dp.reference)
         return object_properties
@@ -790,47 +1365,47 @@
     - **concept_type**: Type of the concept
     - **concept_type_info**: Information on the concept type
     - **visibility**: Visibility of the entity
     - **use_for_nel**: Use the entity for named entity linking
 
     Parameters
     ----------
-    label: List[Label]
+    label: list[Label]
         List of labels
     icon: str (optional)
         Icon
-    description: List[Description] (optional)
+    description: list[Description] (optional)
         List of descriptions
     concept_type: OntologyClassReference
         Type of the concept
     uri: str
          URI for entity. For new entities the URI is None, as the knowledge graph backend assigns this.
     tenant_rights: TenantAccessRight
         Rights for tenants
     owner: bool
         Is the logged-in user the owner of the entity
     """
 
-    def __init__(self, label: List[Label] = None, concept_type: OntologyClassReference = THING_CLASS,
-                 description: Optional[List[Description]] = None, uri: Optional[str] = None, icon: Optional[str] = None,
+    def __init__(self, label: list[Label] = None, concept_type: OntologyClassReference = THING_CLASS,
+                 description: Optional[list[Description]] = None, uri: Optional[str] = None, icon: Optional[str] = None,
                  tenant_rights: TenantAccessRight = TenantAccessRight(), owner: bool = True, use_for_nel: bool = True):
         self.__uri: str = uri
         self.__icon: Optional[str] = icon
-        self.__label: List[Label] = label if label else []
-        self.__description: List[Description] = description if description else []
-        self.__alias: List[Label] = []
+        self.__label: list[Label] = label if label else []
+        self.__description: list[Description] = description if description else []
+        self.__alias: list[Label] = []
         self.__concept_type: OntologyClassReference = concept_type
-        self.__data_properties: Dict[OntologyPropertyReference, List[DataProperty]] = {}
-        self.__object_properties: Dict[OntologyPropertyReference, ObjectProperty] = {}
+        self.__data_properties: dict[OntologyPropertyReference, list[DataProperty]] = {}
+        self.__object_properties: dict[OntologyPropertyReference, ObjectProperty] = {}
         self.__tenants_rights: TenantAccessRight = tenant_rights
         self.__status_flag: EntityStatus = EntityStatus.UNKNOWN
-        self.__ontology_types: Optional[Set[str]] = None
+        self.__ontology_types: Optional[set[str]] = None
         self.__owner: bool = owner
         self.__owner_id: Optional[str] = None
-        self.__group_ids: List[str] = []
+        self.__group_ids: list[str] = []
         self.__use_for_nel: bool = use_for_nel
         self.__visibility: Optional[str] = None
 
     @property
     def uri(self) -> str:
         """Unique identifier for entity."""
         return self.__uri
@@ -868,61 +1443,61 @@
         return self.__owner_id
 
     @owner_id.setter
     def owner_id(self, value: str):
         self.__owner_id = value
 
     @property
-    def group_ids(self) -> List[str]:
+    def group_ids(self) -> list[str]:
         """List of group ids."""
         return self.__group_ids
 
     @group_ids.setter
-    def group_ids(self, value: List[str]):
+    def group_ids(self, value: list[str]):
         self.__group_ids = value
 
     @property
     def status_flag(self) -> EntityStatus:
         """Status flag."""
         return self.__status_flag
 
     @status_flag.setter
     def status_flag(self, flag: EntityStatus):
         self.__status_flag = flag
 
     @property
-    def label(self) -> List[Label]:
+    def label(self) -> list[Label]:
         """Labels of the entity."""
         return self.__label
 
     @label.setter
-    def label(self, value: List[Label]):
+    def label(self, value: list[Label]):
         self.__label = value
 
     def add_label(self, label: str, language_code: LanguageCode):
         """Adding a label for entity.
 
         Parameters
         ----------
         label: str
             Label
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         self.__label.append(Label(label, language_code, True))
 
     def update_label(self, value: str, language_code: LanguageCode):
         """Update or creates a label for a specific language.
 
         Parameters
         ----------
         value: str
             Value to be set
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         for label in self.label:
             if label.language_code == language_code:
                 label.content = value
                 return
         # Label with language does not exist, so create a new label
         self.add_label(value, language_code)
@@ -930,15 +1505,15 @@
     def remove_label(self, language_code: LanguageCode):
         """
         Remove label for entity if it exists for language.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         for idx, label in enumerate(self.label):
             if label.language_code == language_code:
                 del self.label[idx]
                 break
 
     def remove_alias(self, label: Label):
@@ -969,21 +1544,14 @@
             Returns the label for a specific language code
         """
         for label in self.label:
             if label.language_code == language_code:
                 return label
         return None
 
-    @property
-    def source_system(self) -> Optional[List[DataProperty]]:
-        """Source of the entity."""
-        if SYSTEM_SOURCE_SYSTEM in self.__data_properties:
-            return self.__data_properties[SYSTEM_SOURCE_SYSTEM]
-        return None
-
     def add_source_system(self, value: DataProperty):
         """
         Adding the source system  of the entity.
 
         Parameters
         -----------
         value: DataProperty
@@ -997,15 +1565,15 @@
             self.__data_properties[SYSTEM_SOURCE_SYSTEM] = []
         for idx in range(0, len(self.__data_properties[SYSTEM_SOURCE_SYSTEM])):
             if self.__data_properties[SYSTEM_SOURCE_SYSTEM][idx].language_code == value.language_code:
                 del self.__data_properties[SYSTEM_SOURCE_SYSTEM][idx]
         self.__data_properties[SYSTEM_SOURCE_SYSTEM].append(value)
 
     @property
-    def source_reference_id(self) -> Optional[List[DataProperty]]:
+    def source_reference_id(self) -> Optional[list[DataProperty]]:
         """Reference id for to the source."""
         if SYSTEM_SOURCE_REFERENCE_ID in self.__data_properties:
             return self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID]
         return None
 
     def add_source_reference_id(self, value: DataProperty):
         """
@@ -1082,15 +1650,15 @@
     def default_source_reference_id(self, language_code: LanguageCode = LanguageCode('en_US')) -> Optional[str]:
         """
         Getting the source reference id for a certain language code.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
 
         Returns
         -------
         id: str
             Source reference id.
         """
         if SYSTEM_SOURCE_REFERENCE_ID in self.__data_properties:
@@ -1102,15 +1670,15 @@
     def default_source_system(self, language_code: LanguageCode = LanguageCode('en_US')) -> Optional[str]:
         """
         Getting the source system for a certain language code.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
 
         Returns
         -------
         id: str
             Source system.
         """
         if SYSTEM_SOURCE_SYSTEM in self.__data_properties:
@@ -1125,43 +1693,43 @@
         return self.__icon
 
     @image.setter
     def image(self, value: str):
         self.__icon = value
 
     @property
-    def description(self) -> Optional[List[Description]]:
+    def description(self) -> Optional[list[Description]]:
         """Description of the thing (optional)."""
         return self.__description
 
     @description.setter
-    def description(self, value: List[Description]):
+    def description(self, value: list[Description]):
         self.__description = value
 
     def add_description(self, description: str, language_code: LanguageCode):
-        """Adding an description for entity.
+        """Adding the description for entity.
 
         Parameters
         ----------
         description: str
             Description
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         self.__description.append(Description(description=description, language_code=language_code))
 
     def update_description(self, value: str, language_code: LanguageCode):
         """Update or creates a description for a specific language.
 
         Parameters
         ----------
         value: str
             Value to be set
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         for desc in self.description:
             if desc.language_code == language_code:
                 desc.content = value
                 return
         # Description with language does not exist, so create a new description
         self.add_description(value, language_code)
@@ -1169,15 +1737,15 @@
     def description_lang(self, language_code: str) -> Optional[Description]:
         """
         Get description for entity.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         Returns
         -------
         label: LocalizedContent
             Returns the  label for a specific language_code code
         """
         for desc in self.description:
             if desc.language_code == language_code:
@@ -1187,15 +1755,15 @@
     def remove_description(self, language_code: LanguageCode):
         """
         Remove description for entity if it exists for language.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         for idx in range(len(self.description)):
             if self.description[idx].language_code == language_code:
                 del self.__description[idx]
                 break
 
     @property
@@ -1204,55 +1772,55 @@
         return self.__concept_type
 
     @concept_type.setter
     def concept_type(self, value: OntologyClassReference):
         self.__concept_type = value
 
     @property
-    def ontology_types(self) -> Set[str]:
+    def ontology_types(self) -> set[str]:
         """Ontology types. For public entities."""
         return self.__ontology_types
 
     @ontology_types.setter
-    def ontology_types(self, value: Set[str]):
+    def ontology_types(self, value: set[str]):
         self.__ontology_types = value
 
     @property
-    def data_properties(self) -> Dict[OntologyPropertyReference, List[DataProperty]]:
+    def data_properties(self) -> dict[OntologyPropertyReference, list[DataProperty]]:
         """Literals of the concept."""
         return self.__data_properties
 
     @data_properties.setter
-    def data_properties(self, data_properties: Dict[OntologyPropertyReference, List[DataProperty]]):
+    def data_properties(self, data_properties: dict[OntologyPropertyReference, list[DataProperty]]):
         """Literals of the concept."""
         self.__data_properties = data_properties
 
     @property
-    def object_properties(self) -> Dict[OntologyPropertyReference, ObjectProperty]:
+    def object_properties(self) -> dict[OntologyPropertyReference, ObjectProperty]:
         """Relations of the concept."""
         return self.__object_properties
 
     @object_properties.setter
-    def object_properties(self, relations: Dict[OntologyPropertyReference, ObjectProperty]):
+    def object_properties(self, relations: dict[OntologyPropertyReference, ObjectProperty]):
         self.__object_properties = relations
 
     def data_property_lang(self, data_property: OntologyPropertyReference, language_code: LanguageCode) \
-            -> List[DataProperty]:
+            -> list[DataProperty]:
         """
         Get data property for language_code code.
 
         Parameters
         ----------
         data_property: OntologyPropertyReference
             Data property.
         language_code: LanguageCode
             Requested language_code code
         Returns
         -------
-        data_properties: List[DataProperty]
+        data_properties: list[DataProperty]
             Returns a list of data properties for a specific language code
         """
         return [d for d in self.data_properties.get(data_property, []) if d.language_code == language_code]
 
     def remove_data_property(self, data_property: OntologyPropertyReference):
         """Remove data property.
 
@@ -1260,50 +1828,50 @@
         ----------
         data_property: OntologyPropertyReference
             Data property to be removed.
         """
         self.__data_properties.pop(data_property, None)
 
     @property
-    def alias(self) -> List[Label]:
+    def alias(self) -> list[Label]:
         """Alternative labels of the concept."""
         return self.__alias
 
     @alias.setter
-    def alias(self, alias: List[Label]):
+    def alias(self, alias: list[Label]):
         self.__alias = alias
 
-    def alias_lang(self, language_code: LanguageCode) -> List[Label]:
+    def alias_lang(self, language_code: LanguageCode) -> list[Label]:
         """
         Get alias for language_code code.
 
         Parameters
         ----------
         language_code: LanguageCode
             Requested language_code code
         Returns
         -------
-        aliases: List[Label]
+        aliases: list[Label]
             Returns a list of aliases for a specific language code
         """
-        aliases: List[Label] = []
+        aliases: list[Label] = []
         for alias in self.alias:
             if alias.language_code == language_code:
                 aliases.append(alias)
         return aliases
 
     def update_alias(self, value: str, language_code: LanguageCode):
         """Update or creates an alias for a specific language.
 
         Parameters
         ----------
         value: str
             Value to be set
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         for a in self.alias:
             if a.language_code == language_code:
                 a.content = value
                 return
         # Label with language does not exist, so create a new label
         self.add_alias(value, language_code=language_code)
@@ -1338,32 +1906,32 @@
         """Adding an alias for entity.
 
         Parameters
         ----------
         alias: str
             Alias
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         self.__alias.append(Label(alias, language_code, False))
 
     @property
     def tenant_access_right(self) -> TenantAccessRight:
         """Access rights for tenant. """
         return self.__tenants_rights
 
     @tenant_access_right.setter
     def tenant_access_right(self, rights: TenantAccessRight):
         self.__tenants_rights = rights
 
     def __dict__(self):
-        labels: List[Dict[str, Any]] = []
+        labels: list[dict[str, Any]] = []
         labels.extend([la.__dict__() for la in self.label])
         labels.extend([la.__dict__() for la in self.alias])
-        dict_object: Dict[str, Any] = {
+        dict_object: dict[str, Any] = {
             URI_TAG: self.uri,
             IMAGE_TAG: self.image,
             LABELS_TAG: labels,
             DESCRIPTIONS_TAG: [desc.__dict__() for desc in self.description],
             TYPE_TAG: self.concept_type.iri,
             STATUS_FLAG_TAG: self.status_flag.value,
             DATA_PROPERTIES_TAG: {},
@@ -1374,42 +1942,114 @@
         }
         for literal_type, items in self.data_properties.items():
             dict_object[DATA_PROPERTIES_TAG][literal_type.iri] = [i.__dict__() for i in items]
         for relation_type, item in self.object_properties.items():
             dict_object[OBJECT_PROPERTIES_TAG][relation_type.iri] = item.__dict__()
         return dict_object
 
-    def __import_format_dict__(self, group_ids: List[Dict[str, str]] = None):
-        labels: List[Dict[str, Any]] = []
+    def __import_format_dict__(self, group_ids: list[dict[str, str]] = None):
+        labels: list[dict[str, Any]] = []
         labels.extend([la.__dict__() for la in self.label])
         labels.extend([la.__dict__() for la in self.alias])
-        dict_object: Dict[str, Any] = {
+        dict_object: dict[str, Any] = {
             SOURCE_REFERENCE_ID_TAG: self.reference_id,
             SOURCE_SYSTEM_TAG: self.source_system,
             IMAGE_TAG: self.image,
             LABELS_TAG: labels,
             DESCRIPTIONS_TAG: [desc.__dict__() for desc in self.description],
             TYPE_TAG: self.concept_type.iri,
             DATA_PROPERTIES_TAG: [],
             OBJECT_PROPERTIES_TAG: [],
             TENANT_RIGHTS_TAG: self.tenant_access_right.to_list(),
             GROUP_IDS: group_ids if group_ids else [],
             SEND_TO_NEL_TAG: self.use_for_nel
         }
-        for literal_type, items in self.data_properties.items():
+        for _, items in self.data_properties.items():
             dict_object[DATA_PROPERTIES_TAG].extend([i.__dict__() for i in items])
-        for relation_type, item in self.object_properties.items():
+        for _, item in self.object_properties.items():
             dict_object[OBJECT_PROPERTIES_TAG].append(item.__dict__())
         return dict_object
 
     @staticmethod
-    def from_dict(entity: Dict[str, Any]) -> 'ThingObject':
-        labels: List[Label] = []
-        alias: List[Label] = []
-        descriptions: List[Description] = []
+    def from_import_dict(entity: dict[str, Any]) -> 'ThingObject':
+        """Creates a ThingObject from a dict.
+
+        Parameters
+        ----------
+        entity: dict[str, Any]
+            Dictionary that contains the data of the entity
+
+        Returns
+        -------
+        instance: ThingObject
+            ThingObject that is created from the dict
+        """
+        labels: list[Label] = []
+        alias: list[Label] = []
+        descriptions: list[Description] = []
+
+        for label in entity[LABELS_TAG]:
+            if label[LOCALE_TAG] in SUPPORTED_LOCALES:
+                if label[IS_MAIN_TAG]:
+                    labels.append(Label.create_from_dict(label))
+                else:
+                    alias.append(Label.create_from_dict(label))
+
+        for desc in entity[DESCRIPTIONS_TAG]:
+            if desc[LOCALE_TAG] in SUPPORTED_LOCALES:
+                descriptions.append(Description.create_from_dict(desc))
+
+        use_nel: bool = entity.get(USE_NEL_TAG, True)
+
+        thing: ThingObject = ThingObject(label=labels, icon=entity[IMAGE_TAG], description=descriptions,
+                                         concept_type=OntologyClassReference.parse(entity[TYPE_TAG]),
+                                         use_for_nel=use_nel)
+        if DATA_PROPERTIES_TAG in entity:
+            if isinstance(entity[DATA_PROPERTIES_TAG], dict):
+                for data_property_type_str, data_properties in entity[DATA_PROPERTIES_TAG].items():
+                    data_property_type: OntologyPropertyReference = \
+                        OntologyPropertyReference.parse(data_property_type_str)
+                    for data_property in data_properties:
+                        language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
+                        value: str = data_property[VALUE_TAG]
+                        thing.add_data_property(DataProperty(value, data_property_type, language_code))
+            elif isinstance(entity[DATA_PROPERTIES_TAG], list):
+                for data_property in entity[DATA_PROPERTIES_TAG]:
+                    language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
+                    value: str = data_property[VALUE_TAG]
+                    data_property_type: OntologyPropertyReference = \
+                        OntologyPropertyReference.parse(data_property[DATA_PROPERTY_TAG])
+                    thing.add_data_property(DataProperty(value, data_property_type, language_code))
+        if OBJECT_PROPERTIES_TAG in entity:
+            for object_property in entity[OBJECT_PROPERTIES_TAG]:
+                _, obj = ObjectProperty.create_from_dict(object_property)
+                thing.add_relation(obj)
+        thing.alias = alias
+        # Finally, retrieve rights
+        if TENANT_RIGHTS_TAG in entity:
+            thing.tenant_access_right = TenantAccessRight.parse(entity[TENANT_RIGHTS_TAG])
+        return thing
+
+    @staticmethod
+    def from_dict(entity: dict[str, Any]) -> 'ThingObject':
+        """Creates a ThingObject from a dict.
+
+        Parameters
+        ----------
+        entity: dict[str, Any]
+            Dictionary that contains the data of the entity
+
+        Returns
+        -------
+        instance: ThingObject
+            ThingObject that is created from the dict
+        """
+        labels: list[Label] = []
+        alias: list[Label] = []
+        descriptions: list[Description] = []
 
         for label in entity[LABELS_TAG]:
             if label[LOCALE_TAG] in SUPPORTED_LOCALES:
                 if label[IS_MAIN_TAG]:
                     labels.append(Label.create_from_dict(label))
                 else:
                     alias.append(Label.create_from_dict(label))
@@ -1440,35 +2080,35 @@
                     language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
                     value: str = data_property[VALUE_TAG]
                     data_property_type: OntologyPropertyReference = \
                         OntologyPropertyReference.parse(data_property[DATA_PROPERTY_TAG])
                     thing.add_data_property(DataProperty(value, data_property_type, language_code))
         if OBJECT_PROPERTIES_TAG in entity:
             for object_property in entity[OBJECT_PROPERTIES_TAG].values():
-                prop, obj = ObjectProperty.create_from_dict(object_property)
+                _, obj = ObjectProperty.create_from_dict(object_property)
                 thing.add_relation(obj)
         thing.alias = alias
         # Finally, retrieve rights
         if TENANT_RIGHTS_TAG in entity:
             thing.tenant_access_right = TenantAccessRight.parse(entity[TENANT_RIGHTS_TAG])
         return thing
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         return self.__dict__()
 
-    def __setstate__(self, state: Dict[str, Any]):
-        self.__label: List[Label] = []
-        self.__description: List[Description] = []
-        self.__alias: List[Label] = []
-        self.__data_properties: Dict[OntologyPropertyReference, List[DataProperty]] = {}
-        self.__object_properties: Dict[OntologyPropertyReference, ObjectProperty] = {}
+    def __setstate__(self, state: dict[str, Any]):
+        self.__label: list[Label] = []
+        self.__description: list[Description] = []
+        self.__alias: list[Label] = []
+        self.__data_properties: dict[OntologyPropertyReference, list[DataProperty]] = {}
+        self.__object_properties: dict[OntologyPropertyReference, ObjectProperty] = {}
         self.__status_flag: EntityStatus = EntityStatus.UNKNOWN
-        self.__ontology_types: Optional[Set[str]] = None
+        self.__ontology_types: Optional[set[str]] = None
         self.__owner_id: Optional[str] = None
-        self.__group_ids: List[str] = []
+        self.__group_ids: list[str] = []
         self.__visibility: Optional[str] = None
 
         for label in state[LABELS_TAG]:
             if label[LOCALE_TAG] in SUPPORTED_LOCALES:
                 if label[IS_MAIN_TAG]:
                     self.__label.append(Label.create_from_dict(label))
                 else:
@@ -1501,15 +2141,15 @@
                     language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
                     value: str = data_property[VALUE_TAG]
                     data_property_type: OntologyPropertyReference = \
                         OntologyPropertyReference.parse(data_property[DATA_PROPERTY_TAG])
                     self.add_data_property(DataProperty(value, data_property_type, language_code))
         if OBJECT_PROPERTIES_TAG in state:
             for object_property in state[OBJECT_PROPERTIES_TAG].values():
-                prop, obj = ObjectProperty.create_from_dict(object_property)
+                _, obj = ObjectProperty.create_from_dict(object_property)
                 self.add_relation(obj)
         # Finally, retrieve rights
         if TENANT_RIGHTS_TAG in state:
             self.tenant_access_right = TenantAccessRight.parse(state[TENANT_RIGHTS_TAG])
 
     def __hash__(self):
         return 0
@@ -1557,29 +2197,46 @@
 
     @property
     def case_sensitive(self) -> bool:
         """Are entity labels of the class treated case-sensitive."""
         return self.__case_sensitive
 
     @staticmethod
-    def from_dict(entity: Dict[str, Any]) -> 'InflectionSetting':
+    def from_dict(entity: dict[str, Any]) -> 'InflectionSetting':
+        """
+        Create inflection setting from dictionary.
+        Parameters
+        ----------
+        entity: dict[str, Any]
+            Entity dictionary
+
+        Returns
+        -------
+        instance: InflectionSetting
+            Inflection setting instance
+        """
         concept_class: str = ''
         inflection_setting: str = ''
         case_sensitive: bool = False
         if INFLECTION_CONCEPT_CLASS in entity:
             concept_class = entity[INFLECTION_CONCEPT_CLASS]
         if INFLECTION_SETTING in entity:
             inflection_setting = entity[INFLECTION_SETTING]
         if INFLECTION_CASE_SENSITIVE in entity:
             case_sensitive = entity[INFLECTION_CASE_SENSITIVE]
         return InflectionSetting(concept=concept_class, inflection=inflection_setting, case_sensitive=case_sensitive)
 
 
 # -------------------------------------------------- Encoder -----------------------------------------------------------
 class ThingEncoder(JSONEncoder):
+    """
+    Thing encoder
+    -------------
+    Encoder for ThingObject, Label and Description objects.
+    """
     def default(self, o):
         if isinstance(o, Label):
             return o.__dict__()
         elif isinstance(o, Description):
             return o.__dict__()
         elif isinstance(o, ThingObject):
             return o.__dict__()
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/nel/base.py` & `personal_knowledge_library-1.0.0/knowledge/nel/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 import abc
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
 
 from knowledge.base.entity import LanguageCode
 from knowledge.base.ontology import THING_CLASS, OntologyClassReference
 from knowledge.services.base import WacomServiceAPIClient, RESTAPIClient
 
 
 class EntityType(Enum):
@@ -37,26 +37,26 @@
     """Wacom Personal Knowledge"""
 
 
 class BasicType(Enum):
     """
     Basic type
     ----------
-    Basic type of entities.
+    Basic type of entities use for instance in named entity recognition.
     """
     UNKNOWN = 'Unknown'
     MONEY = 'Money'
     PERSON = 'Person'
     DATE = 'Date'
     PLACE = 'Place'
     TIME = 'Time'
     NUMBER = 'Number'
 
 
-class EntitySource(object):
+class EntitySource:
     """
     EntitySource
     ------------
     Source of the entity.
 
     Parameters
     ----------
@@ -151,31 +151,31 @@
         Main label of the entity.
     confidence: float
         Confidence value if available
     source: EntitySource
         Source of the entity
     content_link: str
         Link to side with content
-    ontology_types: List[str]
+    ontology_types: list[str]
         List of ontology types (class names)
     entity_type: EntityType
         Type of the entity.
     """
 
     def __init__(self, ref_text: str, start_idx: int, end_idx: int, label: str, confidence: float,
                  source: EntitySource, content_link: str,
-                 ontology_types: List[str], entity_type: EntityType = EntityType.PUBLIC_ENTITY):
+                 ontology_types: list[str], entity_type: EntityType = EntityType.PUBLIC_ENTITY):
         super().__init__(ref_text, start_idx, end_idx, entity_type)
         self.__source: EntitySource = source
         self.__content_link: str = content_link
         self.__label: str = label
         self.__confidence: float = confidence
         self.__description: Optional[str] = None
         self.__thumbnail: Optional[str] = None
-        self.__ontology_types: List[str] = ontology_types
+        self.__ontology_types: list[str] = ontology_types
         self.__relevant_type: OntologyClassReference = THING_CLASS
 
     @property
     def entity_source(self) -> EntitySource:
         """Source of the entity."""
         return self.__source
 
@@ -213,15 +213,15 @@
 
     @property
     def content_link(self) -> str:
         """Link to content page."""
         return self.__content_link
 
     @property
-    def ontology_types(self) -> List[str]:
+    def ontology_types(self) -> list[str]:
         """List of ontology types."""
         return self.__ontology_types
 
     @property
     def relevant_type(self) -> OntologyClassReference:
         """"Most relevant ontology type. That likes to Wacom's personal knowledge base ontology."""
         return self.__relevant_type
@@ -271,28 +271,28 @@
     ------------------------------
     Service that links entities to a entities in a personal knowledge graph.
 
     Parameters
     ----------
     service_url: str
         URL where the service has been deployed
-    supported_languages: List[str] = None
+    supported_languages: list[str] = None
         List of supported languages
     verify_calls: bool (default:=False)
         Verifies all HTTPS calls and the associated certificate.
     """
 
-    def __init__(self, service_url: str = str, supported_languages: List[str] = None, verify_calls: bool = True):
+    def __init__(self, service_url: str = str, supported_languages: list[str] = None, verify_calls: bool = True):
         super().__init__(application_name="Personal entity linking", service_url=service_url,
                          service_endpoint='graph/v1', verify_calls=verify_calls)
-        self.__supported_languages: List[str] = supported_languages if supported_languages else []
+        self.__supported_languages: list[str] = supported_languages if supported_languages else []
 
     @abc.abstractmethod
     def link_personal_entities(self, auth_key: str, text: str, language_code: LanguageCode = 'en_US') \
-            -> List[KnowledgeGraphEntity]:
+            -> list[KnowledgeGraphEntity]:
         """
         Performs Named Entity Linking on a text. It only finds entities which are accessible by the user identified by
         the auth key.
 
         Parameters
         ----------
         auth_key: str
@@ -300,21 +300,21 @@
         text: str
             Text where the entities shall be tagged in.
         language_code: LanguageCode
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
 
         Returns
         -------
-        entities: List[KnowledgeGraphEntity]
+        entities: list[KnowledgeGraphEntity]
             List of knowledge graph entities.
         """
-        raise NotImplemented
+        raise NotImplementedError
 
     @property
-    def supported_language(self) -> List[str]:
+    def supported_language(self) -> list[str]:
         """List of supported languages."""
         return self.__supported_languages
 
     def is_language_supported(self, language_code: LanguageCode) -> bool:
         """Is the language_code code supported by the engine.
 
         Parameters
@@ -339,47 +339,47 @@
     -------------------------------
     Service that recognizes entities.
 
     Parameters
     ----------
     service_url: str
         URL where the service has been deployed
-    supported_languages: List[str] = None
+    supported_languages: list[str] = None
         List of supported languages
     verify_calls: bool (default:=False)
         Verifies all HTTPS calls and the associated certificate.
     """
 
-    def __init__(self, service_url: str, supported_languages: List[LanguageCode] = None,
+    def __init__(self, service_url: str, supported_languages: list[LanguageCode] = None,
                  verify_calls: bool = False):
         super().__init__(application_name='Named Entity Linking', service_url=service_url, service_endpoint="graph",
                          verify_calls=verify_calls)
-        self.__supported_languages: List[LanguageCode] = supported_languages if supported_languages else []
+        self.__supported_languages: list[LanguageCode] = supported_languages if supported_languages else []
 
     @abc.abstractmethod
-    def named_entities(self, text: str, language_code: LanguageCode = 'en_US') -> List[NamedEntity]:
+    def named_entities(self, text: str, language_code: LanguageCode = 'en_US') -> list[NamedEntity]:
         """
         Performs Named Entity Recognition on a text.
 
         Parameters
         ----------
         text: str
             Text where the entities shall be tagged in.
         language_code: LanguageCode
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
 
         Returns
         -------
-        entities: List[NamedEntity]
+        entities: list[NamedEntity]
             List of knowledge named entities.
         """
-        raise NotImplemented
+        raise NotImplementedError
 
     @property
-    def supported_language(self) -> List[LanguageCode]:
+    def supported_language(self) -> list[LanguageCode]:
         """List of supported languages."""
         return self.__supported_languages
 
     def is_language_supported(self, language_code: LanguageCode) -> bool:
         """Is the language_code code supported by the engine.
 
         Parameters
@@ -404,45 +404,45 @@
     ---------------------
     Service that links entities to a public entities in a knowledge graph.
 
     Parameters
     ----------
     service_url: str
         URL where the service has been deployed
-    supported_languages: List[str] = None
+    supported_languages: list[str] = None
         List of supported languages
     verify_calls: bool (default:=False)
         Verifies all HTTPS calls and the associated certificate.
     """
 
-    def __init__(self, service_url: str = str, supported_languages: List[str] = None, verify_calls: bool = False):
+    def __init__(self, service_url: str = str, supported_languages: list[str] = None, verify_calls: bool = False):
         super().__init__(service_url=service_url, verify_calls=verify_calls)
-        self.__supported_languages: List[str] = supported_languages if supported_languages else []
+        self.__supported_languages: list[str] = supported_languages if supported_languages else []
 
     @abc.abstractmethod
-    def link_public_entities(self, text: str, language_code: LanguageCode = 'en_US') -> List[KnowledgeGraphEntity]:
+    def link_public_entities(self, text: str, language_code: LanguageCode = 'en_US') -> list[KnowledgeGraphEntity]:
         """
         Performs Named Entity Linking on a text. It only finds entities within a large public knowledge graph.
 
         Parameters
         ----------
         text: str
             Text where the entities shall be tagged in.
         language_code: LanguageCode
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
 
         Returns
         -------
-        entities: List[KnowledgeGraphEntity]
+        entities: list[KnowledgeGraphEntity]
             List of knowledge public knowledge entities.
         """
-        raise NotImplemented
+        raise NotImplementedError
 
     @property
-    def supported_language(self) -> List[str]:
+    def supported_language(self) -> list[str]:
         """List of supported languages."""
         return self.__supported_languages
 
     def is_language_supported(self, language_code: str) -> bool:
         """
         Is the language_code code supported by the engine.
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.0/knowledge/nel/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
-from typing import List, Optional, Dict
+# Copyright © 2021-2023 Wacom. All rights reserved.
+from typing import Optional
 
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter, Retry
 
 from knowledge.base.entity import LOCALE_TAG, LanguageCode, TEXT_TAG
 from knowledge.base.ontology import OntologyClassReference
@@ -23,91 +23,92 @@
     Parameter
     ---------
     service_url: str
         URL of the service
     """
     SERVICE_ENDPOINT: str = 'graph/v1/nel/text'
     SERVICE_URL: str = 'https://private-knowledge.wacom.com'
-    LANGUAGES: List[LanguageCode] = [
+    LANGUAGES: list[LanguageCode] = [
         LanguageCode('de_DE'),
         LanguageCode('en_US'),
         LanguageCode('ja_JP')
     ]
 
     def __init__(self, service_url: str = SERVICE_URL, service_endpoint: str = SERVICE_ENDPOINT):
         self.__service_endpoint: str = service_endpoint
         super().__init__(supported_languages=WacomEntityLinkingEngine.LANGUAGES, service_url=service_url)
 
-    def link_personal_entities(self, auth_key: str, text: str, locale: str = 'en_US', max_retries: int = 5) \
-            -> List[KnowledgeGraphEntity]:
+    def link_personal_entities(self, auth_key: str, text: str, language_code: LanguageCode = 'en_US',
+                               max_retries: int = 5) -> list[KnowledgeGraphEntity]:
         """
         Performs Named Entity Linking on a text. It only finds entities which are accessible by the user identified by
         the auth key.
 
         Parameters
         ----------
         auth_key: str
             Auth key identifying a user within the Wacom personal knowledge service.
         text: str
             Text where the entities shall be tagged in.
-        locale: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., en_US.
+        language_code: LanguageCode
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         max_retries: int
             Maximum number of retries, if the service is not available.
 
         Returns
         -------
-        entities: List[KnowledgeGraphEntity]
+        entities: list[KnowledgeGraphEntity]
             List of knowledge graph entities.
 
         Raises
         ------
         WacomServiceException
             If the Named Entity Linking service returns an error code.
         """
-        named_entities: List[KnowledgeGraphEntity] = []
+        named_entities: list[KnowledgeGraphEntity] = []
         url: str = f'{self.service_url}/{self.__service_endpoint}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
-        payload: Dict[str, str] = {
-            LOCALE_TAG: locale,
+        payload: dict[str, str] = {
+            LOCALE_TAG: language_code,
             TEXT_TAG: text
         }
         # Define the retry policy
         retry_policy: Retry = Retry(
             total=max_retries,  # maximum number of retries
             backoff_factor=0.5,  # factor by which to multiply the delay between retries
             status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
-            method_whitelist=["POST"],  # HTTP methods to retry on
             respect_retry_after_header=True  # respect the Retry-After header
         )
 
         # Create a session and mount the retry adapter
         with requests.Session() as session:
             retry_adapter = HTTPAdapter(max_retries=retry_policy)
             session.mount("https://", retry_adapter)
             response: Response = session.post(url, headers=headers, json=payload, verify=self.verify_calls)
             if response.ok:
                 results: dict = response.json()
                 for e in results:
-                    entity_types: List[str] = []
+                    entity_types: list[str] = []
                     # --------------------------- Entity content -------------------------------------------------------
                     source: Optional[EntitySource] = None
                     if 'uri' in e:
                         source = EntitySource(e['uri'], KnowledgeSource.WACOM_KNOWLEDGE)
                     # --------------------------- Ontology types -------------------------------------------------------
                     if 'type' in e:
                         entity_types.append(e['type'])
                     # --------------------------------------------------------------------------------------------------
-                    ne: KnowledgeGraphEntity = KnowledgeGraphEntity(ref_text=text[e['startPosition']:e['endPosition'] + 1],
-                                                                    start_idx=e['startPosition'], end_idx=e['endPosition'],
+                    start: int = e['startPosition']
+                    end: int = e['endPosition']
+                    ne: KnowledgeGraphEntity = KnowledgeGraphEntity(ref_text=text[start:end + 1],
+                                                                    start_idx=start, end_idx=end,
                                                                     label=e['value'], confidence=0.,
                                                                     source=source, content_link='',
                                                                     ontology_types=entity_types,
                                                                     entity_type=EntityType.PERSONAL_ENTITY)
                     ne.relevant_type = OntologyClassReference.parse(e['type'])
                     named_entities.append(ne)
                 return named_entities
-        raise WacomServiceException(f'Named entity linking for text:={text}@{locale}. '
+        raise WacomServiceException(f'Named entity linking for text:={text}@{language_code}. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.0/knowledge/ontomapping/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
 import enum
 import json
+from datetime import datetime
 from pathlib import Path
 from typing import Dict, Any, List, Optional
 
 from rdflib import Graph, RDFS, URIRef
 
-from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference
+from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, DataPropertyType
 from knowledge.public.wikidata import WikidataClass
 
 # Classes
 TOPIC_CLASS: str = 'wacom:core#Topic'
 IS_RELATED: OntologyPropertyReference = OntologyPropertyReference.parse("wacom:core#isRelated")
 # Constants
 DBPEDIA_TYPES: str = "dbpedia_types"
@@ -23,70 +24,103 @@
 CONTEXT_NAME: str = 'core'
 CWD: Path = Path(__file__).parent
 CONFIGURATION_FILE: Path = CWD / '../../pkl-cache/ontology_mapping.json'
 TAXONOMY_FILE: Path = CWD / '../../pkl-cache/taxonomy_cache.json'
 ontology_graph: Graph = Graph()
 
 
-def subclasses_of(iri: str) -> List[str]:
-    global ontology_graph
-    sub_classes: List[str] = [str(s) for s, p, o in ontology_graph.triples((None, RDFS.subClassOf, URIRef(iri)))]
+def subclasses_of(iri: str) -> list[str]:
+    """
+    Returns the subclasses of an ontology class.
+    Parameters
+    ----------
+    iri: str
+        Ontology class IRI.
+
+    Returns
+    -------
+    subclasses: list[str]
+        Subclasses of the ontology class.
+    """
+    sub_classes: list[str] = [str(s) for s, p, o in ontology_graph.triples((None, RDFS.subClassOf, URIRef(iri)))]
     for sub_class in sub_classes:
         sub_classes.extend(subclasses_of(sub_class))
     return sub_classes
 
 
+def is_iso_date(date_string: str) -> bool:
+    """
+    Checks if a date string is an ISO date.
+    Parameters
+    ----------
+    date_string: str
+        Date string.
+
+    Returns
+    -------
+    is_iso_date: bool
+        True if the date string is an ISO date, otherwise False.
+    """
+    try:
+        datetime.fromisoformat(date_string)
+        return True
+    except ValueError as _:
+        return False
+
+
 class WikidataClassEncoder(json.JSONEncoder):
     """
     Wikidata Class encoder
     ----------------------
     This class encodes a Wikidata class to JSON.
     """
     def default(self, o):
         if isinstance(o, WikidataClass):
             return o.__dict__()
         return json.JSONEncoder.default(self, o)
 
 
-class ClassConfiguration(object):
+class ClassConfiguration:
     """
     Class configuration
     -------------------
     This class contains the configuration for a class.
 
     """
     def __init__(self, ontology_class: str):
         self.__ontology_class: str = ontology_class
-        self.__wikidata_classes: List[str] = []
-        self.__dbpedia_classes: List[str] = []
+        self.__wikidata_classes: list[str] = []
+        self.__dbpedia_classes: list[str] = []
 
     @property
     def ontology_class(self) -> str:
+        """Ontology class."""
         return self.__ontology_class
 
     @property
-    def wikidata_classes(self) -> List[str]:
+    def wikidata_classes(self) -> list[str]:
         """Wikidata classes."""
         return self.__wikidata_classes
 
     @wikidata_classes.setter
-    def wikidata_classes(self, value: List[str]):
+    def wikidata_classes(self, value: list[str]):
         self.__wikidata_classes = value
 
     @property
-    def dbpedia_classes(self) -> List[str]:
+    def dbpedia_classes(self) -> list[str]:
         """DBpedia classes."""
         return self.__dbpedia_classes
 
     @dbpedia_classes.setter
-    def dbpedia_classes(self, value: List[str]):
+    def dbpedia_classes(self, value: list[str]):
         self.__dbpedia_classes = value
 
     @property
     def concept_type(self) -> OntologyClassReference:
+        """Concept type."""
         return OntologyClassReference.parse(self.__ontology_class)
 
     def __str__(self):
         return f'ClassConfiguration(ontology_class={self.__ontology_class}, ' \
                f'wikidata_classes={self.__wikidata_classes}, dbpedia_classes={self.__dbpedia_classes})'
 
 
@@ -94,37 +128,37 @@
     """
     Property type
     """
     DATA_PROPERTY = 0
     OBJECT_PROPERTY = 1
 
 
-class PropertyConfiguration(object):
+class PropertyConfiguration:
     """
     Property configuration.
     -----------------------
     This class contains the configuration for a property.
 
     Parameters
     ----------
     iri: str
         The IRI of the property.
     property_type: PropertyType
         The property type.
-    pids: Optional[List[str]]
+    pids: Optional[list[str]]
         The list of property PIDs.
     """
 
-    def __init__(self, iri: str, property_type: PropertyType, pids: Optional[List[str]] = None):
+    def __init__(self, iri: str, property_type: PropertyType, pids: Optional[list[str]] = None):
         self.__iri: str = iri
-        self.__pids: List[str] = pids if pids else []
+        self.__pids: list[str] = pids if pids else []
         self.__property: PropertyType = property_type
         self.__inverse: Optional[str] = None
-        self.__ranges: List[str] = []
-        self.__domains: List[str] = []
+        self.__ranges: list[str] = []
+        self.__domains: list[str] = []
 
     @property
     def iri(self) -> str:
         """IRI of the property."""
         return self.__iri
 
     @iri.setter
@@ -138,65 +172,67 @@
 
     @inverse.setter
     def inverse(self, value: str):
         self.__inverse = value
 
     @property
     def type(self) -> PropertyType:
+        """Property type."""
         return self.__property
 
     @property
-    def pids(self) -> List[str]:
+    def pids(self) -> list[str]:
         """List of property PIDs."""
         return self.__pids
 
     @property
-    def ranges(self) -> List[str]:
+    def ranges(self) -> list[str]:
         """List of ranges."""
         return self.__ranges
 
     @property
-    def domains(self) -> List[str]:
+    def domains(self) -> list[str]:
         """List of domains."""
         return self.__domains
 
     def __str__(self):
         return f'PropertyConfiguration(ontology_property={self.iri})'
 
 
-class MappingConfiguration(object):
+class MappingConfiguration:
     """
     Mapping configuration
     ---------------------
     This class contains the configuration for the mapping.
 
     """
 
     def __init__(self):
-        self.__classes: List[ClassConfiguration] = []
-        self.__properties: List[PropertyConfiguration] = []
-        self.__index: Dict[str, int] = {}
-        self.__index_properties: Dict[str, int] = {}
+        self.__classes: list[ClassConfiguration] = []
+        self.__properties: list[PropertyConfiguration] = []
+        self.__index: dict[str, int] = {}
+        self.__index_properties: dict[str, list[int]] = {}
+        self.__index_iri: dict[str, int] = {}
 
     @property
-    def classes(self) -> List[ClassConfiguration]:
+    def classes(self) -> list[ClassConfiguration]:
         """List of classes."""
         return self.__classes
 
     @property
-    def properties(self) -> List[PropertyConfiguration]:
+    def properties(self) -> list[PropertyConfiguration]:
         """List of properties."""
         return self.__properties
 
-    def guess_classed(self, classes: List[str]) -> Optional[ClassConfiguration]:
+    def guess_classed(self, classes: list[str]) -> Optional[ClassConfiguration]:
         """
         Guesses the class from the label.
         Parameters
         ----------
-        classes: List[str]
+        classes: list[str]
             The list of classes
 
         Returns
         -------
         class: Optional[ClassConfiguration]
             If a mapping exists, the class configuration, otherwise None.
         """
@@ -213,43 +249,43 @@
         ----------
         property_pid: str
             PID of the property
         concept_type: OntologyClassReference
             The concept type.
         Returns
         -------
-        property: Optional[PropertyConfiguration]
+        property_config: Optional[PropertyConfiguration]
             If a mapping exists, the property configuration, otherwise None.
         """
         if property_pid in self.__index_properties:
-            prop_conf: PropertyConfiguration = self.__properties[self.__index_properties[property_pid]]
-            if concept_type.iri in prop_conf.domains or 'wacom:core#Thing' in prop_conf.domains:
-                return prop_conf
+            for pid_idx in self.__index_properties[property_pid]:
+                prop_conf: PropertyConfiguration = self.__properties[pid_idx]
+                if concept_type.iri in prop_conf.domains:
+                    return prop_conf
         return None
 
     def property_for(self, class_ref: OntologyClassReference, property_type: Optional[PropertyType]) \
-            -> List[PropertyConfiguration]:
+            -> list[PropertyConfiguration]:
         """
         Returns the properties for a class.
         Parameters
         ----------
         class_ref: OntologyClassReference
             The class reference.
         property_type: Optional[PropertyType]
             The property type, if None, all properties are returned.
         Returns
         -------
-        properties: List[PropertyConfiguration]
+        properties: list[PropertyConfiguration]
             The list of properties.
         """
-        global ontology_graph
-        domain_classes: List[str] = [class_ref.iri]
+        domain_classes: list[str] = [class_ref.iri]
         domain_classes += subclasses_of(class_ref.iri)
-        domain_subclasses: Dict[str, List[str]] = {}
-        properties: List[PropertyConfiguration] = []
+        domain_subclasses: dict[str, list[str]] = {}
+        properties: list[PropertyConfiguration] = []
         for prop_conf in self.properties:
             for d in prop_conf.domains:
                 if d not in domain_subclasses:
                     domain_subclasses[d] = [d] + subclasses_of(d)
                 if class_ref.iri in domain_subclasses[d]:
                     if property_type is None or prop_conf.type == property_type:
                         properties.append(prop_conf)
@@ -277,27 +313,116 @@
         Parameters
         ----------
         property_configuration: PropertyConfiguration
             The property configuration
         """
         self.__properties.append(property_configuration)
         for pid in property_configuration.pids:
-            self.__index_properties[pid] = len(self.__properties) - 1
+            idx: int = len(self.__properties) - 1
+            if pid not in self.__index_properties:
+                self.__index_properties[pid] = []
+            self.__index_properties[pid].append(idx)
+            self.__index_iri[property_configuration.iri] = idx
+
+    def property_for_iri(self, property_iri: str) -> PropertyConfiguration:
+        """
+        Returns the property configuration for an IRI.
+
+        Parameters
+        ----------
+        property_iri: str
+            The property IRI
+
+        Returns
+        -------
+        property: PropertyConfiguration
+            The property configuration
+
+        Raises
+        ------
+        ValueError
+            If the property is not found.
+        """
+        if property_iri not in self.__index_iri:
+            raise ValueError(f'Property {property_iri} not found.')
+        return self.__properties[self.__index_iri[property_iri]]
+
+    def check_data_property_range(self, property_type: OntologyPropertyReference,
+                                  content: Optional[Any]) -> bool:
+        """
+        Checks if the content is in the range of the property.
+
+        Parameters
+        ----------
+        property_type: OntologyPropertyReference
+            The property type
+        content: Optional[Any]
+            The content
+
+        Returns
+        -------
+        evaluation: bool
+            True if the content is in the range, False otherwise.
+        """
+        if content is None:
+            return False
+        prop_config: Optional[PropertyConfiguration] = self.property_for_iri(property_type.iri)
+        if prop_config:
+            for r in prop_config.ranges:
+                if r == DataPropertyType.STRING.value:
+                    return content is not None and isinstance(content, str)
+                elif r == DataPropertyType.INTEGER.value:
+                    return content is not None and isinstance(content, int)
+                elif r == DataPropertyType.FLOAT.value:
+                    return content is not None and isinstance(content, float)
+                elif r == DataPropertyType.BOOLEAN.value:
+                    return content is not None and isinstance(content, bool)
+                elif r in {DataPropertyType.DATE.value, DataPropertyType.DATE_TIME.value}:
+                    return content is not None and isinstance(content, str) and is_iso_date(content)
+                return True
+        return False
+
+    def check_object_property_range(self, property_type: OntologyPropertyReference,
+                                    source_type: OntologyClassReference,
+                                    target_type: OntologyClassReference) -> bool:
+        """
+        Checks if the target is in the range of the property.
+        Parameters
+        ----------
+        property_type: OntologyPropertyReference
+            The property
+        source_type: OntologyClassReference
+            The concept type
+        target_type: OntologyClassReference
+            The target type
+
+        Returns
+        -------
+        valid: bool
+            True if the target is in the range, False otherwise.
+        """
+        prop_config: Optional[PropertyConfiguration] = self.property_for_iri(property_type.iri)
+        if prop_config:
+            if prop_config.type == PropertyType.OBJECT_PROPERTY:
+                if source_type.iri in prop_config.domains and target_type.iri in prop_config.ranges:
+                    return True
+                return False
+        return False
 
     def __str__(self):
         return f"Mapping Configuration(#classes={len(self.__classes)}" \
                f", #properties={len(self.__properties)})"
 
 
-def build_configuration(mapping: Dict[str, Any]) -> MappingConfiguration:
+def build_configuration(mapping: dict[str, Any]) -> MappingConfiguration:
     """
     Builds the configuration from the mapping file.
     Parameters
     ----------
-    mapping: Dict[str, Any]
+    mapping: dict[str, Any]
         The mapping file
 
     Returns
     -------
     conf: MappingConfiguration
         The mapping configuration
     """
@@ -307,59 +432,95 @@
         class_config.dbpedia_classes = c_conf[DBPEDIA_TYPES]
         class_config.wikidata_classes = c_conf[WIKIDATA_TYPES]
         conf.add_class(class_config)
     for p, p_conf in mapping['data_properties'].items():
         property_config: PropertyConfiguration = PropertyConfiguration(p, PropertyType.DATA_PROPERTY,
                                                                        p_conf['wikidata_types'])
         if 'ranges' in p_conf:
-            property_config.ranges.extend(p_conf['ranges'])
+            for ra in p_conf['ranges']:
+                property_config.ranges.append(ra)
+                property_config.ranges.extend(subclasses_of(ra))
         if 'domains' in p_conf:
-            property_config.domains.extend(p_conf['domains'])
+            for do in p_conf['domains']:
+                property_config.domains.append(do)
+                property_config.domains.extend(subclasses_of(do))
+
         conf.add_property(property_config)
     for p, p_conf in mapping['object_properties'].items():
         property_config: PropertyConfiguration = PropertyConfiguration(p, PropertyType.OBJECT_PROPERTY,
                                                                        p_conf['wikidata_types'])
         if 'ranges' in p_conf:
-            property_config.ranges.extend(p_conf['ranges'])
+            for ra in p_conf['ranges']:
+                property_config.ranges.append(ra)
+                property_config.ranges.extend(subclasses_of(ra))
         if 'domains' in p_conf:
-            property_config.domains.extend(p_conf['domains'])
+            for do in p_conf['domains']:
+                property_config.domains.append(do)
+                property_config.domains.extend(subclasses_of(do))
         if 'inverse' in p_conf:
             property_config.inverse = p_conf['inverse']
         conf.add_property(property_config)
     return conf
 
 
 def update_taxonomy_cache():
     """
     Updates the taxonomy cache.
     """
-    global taxonomy_cache
-    with open(TAXONOMY_FILE, 'w') as f:
-        f.write(json.dumps(taxonomy_cache, indent=2, cls=WikidataClassEncoder))
+    with open(TAXONOMY_FILE, 'w', encoding='uft-8') as fp_taxonomy:
+        fp_taxonomy.write(json.dumps(taxonomy_cache, indent=2, cls=WikidataClassEncoder))
 
 
 def register_ontology(rdf_str: str):
     """
     Registers the ontology.
     Parameters
     ----------
     rdf_str: str
         The ontology in RDF/XML format.
     """
-    global ontology_graph
     ontology_graph.parse(data=rdf_str, format='xml')
 
 
 # Mapping configuration
 mapping_configuration: Optional[MappingConfiguration] = None
-taxonomy_cache: Optional[Dict[str, WikidataClass]] = None
+taxonomy_cache: Optional[dict[str, WikidataClass]] = None
+
+
+def load_configuration():
+    """
+    Loads the configuration.
+
+    Raises
+    ------
+    ValueError
+        If the configuration file is not found.
+    """
+    global mapping_configuration, taxonomy_cache
+    if CONFIGURATION_FILE.exists():
+        configuration = json.loads(CONFIGURATION_FILE.open('r').read())
+        mapping_configuration = build_configuration(configuration)
+    else:
+        raise ValueError(f'Configuration file {CONFIGURATION_FILE} not found.')
+
+
+def get_mapping_configuration() -> MappingConfiguration:
+    """
+    Returns the mapping configuration.
+
+    Returns
+    -------
+    mapping_configuration: MappingConfiguration
+        The mapping configuration
+    """
+    global mapping_configuration
+    if mapping_configuration is None:
+        load_configuration()
+    return mapping_configuration
 
-if mapping_configuration is None and CONFIGURATION_FILE.exists():
-    configuration = json.loads(CONFIGURATION_FILE.open('r').read())
-    mapping_configuration = build_configuration(configuration)
 
 if taxonomy_cache is None:
     if TAXONOMY_FILE.exists():
         try:
             taxonomy = json.loads(TAXONOMY_FILE.open('r').read())
         except json.decoder.JSONDecodeError:
             taxonomy = {}
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.0/knowledge/public/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2022 Wacom. All rights reserved.
-""""Mapping of Wikidata property ids to its string."""
+# Copyright © 2022-2023 Wacom. All rights reserved.
+"""Mapping of Wikidata property ids to its string."""
 import json
 from pathlib import Path
 from typing import Dict
 
 # OntologyPropertyReference constants
 INSTANCE_OF_PROPERTY: str = 'P31'
 IMAGE_PROPERTY: str = 'P18'
 
 # Mapping for property names
-PROPERTY_MAPPING: Dict[str, str] = {}
+PROPERTY_MAPPING: dict[str, str] = {}
 
 CWD: Path = Path(__file__).parent
 CONFIGURATION_FILE: Path = CWD / '../../pkl-cache/property_cache.json'
 if CONFIGURATION_FILE.exists():
     with CONFIGURATION_FILE.open('r') as f:
         PROPERTY_MAPPING = json.load(f)
 
 from knowledge.public import wikidata
 from knowledge.public import helper
 from knowledge.public import relations
+from knowledge.public import cache
 
-__all__ = ['wikidata', 'helper', 'relations', 'PROPERTY_MAPPING', 'INSTANCE_OF_PROPERTY', 'IMAGE_PROPERTY']
+
+__all__ = ['wikidata', 'helper', 'relations', 'cache', 'PROPERTY_MAPPING', 'INSTANCE_OF_PROPERTY', 'IMAGE_PROPERTY']
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/public/helper.py` & `personal_knowledge_library-1.0.0/knowledge/public/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
 import hashlib
 import math
 import urllib
 from datetime import datetime
 from enum import Enum
-from typing import Dict, Any, List
+from typing import Any, Optional
 
-import dateutil
 import requests
-from dateutil.parser import parse
+from dateutil import parser
 from requests import Response
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from knowledge import logger
 
 
@@ -36,15 +35,14 @@
 
 class WikiDataAPIException(Exception):
     """
     WikiDataAPIException
     --------------------
     Exception thrown when accessing WikiData fails.
     """
-    pass
 
 
 # --------------------------------------- Tags -------------------------------------------------------------------------
 CLASS_TAG: str = "class"
 ALIASES_TAG: str = "aliases"
 ID_TAG: str = 'id'
 QID_TAG: str = 'qid'
@@ -88,14 +86,15 @@
 COUNTRY: str = 'P17'
 INSTANCE_OF: str = 'P31'
 IMAGE: str = 'P18'
 # URL - Wikidata
 GREGORIAN_CALENDAR_URL: str = 'http://www.wikidata.org/entity/Q1985786'
 # URL - Wikidata service
 WIKIDATA_SPARQL_URL: str = "https://query.wikidata.org/sparql"
+WIKIDATA_SEARCH_URL: str = "https://www.wikidata.org/w/api.php"
 
 
 # --------------------------------------- Helper functions -------------------------------------------------------------
 def image_url(img: str, dpi: int = 500):
     """
     Helper to generate image URL for Wikipedia.
 
@@ -122,35 +121,91 @@
         conversion: str = 'lossy-page1-'
     hash_img: str = hashlib.md5(fixed_img.encode('utf-8')).hexdigest()
     url_img_part: str = urllib.parse.quote_plus(fixed_img)
     return f'https://upload.wikimedia.org/wikipedia/commons/thumb/' \
            f'{hash_img[0]}/{hash_img[:2]}/{url_img_part}/{dpi}px-{conversion + url_img_part + extension}'
 
 
-def wikidate(param: Dict[str, Any]) -> Dict[str, Any]:
+def parse_date(date_string: str) -> Optional[datetime]:
+    """
+    Parse date string to datetime object.
+    Parameters
+    ----------
+    date_string: str
+        Date string
+
+    Returns
+    -------
+    parsed_date: datetime
+        Parsed date
+    """
+    try:
+        parsed_date = parser.parse(timestr=date_string)
+        return parsed_date
+    except parser.ParserError:
+        date_part, _ = date_string.split('T')
+        year, month, day = date_part.split('-')
+        if month == '00':
+            month = '01'
+        if day == '00':
+            day = '01'
+        iso_date = f'{year}-{month.zfill(2)}-{day.zfill(2)}'
+        try:
+            parsed_date = parser.parse(timestr=iso_date)
+            return parsed_date
+        except parser.ParserError:
+            return None
+
+
+def wikidate(param: dict[str, Any]) -> dict[str, Any]:
     """
     Parse and extract wikidata structure.
     Parameters
     ----------
-    param: Dict[str, Any]
+    param: dict[str, Any]
         Entity wikidata
 
     Returns
     -------
-    result: Dict[str, Any]
+    result: dict[str, Any]
         Dict with pretty print of date
     """
     time: str = param['time']
     timezone: int = param['timezone']
     before: int = param['before']
     after: int = param['after']
     precision: int = param['precision']
     calendar_model: str = param['calendarmodel']
+    iso_encoded: Optional[str] = None
     after_christ: bool = True
     pretty: str = ''
+    if calendar_model != 'https://www.wikidata.org/wiki/Q1985727':
+        if time.startswith('+'):
+            time = time[1:]
+        elif time.startswith('-'):
+            time = time[1:]
+            after_christ = False
+        date_obj: Optional[datetime] = parse_date(date_string=time)
+        if date_obj:
+            if date_obj.day == 0:
+                # Set the day component to 1
+                date_obj = date_obj.replace(day=1)
+            iso_encoded = date_obj.isoformat()
+            pretty = date_obj.strftime('%Y-%m-%d')
+        return {
+            'time': time,
+            'timezone': timezone,
+            'before': before,
+            'after': after,
+            'precision': precision,
+            'calendar-model': calendar_model,
+            'pretty': pretty,
+            'after-christ': after_christ,
+            'iso': iso_encoded
+        }
     if time.startswith('+'):
         time = time[1:]
     elif time.startswith('-'):
         time = time[1:]
         after_christ = False
     # Probably not necessary
     date_str = time.strip()
@@ -168,108 +223,115 @@
         elif Precision.HUNDREDS_THOUSAND_YEARS.value == precision:
             pretty = date_str
         elif Precision.MILLENIUM.value == precision:
             pretty = date_str
         elif Precision.TEN_THOUSAND_YEARS.value == precision:
             pretty = date_str
         else:
-            dt_obj: datetime = dateutil.parser.parse(date_str)
-            if Precision.CENTURY.value == precision:
-                century: int = int(math.ceil(dt_obj.year / 100))
-                pretty = f'{century}th century'
-            elif Precision.DECADE.value == precision:
-                pretty = f"{dt_obj.year}s{'' if after_christ else ' BC'}"
-            elif Precision.YEAR.value == precision:
-                pretty = f"{dt_obj.year}{'' if after_christ else ' BC'}"
-            elif Precision.MONTH.value == precision:
-                pretty = dt_obj.strftime("%B %Y")
-            elif Precision.DAY.value == precision:
-                pretty = dt_obj.strftime("%-d %B %Y")
+            dt_obj: Optional[datetime] = parse_date(date_str)
+            if dt_obj:
+                if Precision.CENTURY.value == precision:
+                    century: int = int(math.ceil(dt_obj.year / 100))
+                    pretty = f'{century}th century'
+                elif Precision.DECADE.value == precision:
+                    pretty = f"{dt_obj.year}s{'' if after_christ else ' BC'}"
+                elif Precision.YEAR.value == precision:
+                    pretty = f"{dt_obj.year}{'' if after_christ else ' BC'}"
+                elif Precision.MONTH.value == precision:
+                    pretty = dt_obj.strftime("%B %Y")
+                elif Precision.DAY.value == precision:
+                    pretty = dt_obj.strftime("%-d %B %Y")
+                iso_encoded = dt_obj.isoformat()
+                try:
+                    parse_date(iso_encoded)
+                except parser.ParserError:
+                    iso_encoded = None
     except Exception as pe:
         logger.error(param)
         logger.exception(pe)
 
     return {
         'time': time,
         'timezone': timezone,
         'before': before,
         'after': after,
         'precision': precision,
         'calendar-model': calendar_model,
-        'pretty': pretty
+        'pretty': pretty,
+        'after_christ': after_christ,
+        'iso': iso_encoded
     }
 
 
 def __waiting_request__(
         entity_id: str, base_url: str = WIKIDATA_LDI_URL
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Sena a request with retry policy.
 
     Parameters
     ----------
     entity_id: str
         Entity QID
     base_url: Base URL
         Base URL
     Returns
     -------
-    result_dict: Dict[str, Any]
+    result_dict: dict[str, Any]
         Result dict
     """
     url: str = f"{base_url}/{entity_id}.json"
 
     # Define the retry policy
     retry_policy: Retry = Retry(
         total=3,  # maximum number of retries
         backoff_factor=1,  # factor by which to multiply the delay between retries
         status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
-        method_whitelist=["GET"],  # HTTP methods to retry on
         respect_retry_after_header=True  # respect the Retry-After header
     )
 
     # Create a session and mount the retry adapter
     with requests.Session() as session:
         retry_adapter = HTTPAdapter(max_retries=retry_policy)
         session.mount("https://", retry_adapter)
 
         # Make a request using the session
         response: Response = session.get(url)
 
         # Check the response status code
         if not response.ok:
             raise WikiDataAPIException(f"Request failed with status code : {response.status_code}. URL:= {url}")
-        entity_dict_full: Dict[str, Any] = response.json()
+        entity_dict_full: dict[str, Any] = response.json()
         # remove redundant top level keys
         returned_entity_id: str = next(iter(entity_dict_full["entities"]))
         entity_dict = entity_dict_full["entities"][returned_entity_id]
 
         if entity_id != returned_entity_id:
             logger.warning(
                f"Wikidata redirect detected.  Input entity id={entity_id}. Returned entity id={returned_entity_id}."
             )
 
         return entity_dict
 
 
 def __waiting_multi_request__(
-        entity_ids: List[str], base_url: str = MULTIPLE_ENTITIES_API
-) -> List[Dict[str, Any]]:
+        entity_ids: list[str], base_url: str = MULTIPLE_ENTITIES_API
+) -> list[dict[str, Any]]:
     """
     Sena a request to retrieve multiple entities with retry policy.
 
     Parameters
     ----------
-    entity_ids: List[str]
+    entity_ids: list[str]
         Entity QID
     base_url: Base URL
         Base URL
     Returns
     -------
-    result_dict: Dict[str, Any]
+    result_dict: dict[str, Any]
         Result dict
     Raises
     ------
     ValueError - Empty list or to many entities
     """
     if not (0 < len(entity_ids) <= API_LIMIT):
         raise ValueError(f"Number of entities must be within [1, {API_LIMIT}]. Number of QIDs: {len(entity_ids)}")
@@ -277,31 +339,30 @@
     url: str = f"{base_url}{query}&format=json"
 
     # Define the retry policy
     retry_policy: Retry = Retry(
         total=3,  # maximum number of retries
         backoff_factor=1,  # factor by which to multiply the delay between retries
         status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
-        method_whitelist=["GET"],  # HTTP methods to retry on
         respect_retry_after_header=True  # respect the Retry-After header
     )
 
     # Create a session and mount the retry adapter
     with requests.Session() as session:
         retry_adapter = HTTPAdapter(max_retries=retry_policy)
         session.mount("https://", retry_adapter)
 
         # Make a request using the session
         response: Response = session.get(url)
 
         # Check the response status code
         if not response.ok:
             raise WikiDataAPIException(f"Request failed with status code : {response.status_code}. URL:= {url}")
-        entity_dict_full: Dict[str, Any] = response.json()
-        results: List[Dict[str, Any]] = []
+        entity_dict_full: dict[str, Any] = response.json()
+        results: list[dict[str, Any]] = []
         for qid, e in entity_dict_full["entities"].items():
             if qid not in entity_ids:
                 logger.warning(f"Wikidata redirect detected. "
                                f"Returned entity id={qid} is not in list of entity ids.")
             if 'missing' in e:
                 logger.warning(f"Missing entity detected. Returned entity id={qid} is not in Wikidata found.")
                 continue
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/public/relations.py` & `personal_knowledge_library-1.0.0/knowledge/public/relations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
 import functools
 import multiprocessing
-from typing import Dict, List, Any, Set, Tuple
+from typing import Any
 
 from tqdm import tqdm
 
 from knowledge.public.helper import CLAIMS_TAG, PID_TAG, LABEL_TAG, QID_TAG
 from knowledge.public.wikidata import LITERALS_TAG, WikidataThing, WikiDataAPIClient
 
 
-def __relations__(thing: Dict[str, Any], wikidata: Set[str]) -> Tuple[str, List[Dict[str, Any]]]:
-    relations: List[Dict[str, Any]] = []
-    for pid, p_value in thing[CLAIMS_TAG].items():
+def __relations__(thing: dict[str, Any], wikidata: set[str]) -> tuple[str, list[dict[str, Any]]]:
+    """
+    Extracts relations from Wikidata.
+    Parameters
+    ----------
+    thing: dict[str, Any]
+        Wikidata thing
+    wikidata: set[str]
+        Set of unique QIDs
+
+    Returns
+    -------
+    qid: str
+        QID of the Wikidata thing
+    relations: list[dict[str, Any]]
+        Relations of the Wikidata thing
+    """
+    relations: list[dict[str, Any]] = []
+    for _, p_value in thing[CLAIMS_TAG].items():
         for v in p_value[LITERALS_TAG]:
-            if isinstance(v, dict) and v.get('type') in ['wikibase-entityid', 'wikibase-item']:
+            if isinstance(v, dict) and v.get('type') in {'wikibase-entityid', 'wikibase-item'}:
                 ref_qid = v['value']['id']
                 prop = p_value[PID_TAG][LABEL_TAG]
                 if ref_qid in wikidata:
                     relations.append({
                         'subject': {
                             'qid': thing[QID_TAG],
                         },
@@ -29,35 +45,46 @@
                         'target': {
                             'qid': ref_qid
                         }
                     })
     return thing[QID_TAG], relations
 
 
-def wikidata_extractor_entities(qids: Set[str]) -> Dict[str, WikidataThing]:
+def wikidata_extractor_entities(qids: set[str]) -> dict[str, WikidataThing]:
     """
     Extracts an entity from Wikidata.
 
     Parameters
     ----------
-    qids: Set[str]
+    qids: set[str]
         Set of unique QIDs
 
     Returns
     -------
-    wikidata_extractor: Dict[str, WikidataThing]
+    wikidata_extractor: dict[str, WikidataThing]
         Wikidata map
     """
     return dict([(e.qid, e) for e in WikiDataAPIClient.retrieve_entities(qids)])
 
 
-def wikidata_relations_extractor(wikidata: Dict[str, WikidataThing]) \
-        -> Dict[str, List[Dict[str, Any]]]:
-    relations: Dict[str, List[Dict[str, Any]]] = {}
-    quis: Set[str] = set(wikidata.keys())
+def wikidata_relations_extractor(wikidata: dict[str, WikidataThing]) -> dict[str, list[dict[str, Any]]]:
+    """Extracts relations from Wikidata.
+
+    Parameters
+    ----------
+    wikidata: dict[str, WikidataThing]
+        Wikidata map
+
+    Returns
+    -------
+    relations: dict[str, list[dict[str, Any]]]
+        Relations map.
+    """
+    relations: dict[str, list[dict[str, Any]]] = {}
+    quis: set[str] = set(wikidata.keys())
     num_processes: int = min(len(wikidata), multiprocessing.cpu_count())
     with multiprocessing.Pool(processes=num_processes) as pool:
         # Wikidata thing is not support in multiprocessing
         with tqdm(total=round(len(wikidata) / num_processes), desc='Check Wikidata relations.') as pbar:
             for qid, rels in pool.map(functools.partial(__relations__, wikidata=quis),
                                       [e.__dict__() for e in wikidata.values()]):
                 relations[qid] = rels
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.0/knowledge/public/wikidata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
+import hashlib
 import multiprocessing
+import urllib
 from abc import ABC
+from datetime import datetime
 from multiprocessing import Pool
-from typing import List, Optional, Tuple, Union, Set
+from typing import Optional, Union, Any
 
+import requests
+from requests import Response
+from requests.adapters import HTTPAdapter
 from tqdm import tqdm
+from urllib3 import Retry
 
-from knowledge.base.entity import Description, DESCRIPTIONS_TAG, Label, LanguageCode, LABELS_TAG
-from knowledge.base.ontology import LANGUAGE_LOCALE_MAPPING
+from knowledge import logger
+from knowledge.base.entity import Description, DESCRIPTIONS_TAG, Label, LanguageCode, LABELS_TAG, REPOSITORY_TAG, \
+    DISPLAY_TAG, DESCRIPTION_TAG
+from knowledge.base.ontology import LANGUAGE_LOCALE_MAPPING, EN_US
 from knowledge.public import PROPERTY_MAPPING, INSTANCE_OF_PROPERTY, IMAGE_PROPERTY
-from knowledge.public.helper import *
-from knowledge.public.helper import __waiting_request__, __waiting_multi_request__
+from knowledge.public.helper import __waiting_request__, __waiting_multi_request__, QID_TAG, REVISION_TAG, \
+    PID_TAG, LABEL_TAG, CLAIMS_TAG, LABEL_VALUE_TAG, WIKIDATA_LANGUAGE_TAG, ALIASES_TAG, MODIFIED_TAG, \
+    ONTOLOGY_TYPES_TAG, SITELINKS_TAG, parse_date, ID_TAG, LAST_REVID_TAG, wikidate, WikiDataAPIException, \
+    WIKIDATA_SPARQL_URL, SOURCE_TAG, URLS_TAG, TITLES_TAG, image_url, WIKIDATA_SEARCH_URL, SUPERCLASSES_TAG, API_LIMIT
 
 # Constants
 QUALIFIERS_TAG: str = "QUALIFIERS"
 LITERALS_TAG: str = "LITERALS"
 
 
-def chunks(lst: List[str], chunk_size: int):
+def chunks(lst: list[str], chunk_size: int):
     """
     Yield successive n-sized chunks from lst.Yield successive n-sized chunks from lst.
     Parameters
     ----------
-    lst: List[str]
+    lst: list[str]
         Full length.
     chunk_size: int
         Chunk size.
 
     """
     for i in range(0, len(lst), chunk_size):
         yield lst[i:i + chunk_size]
 
 
-class WikidataProperty(object):
+class WikidataProperty:
     """
     WikidataProperty
     ----------------
     Property id and its label from wikidata.
 
     Parameters
     ----------
@@ -79,22 +90,112 @@
     def __dict__(self):
         return {
             PID_TAG: self.pid,
             LABEL_TAG: self.label_cached
         }
 
     @classmethod
-    def create_from_dict(cls, prop_dict: Dict[str, Any]) -> 'WikidataProperty':
+    def create_from_dict(cls, prop_dict: dict[str, Any]) -> 'WikidataProperty':
+        """Create a property from a dictionary.
+        Parameters
+        ----------
+        prop_dict: dict[str, Any]
+            Property dictionary.
+
+        Returns
+        -------
+        instance: WikidataProperty
+            Instance of WikidataProperty.
+        """
         return WikidataProperty(prop_dict[PID_TAG], prop_dict.get(LABEL_TAG))
 
     def __repr__(self):
         return f'<Property:={self.pid}]>'
 
 
-class WikidataClass(object):
+class WikidataSearchResult:
+    """
+    WikidataSearchResult
+    --------------------
+    Search result from wikidata.
+    """
+
+    def __init__(self, qid: str, label: Label, description: Optional[Description], repository: str, aliases: list[str]):
+        self.__qid: str = qid
+        self.__label: Label = label
+        self.__description: Optional[Description] = description
+        self.__repository: str = repository
+        self.__aliases: list[str] = aliases
+
+    @property
+    def qid(self) -> str:
+        """QID of the search result."""
+        return self.__qid
+
+    @property
+    def label(self) -> Label:
+        """Label of the search result."""
+        return self.__label
+
+    @property
+    def description(self) -> Optional[Description]:
+        """Description of the search result."""
+        return self.__description
+
+    @property
+    def repository(self) -> str:
+        """Repository of the search result."""
+        return self.__repository
+
+    @property
+    def aliases(self) -> list[str]:
+        """Aliases of the search result."""
+        return self.__aliases
+
+    @classmethod
+    def from_dict(cls, search_result: dict[str, Any]) -> 'WikidataSearchResult':
+        """
+        Create a search result from a dictionary.
+        Parameters
+        ----------
+        search_result: dict[str, Any]
+            Search result dictionary.
+
+        Returns
+        -------
+        WikidataSearchResult
+            Instance of WikidataSearchResult.
+        """
+        qid: str = search_result[ID_TAG]
+        display: dict[str, Any] = search_result[DISPLAY_TAG]
+        label: Label = Label(content=display[LABEL_TAG]['value'],
+                             language_code=LanguageCode(LANGUAGE_LOCALE_MAPPING.get(display[LABEL_TAG]['language'],
+                                                                                    EN_US)))
+        description: Optional[Description] = None
+        if DESCRIPTION_TAG in display:
+            description: Description = Description(description=display[DESCRIPTION_TAG]['value'],
+                                                   language_code=display[DESCRIPTION_TAG]['language'])
+        aliases: list[str] = [alias['value'] for alias in display.get(ALIASES_TAG, [])]
+        repository: str = search_result[REPOSITORY_TAG]
+        return WikidataSearchResult(
+            qid=qid,
+            label=label,
+            description=description,
+            repository=repository,
+            aliases=aliases
+        )
+
+    def __repr__(self):
+        desc_str: str = ''
+        if self.description:
+            desc_str: str = f' - description:= {self.description}'
+        return f'<Search Result:={self.qid} - label:= {self.label}{desc_str}>'
+
+
+class WikidataClass:
     """
     WikidataClass
     ----------------
     In Wikidata, classes are used to group items together based on their common characteristics.
     Classes in Wikidata are represented as items themselves, and they are typically identified by the prefix "Q"
     followed by a unique number.
 
@@ -122,15 +223,15 @@
         Class QID.
 
     """
     def __init__(self, qid: str, label: Optional[str] = None):
         super().__init__()
         self.__qid: str = qid
         self.__label: Optional[str] = label
-        self.__superclasses: List[WikidataClass] = []
+        self.__superclasses: list[WikidataClass] = []
 
     @property
     def qid(self):
         """Property id."""
         return self.__qid
 
     @property
@@ -141,19 +242,19 @@
 
         class_dict = __waiting_request__(self.qid)
         self.__label = class_dict['labels'].get('en').get('value', self.__qid) \
             if class_dict.get('labels') and class_dict['labels'].get('en') else self.__qid
         return self.__label
 
     @property
-    def superclasses(self) -> List['WikidataClass']:
+    def superclasses(self) -> list['WikidataClass']:
         return self.__superclasses
 
     @classmethod
-    def create_from_dict(cls, class_dict: Dict[str, Any]) -> 'WikidataClass':
+    def create_from_dict(cls, class_dict: dict[str, Any]) -> 'WikidataClass':
         wiki_cls: WikidataClass = cls(class_dict[QID_TAG], class_dict.get(LABEL_TAG))
         for superclass in class_dict.get(SUPERCLASSES_TAG, []):
             wiki_cls.__superclasses.append(WikidataClass.create_from_dict(superclass))
 
         return wiki_cls
 
     def __dict__(self):
@@ -171,15 +272,15 @@
         ret: str = f'{padding}|-- {self.qid} ({self.label})\n'
         for parent in self.superclasses:
             ret += parent.__str__(padding + '|   ')
         return ret
     """
 
 
-class Claim(object):
+class Claim:
     """
     Claim
     ------
     A Wikidata claim is a statement that describes a particular property-value relationship about an item in the
     Wikidata knowledge base. In Wikidata, an item represents a specific concept, such as a person, place, or
     organization, and a property describes a particular aspect of that concept, such as its name, date of birth,
     or location.
@@ -191,32 +292,32 @@
     - Object: The value of the property for the given item
 
     For example, a claim could be "Barack Obama (subject) has a birth-date (predicate) of August 4, 1961 (object)."
     Claims in Wikidata help to organize information and provide a structured way to represent knowledge that can
     be easily queried, analyzed, and visualized.
     """
 
-    def __init__(self, pid: WikidataProperty, literal: List[Dict[str, Any]], qualifiers: List[Dict[str, Any]]):
+    def __init__(self, pid: WikidataProperty, literal: list[dict[str, Any]], qualifiers: list[dict[str, Any]]):
         super().__init__()
         self.__pid: WikidataProperty = pid
-        self.__literals: List[Dict[str, Any]] = literal
-        self.__qualifiers: List[Dict[str, Any]] = qualifiers
+        self.__literals: list[dict[str, Any]] = literal
+        self.__qualifiers: list[dict[str, Any]] = qualifiers
 
     @property
     def pid(self) -> WikidataProperty:
         """Property name. Predicate of the claim."""
         return self.__pid
 
     @property
-    def literals(self) -> List[Dict[str, Any]]:
+    def literals(self) -> list[dict[str, Any]]:
         """Literals. Objects of the statement."""
         return self.__literals
 
     @property
-    def qualifiers(self) -> List[Dict[str, Any]] :
+    def qualifiers(self) -> list[dict[str, Any]]:
         """Qualifiers."""
         return self.__qualifiers
 
     def __dict__(self):
         return {
             PID_TAG: self.pid.__dict__(),
             LITERALS_TAG: self.literals,
@@ -239,15 +340,15 @@
         """Create a claim from a dictionary."""
         pid: WikidataProperty = WikidataProperty.create_from_dict(claim['pid'])
         literals = claim[LITERALS_TAG]
         qualifiers = claim[QUALIFIERS_TAG]
         return cls(pid, literals, qualifiers)
 
 
-class SiteLinks(object):
+class SiteLinks:
     """
     SiteLinks
     ---------
     Sitelinks in Wikidata are links between items in Wikidata and pages on external websites, such as Wikipedia,
     Wikimedia Commons, and other Wikimedia projects. A sitelink connects a Wikidata item to a specific page on an
     external website that provides more information about the topic represented by the item.
 
@@ -261,90 +362,109 @@
 
     Parameters
     ----------
     source: str
         Source of sitelinks.
     """
 
-    def __init__(self, source: str):
+    def __init__(self, source: str,
+                 urls: Union[dict[str, str], None] = None,
+                 titles: Union[dict[str, str], None] = None):
         self.__source: str = source
-        self.__urls: Dict[str, str] = {}
-        self.__title: Dict[str, str] = {}
+        self.__urls: dict[str, str] = {} if urls is None else urls
+        self.__title: dict[str, str] = {} if titles is None else titles
 
     @property
-    def urls(self) -> Dict[str, str]:
+    def urls(self) -> dict[str, str]:
         """URLs for the source."""
         return self.__urls
 
     @property
-    def titles(self) -> Dict[str, str]:
+    def titles(self) -> dict[str, str]:
         """Titles for the source."""
         return self.__title
 
     @property
-    def urls_languages(self) -> List[str]:
+    def urls_languages(self) -> list[str]:
         """List of all supported languages."""
         return list(self.__urls.keys())
 
     @property
     def source(self) -> str:
         """Sitelinks source."""
         return self.__source
 
     @classmethod
-    def create_from_dict(cls, entity_dict: Dict[str, Any]) -> 'SiteLinks':
-        site: SiteLinks = SiteLinks(source=entity_dict[SOURCE_TAG])
-        site.__urls = entity_dict[URLS_TAG]
-        site.__title = entity_dict[TITLES_TAG]
-        return site
+    def create_from_dict(cls, entity_dict: dict[str, Any]) -> 'SiteLinks':
+        """
+        Create a SiteLinks object from a dictionary.
+
+        Parameters
+        ----------
+        entity_dict: dict[str, Any]
+            dictionary containing the entity information.
+
+        Returns
+        -------
+        instance: SiteLinks
+            SiteLinks instance.
+        """
+        return SiteLinks(source=entity_dict[SOURCE_TAG], urls=entity_dict.get(URLS_TAG),
+                         titles=entity_dict.get(TITLES_TAG))
 
     def __dict__(self):
         return {
             SOURCE_TAG: self.__source,
             URLS_TAG: self.__urls,
             TITLES_TAG: self.__title
         }
 
     def __repr__(self):
         return f'<SiteLinks:={self.source}, supported languages:=[{"|".join(self.urls_languages)}]>'
 
 
-class WikidataThing(object):
+class WikidataThing:
     """
     WikidataEntity
     -----------
     Generic entity within wikidata.
 
     Each entity is derived from this object, thus all entity shares:
     - **qid**: A unique resource identity to identify the entity and reference it in relations
     - **label**: Human understandable label
     - **description**: Description of entity
 
     Parameters
     ----------
-    label: List[Label]
+    revision: str
+        Revision of the entity
+    qid: str
+        QID for entity. For new entities the URI is None, as the knowledge graph backend assigns this.
+    modified: datetime
+        Last modified date
+    label: list[Label]
         List of labels
-    description: List[Description] (optional)
+    description: list[Description] (optional)
         List of descriptions
     qid: str
          QID for entity. For new entities the URI is None, as the knowledge graph backend assigns this.
     """
 
     def __init__(self, revision: str, qid: str, modified: datetime,
-                 label: Optional[Dict[str, Label]] = None, aliases: Optional[Dict[str, List[Label]]] = None,
-                 description: Optional[Dict[str, Description]] = None):
+                 label: Optional[dict[str, Label]] = None, aliases: Optional[dict[str, list[Label]]] = None,
+                 description: Optional[dict[str, Description]] = None):
         self.__qid: str = qid
         self.__revision: str = revision
         self.__modified: datetime = modified
-        self.__label: Dict[str, Label] = label if label else {}
-        self.__description: Dict[str, Description] = description if description else {}
-        self.__aliases: Dict[str, List[Label]] = aliases if aliases else {}
-        self.__claims: Dict[str, Claim] = {}
-        self.__sitelinks: Dict[str, SiteLinks] = {}
-        self.__ontology_types: List[str] = []
+        self.__label: dict[str, Label] = label if label else {}
+        self.__description: dict[str, Description] = description if description else {}
+        self.__aliases: dict[str, list[Label]] = aliases if aliases else {}
+        self.__claims: dict[str, Claim] = {}
+        self.__sitelinks: dict[str, SiteLinks] = {}
+        self.__ontology_types: list[str] = []
 
     @property
     def qid(self) -> str:
         """QID for entity."""
         return self.__qid
 
     @property
@@ -354,64 +474,65 @@
 
     @property
     def modified(self) -> datetime:
         """Modification date of entity."""
         return self.__modified
 
     @property
-    def label(self) -> Dict[str, Label]:
+    def label(self) -> dict[str, Label]:
         """Labels of the entity."""
         return self.__label
 
     @property
-    def ontology_types(self) -> List[str]:
+    def ontology_types(self) -> list[str]:
         """Ontology types of the entity."""
         return self.__ontology_types
 
     @ontology_types.setter
-    def ontology_types(self, ontology_types: List[str]):
+    def ontology_types(self, ontology_types: list[str]):
         self.__ontology_types = ontology_types
 
     @property
-    def label_languages(self) -> List[str]:
+    def label_languages(self) -> list[str]:
         """All available languages for a labels."""
         return list(self.__label.keys())
 
     @property
-    def aliases(self) -> Dict[str, List[Label]]:
+    def aliases(self) -> dict[str, list[Label]]:
         """Alternative labels of the concept."""
         return self.__aliases
 
     @property
-    def alias_languages(self) -> List[str]:
+    def alias_languages(self) -> list[str]:
         """All available languages for a aliaes."""
         return list(self.__aliases.keys())
 
     @property
-    def description(self) -> Dict[str, Description]:
+    def description(self) -> dict[str, Description]:
         """Description of the thing (optional)."""
         return self.__description
 
     @description.setter
-    def description(self, description: Dict[str, Description]):
+    def description(self, description: dict[str, Description]):
         self.__description = description
 
     @property
-    def description_languages(self) -> List[str]:
+    def description_languages(self) -> list[str]:
+        """All available languages for a description."""
         return list(self.__description.keys())
 
     def add_label(self, label: str, language_code: str):
         """Adding a label for entity.
 
         Parameters
         ----------
         label: str
             Label
         language_code: str
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         self.__label[language_code] = Label(label, LanguageCode(language_code), True)
 
     def label_lang(self, language_code: str) -> Optional[Label]:
         """
         Get label for language_code code.
 
@@ -430,58 +551,58 @@
         """Adding a description for entity.
 
         Parameters
         ----------
         description: str
             Description
         language_code: str
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         self.__description[language_code] = Description(description=description,
                                                         language_code=LanguageCode(language_code))
 
     def description_lang(self, language_code: str) -> Optional[Description]:
         """
         Get description for entity.
 
         Parameters
         ----------
         language_code: LanguageCode
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         Returns
         -------
         label: LocalizedContent
             Returns the  label for a specific language_code code
         """
         return self.description.get(language_code)
 
-    def alias_lang(self, language_code: LanguageCode) -> List[Label]:
+    def alias_lang(self, language_code: LanguageCode) -> list[Label]:
         """
         Get alias for language_code code.
 
         Parameters
         ----------
         language_code: LanguageCode
             Requested language_code code
         Returns
         -------
-        aliases: List[Label]
+        aliases: list[Label]
             Returns a list of aliases for a specific language code
         """
         return self.aliases.get(language_code)
 
     def add_alias(self, alias: str, language_code: str):
         """Adding an alias for entity.
 
         Parameters
         ----------
         alias: str
             Alias
         language_code: str
-            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>, e.g., en_US.
+            ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., 'en_US'.
         """
         if language_code not in self.__aliases:
             self.aliases[language_code] = []
         self.__aliases[language_code].append(Label(alias, LanguageCode(language_code), False))
 
     def image(self, dpi: int = 500) -> Optional[str]:
         """
@@ -500,112 +621,114 @@
         if not (50 <= dpi <= 1000):
             raise ValueError(f"DPI should bei with range of [50-1000]. Value:={dpi}")
         claim: Optional[Claim] = self.claims.get(IMAGE_PROPERTY)
         if claim and len(claim.literals) > 0:
             img = claim.literals[0]['value']
             if isinstance(img, dict) and 'image_url' in img:
                 return img['image_url']
-            else:
-                extension: str = ''
-                conversion: str = ''
-                fixed_img: str = img.replace(' ', '_')
-                if fixed_img.lower().endswith('svg'):
-                    extension: str = '.png'
-                if fixed_img.lower().endswith('tif') or fixed_img.lower().endswith('tiff'):
-                    extension: str = '.jpg'
-                    conversion: str = 'lossy-page1-'
-                hash_img: str = hashlib.md5(fixed_img.encode('utf-8')).hexdigest()
-                url_img_part: str = urllib.parse.quote_plus(fixed_img)
-                return f'https://upload.wikimedia.org/wikipedia/commons/thumb/' \
-                       f'{hash_img[0]}/{hash_img[:2]}/{url_img_part}/{dpi}px-{conversion + url_img_part + extension}'
+            extension: str = ''
+            conversion: str = ''
+            fixed_img: str = img.replace(' ', '_')
+            if fixed_img.lower().endswith('svg'):
+                extension: str = '.png'
+            if fixed_img.lower().endswith('tif') or fixed_img.lower().endswith('tiff'):
+                extension: str = '.jpg'
+                conversion: str = 'lossy-page1-'
+            hash_img: str = hashlib.md5(fixed_img.encode('utf-8')).hexdigest()
+            url_img_part: str = urllib.parse.quote_plus(fixed_img)
+            return f'https://upload.wikimedia.org/wikipedia/commons/thumb/' \
+                   f'{hash_img[0]}/{hash_img[:2]}/{url_img_part}/{dpi}px-{conversion + url_img_part + extension}'
         return None
 
     @property
-    def instance_of(self) -> List[WikidataClass]:
+    def instance_of(self) -> list[WikidataClass]:
+        """Instance of."""
         claim: Optional[Claim] = self.claims.get(INSTANCE_OF_PROPERTY)
         if claim:
-            return [WikidataClass(l['value'].get('id')) for l in claim.literals if 'value' in l]
+            return [WikidataClass(li['value'].get('id')) for li in claim.literals if 'value' in li]
         return []
 
     @property
-    def sitelinks(self) -> Dict[str, SiteLinks]:
+    def sitelinks(self) -> dict[str, SiteLinks]:
         """Different sitelinks assigned to entity."""
         return self.__sitelinks
 
     def __dict__(self):
         return {
             QID_TAG: self.qid,
             REVISION_TAG: self.revision,
             MODIFIED_TAG: self.modified.isoformat(),
             LABELS_TAG: dict([(lang, la.__dict__()) for lang, la in self.label.items()]),
             DESCRIPTIONS_TAG: dict([(lang, la.__dict__()) for lang, la in self.description.items()]),
-            ALIASES_TAG: dict([(l, [a.__dict__() for a in al]) for l, al in self.aliases.items()]),
+            ALIASES_TAG: dict([(lang, [a.__dict__() for a in al]) for lang, al in self.aliases.items()]),
             CLAIMS_TAG: dict([(pid, cl.__dict__()) for pid, cl in self.claims.items()]),
             ONTOLOGY_TYPES_TAG: self.ontology_types,
             SITELINKS_TAG: dict([(source, site.__dict__()) for source, site in self.sitelinks.items()])
         }
 
     @classmethod
-    def create_from_dict(cls, entity_dict: Dict[str, Any]) -> 'WikidataThing':
+    def create_from_dict(cls, entity_dict: dict[str, Any]) -> 'WikidataThing':
         """
         Create WikidataThing from dict.
+
         Parameters
         ----------
-        entity_dict: Dict[str, Any]
-            Dictionary with WikidataThing information.
+        entity_dict: dict[str, Any]
+            dictionary with WikidataThing information.
 
         Returns
         -------
         thing: WikidataThing
             Instance of WikidataThing
         """
-        labels: Dict[str, Label] = {}
-        aliases: Dict[str, List[Label]] = {}
-        descriptions: Dict[str, Description] = {}
+        labels: dict[str, Label] = {}
+        aliases: dict[str, list[Label]] = {}
+        descriptions: dict[str, Description] = {}
         for language, la in entity_dict[LABELS_TAG].items():
             labels[language] = Label.create_from_dict(la)
         for language, de in entity_dict[DESCRIPTIONS_TAG].items():
             descriptions[language] = Description.create_from_dict(de)
         for language, al in entity_dict[ALIASES_TAG].items():
             aliases[language] = []
             for a in al:
                 aliases[language].append(Label.create_from_dict(a))
         # Initiate the wikidata thing
         thing: WikidataThing = WikidataThing(qid=entity_dict[QID_TAG], revision=entity_dict[REVISION_TAG],
-                                             modified=parse(entity_dict[MODIFIED_TAG]), label=labels, aliases=aliases,
+                                             modified=parse_date(entity_dict[MODIFIED_TAG]), label=labels,
+                                             aliases=aliases,
                                              description=descriptions)
         # Load the ontology types
         thing.ontology_types = entity_dict.get(ONTOLOGY_TYPES_TAG, [])
         # Load the claims
         for pid, claim in entity_dict[CLAIMS_TAG].items():
             thing.claims[pid] = Claim.create_from_dict(claim)
         # Load the sitelinks
         for wiki_source, site_link in entity_dict[SITELINKS_TAG].items():
             thing.sitelinks[wiki_source] = SiteLinks.create_from_dict(site_link)
         return thing
 
     @staticmethod
-    def from_wikidata(entity_dict: Dict[str, Any], supported_languages: Optional[List[str]] = None) -> 'WikidataThing':
+    def from_wikidata(entity_dict: dict[str, Any], supported_languages: Optional[list[str]] = None) -> 'WikidataThing':
         """
         Create WikidataThing from Wikidata JSON response.
         Parameters
         ----------
-        entity_dict: Dict[str, Any]
-            Dictionary with WikidataThing information.
-        supported_languages: Optional[List[str]]
+        entity_dict: dict[str, Any]
+            dictionary with WikidataThing information.
+        supported_languages: Optional[list[str]]
             List of supported languages. If None, all languages are supported.
 
         Returns
         -------
         thing: WikidataThing
             Instance of WikidataThing.
         """
-        labels: Dict[str, Label] = {}
-        aliases: Dict[str, List[Label]] = {}
-        descriptions: Dict[str, Description] = {}
+        labels: dict[str, Label] = {}
+        aliases: dict[str, list[Label]] = {}
+        descriptions: dict[str, Description] = {}
         if LABELS_TAG in entity_dict:
             # Extract the labels
             for label in entity_dict[LABELS_TAG].values():
                 if supported_languages is None or label[WIKIDATA_LANGUAGE_TAG] in supported_languages:
                     la_content: str = label[LABEL_VALUE_TAG]
                     la_lang: str = label[WIKIDATA_LANGUAGE_TAG]
                     if la_lang in LANGUAGE_LOCALE_MAPPING:
@@ -635,32 +758,31 @@
                     desc_lang: str = desc[WIKIDATA_LANGUAGE_TAG]
                     if desc_lang in LANGUAGE_LOCALE_MAPPING:
                         de: Description = Description(description=desc_content,
                                                       language_code=LanguageCode(LANGUAGE_LOCALE_MAPPING[desc_lang]))
                         descriptions[de.language_code] = de
         # Initiate the wikidata thing
         thing: WikidataThing = WikidataThing(qid=entity_dict[ID_TAG], revision=entity_dict[LAST_REVID_TAG],
-                                             modified=parse(entity_dict[MODIFIED_TAG]), label=labels, aliases=aliases,
-                                             description=descriptions)
+                                             modified=parse_date(entity_dict[MODIFIED_TAG]), label=labels,
+                                             aliases=aliases, description=descriptions)
 
         # Iterate over the claims
         for pid, claim_group in entity_dict[CLAIMS_TAG].items():
-            literal: List[Dict[str, Any]] = []
-            qualifiers: List[Dict[str, Any]] = []
+            literal: list[dict[str, Any]] = []
+            qualifiers: list[dict[str, Any]] = []
             for claim in claim_group:
                 try:
-
                     snak_type: str = claim['mainsnak']['snaktype']
                     if snak_type == "value":
-                        data_value: Dict[str, Any] = claim['mainsnak']['datavalue']
+                        data_value: dict[str, Any] = claim['mainsnak']['datavalue']
                         data_type: str = claim['mainsnak']['datatype']
-                        val: Dict[str, Any] = {}
+                        val: dict[str, Any] = {}
                         if data_type == 'monolingualtext':
                             val = data_value['value']
-                        elif data_type in ['string', 'external-id', 'url']:
+                        elif data_type in {'string', 'external-id', 'url'}:
                             val = data_value['value']
                         elif data_type == 'commonsMedia':
                             val = {
                                 'image_url': image_url(data_value['value'])
                             }
                         elif data_type == 'time':
                             val = wikidate(data_value['value'])
@@ -670,26 +792,26 @@
                                     "amount": data_value['value']['amount'],
                                     "unit": data_value['value']['unit']
                                 }
                         elif data_type == 'wikibase-lexeme':
                             val = {
                                 'id': data_value['value']['id']
                             }
-                        elif data_type in ['geo-shape', 'wikibase-property']:
+                        elif data_type in {'geo-shape', 'wikibase-property'}:
                             # Not supported
-                            val =  data_value['value']
-                        elif data_type in ['globe-coordinate', 'globecoordinate']:
+                            val = data_value['value']
+                        elif data_type in {'globe-coordinate', 'globecoordinate'}:
                             val = {
                                 'longitude': data_value['value'].get('longitude'),
                                 'latitude': data_value['value'].get('latitude'),
                                 'altitude': data_value['value'].get('altitude'),
                                 'globe': data_value['value'].get('globe'),
                                 'precision': data_value['value'].get('precision')
                             }
-                        elif data_type in ["wikibase-entityid", 'wikibase-item']:
+                        elif data_type in {"wikibase-entityid", 'wikibase-item'}:
                             val = {
                                 'id': data_value['value']['id']
                             }
                         elif data_type == 'math':
                             val = {
                                 'math': data_value['value']
                             }
@@ -732,23 +854,26 @@
                     if title and language_code not in thing.sitelinks[wiki_source].titles:
                         thing.sitelinks[wiki_source].titles[language_code] = title
                 except Exception as e:
                     logger.warning(f"Unexpected source: {source}. Exception: {e}")
         return thing
 
     @property
-    def claims(self) -> Dict[str, Claim]:
+    def claims(self) -> dict[str, Claim]:
+        """ Returns the claims. """
         return self.__claims
 
     @property
-    def claims_dict(self) -> Dict[str, Claim]:
+    def claims_dict(self) -> dict[str, Claim]:
+        """ Returns the claims as a dictionary. """
         return dict([(p, c) for p, c in self.__claims.items()])
 
     @property
-    def claim_properties(self) -> List[WikidataProperty]:
+    def claim_properties(self) -> list[WikidataProperty]:
+        """ Returns the list of properties of the claims. """
         return [p.pid for p in self.__claims.values()]
 
     def add_claim(self, pid: str, claim: Claim):
         """
         Adding a claim.
 
         Parameters
@@ -767,33 +892,33 @@
         # another object is equal to self, iff
         # it is an instance of MyClass
         return isinstance(other, WikidataThing) and other.qid == self.qid
 
     def __repr__(self):
         return f'<WikidataThing [QID:={self.qid}]>'
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         return self.__dict__().copy()
 
-    def __setstate__(self, state: Dict[str, Any]):
-        labels: Dict[str, Label] = {}
-        aliases: Dict[str, List[Label]] = {}
-        descriptions: Dict[str, Description] = {}
+    def __setstate__(self, state: dict[str, Any]):
+        labels: dict[str, Label] = {}
+        aliases: dict[str, list[Label]] = {}
+        descriptions: dict[str, Description] = {}
         for language, la in state[LABELS_TAG].items():
             labels[language] = Label.create_from_dict(la)
         for language, de in state[DESCRIPTIONS_TAG].items():
             descriptions[language] = Description.create_from_dict(de)
         for language, al in state[ALIASES_TAG].items():
             aliases[language] = []
             for a in al:
                 aliases[language].append(Label.create_from_dict(a))
         # Initiate the wikidata thing
         self.__qid = state[QID_TAG]
         self.__revision = state.get(REVISION_TAG)
-        self.__modified = parse(state[MODIFIED_TAG]) if MODIFIED_TAG in state else None
+        self.__modified = parse_date(state[MODIFIED_TAG]) if MODIFIED_TAG in state else None
         self.__label = labels
         self.__aliases = aliases
         self.__description = descriptions
         # Load the ontology types
         self.__ontology_types = state.get(ONTOLOGY_TYPES_TAG, [])
         # Load the claims
         self.__claims = {}
@@ -801,19 +926,30 @@
             self.__claims[pid] = Claim.create_from_dict(claim)
         # Load the sitelinks
         self.__sitelinks = {}
         for wiki_source, site_link in state[SITELINKS_TAG].items():
             self.__sitelinks[wiki_source] = SiteLinks.create_from_dict(site_link)
 
 
-def detect_cycle(super_class_qid: str, cycle_detector: List[Tuple[str, str]]):
-    for e in cycle_detector:
-        if e[0] == super_class_qid:
-            return True
-    return False
+def detect_cycle(super_class_qid: str, cycle_detector: list[tuple[str, str]]) -> bool:
+    """
+    Detects if there is a cycle in the super class hierarchy.
+    Parameters
+    ----------
+    super_class_qid: str
+        Super class QID
+    cycle_detector: list[tuple[str, str]]
+        List of tuples of the form (subclass_qid, super_class_qid)
+
+    Returns
+    -------
+    cycle: bool
+        True if there is a cycle, False otherwise.
+    """
+    return any(e[0] == super_class_qid for e in cycle_detector)
 
 
 class WikiDataAPIClient(ABC):
     """
     WikiDataAPIClient
     -----------------
     Utility class for the WikiData.
@@ -822,30 +958,31 @@
 
     def __init__(self):
         pass
 
     @staticmethod
     def sparql_query(
             query_string: str, wikidata_sparql_url: str = WIKIDATA_SPARQL_URL, max_retries: int = 3
-    ) -> Dict:
+    ) -> dict:
         """Send a SPARQL query and return the JSON formatted result.
 
         Parameters
         -----------
         query_string: str
           SPARQL query string
         wikidata_sparql_url: str
           Wikidata SPARQL endpoint to use
+        max_retries: int
+            Maximum number of retries
         """
         # Define the retry policy
         retry_policy: Retry = Retry(
             total=max_retries,  # maximum number of retries
             backoff_factor=1,  # factor by which to multiply the delay between retries
             status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
-            method_whitelist=["GET"],  # HTTP methods to retry on
             respect_retry_after_header=True  # respect the Retry-After header
         )
 
         # Create a session and mount the retry adapter
         with requests.Session() as session:
             retry_adapter = HTTPAdapter(max_retries=retry_policy)
             session.mount("https://", retry_adapter)
@@ -856,24 +993,36 @@
         if response.ok:
             return response.json()
         raise WikiDataAPIException(f'Failed to query entities. '
                                    f'Response code:={response.status_code}, Exception:= {response.content}.')
 
     @staticmethod
     def superclasses(qid: str) -> Optional[WikidataClass]:
+        """
+        Returns the superclasses of the given QID.
+        Parameters
+        ----------
+        qid: str
+            Wikidata QID
+
+        Returns
+        -------
+        wikidata_classes: Optional[WikidataClass]
+            Wikidata class
+        """
         query: str = f'''SELECT ?class ?classLabel ?superclass ?superclassLabel
         WHERE
         {{
             wd:{qid} wdt:P279* ?class.
             ?class wdt:P279 ?superclass.
             SERVICE wikibase:label {{ bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }}
         }}'''
-        reply: Dict[str, Any] = WikiDataAPIClient.sparql_query(query)
-        wikidata_classes: Dict[str, WikidataClass] = {}
-        cycle_detector: List[Tuple[str, str]] = []
+        reply: dict[str, Any] = WikiDataAPIClient.sparql_query(query)
+        wikidata_classes: dict[str, WikidataClass] = {}
+        cycle_detector: list[tuple[str, str]] = []
         if 'results' in reply:
             for b in reply['results']['bindings']:
                 superclass_qid: str = b['superclass']['value'].split('/')[-1]
                 class_qid: str = b['class']['value'].split('/')[-1]
                 superclass_label: str = b['superclassLabel']['value']
                 class_label: str = b['classLabel']['value']
                 if class_qid not in wikidata_classes:
@@ -882,23 +1031,96 @@
                     wikidata_classes[superclass_qid] = WikidataClass(qid=superclass_qid, label=superclass_label)
                 if not detect_cycle(superclass_qid, cycle_detector):
                     wikidata_classes[class_qid].superclasses.append(wikidata_classes[superclass_qid])
                     cycle_detector.append((class_qid, superclass_qid))
         return wikidata_classes.get(qid)
 
     @staticmethod
+    def search_term(search_term: str, language: str, url: str = WIKIDATA_SEARCH_URL) -> list[WikidataSearchResult]:
+        """
+        Search for a term in the WikiData.
+        Parameters
+        ----------
+        search_term: str
+            The term to search for.
+        language: str
+            The language to search in.
+        url: str
+            The URL of the WikiData search API.
+
+        Returns
+        -------
+        search_results_dict: list[WikidataSearchResult]
+            The search results.
+        """
+        search_results_dict: list[WikidataSearchResult] = []
+        # Define the retry policy
+        retry_policy: Retry = Retry(
+            total=3,  # maximum number of retries
+            backoff_factor=1,  # factor by which to multiply the delay between retries
+            status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
+            respect_retry_after_header=True  # respect the Retry-After header
+        )
+
+        # Create a session and mount the retry adapter
+        with requests.Session() as session:
+            retry_adapter = HTTPAdapter(max_retries=retry_policy)
+            session.mount("https://", retry_adapter)
+            params: dict[str, str] = {
+                "action": "wbsearchentities",
+                "format": "json",
+                "language": language,
+                "search": search_term
+            }
+            # Make a request using the session
+            response: Response = session.get(url, params=params, timeout=200000)
+
+            # Check the response status code
+            if not response.ok:
+                raise WikiDataAPIException(f"Search request failed with status code : {response.status_code}. "
+                                           f"URL:= {url}")
+            search_result_dict_full: dict[str, Any] = response.json()
+            for search_result_dict in search_result_dict_full['search']:
+                search_results_dict.append(WikidataSearchResult.from_dict(search_result_dict))
+            return search_results_dict
+
+    @staticmethod
     def __wikidata_task__(qid: str) -> WikidataThing:
+        """Retrieve a single Wikidata thing.
+
+        Parameters
+        ----------
+        qid: str
+            QID of the entity.
+
+        Returns
+        -------
+        instance: WikidataThing
+            Single wikidata thing
+        """
         try:
             return WikidataThing.from_wikidata(__waiting_request__(qid))
         except Exception as e:
             logger.exception(e)
             raise WikiDataAPIException(e)
 
     @staticmethod
-    def __wikidata_multiple_task__(qids: List[str]) -> List[WikidataThing]:
+    def __wikidata_multiple_task__(qids: list[str]) -> list[WikidataThing]:
+        """Retrieve multiple Wikidata things.
+
+        Parameters
+        ----------
+        qids: list[str]
+            QIDs of the entities.
+
+        Returns
+        -------
+        instances: list[WikidataThing]
+            List of wikidata things
+        """
         try:
             return [WikidataThing.from_wikidata(e) for e in __waiting_multi_request__(qids)]
         except Exception as e:
             logger.exception(e)
             raise WikiDataAPIException(e)
 
     @staticmethod
@@ -915,19 +1137,31 @@
         -------
         instance: WikidataThing
             Single wikidata thing
         """
         return WikiDataAPIClient.__wikidata_task__(qid)
 
     @staticmethod
-    def retrieve_entities(qids: Union[List[str], Set[str]]) -> List[WikidataThing]:
-        pulled: List[WikidataThing] = []
+    def retrieve_entities(qids: Union[list[str], set[str]]) -> list[WikidataThing]:
+        """
+        Retrieve multiple Wikidata things.
+        Parameters
+        ----------
+        qids: list[str]
+            QIDs of the entities.
+
+        Returns
+        -------
+        instances: list[WikidataThing]
+            List of wikidata things.
+        """
+        pulled: list[WikidataThing] = []
         if len(qids) == 0:
             return []
-        jobs: List[List[str]] = [ch for ch in chunks(list(qids), API_LIMIT)]
+        jobs: list[list[str]] = [ch for ch in chunks(list(qids), API_LIMIT)]
         num_processes: int = min(len(jobs), multiprocessing.cpu_count())
         if num_processes > 1:
             with Pool(processes=num_processes) as pool:
                 # Wikidata thing is not support in multiprocessing
                 with tqdm(total=len(jobs)) as pbar:
                     for lst in pool.imap_unordered(__waiting_multi_request__, jobs):
                         pulled.extend([WikidataThing.from_wikidata(e) for e in lst])
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/base.py` & `personal_knowledge_library-1.0.0/knowledge/services/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 from abc import ABC
 from datetime import timezone, datetime
-from typing import Any, Dict, Tuple
+from typing import Any
 
 import jwt
 import requests
 from dateutil.parser import parse, ParserError
 from requests import Response
 
 from knowledge.services import USER_AGENT_STR
 
 # Constants for header tags
 USER_AGENT_HEADER_FLAG: str = 'User-Agent'
 AUTHORIZATION_HEADER_FLAG: str = 'Authorization'
 CONTENT_TYPE_HEADER_FLAG: str = 'Content-Type'
 TENANT_API_KEY: str = 'x-tenant-api-key'
 REFRESH_TOKEN_TAG: str = 'refreshToken'
+EXPIRATION_DATE_TAG: str = 'expirationDate'
+ACCESS_TOKEN_TAG: str = 'accessToken'
+DEFAULT_TIMEOUT: int = 60
 
 
 class WacomServiceException(Exception):
     """Exception thrown if Wacom service fails."""
     def __init__(self, message: str, status_code: int = 500):
         super().__init__(message)
         self.__status_code: int = status_code
@@ -73,30 +76,41 @@
     ----------
     application_name: str
         Name of the application using the service
     service_url: str
         URL of the service
     service_endpoint: str
         Base endpoint
+    auth_service_endpoint: str (Default:= 'graph/v1')
+        Authentication service endpoint
     verify_calls: bool (Default:= False)
         Flag if  API calls should be verified.
     """
-    AUTH_ENDPOINT: str = 'auth/user'
     USER_ENDPOINT: str = 'user'
     USER_LOGIN_ENDPOINT: str = f'{USER_ENDPOINT}/login'
     USER_REFRESH_ENDPOINT: str = f'{USER_ENDPOINT}/refresh'
     SERVICE_URL: str = 'https://private-knowledge.wacom.com'
+    """Production service URL"""
     STAGING_SERVICE_URL: str = 'https://stage-private-knowledge.wacom.com'
+    """Staging service URL"""
 
-    def __init__(self, application_name: str, service_url: str, service_endpoint: str, verify_calls: bool = True):
+    def __init__(self, application_name: str, service_url: str, service_endpoint: str,
+                 auth_service_endpoint: str = 'graph/v1', verify_calls: bool = True):
         self.__application_name: str = application_name
         self.__service_endpoint: str = service_endpoint
+        self.__auth_service_endpoint: str = auth_service_endpoint
         super().__init__(service_url, verify_calls)
 
-    def request_user_token(self, tenant_key: str, external_id: str) -> Tuple[str, str, datetime]:
+    @property
+    def auth_endpoint(self) -> str:
+        """Authentication endpoint."""
+        # This is in graph service REST API
+        return f'{self.service_url}/{self.__auth_service_endpoint}/{self.USER_LOGIN_ENDPOINT}'
+
+    def request_user_token(self, tenant_key: str, external_id: str) -> tuple[str, str, datetime]:
         """
         Login as user by using the tenant key and its external user id.
 
         Parameters
         ----------
         tenant_key: str
             Tenant key
@@ -113,41 +127,42 @@
             Expiration time
 
         Raises
         ------
         WacomServiceException
             Exception if service returns HTTP error code.
         """
-        url: str = f'{self.service_base_url}{WacomServiceAPIClient.USER_LOGIN_ENDPOINT}/'
+        url: str = f'{self.auth_endpoint}'
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             TENANT_API_KEY: tenant_key,
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
         payload: dict = {
             'ExternalUserId': external_id
         }
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, timeout=DEFAULT_TIMEOUT,
+                                           verify=self.verify_calls)
         if response.ok:
             try:
-                response_token: Dict[str, str] = response.json()
+                response_token: dict[str, str] = response.json()
                 try:
                     date_object: datetime = parse(response_token['expirationDate'])
                 except (ParserError, OverflowError) as _:
                     date_object: datetime = datetime.now()
                 return response_token['accessToken'], response_token['refreshToken'], date_object
             except Exception as e:
                 raise WacomServiceException(f'Login failed'
                                             f'Response code:={response.status_code}, response text:= {response.text}, '
                                             f'exception:= {e} ')
         raise WacomServiceException(f'User login failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}',
                                     status_code=response.status_code)
 
-    def refresh_token(self, refresh_token: str) -> Tuple[str, str, datetime]:
+    def refresh_token(self, refresh_token: str) -> tuple[str, str, datetime]:
         """
         Refreshing a token.
 
         Parameters
         ----------
         refresh_token: str
             Refresh token
@@ -163,34 +178,47 @@
 
         Raises
         ------
         WacomServiceException
             Exception if service returns HTTP error code.
         """
         url: str = f'{self.service_base_url}/{WacomServiceAPIClient.USER_REFRESH_ENDPOINT}/'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
-        payload: Dict[str, str] = {
+        payload: dict[str, str] = {
             REFRESH_TOKEN_TAG: refresh_token
         }
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, timeout=DEFAULT_TIMEOUT,
+                                           verify=self.verify_calls)
         if response.ok:
-            response_token: Dict[str, str] = response.json()
+            response_token: dict[str, str] = response.json()
             try:
-                date_object: datetime = parse(response_token['expirationDate'])
+                date_object: datetime = parse(response_token[EXPIRATION_DATE_TAG])
             except (ParserError, OverflowError) as _:
                 date_object: datetime = datetime.now()
-            return response_token['accessToken'], response_token['refreshToken'], date_object
+            return response_token[ACCESS_TOKEN_TAG], response_token[REFRESH_TOKEN_TAG], date_object
         raise WacomServiceException(f'Refresh failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     @staticmethod
-    def unpack_token(auth_token: str) -> Dict[str, Any]:
+    def unpack_token(auth_token: str) -> dict[str, Any]:
+        """Unpacks the token.
+
+        Parameters
+        ----------
+        auth_token: str
+            Authentication token
+
+        Returns
+        -------
+        token_dict: dict[str, Any]
+            Token dictionary
+        """
         return jwt.decode(auth_token, options={"verify_signature": False})
 
     @staticmethod
     def expired(auth_token: str) -> bool:
         """
         Checks if token is expired.
 
@@ -217,15 +245,15 @@
             Authentication token
 
         Returns
         -------
         expired_in: float
             Seconds until token is expired
         """
-        token_dict: Dict[str, Any] = WacomServiceAPIClient.unpack_token(auth_token)
+        token_dict: dict[str, Any] = WacomServiceAPIClient.unpack_token(auth_token)
         timestamp: datetime = datetime.now(tz=timezone.utc)
         expiration_time: datetime = datetime.fromtimestamp(token_dict['exp'], tz=timezone.utc)
         return expiration_time.timestamp() - timestamp.timestamp()
 
     @property
     def service_endpoint(self):
         """Service endpoint."""
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/graph.py` & `personal_knowledge_library-1.0.0/knowledge/services/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 import enum
 import json
 import os
 import urllib
 from pathlib import Path
-from typing import List, Dict, Any, Tuple, Optional
+from typing import Any, Optional
+from urllib.parse import urlparse
 
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from knowledge.base.access import TenantAccessRight
@@ -46,44 +47,61 @@
 GROUP_IDS_TAG: str = 'groupIds'
 OWNER_ID_TAG: str = 'ownerId'
 VISIBILITY_TAG: str = 'visibility'
 ESTIMATE_COUNT: str = 'estimateCount'
 
 RELATION_TAG: str = 'relation'
 APPLICATION_JSON_HEADER: str = 'application/json'
+DEFAULT_TIMEOUT: int = 60
 
-MIME_TYPE: Dict[str, str] = {
+MIME_TYPE: dict[str, str] = {
     '.jpg': 'image/jpeg',
     '.jpeg': 'image/jpeg',
     '.png': 'image/png'
 }
 
-SUPPORTED_LANGUAGES: List[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'ru_RU']
+SUPPORTED_LANGUAGES: list[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'ru_RU']
 
 
 # ------------------------------- Enum ---------------------------------------------------------------------------------
 class SearchPattern(enum.Enum):
     """
     SearchPattern
     -------------
     Different search pattern for literal search.
     """
     REGEX = 'regex'
+    """Regular expression search pattern."""
     GT = 'gt'
+    """Greater than search pattern."""
     GTE = 'gte'
+    """Greater than or equal search pattern."""
     LT = 'lt'
+    """Less than search pattern."""
     LTE = 'lte'
+    """Less than or equal search pattern."""
     EQ = 'eq'
+    """Equal search pattern."""
     RANGE = 'range'
+    """Range search pattern."""
 
 
 class Visibility(enum.Enum):
+    """
+    Visibility
+    ----------
+    Visibility of an entity.
+    The visibility of an entity determines who can see the entity.
+    """
     PRIVATE = 'Private'
+    """Only the owner of the entity can see the entity."""
     PUBLIC = 'Public'
+    """Everyone in the tenant can see the entity."""
     SHARED = 'Shared'
+    """Everyone who joined the group can see the entity."""
 
 
 # -------------------------------------------- Service API Client ------------------------------------------------------
 class WacomKnowledgeService(WacomServiceAPIClient):
     """
     WacomKnowledgeService
     ---------------------
@@ -143,23 +161,23 @@
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code or the entity is not found in the knowledge graph
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{uri}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
-            e: Dict[str, Any] = response.json()
-            pref_label: List[Label] = []
-            aliases: List[Label] = []
+            e: dict[str, Any] = response.json()
+            pref_label: list[Label] = []
+            aliases: list[Label] = []
             # Extract labels and alias
             for label in e[LABELS_TAG]:
                 if label[IS_MAIN_TAG]:  # Labels
                     pref_label.append(Label.create_from_dict(label))
                 else:  # Alias
                     aliases.append(Label.create_from_dict(label))
             # Create ThingObject
@@ -184,24 +202,24 @@
                 thing.tenant_access_right = TenantAccessRight.parse(e[TENANT_RIGHTS_TAG])
             else:
                 thing.tenant_access_right = TenantAccessRight()
             return thing
         raise WacomServiceException(f'Retrieving of entity content failed. URI:={uri}. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def delete_entities(self, auth_key: str, uris: List[str], force: bool = False, max_retries: int = 3,
+    def delete_entities(self, auth_key: str, uris: list[str], force: bool = False, max_retries: int = 3,
                         backoff_factor: float = 0.1):
         """
         Delete a list of entities.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
-        uris: List[str]
+        uris: list[str]
             List of URI of entities. **Remark:** More than 100 entities are not possible in one request
         force: bool
             Force deletion process
         max_retries: int
             Maximum number of retries
         backoff_factor: float
             A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
@@ -211,19 +229,19 @@
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         if len(uris) > 100:
             raise WacomServiceException("Please delete less than 100 entities.")
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        params: Dict[str, Any] = {
+        params: dict[str, Any] = {
             URIS_TAG: uris,
             FORCE_TAG: force
         }
         mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(total=max_retries,
                                    backoff_factor=backoff_factor,
@@ -255,15 +273,15 @@
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{uri}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(total=max_retries,
                                    backoff_factor=backoff_factor,
@@ -296,17 +314,17 @@
             return obj is not None
         except WacomServiceException:
             return False
 
     @staticmethod
     def __entity__(entity: ThingObject):
         # Different localized content
-        labels: List[dict] = []
-        descriptions: List[dict] = []
-        literals: List[dict] = []
+        labels: list[dict] = []
+        descriptions: list[dict] = []
+        literals: list[dict] = []
         # Add description in different languages
         for desc in entity.description:
             if len(desc.content) > 0 and not desc.content == ' ':
                 descriptions.append({
                     DESCRIPTION_TAG: desc.content,
                     LOCALE_TAG: desc.language_code
                 })
@@ -341,34 +359,34 @@
                 if li.data_property_type:
                     literals.append({
                         VALUE_TAG: li.value,
                         LOCALE_TAG: li.language_code
                         if li.language_code and li.language_code in SUPPORTED_LANGUAGES else "en_US",
                         DATA_PROPERTY_TAG: li.data_property_type.iri
                     })
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             TYPE_TAG: entity.concept_type.iri,
             DESCRIPTIONS_TAG: descriptions,
             LABELS_TAG: labels,
             DATA_PROPERTIES_TAG: literals,
             SEND_TO_NEL_TAG: entity.use_for_nel
         }
         if entity.tenant_access_right:
             payload[TENANT_RIGHTS_TAG] = entity.tenant_access_right.to_list()
         return payload
 
-    def create_entity_bulk(self, auth_key: str, entities: List[ThingObject], batch_size: int = 10) -> List[ThingObject]:
+    def create_entity_bulk(self, auth_key: str, entities: list[ThingObject], batch_size: int = 10) -> list[ThingObject]:
         """
         Creates entity in graph.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
-        entities: List[ThingObject]
+        entities: list[ThingObject]
             Entities
         batch_size: int
             Batch size
 
         Returns
         -------
         uri: str
@@ -377,27 +395,27 @@
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_BULK_ENDPOINT}'
         # Header info
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             CONTENT_TYPE_HEADER_FLAG: APPLICATION_JSON_HEADER,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: List[Dict[str, Any]] = [WacomKnowledgeService.__entity__(e) for e in entities]
+        payload: list[dict[str, Any]] = [WacomKnowledgeService.__entity__(e) for e in entities]
         for bulk_idx in range(0, len(entities), batch_size):
             bulk = payload[bulk_idx:bulk_idx + batch_size]
 
-            response: Response = requests.post(url, json=bulk, headers=headers,
+            response: Response = requests.post(url, json=bulk, headers=headers, timeout=DEFAULT_TIMEOUT,
                                                verify=self.verify_calls)
             if response.ok:
-                response_dict: Dict[str, Any] = response.json()
+                response_dict: dict[str, Any] = response.json()
                 for idx, uri in enumerate(response_dict[URIS_TAG]):
                     if entities[bulk_idx + idx].image is not None and entities[bulk_idx + idx].image != '':
                         self.set_entity_image_url(auth_key, uri, entities[bulk_idx + idx].image)
                     entities[bulk_idx + idx].uri = response_dict[URIS_TAG][idx]
 
         return entities
 
@@ -430,33 +448,32 @@
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}'
         # Header info
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             CONTENT_TYPE_HEADER_FLAG: APPLICATION_JSON_HEADER,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = WacomKnowledgeService.__entity__(entity)
+        payload: dict[str, Any] = WacomKnowledgeService.__entity__(entity)
         mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(total=max_retries,
                                    backoff_factor=backoff_factor,
                                    status_forcelist=[502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.post(url, json=payload, headers=headers, verify=self.verify_calls, timeout=5)
 
             if response.ok and not ignore_image:
                 uri: str = response.json()[URI_TAG]
                 # Set image
                 if entity.image is not None and entity.image.startswith('file:'):
-                    from urllib.parse import urlparse
                     p = urlparse(entity.image)
                     self.set_entity_image_local(auth_key, uri, Path(p.path))
                 elif entity.image is not None and entity.image != '':
                     self.set_entity_image_url(auth_key, uri, entity.image)
                 return uri
         raise WacomServiceException(f'Pushing entity failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}. '
@@ -469,30 +486,25 @@
         Parameters
         ----------
         auth_key: str
             Auth key from user
         entity: ThingObject
             entity object
 
-        Returns
-        -------
-        uri: str
-            URI of entity
-
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         uri: str = entity.uri
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{uri}'
         # Different localized content
-        labels: List[dict] = []
-        descriptions: List[dict] = []
-        literals: List[dict] = []
+        labels: list[dict] = []
+        descriptions: list[dict] = []
+        literals: list[dict] = []
         # Header info
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             CONTENT_TYPE_HEADER_FLAG: APPLICATION_JSON_HEADER,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         # Add description in different languages
@@ -540,34 +552,35 @@
             TYPE_TAG: entity.concept_type.iri,
             DESCRIPTIONS_TAG: descriptions,
             LABELS_TAG: labels,
             DATA_PROPERTIES_TAG: literals
         }
         if entity.tenant_access_right:
             payload[TENANT_RIGHTS_TAG] = entity.tenant_access_right.to_list()
-        response: Response = requests.patch(url, json=payload, headers=headers, verify=self.verify_calls)
+        response: Response = requests.patch(url, json=payload, headers=headers, timeout=DEFAULT_TIMEOUT,
+                                            verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Pushing entity failed. '
                                         f'Response code:={response.status_code}, exception:= {response.content}. '
                                         f'Payload: \n{json.dumps(payload, indent=4)}')
 
-    def relations(self, auth_key: str, uri: str) -> Dict[OntologyPropertyReference, ObjectProperty]:
+    def relations(self, auth_key: str, uri: str) -> dict[OntologyPropertyReference, ObjectProperty]:
         """
         Retrieve the relations (object properties) of an entity.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         uri: str
             Entity URI of the source
 
         Returns
         -------
-        relations: Dict[OntologyPropertyReference, ObjectProperty]
+        relations: dict[OntologyPropertyReference, ObjectProperty]
             All relations a dict
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
@@ -585,69 +598,69 @@
             response: Response = session.get(url, headers=headers, verify=self.verify_calls)
             if response.ok:
                 rel: list = response.json().get(RELATIONS_TAG)
                 return ObjectProperty.create_from_list(rel)
         raise WacomServiceException(f'Failed to pull relations. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def labels(self, auth_key: str, uri: str, locale: str = 'en_US') -> List[Label]:
+    def labels(self, auth_key: str, uri: str, locale: str = 'en_US') -> list[Label]:
         """
         Extract list labels of entity.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         uri: str
             Entity URI of the source
         locale: str
             ISO-3166 Country Codes and ISO-639 Language Codes in the format <language_code>_<country>, e.g., en_US.
 
         Returns
         -------
-        labels: List[Label]
+        labels: list[Label]
             List of labels of an entity.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{uri}/labels'
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         response: Response = requests.get(url, headers=headers,  params={
             LOCALE_TAG: locale,
-        }, verify=self.verify_calls)
+        }, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
             response_dict: dict = response.json()
             if LABELS_TAG in response_dict:
                 return [Label.create_from_dict(label) for label in response_dict[LABELS_TAG]]
             return []
-        raise WacomServiceException('Failed to pull literals. Response code:={}, exception:= {}'
-                                    .format(response.status_code, response.content))
+        raise WacomServiceException(f'Failed to pull literals. Response code:={response.status_code}, '
+                                    'exception:= {response.content}')
 
-    def literals(self, auth_key: str, uri: str, locale: str = 'en_US') -> List[DataProperty]:
+    def literals(self, auth_key: str, uri: str, locale: str = 'en_US') -> list[DataProperty]:
         """
         Collect all literals of entity.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         uri: str
             Entity URI of the source
         locale: str
             ISO-3166 Country Codes and ISO-639 Language Codes in the format <language_code>_<country>, e.g., en_US.
 
         Returns
         -------
-        labels: List[DataProperty]
+        labels: list[DataProperty]
             List of data properties of an entity.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
@@ -655,20 +668,20 @@
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
 
         response: Response = requests.get(url, headers=headers, params={
             LOCALE_TAG: locale,
-        }, verify=self.verify_calls)
+        }, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
             literals: list = response.json().get(DATA_PROPERTIES_TAG)
             return DataProperty.create_from_list(literals)
-        raise WacomServiceException('Failed to pull literals. Response code:={}, exception:= {}'
-                                    .format(response.status_code, response.content))
+        raise WacomServiceException(f'Failed to pull literals. Response code:={response.status_code}, '
+                                    f'exception:= {response.content}')
 
     def create_relation(self, auth_key: str, source: str, relation: OntologyPropertyReference, target: str):
         """
         Creates a relation for an entity to a source entity.
 
         Parameters
         ----------
@@ -725,84 +738,86 @@
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{source}/relation'
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             RELATION_TAG: relation.iri,
             TARGET: target
         }
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         # Get response
-        response: Response = requests.delete(url, params=params, headers=headers, verify=self.verify_calls)
+        response: Response = requests.delete(url, params=params, headers=headers, timeout=DEFAULT_TIMEOUT,
+                                             verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Deletion of relation failed. '
                                         f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def activations(self, auth_key: str, uris: List[str], depth: int) \
-            -> Tuple[Dict[str, ThingObject], List[Tuple[str, OntologyPropertyReference, str]]]:
+    def activations(self, auth_key: str, uris: list[str], depth: int) \
+            -> tuple[dict[str, ThingObject], list[tuple[str, OntologyPropertyReference, str]]]:
         """
         Spreading activation, retrieving the entities related to an entity.
 
         Parameters
         ----------
         auth_key: str
             Auth key for user
-        uris: List[str]
+        uris: list[str]
             List of URIS for entity.
         depth: int
             Depth of activations
 
         Returns
         -------
-        entity_map: Dict[str, ThingObject]
+        entity_map: dict[str, ThingObject]
             Map with entity and its URI as key.
-        relations: List[Tuple[str, OntologyPropertyReference, str]]
+        relations: list[tuple[str, OntologyPropertyReference, str]]
             List of relations with subject predicate, (Property), and subject
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code, and activation failed.
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ACTIVATIONS_ENDPOINT}'
 
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: dict = {
             'uris': uris,
             ACTIVATION_TAG: depth
         }
 
-        response: Response = requests.get(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=params, timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
-            entities: Dict[str, Any] = response.json()
-            things: Dict[str, ThingObject] = dict([(e[URI_TAG], ThingObject.from_dict(e))
+            entities: dict[str, Any] = response.json()
+            things: dict[str, ThingObject] = dict([(e[URI_TAG], ThingObject.from_dict(e))
                                                    for e in entities['entities']])
-            relations: List[Tuple[str, OntologyPropertyReference, str]] = []
+            relations: list[tuple[str, OntologyPropertyReference, str]] = []
             for r in entities[RELATIONS_TAG]:
                 relation: OntologyPropertyReference = OntologyPropertyReference.parse(r[PREDICATE])
                 relations.append((r[SUBJECT], relation, r[OBJECT]))
                 if r[SUBJECT] in things:
                     things[r[SUBJECT]].add_relation(ObjectProperty(relation, outgoing=[r[OBJECT]]))
             return things, relations
         raise WacomServiceException(f'Activation failed, uris:= {uris} activation:={depth}). '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def listing(self, auth_key: str, filter_type: OntologyClassReference, page_id: Optional[str] = None,
                 limit: int = 30, locale: Optional[LanguageCode] = None, visibility: Optional[Visibility] = None,
                 estimate_count: bool = False, max_retries: int = 3, backoff_factor: float = 0.1) \
-            -> Tuple[List[ThingObject], int, str]:
+            -> tuple[list[ThingObject], int, str]:
         """
         List all entities visible to users.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
@@ -822,34 +837,34 @@
             Maximum number of retries
         backoff_factor: float
             A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
             second try without a delay)
 
         Returns
         -------
-        entities: List[ThingObject]
+        entities: list[ThingObject]
             List of entities
         estimated_total_number: int
             Number of all entities
         next_page_id: str
             Identifier of the next page
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.LISTING_ENDPOINT}'
         # Header with auth token
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         # Parameter with filtering and limit
-        parameters: Dict[str, str] = {
+        parameters: dict[str, str] = {
             TYPE_TAG: filter_type.iri,
             LIMIT_PARAMETER: limit,
             ESTIMATE_COUNT: estimate_count
         }
         if locale:
             parameters[LOCALE_TAG] = locale
         if visibility:
@@ -859,28 +874,28 @@
             parameters[NEXT_PAGE_ID_TAG] = page_id
         mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(total=max_retries,
                                    backoff_factor=backoff_factor,
                                    status_forcelist=[502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
-        # Send request
-        response: Response = requests.get(url, params=parameters, headers=headers, verify=self.verify_calls)
-        # If response is successful
-        if response.ok:
-            entities_resp: dict = response.json()
-            next_page_id: str = entities_resp[NEXT_PAGE_ID_TAG]
-            estimated_total_number: int = entities_resp.get(TOTAL_COUNT, 0)
-            entities: List[ThingObject] = []
-            if LISTING in entities_resp:
-                for e in entities_resp[LISTING]:
-                    thing: ThingObject = ThingObject.from_dict(e)
-                    thing.status_flag = EntityStatus.SYNCED
-                    entities.append(thing)
-            return entities, estimated_total_number, next_page_id
+            # Send request
+            response: Response = session.get(url, params=parameters, headers=headers, verify=self.verify_calls)
+            # If response is successful
+            if response.ok:
+                entities_resp: dict = response.json()
+                next_page_id: str = entities_resp[NEXT_PAGE_ID_TAG]
+                estimated_total_number: int = entities_resp.get(TOTAL_COUNT, 0)
+                entities: list[ThingObject] = []
+                if LISTING in entities_resp:
+                    for e in entities_resp[LISTING]:
+                        thing: ThingObject = ThingObject.from_dict(e)
+                        thing.status_flag = EntityStatus.SYNCED
+                        entities.append(thing)
+                return entities, estimated_total_number, next_page_id
 
         raise WacomServiceException(f'Failed to list the entities (since:= {page_id}, limit:={limit}). '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def ontology_update(self, auth_key: str):
         """
         Update the ontology.
@@ -900,72 +915,73 @@
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ONTOLOGY_UPDATE_ENDPOINT}'
         # Header with auth token
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.patch(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.patch(url, headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Ontology update fails. '
                                         f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_all(self, auth_key: str, search_term: str, language_code: LanguageCode,
-                   types: List[OntologyClassReference], limit: int = 30, next_page_id: str = None) \
-            -> Tuple[List[ThingObject], str]:
+                   types: list[OntologyClassReference], limit: int = 30, next_page_id: str = None) \
+            -> tuple[list[ThingObject], str]:
         """Search term in labels, literals and description.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         search_term: str
             Search term.
         language_code: LanguageCode
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., en_US.
-        types: List[OntologyClassReference]
+        types: list[OntologyClassReference]
             Limits the types for search.
         limit: int  (default:= 30)
             Size of the page for pagination.
         next_page_id: str (default:=None)
             ID of the next page within pagination.
 
         Returns
         -------
-        results: List[ThingObject]
+        results: list[ThingObject]
             List of things matching the search term
         next_page_id: str
             ID of the next page.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        parameters: Dict[str, Any] = {
+        parameters: dict[str, Any] = {
             SEARCH_TERM: search_term,
             LANGUAGE_PARAMETER: language_code,
             TYPES_PARAMETER: [ot.iri for ot in types],
             LIMIT: limit,
             NEXT_PAGE_ID_TAG: next_page_id
         }
         url: str = f'{self.service_base_url}{WacomKnowledgeService.SEARCH_TYPES_ENDPOINT}'
-        response: Response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=parameters, timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
             return WacomKnowledgeService.__search_results__(response.json())
         raise WacomServiceException(f'Search on labels {search_term} failed. '
                                     f'{parameters}'
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_labels(self, auth_key: str, search_term: str, language_code: LanguageCode, limit: int = 30,
-                      next_page_id: str = None) -> Tuple[List[ThingObject], str]:
+                      next_page_id: str = None) -> tuple[list[ThingObject], str]:
         """Search for matches in labels.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         search_term: str
@@ -975,45 +991,46 @@
         limit: int  (default:= 30)
             Size of the page for pagination.
         next_page_id: str (default:=None)
             ID of the next page within pagination.
 
         Returns
         -------
-        results: List[ThingObject]
+        results: list[ThingObject]
             List of things matching the search term
         next_page_id: str
             ID of the next page.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        parameters: Dict[str, Any] = {
+        parameters: dict[str, Any] = {
             SEARCH_TERM: search_term,
             LOCALE_TAG: language_code,
             LIMIT: limit,
             NEXT_PAGE_ID_TAG: next_page_id
         }
         url: str = f'{self.service_base_url}{WacomKnowledgeService.SEARCH_LABELS_ENDPOINT}'
-        response: Response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=parameters, timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
             return WacomKnowledgeService.__search_results__(response.json())
         raise WacomServiceException(f'Search on labels {search_term} failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_literal(self, auth_key: str, search_term: str, literal: OntologyPropertyReference,
                        pattern: SearchPattern = SearchPattern.REGEX,
                        language_code: LanguageCode = LanguageCode('en_US'),
-                       limit: int = 30, next_page_id: str = None) -> Tuple[List[ThingObject], str]:
+                       limit: int = 30, next_page_id: str = None) -> tuple[list[ThingObject], str]:
         """
         Search for matches in literals.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
@@ -1028,45 +1045,46 @@
         limit: int (default:= 30)
             Size of the page for pagination.
         next_page_id: str (default:=None)
             ID of the next page within pagination.
 
         Returns
         -------
-        results: List[ThingObject]
+        results: list[ThingObject]
            List of things matching the search term
        next_page_id: str
            ID of the next page.
 
        Raises
        ------
        WacomServiceException
            If the graph service returns an error code.
        """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.SEARCH_LITERALS_ENDPOINT}'
-        parameters: Dict[str, Any] = {
+        parameters: dict[str, Any] = {
             VALUE: search_term,
             LITERAL_PARAMETER: literal.iri,
             LANGUAGE_PARAMETER: language_code,
             LIMIT_PARAMETER: limit,
             SEARCH_PATTERN_PARAMETER: pattern.value,
             NEXT_PAGE_ID_TAG: next_page_id
         }
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=parameters,  timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
             return WacomKnowledgeService.__search_results__(response.json())
         raise WacomServiceException(f'Search on labels {search_term} failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_relation(self, auth_key: str, relation: OntologyPropertyReference,
                         language_code: LanguageCode, subject_uri: str = None, object_uri: str = None,
-                        limit: int = 30, next_page_id: str = None) -> Tuple[List[ThingObject], str]:
+                        limit: int = 30, next_page_id: str = None) -> tuple[list[ThingObject], str]:
         """
         Search for matches in literals.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
@@ -1081,46 +1099,47 @@
         limit: int (default:= 30)
             Size of the page for pagination.
         next_page_id: str (default:=None)
             ID of the next page within pagination.
 
         Returns
         -------
-        results: List[ThingObject]
+        results: list[ThingObject]
            List of things matching the search term
         next_page_id: str
            ID of the next page.
 
        Raises
        ------
        WacomServiceException
            If the graph service returns an error code.
        """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.SEARCH_RELATION_ENDPOINT}'
-        parameters: Dict[str, Any] = {
+        parameters: dict[str, Any] = {
             SUBJECT_URI: subject_uri,
             RELATION_URI: relation.iri,
             OBJECT_URI: object_uri,
             LANGUAGE_PARAMETER: language_code,
             LIMIT: limit,
             NEXT_PAGE_ID_TAG: next_page_id
         }
         headers: dict = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
 
-        response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response = requests.get(url, headers=headers, params=parameters, timeout=DEFAULT_TIMEOUT,
+                                verify=self.verify_calls)
         if response.ok:
             return WacomKnowledgeService.__search_results__(response.json())
         raise WacomServiceException(f'Search on: subject:={subject_uri}, relation {relation.iri}, '
                                     f'object:= {object_uri} failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_description(self, auth_key: str, search_term: str, language_code: LanguageCode, limit: int = 30,
-                           next_page_id: str = None) -> Tuple[List[ThingObject], str]:
+                           next_page_id: str = None) -> tuple[list[ThingObject], str]:
         """Search for matches in description.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         search_term: str
@@ -1130,44 +1149,45 @@
         limit: int  (default:= 30)
             Size of the page for pagination.
         next_page_id: str (default:=None)
             ID of the next page within pagination.
 
         Returns
         -------
-        results: List[ThingObject]
+        results: list[ThingObject]
             List of things matching the search term
         next_page_id: str
             ID of the next page.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code.
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.SEARCH_DESCRIPTION_ENDPOINT}'
-        parameters: Dict[str, Any] = {
+        parameters: dict[str, Any] = {
             SEARCH_TERM: search_term,
             LOCALE_TAG: language_code,
             LIMIT: limit,
             NEXT_PAGE_ID_TAG: next_page_id
         }
         headers: dict = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
 
-        response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response = requests.get(url, headers=headers, params=parameters, timeout=DEFAULT_TIMEOUT,
+                                verify=self.verify_calls)
         if response.ok:
             return WacomKnowledgeService.__search_results__(response.json())
         raise WacomServiceException(f'Search on labels {search_term} failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     @staticmethod
-    def __search_results__(response: Dict[str, Any]) -> Tuple[List[ThingObject], str]:
-        results: List[ThingObject] = []
+    def __search_results__(response: dict[str, Any]) -> tuple[list[ThingObject], str]:
+        results: list[ThingObject] = []
         for elem in response['result']:
             results.append(ThingObject.from_dict(elem))
         return results, response[NEXT_PAGE_ID_TAG]
 
     def set_entity_image_local(self, auth_key: str, entity_uri: str, path: Path) -> str:
         """Setting the image of the entity.
        The image is stored locally.
@@ -1224,18 +1244,16 @@
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code.
         """
         with requests.session() as session:
-            headers: Dict[str, str] = {
-                USER_AGENT_HEADER_FLAG:
-                    f'ImageFetcher/0.1 (https://github.com/Wacom-Developer/personal-knowledge-library)'
-                    f' personal-knowledge-library/0.9.5'
+            headers: dict[str, str] = {
+                USER_AGENT_HEADER_FLAG: USER_AGENT_STR
             }
             response: Response = session.get(image_url, headers=headers)
             if response.ok:
                 image_bytes: bytes = response.content
                 file_name: str = image_url if file_name is None else file_name
                 if mime_type is None:
                     _, file_extension = os.path.splitext(file_name.lower())
@@ -1278,16 +1296,16 @@
        ------
        WacomServiceException
            If the graph service returns an error code.
        """
         headers: dict = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        files: List[Tuple[str, Tuple[str, bytes, str]]] = [
+        files: list[tuple[str, tuple[str, bytes, str]]] = [
             ('file', (file_name, image_byte, mime_type))
         ]
         url: str = f'{self.service_base_url}{self.ENTITY_IMAGE_ENDPOINT}{urllib.parse.quote(entity_uri)}'
-        response = requests.patch(url, headers=headers, files=files, verify=self.verify_calls)
+        response = requests.patch(url, headers=headers, files=files, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
             return response.json()['imageId']
         raise WacomServiceException(f'Creation of entity image failed'
                                     f'Response code:={response.status_code}, exception:= {response.content}')
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/group.py` & `personal_knowledge_library-1.0.0/knowledge/services/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 import urllib.parse
-from typing import Dict, List, Any, Optional
+from typing import List, Any, Optional
 
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from knowledge.base.access import GroupAccessRight
 from knowledge.base.ontology import NAME_TAG
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException
 from knowledge.services.graph import AUTHORIZATION_HEADER_FLAG, CONTENT_TYPE_HEADER_FLAG
-
 # -------------------------------------- Constant flags ----------------------------------------------------------------
 from knowledge.services.users import User
 
 GROUP_USER_RIGHTS_TAG: str = "groupUserRights"
 JOIN_KEY_PARAM: str = "joinKey"
 USER_TO_ADD_PARAM: str = "userToAddId"
 USER_TO_REMOVE_PARAM: str = "userToRemoveId"
 FORCE_PARAM: str = "force"
 DEFAULT_TIMEOUT: int = 30
 
 
-class Group(object):
+class Group:
     """
     Group
     -----
     In Personal Knowledge backend users can be logically grouped.
 
     Parameters
     ----------
@@ -81,15 +80,27 @@
 
     @property
     def group_access_rights(self) -> GroupAccessRight:
         """Rights for group."""
         return self.__rights
 
     @classmethod
-    def parse(cls, param: Dict[str, Any]) -> 'Group':
+    def parse(cls, param: dict[str, Any]) -> 'Group':
+        """Parse group from dictionary.
+
+        Arguments
+        ---------
+        param: dict[str, Any]
+            Dictionary containing group information.
+
+        Returns
+        -------
+        instance: Group
+            Group object
+        """
         tenant_id: str = param.get('tenantId')
         owner_id: str = param.get('ownerId')
         join_key: str = param.get('joinKey')
         group_id: str = param.get('id')
         name: str = param.get('name')
         rights: GroupAccessRight = GroupAccessRight.parse(param.get('groupUserRights', ['Read']))
         return Group(tenant_id=tenant_id, group_id=group_id, owner=owner_id, join_key=join_key, name=name,
@@ -104,25 +115,25 @@
     Group Information
     -----------------
     Provides additional information on the group.
     Users within the group are listed.
     """
 
     def __init__(self, tenant_id: str, group_id: str, owner: str, name: str, join_key: str, rights: GroupAccessRight,
-                 group_users: List[User]):
-        self.__users: List[User] = group_users
+                 group_users: list[User]):
+        self.__users: list[User] = group_users
         super().__init__(tenant_id, group_id, owner, name, join_key, rights)
 
     @property
     def group_users(self) -> List:
         """List of all users that are part of the group."""
         return self.__users
 
     @classmethod
-    def parse(cls, param: Dict[str, Any]) -> 'GroupInfo':
+    def parse(cls, param: dict[str, Any]) -> 'GroupInfo':
         tenant_id: str = param.get('tenantId')
         owner_id: str = param.get('ownerId')
         join_key: str = param.get('joinKey')
         group_id: str = param.get('id')
         name: str = param.get('name')
         rights: GroupAccessRight = GroupAccessRight.parse(param.get('groupUserRights', ['Read']))
         return GroupInfo(tenant_id=tenant_id, group_id=group_id, owner=owner_id, join_key=join_key, name=name,
@@ -182,19 +193,19 @@
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
-        payload: Dict[str, str] = {
+        payload: dict[str, str] = {
             NAME_TAG: name,
             GROUP_USER_RIGHTS_TAG: rights.to_list()
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
@@ -224,19 +235,19 @@
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
-        payload: Dict[str, str] = {
+        payload: dict[str, str] = {
             NAME_TAG: name,
             GROUP_USER_RIGHTS_TAG: rights.to_list()
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
@@ -261,118 +272,118 @@
 
          Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
             if not response.ok:
                 raise WacomServiceException(f'Deletion of group failed.'
                                             f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def listing_groups(self, auth_key: str, admin: bool = False) -> List[Group]:
+    def listing_groups(self, auth_key: str, admin: bool = False) -> list[Group]:
         """
         Listing all groups configured for this instance.
 
         Parameters
         ----------
         auth_key: str
             API key for authentication
 
         admin: bool (default:= False)
             Uses admin privilege to show all groups of the tenant.
             Requires user to have the role: TenantAdmin
 
         Returns
         -------
-        user:  List[Groups]
+        user:  list[Groups]
             List of groups.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}'
         if admin:
             url += '/admin'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
             if response.ok:
-                groups: List[Dict[str, Any]] = response.json()
+                groups: list[dict[str, Any]] = response.json()
                 return [Group.parse(g) for g in groups]
         raise WacomServiceException(f'Listing of group failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def group(self, auth_key: str, group_id: str) -> GroupInfo:
         """Get a group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
 
         Returns
         -------
         group: Group
             Instance of the group
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
-            group: Dict[str, Any] = response.json()
+            group: dict[str, Any] = response.json()
             return GroupInfo.parse(group)
         raise WacomServiceException(f'Getting of group information failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def join_group(self, auth_key: str, group_id: str, join_key: str):
         """User joining a group with his auth token.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
         join_key: str
             Key which is used to join the group.
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/join'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             JOIN_KEY_PARAM: join_key,
         }
         response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
                                            timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Joining the group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
@@ -381,23 +392,23 @@
         """User leaving a group with his auth token.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/leave'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
 
         response: Response = requests.post(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Leaving group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
@@ -406,28 +417,28 @@
         """Adding a user to group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
         user_id: str
             User who is added to the group
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/user/add'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             USER_TO_ADD_PARAM: user_id,
         }
         response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
                                            timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Adding of user to group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
@@ -436,92 +447,92 @@
         """Remove a user from group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
         user_id: str
             User who is remove from the group
         force: bool
             If true remove user and entities owned by the user if any
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/user/remove'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             USER_TO_REMOVE_PARAM: user_id,
             FORCE_PARAM: force
         }
         response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
                                            timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Removing of user from group failed. URL: {url}'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def add_entity_to_group(self, auth_key: str, group_id: str, entity_uri: str):
-        """Adding a entity to group.
+        """Adding an entity to group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
         entity_uri: str
             Entity URI
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         uri: str = urllib.parse.quote(entity_uri)
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/entity/{uri}/add'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.post(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
             if not response.ok:
                 raise WacomServiceException(f'Adding of entity to group failed.'
                                             f'Response code:={response.status_code}, exception:= {response.text}')
 
     def remove_entity_to_group(self, auth_key: str, group_id: str, entity_uri: str):
-        """Remove a entity from group.
+        """Remove an entity from group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
-            Id of group
+            Group ID
         entity_uri: str
             URI of entity
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         uri: str = urllib.parse.quote(entity_uri)
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/entity/{uri}/remove'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
         with requests.Session() as session:
             retries: Retry = Retry(backoff_factor=0.1,
                                    status_forcelist=[500, 502, 503, 504])
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.0/knowledge/services/ontology.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 import urllib.parse
 from http import HTTPStatus
-from typing import Dict, List, Any, Optional, Tuple
+from typing import Any, Optional
 
 import requests
 from requests import Response
 
-from knowledge.base.entity import Comment, OntologyContext, OntologyLabel
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, OntologyProperty, OntologyClass, \
-    PropertyType, THING_CLASS, DataPropertyType, InflectionSetting
+    PropertyType, THING_CLASS, DataPropertyType, InflectionSetting, Comment, OntologyContext, OntologyLabel
 from knowledge.services import USER_AGENT_STR
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException
 from knowledge.services.graph import AUTHORIZATION_HEADER_FLAG
 
 # ------------------------------------------------- Constants ----------------------------------------------------------
 BASE_URI_TAG: str = "baseUri"
 COMMENTS_TAG: str = "comments"
@@ -68,120 +67,122 @@
             Auth key from user.
 
         Returns
         -------
         context_description: Optional[OntologyContext]
             Context of the Ontology
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         response: Response = requests.get(f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}',
-                                          headers=headers, verify=self.verify_calls)
+                                          headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
             return OntologyContext.from_dict(response.json())
         return None
 
-    def context_metadata(self, auth_key: str, context: str) -> List[InflectionSetting]:
+    def context_metadata(self, auth_key: str, context: str) -> list[InflectionSetting]:
         """
         Getting the meta-data on the context.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user.
         context: str
             Name of the context.
 
         Returns
         -------
-        list_inflection_settings: List[InflectionSetting]
+        list_inflection_settings: list[InflectionSetting]
             List of inflection settings.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         response: Response = requests.get(f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}'
                                           f'/metadata',
-                                          headers=headers, verify=self.verify_calls)
+                                          headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         if response.ok:
-            return [InflectionSetting.from_dict(c) for c in response.json()]
+            return [InflectionSetting.from_dict(c) for c in response.json() if c.get('concept') is not None
+                    and not c.get('concept').startswith('http')]
+        raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def concepts(self, auth_key: str, context: str) -> List[Tuple[OntologyClassReference, OntologyClassReference]]:
+    def concepts(self, auth_key: str, context: str) -> list[tuple[OntologyClassReference, OntologyClassReference]]:
         """Retrieve all concept classes.
 
         **Remark:**
         Works for users with role 'User' and 'TenantAdmin'.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user.
         context: str
             Context of the ontology
 
         Returns
         -------
-        concepts: List[Tuple[OntologyClassReference, OntologyClassReference]]
+        concepts: list[tuple[OntologyClassReference, OntologyClassReference]]
             List of ontology classes. Tuple<Classname, Superclass>
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}/' \
                    f'{OntologyService.CONCEPTS_ENDPOINT}'
         response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
-            response_list: List[Tuple[OntologyClassReference, OntologyClassReference]] = []
+            response_list: list[tuple[OntologyClassReference, OntologyClassReference]] = []
             result = response.json()
             for struct in result:
                 response_list.append((OntologyClassReference.parse(struct[NAME_TAG]),
                                       None if struct[SUB_CLASS_OF_TAG] is None else
                                       OntologyClassReference.parse(struct[SUB_CLASS_OF_TAG])))
             return response_list
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def properties(self, auth_key: str, context: str) \
-            -> List[Tuple[OntologyPropertyReference, OntologyPropertyReference]]:
+            -> list[tuple[OntologyPropertyReference, OntologyPropertyReference]]:
         """List all properties.
 
         **Remark:**
         Works for users with role 'User' and 'TenantAdmin'.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user.
         context: str
             Name of the context
 
         Returns
         -------
-        contexts: List[Tuple[OntologyPropertyReference, OntologyPropertyReference]]
+        contexts: list[tuple[OntologyPropertyReference, OntologyPropertyReference]]
             List of ontology contexts
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         response: Response = requests.get(f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/'
                                           f'{context_url}/{OntologyService.PROPERTIES_ENDPOINT}',
-                                          headers=headers, verify=self.verify_calls)
+                                          headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
         # Return empty list if the NOT_FOUND is reported
         if response.status_code == HTTPStatus.NOT_FOUND:
             return []
         if response.ok:
-            response_list: List[Tuple[OntologyPropertyReference, OntologyPropertyReference]] = []
+            response_list: list[tuple[OntologyPropertyReference, OntologyPropertyReference]] = []
             for c in response.json():
                 response_list.append((OntologyPropertyReference.parse(c[NAME_TAG]),
-                                      None if c[SUB_PROPERTY_OF_TAG] is None else
+                                      None if c[SUB_PROPERTY_OF_TAG] is None or c.get(SUB_PROPERTY_OF_TAG) == '' else
                                       OntologyPropertyReference.parse(c[SUB_PROPERTY_OF_TAG])))
             return response_list
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def concept(self, auth_key: str, context: str, concept_name: str) -> OntologyClass:
         """Retrieve a concept instance.
 
@@ -198,25 +199,25 @@
             IRI of the concept
 
         Returns
         -------
         instance: OntologyClass
             Instance of the concept
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(concept_name)
         response: Response = requests.get(f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context_url}'
                                           f'/{OntologyService.CONCEPTS_ENDPOINT}/{concept_url}',
                                           headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
-            result: Dict[str, Any] = response.json()
+            result: dict[str, Any] = response.json()
             return OntologyClass.from_dict(result)
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def property(self, auth_key: str, context: str, property_name: str) -> OntologyProperty:
         """Retrieve a property instance.
 
         **Remark:**
@@ -232,31 +233,31 @@
             IRI of the property
 
         Returns
         -------
         instance: OntologyProperty
             Instance of the property
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(property_name)
         param: str = f"context/{context_url}/properties/{concept_url}"
         response: Response = requests.get(f'{self.service_base_url}{param}', headers=headers, verify=self.verify_calls,
                                           timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return OntologyProperty.from_dict(response.json())
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_concept(self, auth_key: str, context: str, reference: OntologyClassReference,
                        subclass_of: OntologyClassReference = THING_CLASS,
-                       icon: Optional[str] = None, labels: Optional[List[OntologyLabel]] = None,
-                       comments: Optional[List[Comment]] = None) -> Dict[str, str]:
+                       icon: Optional[str] = None, labels: Optional[list[OntologyLabel]] = None,
+                       comments: Optional[list[Comment]] = None) -> dict[str, str]:
         """Create concept class.
 
         **Remark:**
         Only works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
@@ -266,33 +267,33 @@
             Context of ontology
         reference: OntologyClassReference
             Name of the concept
         subclass_of: OntologyClassReference (default:=wacom:core#Thing)
             Super class of the concept
         icon: Optional[str] (default:= None)
             Icon representing the concept
-        labels: Optional[List[OntologyLabel]] (default:= None)
+        labels: Optional[list[OntologyLabel]] (default:= None)
             Labels for the class
-        comments: Optional[List[Comment]] (default:= None)
+        comments: Optional[list[Comment]] (default:= None)
             Comments for the class
         Returns
         -------
-        result: Dict[str, str]
+        result: dict[str, str]
             Result from the service
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             SUB_CLASS_OF_TAG: subclass_of.iri,
             NAME_TAG: reference.iri,
             LABELS_TAG: [],
             COMMENTS_TAG: [],
             ICON_TAG: icon
         }
         for label in labels if labels is not None else []:
@@ -300,22 +301,22 @@
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}/' \
                    f'{OntologyService.CONCEPTS_ENDPOINT}'
         response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls,
                                            timeout=DEFAULT_TIMEOUT)
         if response.ok:
-            result_dict: Dict[str, str] = response.json()
+            result_dict: dict[str, str] = response.json()
             return result_dict
         raise WacomServiceException(f'Creation of concept failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def update_concept(self, auth_key: str, context: str, name: str, subclass_of: Optional[str],
-                       icon: Optional[str] = None, labels: Optional[List[OntologyLabel]] = None,
-                       comments: Optional[List[Comment]] = None) -> Dict[str, str]:
+                       icon: Optional[str] = None, labels: Optional[list[OntologyLabel]] = None,
+                       comments: Optional[list[Comment]] = None) -> dict[str, str]:
         """Update concept class.
 
         **Remark:**
         Only works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
@@ -325,34 +326,34 @@
             Context of ontology
         name: str
             Name of the concept
         subclass_of: Optional[str]
             Super class of the concept
         icon: Optional[str] (default:= None)
             Icon representing the concept
-        labels: Optional[List[OntologyLabel]] (default:= None)
+        labels: Optional[list[OntologyLabel]] (default:= None)
             Labels for the class
-        comments: Optional[List[Comment]] (default:= None)
+        comments: Optional[list[Comment]] (default:= None)
             Comments for the class
 
         Returns
         -------
-        response: Dict[str, str]
+        response: dict[str, str]
             Response from service
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             SUB_CLASS_OF_TAG: subclass_of,
             NAME_TAG: name,
             LABELS_TAG: [],
             COMMENTS_TAG: [],
             ICON_TAG: icon
         }
         for label in labels if labels is not None else []:
@@ -384,77 +385,77 @@
             Name of the concept
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(reference.iri)
         url: str = f'{self.service_base_url}context/{context_url}/concepts/{concept_url}'
         response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Deletion of concept failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_object_property(self, auth_key: str, context: str,
                                reference: OntologyPropertyReference,
-                               domains_cls: List[OntologyClassReference], ranges_cls: List[OntologyClassReference],
+                               domains_cls: list[OntologyClassReference], ranges_cls: list[OntologyClassReference],
                                inverse_of: Optional[OntologyPropertyReference] = None,
                                subproperty_of: Optional[OntologyPropertyReference] = None,
                                icon: Optional[str] = None,
-                               labels: Optional[List[OntologyLabel]] = None,
-                               comments: Optional[List[Comment]] = None) -> Dict[str, str]:
+                               labels: Optional[list[OntologyLabel]] = None,
+                               comments: Optional[list[Comment]] = None) -> dict[str, str]:
         """Create property.
 
         **Remark:**
         Only works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user.
         context: str
             Context of ontology
         reference: OntologyPropertyReference
             Name of the concept
-        domains_cls: List[OntologyClassReference]
+        domains_cls: list[OntologyClassReference]
             IRI of the domain
-        ranges_cls: List[OntologyClassReference]
+        ranges_cls: list[OntologyClassReference]
             IRI of the range
         inverse_of: Optional[OntologyPropertyReference] (default:= None)
             Inverse property
         subproperty_of: Optional[OntologyPropertyReference] = None,
             Super property of the concept
         icon: Optional[str] (default:= None)
             Icon representing the concept
-        labels: Optional[List[OntologyLabel]] (default:= None)
+        labels: Optional[list[OntologyLabel]] (default:= None)
             Labels for the class
-        comments: Optional[List[Comment]] (default:= None)
+        comments: Optional[list[Comment]] (default:= None)
             Comments for the class
 
         Returns
         -------
-        result: Dict[str, str]
+        result: dict[str, str]
             Result from the service
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             KIND_TAG: PropertyType.OBJECT_PROPERTY.value,
             DOMAIN_TAG: [d.iri for d in domains_cls],
             RANGE_TAG: [r.iri for r in ranges_cls],
             SUB_PROPERTY_OF_TAG: subproperty_of.iri if subproperty_of is not None else None,
             INVERSE_OF_TAG: inverse_of.iri if inverse_of is not None else None,
             NAME_TAG: reference.iri,
             LABELS_TAG: [],
@@ -473,60 +474,60 @@
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Creation of object property failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_data_property(self, auth_key: str, context: str,
                              reference: OntologyPropertyReference,
-                             domains_cls: List[OntologyClassReference], ranges_cls: List[DataPropertyType],
+                             domains_cls: list[OntologyClassReference], ranges_cls: list[DataPropertyType],
                              subproperty_of: Optional[OntologyPropertyReference] = None,
                              icon: Optional[str] = None,
-                             labels: Optional[List[OntologyLabel]] = None,
-                             comments: Optional[List[Comment]] = None) -> Dict[str, str]:
+                             labels: Optional[list[OntologyLabel]] = None,
+                             comments: Optional[list[Comment]] = None) -> dict[str, str]:
         """Create data property.
 
         **Remark:**
         Only works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user.
         context: str
             Context of ontology
         reference: OntologyPropertyReference
             Name of the concept
-        domains_cls: List[OntologyClassReference]
+        domains_cls: list[OntologyClassReference]
             IRI of the domain
-        ranges_cls: List[DataPropertyType]
+        ranges_cls: list[DataPropertyType]
             Data property type
         subproperty_of: Optional[OntologyPropertyReference] = None,
             Super property of the concept
         icon: Optional[str] (default:= None)
             Icon representing the concept
-        labels: Optional[List[Label]] (default:= None)
+        labels: Optional[list[Label]] (default:= None)
             Labels for the class
-        comments: Optional[List[Comment]] (default:= None)
+        comments: Optional[list[Comment]] (default:= None)
             Comments for the class
 
         Returns
         -------
-        result: Dict[str, str]
+        result: dict[str, str]
             Result from the service
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             KIND_TAG: PropertyType.DATA_PROPERTY.value,
             DOMAIN_TAG: [d.iri for d in domains_cls],
             RANGE_TAG: [r.value for r in ranges_cls],
             SUB_PROPERTY_OF_TAG: subproperty_of.iri if subproperty_of is not None else None,
             NAME_TAG: reference.iri,
             LABELS_TAG: [],
             COMMENTS_TAG: [],
@@ -562,28 +563,28 @@
             Name of the property
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         property_url: str = urllib.parse.quote_plus(reference.iri)
         url: str = f'{self.service_base_url}context/{context_url}/properties/{property_url}'
         response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Deletion of property: {reference.iri} failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_context(self, auth_key: str, name: str, base_uri: Optional[str] = None, icon: Optional[str] = None,
-                       labels: List[OntologyLabel] = None, comments: List[Comment] = None) -> Dict[str, str]:
+                       labels: list[OntologyLabel] = None, comments: list[Comment] = None) -> dict[str, str]:
         """Create context.
 
         **Remark:**
         Only works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
@@ -591,34 +592,34 @@
             Auth key from user.
         base_uri: str
             Base URI
         name: str
             Name of the context
         icon: Optional[str] (default:= None)
             Icon representing the concept
-        labels: Optional[List[OntologyLabel]] (default:= None)
+        labels: Optional[list[OntologyLabel]] (default:= None)
             Labels for the context
-        comments: Optional[List[Comment]] (default:= None)
+        comments: Optional[list[Comment]] (default:= None)
             Comments for the context
 
         Returns
         -------
-        result: Dict[str, str]
+        result: dict[str, str]
             Result from the service
 
         Raises
         ------
         WacomServiceException
             If the ontology service returns an error code, exception is thrown.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             BASE_URI_TAG: base_uri if base_uri is not None else f'wacom:{name}',
             NAME_TAG: name,
             LABELS_TAG: [],
             COMMENTS_TAG: [],
             ICON_TAG: icon
         }
         for label in labels if labels is not None else []:
@@ -630,15 +631,31 @@
                                            timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Creation of concept failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def remove_context(self, auth_key: str, name: str, force: bool = False):
-        headers: Dict[str, str] = {
+        """Remove context.
+
+        Parameters
+        ----------
+        auth_key: str
+            Auth key from user.
+        name: str
+            Name of the context
+        force: bool (default:= False)
+            Force removal of context
+
+        Returns
+        -------
+        result: dict[str, str]
+            Result from the service
+        """
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{name}{"/force" if force else ""}'
         response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
 
@@ -652,15 +669,15 @@
         Parameters
         ----------
         auth_key: str
             User token (must have TenantAdmin) role
         context: str
             Name of the context.
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         url: str = f'{self.service_base_url}context/{context_url}/commit'
         response: Response = requests.put(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
@@ -679,15 +696,15 @@
             Name of the context.
 
         Returns
         -------
         rdf: str
             Ontology as RDFS / OWL  ontology
         """
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         url: str = f'{self.service_base_url}context/{context_url}/versions/rdf'
         response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.0/knowledge/services/tenant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
-from typing import List, Dict
 
 import requests
 from requests import Response
 
 from knowledge.services import USER_AGENT_STR
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException, USER_AGENT_HEADER_FLAG, \
     CONTENT_TYPE_HEADER_FLAG
 from knowledge.services.graph import AUTHORIZATION_HEADER_FLAG
 
+DEFAULT_TIMEOUT: int = 60
 
 class TenantManagementServiceAPI(WacomServiceAPIClient):
     """
     Tenant Management Service API
     -----------------------------
 
     Functionality:
         - List all tenants
         - Create tenants
-        - Create users
+
+    This is service is used to manage tenants. Only admins can use this service, as it requires the secret key for
+    tenant administration.
 
     Parameters
     ----------
     tenant_token: str
         Tenant Management token
     service_url: str
         URL of the service
@@ -46,26 +48,26 @@
 
     @tenant_management_token.setter
     def tenant_management_token(self, value: str):
         self.__tenant_management_token = value
 
     # ------------------------------------------ Tenants handling ------------------------------------------------------
 
-    def create_tenant(self, name: str) -> Dict[str, str]:
+    def create_tenant(self, name: str) -> dict[str, str]:
         """
         Creates a tenant.
 
         Parameters
         ----------
         name: str -
             Name of the tenant
 
         Returns
         -------
-        tenant_dict: Dict[str, str]
+        tenant_dict: dict[str, str]
 
         Newly created tenant structure.
         >>>     {
         >>>       "id": "<Tenant-ID>",
         >>>       "apiKey": "<Tenant-API-Key>",
         >>>       "name": "<Tenant-Name>"
         >>>    }
@@ -80,25 +82,27 @@
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {self.__tenant_management_token}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
         payload: dict = {
             'name': name
         }
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, timeout=DEFAULT_TIMEOUT,
+                                           verify=self.verify_calls)
         if response.ok:
             return response.json()
+        raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def listing_tenant(self) -> List[Dict[str, str]]:
+    def listing_tenant(self) -> list[dict[str, str]]:
         """
         Listing all tenants configured for this instance.
 
         Returns
         -------
-        tenants:  List[Dict[str, str]]
+        tenants:  list[dict[str, str]]
             List of tenants:
             >>> [
             >>>     {
             >>>        "id": "<Tenant-ID>",
             >>>        "ontologyName": "<Name-Of-Ontology>",
             >>>        "ontologyVersion": "<Version-Of-Ontology>",
             >>>        "isLocked": "<Lock-Flag>",
@@ -112,12 +116,12 @@
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{TenantManagementServiceAPI.TENANT_ENDPOINT}'
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {self.__tenant_management_token}'
         }
-        response: Response = requests.get(url, headers=headers, data={}, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, data={}, timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
-
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/services/users.py` & `personal_knowledge_library-1.0.0/knowledge/services/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
-from datetime import datetime
-from typing import Dict, List, Any, Tuple, Union
 import enum
+from datetime import datetime
+from typing import Any, Union
 
 import requests
 from dateutil.parser import parse, ParserError
 from requests import Response
 
 from knowledge.services import USER_AGENT_STR
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException
 
-
 # -------------------------------------- Constant flags ----------------------------------------------------------------
 TENANT_ID: str = 'tenantId'
 USER_ID_TAG: str = 'userId'
 LIMIT_TAG: str = 'limit'
 OFFSET_TAG: str = 'offset'
 ROLES_TAG: str = 'roles'
 META_DATA_TAG: str = 'metadata'
 INTERNAL_USER_ID_TAG: str = 'internalUserId'
 EXTERNAL_USER_ID_TAG: str = 'externalUserId'
 FORCE_TAG: str = 'force'
 CONTENT_TYPE_FLAG: str = 'Content-Type'
 TENANT_API_KEY_FLAG: str = 'x-tenant-api-key'
 USER_AGENT_TAG: str = "User-Agent"
+DEFAULT_TIMEOUT: int = 60
 
 
 class UserRole(enum.Enum):
     """
     UserRole
     --------
     Roles of the users in
     """
     USER = 'User'
     """User only has control over his personal entities."""
     ADMIN = 'TenantAdmin'
     """TenantAdmin has access to all entities independent of the access rights."""
 
 
-USER_ROLE_MAPPING: Dict[str, UserRole] = dict([(str(r.value), r) for r in UserRole])
+USER_ROLE_MAPPING: dict[str, UserRole] = dict([(str(r.value), r) for r in UserRole])
 
 
-class User(object):
+class User:
     """
     User
     -----
     In Personal Knowledge backend is linking a user to a shadow user which is used within the personal knowledge graph.
 
     Parameters
     ----------
     tenant_id: str
         Tenant id
     user_id: str
         User id
     external_user_id: str
         External user id, referencing the user to authentication system.
-    meta_data: Dict[str, Any]
+    meta_data: dict[str, Any]
         Metadata associated with user.
-    user_roles: List[UserRole]
+    user_roles: list[UserRole]
         List of user roles.
     """
 
-    def __init__(self, tenant_id: str, user_id: str, external_user_id: str, meta_data: Dict[str, Any],
-                 user_roles: List[UserRole]):
+    def __init__(self, tenant_id: str, user_id: str, external_user_id: str, meta_data: dict[str, Any],
+                 user_roles: list[UserRole]):
         self.__tenant_id: str = tenant_id
         self.__user_id: str = user_id
         self.__external_user_id: str = external_user_id
-        self.__meta_data: Dict[str, Any] = meta_data
-        self.__user_roles: List[UserRole] = user_roles
+        self.__meta_data: dict[str, Any] = meta_data
+        self.__user_roles: list[UserRole] = user_roles
 
     @property
     def id(self) -> str:
         """User id."""
         return self.__user_id
 
     @property
@@ -82,51 +82,51 @@
 
     @property
     def external_user_id(self) -> str:
         """External user id, referencing to external user authentication."""
         return self.__external_user_id
 
     @property
-    def meta_data(self) -> Dict[str, Any]:
+    def meta_data(self) -> dict[str, Any]:
         """Meta data for user."""
         return self.__meta_data
 
     @meta_data.setter
-    def meta_data(self, value: Dict[str, Any]):
+    def meta_data(self, value: dict[str, Any]):
         self.__meta_data = value
 
     @property
-    def user_roles(self) -> List[UserRole]:
+    def user_roles(self) -> list[UserRole]:
         """List of user roles"""
         return self.__user_roles
 
     @classmethod
-    def parse(cls, param: Dict[str, Any]) -> 'User':
+    def parse(cls, param: dict[str, Any]) -> 'User':
         """
         Parse user from dictionary.
         Parameters
         ----------
-        param: Dict[str, Any]
+        param: dict[str, Any]
             Dictionary containing user information.
 
         Returns
         -------
         user: User
             Instance of user.
         """
         user_id: str = param['id']
         tenant_id: str = param[TENANT_ID]
         external_user_id: str = param['externalUserId']
-        meta_data: Dict[str, Any] = {}
-        if META_DATA_TAG in param:
+        meta_data: dict[str, Any] = {}
+        if META_DATA_TAG in param and param[META_DATA_TAG] is not None:
             meta_data = param[META_DATA_TAG]
         # Support the old version of the user management service
         elif 'metaData' in param:
             meta_data = param['metaData']
-        user_roles: List[UserRole] = [USER_ROLE_MAPPING[r] for r in param['roles']]
+        user_roles: list[UserRole] = [USER_ROLE_MAPPING[r] for r in param['roles']]
         return User(tenant_id=tenant_id, user_id=user_id, external_user_id=external_user_id, meta_data=meta_data,
                     user_roles=user_roles)
 
     def __repr__(self):
         return f'<User: id:={self.id}, external user id:={self.external_user_id}, user roles:= {self.user_roles}]>'
 
 
@@ -150,28 +150,28 @@
     USER_DETAILS_ENDPOINT: str = f'{WacomServiceAPIClient.USER_ENDPOINT}/internal-id'
 
     def __init__(self, service_url: str = WacomServiceAPIClient.SERVICE_URL, service_endpoint: str = 'graph/v1'):
         super().__init__("UserManagementServiceAPI", service_url=service_url, service_endpoint=service_endpoint)
 
     # ------------------------------------------ Users handling --------------------------------------------------------
 
-    def create_user(self, tenant_key: str, external_id: str, meta_data: Dict[str, str] = None,
-                    roles: List[UserRole] = None) -> Tuple[User, str, str, datetime]:
+    def create_user(self, tenant_key: str, external_id: str, meta_data: dict[str, str] = None,
+                    roles: list[UserRole] = None) -> tuple[User, str, str, datetime]:
         """
         Creates user for a tenant.
 
         Parameters
         ----------
         tenant_key: str -
             API key for tenant
         external_id: str -
             External id of user identification service.
-        meta_data: Dict[str, str]
+        meta_data: dict[str, str]
             Meta-data dictionary.
-        roles: List[UserRole]
+        roles: list[UserRole]
             List of roles.
 
         Returns
         -------
         user: User
             Instance of the user
         token: str
@@ -192,65 +192,67 @@
             CONTENT_TYPE_FLAG: 'application/json'
         }
         payload: dict = {
             EXTERNAL_USER_ID_TAG: external_id,
             META_DATA_TAG: meta_data if meta_data is not None else {},
             ROLES_TAG: [r.value for r in roles] if roles is not None else [UserRole.USER.value]
         }
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, timeout=DEFAULT_TIMEOUT,
+                                           verify=self.verify_calls)
         if response.ok:
-            results: Dict[str, Union[str, Dict[str, str], List[str]]] = response.json()
+            results: dict[str, Union[str, dict[str, str], list[str]]] = response.json()
 
             try:
                 date_object: datetime = parse(results['token']['expirationDate'])
             except (ParserError, OverflowError) as _:
                 date_object: datetime = datetime.now()
 
             return User.parse(results['user']), results['token']['accessToken'], results['token']['refreshToken'], \
                 date_object
 
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def update_user(self, tenant_key: str, internal_id: str, external_id: str, meta_data: Dict[str, str] = None,
-                    roles: List[UserRole] = None):
+    def update_user(self, tenant_key: str, internal_id: str, external_id: str, meta_data: dict[str, str] = None,
+                    roles: list[UserRole] = None):
         """Updates user for a tenant.
 
         Parameters
         ----------
         tenant_key: str
             API key for tenant
         internal_id: str
             Internal id of semantic service.
         external_id: str
             External id of user identification service.
-        meta_data: Dict[str, str]
+        meta_data: dict[str, str]
             Meta-data dictionary.
-        roles: List[UserRole]
+        roles: list[UserRole]
             List of roles.
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{UserManagementServiceAPI.USER_ENDPOINT}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             TENANT_API_KEY_FLAG: tenant_key,
             CONTENT_TYPE_FLAG: 'application/json'
         }
-        payload: Dict[str, str] = {
+        payload: dict[str, str] = {
             META_DATA_TAG: meta_data if meta_data is not None else {},
             ROLES_TAG: [r.value for r in roles] if roles is not None else [UserRole.USER.value]
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             USER_ID_TAG: internal_id,
             EXTERNAL_USER_ID_TAG: external_id
         }
-        response: Response = requests.patch(url, headers=headers, json=payload, params=params, verify=self.verify_calls)
+        response: Response = requests.patch(url, headers=headers, json=payload, params=params, timeout=DEFAULT_TIMEOUT,
+                                            verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Updating user failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def delete_user(self, tenant_key: str, external_id: str, internal_id: str, force: bool = False):
         """Deletes user from tenant.
 
@@ -267,24 +269,25 @@
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{UserManagementServiceAPI.USER_ENDPOINT}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             TENANT_API_KEY_FLAG: tenant_key
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             USER_ID_TAG: internal_id,
             EXTERNAL_USER_ID_TAG: external_id,
             FORCE_TAG: force
         }
-        response: Response = requests.delete(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.delete(url, headers=headers, params=params, timeout=DEFAULT_TIMEOUT,
+                                             verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def user_internal_id(self, tenant_key: str, external_id: str) -> str:
         """User internal id.
 
         Parameters
@@ -305,52 +308,54 @@
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{UserManagementServiceAPI.USER_DETAILS_ENDPOINT}'
         headers: dict = {
             USER_AGENT_TAG: USER_AGENT_STR,
             TENANT_API_KEY_FLAG: tenant_key
         }
-        parameters: Dict[str, str] = {
+        parameters: dict[str, str] = {
             EXTERNAL_USER_ID_TAG:  external_id
         }
-        response: Response = requests.get(url, headers=headers, params=parameters, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=parameters, timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
-            response_dict: Dict[str, Any] = response.json()
+            response_dict: dict[str, Any] = response.json()
             return response_dict[INTERNAL_USER_ID_TAG]
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def listing_users(self, tenant_key: str, offset: int = 0, limit: int = 20) -> List[User]:
+    def listing_users(self, tenant_key: str, offset: int = 0, limit: int = 20) -> list[User]:
         """
         Listing all users configured for this instance.
 
         Parameters
         ----------
         tenant_key: str
             API key for tenant
         offset: int - [optional]
             Offset value to define starting position in list. [DEFAULT:= 0]
         limit: int - [optional]
             Define the limit of the list size. [DEFAULT:= 20]
 
         Returns
         -------
-        user: List[User]
+        user: list[User]
             List of users.
         """
         url: str = f'{self.service_base_url}{UserManagementServiceAPI.USER_ENDPOINT}'
-        headers: Dict[str, str] = {
+        headers: dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             TENANT_API_KEY_FLAG: tenant_key
         }
-        params: Dict[str, str] = {
+        params: dict[str, str] = {
             OFFSET_TAG: offset,
             LIMIT_TAG: limit
         }
-        response: Response = requests.get(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, params=params,  timeout=DEFAULT_TIMEOUT,
+                                          verify=self.verify_calls)
         if response.ok:
-            users: List[Dict[str, Any]] = response.json()
-            results: List[User] = []
+            users: list[dict[str, Any]] = response.json()
+            results: list[User] = []
             for u in users:
                 results.append(User.parse(u))
             return results
         raise WacomServiceException(f'Listing of users failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.0/knowledge/utils/rdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2022-23 Wacom Authors. All Rights Reserved.
-from typing import Optional, List
+from typing import Optional
 
 from rdflib import Graph, RDF, RDFS, OWL, URIRef, Literal
 
-from knowledge.base.entity import Comment, LanguageCode, OntologyLabel
-from knowledge.base.ontology import Ontology, OntologyClass, OntologyClassReference, OntologyPropertyReference, \
+from knowledge.base.entity import LanguageCode
+from knowledge.base.ontology import Comment, OntologyLabel, Ontology, OntologyClass, OntologyClassReference, \
+    OntologyPropertyReference, \
     OntologyProperty, PropertyType, INVERSE_DATA_PROPERTY_TYPE_MAPPING, DataPropertyType
 
 PREFERRED_LABEL: URIRef = URIRef('wacom:core#prefLabel')
 
 
 def ontology_import(rdf_content: str, tenant_id: str = '', context: str = '') -> Ontology:
     """Import Ontology from RDF ontology file.
@@ -29,16 +30,16 @@
         Instance of ontology.
     """
     rdf_graph: Graph = Graph().parse(data=rdf_content, format='xml')
     ontology: Ontology = Ontology()
     # Parse classes
     for cls_iri in [s for s, p, o in rdf_graph.triples((None, RDF.type, OWL.Class))]:
         subclass_of: Optional[OntologyClassReference] = None
-        comments: List[Comment] = []
-        labels: List[OntologyLabel] = []
+        comments: list[Comment] = []
+        labels: list[OntologyLabel] = []
         for _, _, o in rdf_graph.triples((cls_iri, RDFS.comment, None)):
             if isinstance(o, Literal):
                 comments.append(Comment(str(o), LanguageCode(o.language)))
         for _, _, o in rdf_graph.triples((cls_iri, PREFERRED_LABEL, None)):
             if isinstance(o, Literal):
                 labels.append(OntologyLabel(str(o), LanguageCode(o.language)))
         for _, _, o in rdf_graph.triples((cls_iri, RDFS.subClassOf, None)):
@@ -46,18 +47,18 @@
         ontology.add_class(OntologyClass(tenant_id=tenant_id, context=context,
                                          reference=OntologyClassReference.parse(str(cls_iri)),
                                          subclass_of=subclass_of, labels=labels, comments=comments))
 
     # Parse data properties
     for data_property_iri in [s for s, p, o in rdf_graph.triples((None, RDF.type, OWL.DatatypeProperty))]:
         subproperty_of: Optional[OntologyPropertyReference] = None
-        range_prop: List[DataPropertyType] = []
-        domain_prop: List[OntologyClassReference] = []
-        comments: List[Comment] = []
-        labels: List[OntologyLabel] = []
+        range_prop: list[DataPropertyType] = []
+        domain_prop: list[OntologyClassReference] = []
+        comments: list[Comment] = []
+        labels: list[OntologyLabel] = []
         inverse_prop: Optional[OntologyPropertyReference] = None
         for _, _, obj in rdf_graph.triples((data_property_iri, RDFS.range, None)):
             range_prop.append(INVERSE_DATA_PROPERTY_TYPE_MAPPING[str(obj)])
         for _, _, obj in rdf_graph.triples((data_property_iri, RDFS.domain, None)):
             domain_prop.append(OntologyClassReference.parse(str(obj)))
         for _, _, obj in rdf_graph.triples((data_property_iri, OWL.inverseOf, None)):
             inverse_prop = OntologyPropertyReference.parse(str(obj))
@@ -68,24 +69,24 @@
                 comments.append(Comment(str(o), LanguageCode(o.language)))
         for _, _, o in rdf_graph.triples((data_property_iri, PREFERRED_LABEL, None)):
             if isinstance(o, Literal):
                 labels.append(OntologyLabel(str(o), LanguageCode(o.language)))
         ontology.add_properties(OntologyProperty(kind=PropertyType.DATA_PROPERTY, tenant_id=tenant_id, context=context,
                                                  name=OntologyPropertyReference.parse(str(data_property_iri)),
                                                  property_range=range_prop, property_domain=domain_prop,
-                                                 subproperty_of=subproperty_of, inverse_property_of=inverse_prop,
+                                                 sub_property_of=subproperty_of, inverse_property_of=inverse_prop,
                                                  labels=labels, comments=comments))
     # Parse object properties
     for object_property_iri in [s for s, p, o in rdf_graph.triples((None, RDF.type, OWL.ObjectProperty))]:
         subproperty_of: Optional[OntologyPropertyReference] = None
-        obj_range_prop: List[OntologyClassReference] = []
-        domain_prop: List[OntologyClassReference] = []
+        obj_range_prop: list[OntologyClassReference] = []
+        domain_prop: list[OntologyClassReference] = []
         inverse_prop: Optional[OntologyPropertyReference] = None
-        comments: List[Comment] = []
-        labels: List[OntologyLabel] = []
+        comments: list[Comment] = []
+        labels: list[OntologyLabel] = []
         for _, _, o in rdf_graph.triples((object_property_iri, RDFS.range, None)):
             obj_range_prop.append(OntologyClassReference.parse(o))
         for _, _, o in rdf_graph.triples((object_property_iri, RDFS.domain, None)):
             domain_prop.append(OntologyClassReference.parse(o))
         for _, _, o in rdf_graph.triples((object_property_iri, OWL.inverseOf, None)):
             inverse_prop = OntologyPropertyReference.parse(o)
         for _, _, o in rdf_graph.triples((object_property_iri, RDFS.subPropertyOf, None)):
@@ -96,9 +97,9 @@
         for _, _, o in rdf_graph.triples((object_property_iri, PREFERRED_LABEL, None)):
             if isinstance(o, Literal):
                 labels.append(OntologyLabel(str(o), LanguageCode(o.language)))
         ontology.add_properties(OntologyProperty(kind=PropertyType.OBJECT_PROPERTY, tenant_id=tenant_id,
                                                  context=context,
                                                  name=OntologyPropertyReference.parse(object_property_iri),
                                                  property_range=obj_range_prop, property_domain=domain_prop,
-                                                 subproperty_of=subproperty_of, inverse_property_of=inverse_prop))
+                                                 sub_property_of=subproperty_of, inverse_property_of=inverse_prop))
     return ontology
```

### Comparing `personal_knowledge_library-0.9.6/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.0/knowledge/utils/wikipedia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
-from typing import Dict, Any
+from typing import Any
 
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
-from knowledge import logger
-from knowledge.base.entity import LanguageCode
-
 
 class ExtractionException(Exception):
     """
     Exception for extraction errors.
     """
-    pass
 
 
 def __extract_abstract__(title: str, language: str = 'en',  max_retries: int = 5, backoff_factor: float = 0.5) -> str:
     """Extracting an abstract.
 
     Parameters
     ----------
@@ -29,15 +25,15 @@
         language_code of Wikipedia
 
     Returns
     -------
     abstract: str
         Abstract of the wikipedia article
     """
-    params: Dict[str, str] = {
+    params: dict[str, str] = {
         "action": "query",
         "format": "json",
         "titles": title,
         "prop": "extracts",
         "exintro": "1",
         "explaintext": "1",
         "redirects": "1"
@@ -48,15 +44,15 @@
     with requests.Session() as session:
         retries: Retry = Retry(total=max_retries,
                                backoff_factor=backoff_factor,
                                status_forcelist=[502, 503, 504])
         session.mount(mount_point, HTTPAdapter(max_retries=retries))
         response: Response = session.get(url, params=params)
         if response.ok:
-            result: Dict[str, Any] = response.json()
+            result: dict[str, Any] = response.json()
             if 'query' in result:
                 pages = result['query']['pages']
                 if len(pages) == 1:
                     for v in pages.values():
                         return v.get('extract', '')
     raise ExtractionException(f"Abstract for article with {title} in language_code {language} cannot be extracted.")
 
@@ -65,28 +61,28 @@
     """
     Extracting thumbnail from Wikipedia.
 
     Parameters
     ----------
     title: str
         Title of wikipedia article
-    language: LanguageCode
+    language: str
         Language code of Wikipedia
     max_retries: int
         Maximum number of retries
     backoff_factor: float
         A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
         second try without a delay)
 
     Returns
     -------
     url: str
         thumb URL
     """
-    params: Dict[str, str] = {
+    params: dict[str, str] = {
         "action": "query",
         "format": "json",
         "titles": title,
         "prop": "pageimages",
         "pithumbsize": "400"
     }
 
@@ -96,23 +92,21 @@
         retries: Retry = Retry(total=max_retries,
                                backoff_factor=backoff_factor,
                                status_forcelist=[502, 503, 504])
         session.mount(mount_point, HTTPAdapter(max_retries=retries))
         response: Response = session.get(url, params=params)
         if response.ok:
             result: dict = response.json()
-            try:
-                if 'query' in result:
-                    pages: dict = result['query']['pages']
-                    if len(pages) == 1:
-                        for v in pages.values():
-                            if 'thumbnail' in v:
-                                return v['thumbnail']['source']
-            except Exception as e:
-                logger.error(e)
+            if 'query' in result:
+                pages: dict = result['query']['pages']
+                if len(pages) == 1:
+                    for v in pages.values():
+                        if 'thumbnail' in v:
+                            return v['thumbnail']['source']
+
     raise ExtractionException(f"Thumbnail for article with {title} in language_code {language} cannot be extracted.")
 
 
 def get_wikipedia_summary(title: str, lang: str = 'en') -> str:
     """
     Extracting summary wikipedia URL.
 
@@ -121,38 +115,38 @@
     title: str
         Title of the Wikipedia article
     lang: str
         Language code
 
     Returns
     -------
-    result: Dict[str, str]
+    result: dict[str, str]
         Summary dict with image and summary text
     """
     try:
         summary: str = __extract_abstract__(title, lang)
     except ExtractionException as _:
         summary = ''
     return summary
 
 
-def get_wikipedia_summary_image(title: str, lang: str = 'en') -> Dict[str, str]:
+def get_wikipedia_summary_image(title: str, lang: str = 'en') -> dict[str, str]:
     """
     Extracting summary image and abstract for wikipedia URL.
 
     Parameters
     ----------
     title: str
         Title of the Wikipedia article
     lang: str
         Language code
 
     Returns
     -------
-    result: Dict[str, str]
+    result: dict[str, str]
         Summary dict with image and summary text
     """
     try:
         thumbnail: str = __extract_thumb__(title, lang)
     except ExtractionException as _:
         thumbnail = ''
     try:
@@ -161,27 +155,27 @@
         summary = ''
     return {
         'summary-image': thumbnail,
         'summary-text': summary
     }
 
 
-def get_wikipedia_summary_url(wiki_url: str, lang: str = 'en') -> Dict[str, str]:
+def get_wikipedia_summary_url(wiki_url: str, lang: str = 'en') -> dict[str, str]:
     """
     Extracting summary image and abstract for wikipedia URL.
     Parameters
     ----------
     wiki_url: str
         Wikipedia URL
     lang: str
         Language code
 
     Returns
     -------
-    result: Dict[str, str]
+    result: dict[str, str]
         Result dictionary.
     """
     title: str = wiki_url.split('/')[-1]
     return {
         'url': wiki_url,
         'summary-image': __extract_thumb__(title, lang),
         'summary-text': __extract_abstract__(title, lang)
```

### Comparing `personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 0.9.6
+Version: 1.0.0
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
@@ -16,34 +16,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Wacom Personal Knowledge Library
+# Wacom Private Knowledge Library
 
-The library and the cloud services are still under development. 
-The required access tokens are only available for selected partner companies.
-
-> :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
+The required tenant API key is only available for selected partner companies.
+Please contact your Wacom representative for more information.
 
 ## Introduction
 
 In knowledge management there is a distinction between data, information and knowledge.
 In the domain of digital ink this means:
 
 - **Data** - The equivalent would be the ink strokes
 - **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
 - **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
 
 The following illustration shows the different layers of knowledge:
 ![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
 
-For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
+For handling semantics, Wacom introduced the Wacom Private Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
 
 This library provide simplified access to Wacom's personal knowledge cloud service.
 It contains:
 
 - Basic datastructures for Ontology object and entities from the knowledge graph
 - Clients for the REST APIs
 - Connector for Wikidata public knowledge graph
@@ -56,19 +54,45 @@
 
 **Entity service:**
 
 - List all entities
 - Add entities to knowledge graph
 - Access object properties
 
+**Search service:**
+
+- Search for entities for labels and descriptions with a given language
+- Search for literals (data properties) 
+- Search for relations (object properties)
+
+**Group service:**
+
+- List all groups
+- Add groups, modify groups, delete groups
+- Add users and entities to groups
+
+**Ontology service:**
+
+- List all Ontology structures
+- Modify Ontology structures
+
+**Named Entity Linking service:**
+
+- Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
+
+**Wikidata connector:**
+
+- Import entities from Wikidata
+- Mapping Wikidata entities to WPK entities
+
 # Technology stack
 
 ## Domain Knowledge
 
-The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
+The tasks of the ontology within Wacom's private knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
 The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
 
 - Foundation for structured data, knowledge representation as concepts and relations among concepts
 - Being explicit definitions of shared vocabularies for interoperability
 - Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
 - Can be used for problem solving
 
@@ -85,23 +109,45 @@
 - Extract knowledge from various sources (Connectors)
 - Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
 - Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
 
 
 # Functionality
 
+## Import Format
+
+For importing entities into the knowledge graph, the tools/import_entities.py script can be used.
+
+The ThingObject support a NDJSON based import format, where the individual JSON files can contain the following structure.
+
+| Field name             | Subfield name | Data Structure | Description                                                                                    |
+|------------------------|---------------|----------------|------------------------------------------------------------------------------------------------|
+| source_reference_id    |               | str            | A unique identifier for the entity used in the source system                                  |
+| source_system          |               | str            | The source system describes the original source of the entity, such as wikidata, youtube, ... |
+| image                  |               | str            | A string representing the URL of the entity's icon.                                           |
+| labels                 |               | array          | An array of label objects, where each object has the following fields:                       |
+|                        | value         | str            | A string representing the label text in the specified locale.                                |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+|                        | isMain        | bool           | A boolean flag indicating if this label is the main label for the entity (true) or an alias (false). |
+| descriptions           |               | array          | An array of description objects, where each object has the following fields:                 |
+|                        | description   | str            | A string representing the description text in the specified locale.                          |
+|                        | locale        | str            | A string combining the ISO-3166 country code and the ISO-639 language code (e.g., "en-US").  |
+| type                   |               | str            | A string representing the IRI of the ontology class for this entity.                         |
+| literals               |               | array[map]     | An array of data property objects, where each object has the following fields:               |
+
+
 ## Access API
 
 The personal knowledge graph backend is implement as a multi-tenancy system.
 Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
 
 ![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
 
 In general, a tenant with their users, groups, and entities are logically separated.
-Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
+Physically the entities are store in the same instance of the Wacom Private Knowledge (WPK) backend database system.
 
 The user management is rather limited, each organisation must provide their own authentication service and user management.
 The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
 
 The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
 While users for each tenant can be created by the owner of the **Tenant API Key**.
 You will receive this token from the system owner after the creation of the tenant.
@@ -169,15 +215,15 @@
 
 ### Entity handling
 
 This samples shows how to work with graph service.
 
 ```python
 import argparse
-from typing import Optional, List, Dict
+from typing import Optional
 
 from knowledge.base.entity import LanguageCode, Description, Label
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.services.graph import WacomKnowledgeService
 
 # ------------------------------- Knowledge entities -------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
@@ -194,69 +240,70 @@
 ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
 IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
 HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
 CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
 HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
 
 
-def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
+def print_entity(display_entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService,
+                 short: bool = False):
     """
     Printing entity details.
 
     Parameters
     ----------
-    entity: ThingObject
+    display_entity: ThingObject
         Entity with properties
     list_idx: int
         Index with a list
     auth_key: str
         Authorization key
     client: WacomKnowledgeService
         Knowledge graph client
     short: bool
         Short summary
     """
-    print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
-    if len(entity.label) > 0:
+    print(f'[{list_idx}] : {display_entity.uri} <{display_entity.concept_type.iri}>')
+    if len(display_entity.label) > 0:
         print('    | [Labels]')
-        for la in entity.label:
+        for la in display_entity.label:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if not short:
-        if len(entity.alias) > 0:
+        if len(display_entity.alias) > 0:
             print('    | [Alias]')
-            for la in entity.alias:
+            for la in display_entity.alias:
                 print(f'    |     |- "{la.content}"@{la.language_code}')
             print('    |')
-        if len(entity.data_properties) > 0:
+        if len(display_entity.data_properties) > 0:
             print('    | [Attributes]')
             for data_property, labels in entity.data_properties.items():
                 print(f'    |    |- {data_property.iri}:')
                 for li in labels:
                     print(f'    |    |-- "{li.value}"@{li.language_code}')
             print('    |')
 
-        relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
+        relations_obj: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
                                                                                           uri=entity.uri)
         if len(relations_obj) > 0:
             print('    | [Relations]')
             for re in relations_obj.values():
                 print(f'    |--- {re.relation.iri}: ')
                 print(f'           |- [Incoming]: {re.incoming_relations} ')
                 print(f'           |- [Outgoing]: {re.outgoing_relations}')
         print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
@@ -268,48 +315,48 @@
     print('-----------------------------------------------------------------------------------------------------------')
     print(' First step: Find Leonardo da Vinci in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     s_idx: int = 1
-    for entity in res_entities:
+    for res_entity in res_entities:
         #  Entity must be a person and the label match with full string
-        if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
-            leo = entity
+        if res_entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [la.content for la in res_entity.label]:
+            leo = res_entity
             break
 
     print('-----------------------------------------------------------------------------------------------------------')
     print(' What artwork exists in the knowledge graph.')
     print('-----------------------------------------------------------------------------------------------------------')
-    relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
+    relations_dict: dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
                                                                                                  uri=leo.uri)
     print(f' Artwork of {leo.label}')
     print('-----------------------------------------------------------------------------------------------------------')
     idx: int = 1
     if CREATED in relations_dict:
         for e in relations_dict[CREATED].outgoing_relations:
             print(f' [{idx}] {e.uri}: {e.label}')
             idx += 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(' Let us create a new piece of artwork.')
     print('-----------------------------------------------------------------------------------------------------------')
 
     # Main labels for entity
-    artwork_labels: List[Label] = [
+    artwork_labels: list[Label] = [
         Label('Ginevra Gherardini', LanguageCode('en_US')),
         Label('Ginevra Gherardini', LanguageCode('de_DE'))
     ]
     # Alias labels for entity
-    artwork_alias: List[Label] = [
+    artwork_alias: list[Label] = [
         Label("Ginevra", LanguageCode('en_US')),
         Label("Ginevra", LanguageCode('de_DE'))
     ]
     # Topic description
-    artwork_description: List[Description] = [
+    artwork_description: list[Description] = [
         Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
         Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
     ]
     # Topic
     artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
                                               description=artwork_description,
                                               icon=ICON)
@@ -404,36 +451,40 @@
     while True:
         # pull
         entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
                                                                         limit=100)
         pulled_entities: int = len(entities)
         if pulled_entities == 0:
             break
-        delete_uris: List[str] = [e.uri for e in entities]
+        delete_uris: list[str] = [e.uri for e in entities]
         print(f'Cleanup. Delete entities: {delete_uris}')
         knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
         page_number += 1
         page_id = next_page_id
     print('-----------------------------------------------------------------------------------------------------------')
 ```
 
 ### Named Entity Linking 
 
 Performing Named Entity Linking (NEL) on text and Universal Ink Model.
 
 ```python
 import argparse
-from typing import List, Dict
+
+import urllib3
 
 from knowledge.base.entity import LanguageCode
 from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
 from knowledge.nel.base import KnowledgeGraphEntity
 from knowledge.nel.engine import WacomEntityLinkingEngine
 from knowledge.services.graph import WacomKnowledgeService
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+
 LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
 TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
 
 
 def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
     """
     Printing entity details.
@@ -457,15 +508,15 @@
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
     if len(thing.label) > 0:
         print('    | [Alias]')
         for la in thing.alias:
             print(f'    |     |- "{la.content}"@{la.language_code}')
         print('    |')
-    relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
+    relations: dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
     if len(thing.data_properties) > 0:
         print('    | [Attributes]')
         for data_property, labels in thing.data_properties.items():
             print(f'    |    |- {data_property.iri}:')
             for li in labels:
                 print(f'    |    |-- "{li.value}"@{li.language_code}')
         print('    |')
@@ -476,34 +527,34 @@
             print(f'           |- [Incoming]: {re.incoming_relations} ')
             print(f'           |- [Outgoing]: {re.outgoing_relations}')
     print()
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Named Entity Linking Knowledge access",
         service_url=args.instance)
     #  Wacom Named Entity Linking
     nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
         service_url=args.instance,
         service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
     )
     # Use special tenant for testing:  Unit-test tenant
     user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-    entities: List[KnowledgeGraphEntity] = nel_client.\
+    entities: list[KnowledgeGraphEntity] = nel_client.\
         link_personal_entities(auth_key=user_token, text=TEXT,
                                language_code=LANGUAGE_CODE)
     idx: int = 1
     print('-----------------------------------------------------------------------------------------------------------')
     print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
     print('-----------------------------------------------------------------------------------------------------------')
     for e in entities:
@@ -514,67 +565,74 @@
 
 ### Access Management
 
 The sample shows, how access to entities can be shared with a group of users or the tenant.
 
 ```python
 import argparse
-from typing import List
+
 from knowledge.base.entity import LanguageCode, Label, Description
 from knowledge.base.ontology import OntologyClassReference, ThingObject
 from knowledge.services.base import WacomServiceException
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.group import GroupManagementServiceAPI, Group
 from knowledge.services.users import UserManagementServiceAPI
 
 # ------------------------------- User credential ----------------------------------------------------------------------
 TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
 
 
 def create_entity() -> ThingObject:
+    """Create a new entity.
+
+    Returns
+    -------
+    entity: ThingObject
+        Entity object
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Hidden', LanguageCode('en_US')),
         Label('Versteckt', LanguageCode('de_DE')),
         Label('隠れた', LanguageCode('ja_JP'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
     # Topic
     topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
     return topic_object
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+    parser.add_argument("-i", "--instance", default='https://private-knowledge.wacom.com',
                         help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom personal knowledge REST API Client
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
                                                                     service_url=args.instance)
     # User Management
     user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
     # Group Management
     group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     # Now, we create a users
-    u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
-    u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
-    u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
+    u1, u1_token, _, _ = user_management.create_user(TENANT_KEY, "u1")
+    u2, u2_token, _, _ = user_management.create_user(TENANT_KEY, "u2")
+    u3, u3_token, _, _ = user_management.create_user(TENANT_KEY, "u3")
 
     # Now, let's create an entity
     thing: ThingObject = create_entity()
     entity_uri: str = knowledge_client.create_entity(u1_token, thing)
     # Only user 1 can access the entity from cloud storage
     my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
     print(f'User is the owner of {my_thing.owner}')
@@ -628,20 +686,34 @@
 ```
 
 ### Ontology Creation
 
 The samples show how the ontology can be extended and new entities can be added using the added classes.
 
 ```python
+# -*- coding: utf-8 -*-
+# Copyright © 2021-2022 Wacom Authors. All Rights Reserved.
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language_code governing permissions and
+#  limitations under the License.
 import argparse
-from typing import List, Optional
+from typing import Optional
 
-from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
+from knowledge.base.entity import Label, LanguageCode, Description
 from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
-    DataProperty
+    DataProperty, OntologyContext
 from knowledge.services.graph import WacomKnowledgeService
 from knowledge.services.ontology import OntologyService
 
 # ------------------------------- Constants ----------------------------------------------------------------------------
 LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
 CONTEXT_NAME: str = 'core'
 # Wacom Base Ontology Types
@@ -651,21 +723,28 @@
 # Demo Object property
 IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
 # Demo Data property
 STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
 
 
 def create_artist() -> ThingObject:
+    """
+    Create a new artist entity.
+    Returns
+    -------
+    instance: ThingObject
+        Artist entity
+    """
     # Main labels for entity
-    topic_labels: List[Label] = [
+    topic_labels: list[Label] = [
         Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
     ]
 
     # Topic description
-    topic_description: List[Description] = [
+    topic_description: list[Description] = [
         Description('Hidden entity to explain access management.', LanguageCode('en_US')),
         Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
     ]
 
     data_property: DataProperty = DataProperty(content='Salaj',
                                                property_ref=STAGE_NAME,
                                                language_code=LanguageCode('en_US'))
@@ -673,52 +752,50 @@
     artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
     artist.add_data_property(data_property)
     return artist
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Private Knowledge.",
                         required=True)
-    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    parser.add_argument("-i", "--instance", default="https://private-knowledge.wacom.com", help="URL of instance")
     args = parser.parse_args()
     TENANT_KEY: str = args.tenant
     EXTERNAL_USER_ID: str = args.user
     # Wacom Ontology REST API Client
     ontology_client: OntologyService = OntologyService(service_url=args.instance)
-    admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    admin_token, refresh_token, expiration_time = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
     knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
         application_name="Ontology Creation Demo",
         service_url=args.instance)
-    contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
-    if len(contexts) == 0:
+    context: Optional[OntologyContext] = ontology_client.context(admin_token)
+    if context is None:
         # First, create a context for the ontology
         ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
         context_name: str = CONTEXT_NAME
     else:
-        context_name: str = contexts[0].context
+        context_name: str = context.context
     # Creating a class which is a subclass of a person
-    ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
+    ontology_client.create_concept(admin_token, context_name, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
 
     # Object properties
-    ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
-                                           ranges_cls=[PERSON_TYPE],
-                                           inverse_of=None, subproperty_of=None)
+    ontology_client.create_object_property(auth_key=admin_token, context=context_name,
+                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE],
+                                           ranges_cls=[PERSON_TYPE], inverse_of=None, subproperty_of=None)
     # Data properties
-    ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
+    ontology_client.create_data_property(auth_key=admin_token, context=context_name,
                                          reference=STAGE_NAME,
                                          domains_cls=[ARTIST_TYPE],
                                          ranges_cls=[DataPropertyType.STRING],
                                          subproperty_of=None)
-
     # Commit the changes of the ontology. This is very important to confirm changes.
-    ontology_client.commit(admin_token, CONTEXT_NAME)
+    ontology_client.commit(admin_token, context_name)
     # Trigger graph service. After the update the ontology is available and the new entities can be created
     knowledge_client.ontology_update(admin_token)
 
     res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
                                                                     language_code=LanguageCode('en_US'), limit=1000)
     leo: Optional[ThingObject] = None
     for entity in res_entities:
@@ -726,14 +803,15 @@
         if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
             leo = entity
             break
 
     artist_student: ThingObject = create_artist()
     artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
     knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
+
 ```
 
 ## Tools
 
 The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
 
 ### Listing script
@@ -743,15 +821,15 @@
 ```bash
 >> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
@@ -759,50 +837,56 @@
 >> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 - _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
 - _-p, --images (optional)_ - Include the images in the dump.
 - _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
  
-### Push entities script
+### Import entities script
 
 Pushing entities to knowledge graph.
 
 ```bash
->> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
+>> python import_entities.py [-h] [-u USER] [-t TENANT] [-g GROUP_NAME] [-r] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge 
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
 - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
-  
-### Reset
+- _-g GROUP_NAME, --group_id GROUP_NAME_ - Group name where the entities will be assigned to. 
+- _-p , --public_ - Group name where the entities will be assigned to.
 
-Resets a tenant by removing entities, groups, and users. 
+### Wikidata scrapper
 
 ```bash
->> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
+usage: wikidata_scrapper.py [-h] -u USER -t TENANT [-i INSTANCE] [-c CACHE]
+                            [-m MAPPING] [-d DEPTH]
+                            [-l LANGUAGES [LANGUAGES ...]]
+wikidata_scrapper.py: error: the following arguments are required: -u/--user, -t/--tenant
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
 - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
+- _-c CACHE, --cache CACHE_ - Path to entities that must are exports in import format.
+- _-m MAPPING, --mapping MAPPING_ - Mapping file to configure the wikidata mapping.
+- _-d DEPTH, --depth DEPTH_ - Depth of the graph to be scrapped.
+- _-l LANGUAGES [LANGUAGES ...], --languages LANGUAGES [LANGUAGES ...]_ - Languages to be scrapped.
   
 # Documentation
 
 You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
 API documentation is available [here](./docs/).
 
 ## Contributing
```

### Comparing `personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.0/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 knowledge/base/ontology.py
 knowledge/nel/__init__.py
 knowledge/nel/base.py
 knowledge/nel/engine.py
 knowledge/ontomapping/__init__.py
 knowledge/ontomapping/manager.py
 knowledge/public/__init__.py
+knowledge/public/cache.py
 knowledge/public/helper.py
 knowledge/public/relations.py
 knowledge/public/wikidata.py
 knowledge/services/__init__.py
 knowledge/services/base.py
 knowledge/services/graph.py
 knowledge/services/group.py
```

### Comparing `personal_knowledge_library-0.9.6/setup.py` & `personal_knowledge_library-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 import pathlib
+import sys
 from setuptools import setup, find_packages
 
-import sys
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 7)
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
-    sys.stderr.write("""
+    sys.stderr.write(f"""
 ==========================
 Unsupported Python version
 ==========================
-This version of personal knowledge lib requires Python {}.{}, but you're trying to
-install it on Python {}.{}.
+This version of personal knowledge lib requires Python {REQUIRED_PYTHON}.
+
 This may be because you are using a version of pip that doesn't
 understand the python_requires classifier. Make sure you
 have pip >= 9.0 and setuptools >= 24.2, then try again:
     $ python -m pip install --upgrade pip setuptools
 This will install the latest version of personal-knowledge-library which works on your
 version of Python. If you can't upgrade your pip (or Python), request
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
-""".format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
+""")
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "0.9.6"
+__version__ = "1.0.0"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
@@ -47,21 +47,25 @@
     include_package_data=True,
     install_requires=[
         "requests>=2.25.1",
         "python-dateutil>=2.8.2",
         "PyJWT>=2.6.0",
         "tqdm>=4.62.0",
         "ndjson>=0.3.1",
-        "rdflib>=6.3.2"
+        "rdflib>=6.3.2",
+        "python-dateutil"
     ],
     extras_require={
     },
     tests_require=(
         'pytest',
-        'pytest-cov'
+        'pytest-cov',
+        'faker',
+        'ontospy',
+        'pytest-env'
     ),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

