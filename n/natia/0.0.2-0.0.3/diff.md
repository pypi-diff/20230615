# Comparing `tmp/natia-0.0.2.tar.gz` & `tmp/natia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natia-0.0.2.tar", last modified: Thu Jun 15 10:01:53 2023, max compression
+gzip compressed data, was "natia-0.0.3.tar", last modified: Thu Jun 15 16:54:47 2023, max compression
```

## Comparing `natia-0.0.2.tar` & `natia-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.434562 natia-0.0.2/
--rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 10:01:53.434421 natia-0.0.2/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)       92 2023-06-11 20:41:21.000000 natia-0.0.2/README.md
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431172 natia-0.0.2/natia/
--rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-08 18:38:30.000000 natia-0.0.2/natia/__init__.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431879 natia-0.0.2/natia/kb/
--rw-r--r--   0 isaac      (501) staff       (20)       81 2023-06-13 12:56:54.000000 natia-0.0.2/natia/kb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     4545 2023-06-15 09:17:24.000000 natia-0.0.2/natia/kb/client.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432338 natia-0.0.2/natia/kb/docdb/
--rw-r--r--   0 isaac      (501) staff       (20)       69 2023-06-11 13:40:05.000000 natia-0.0.2/natia/kb/docdb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     3509 2023-06-15 08:41:14.000000 natia-0.0.2/natia/kb/docdb/base.py
--rw-r--r--   0 isaac      (501) staff       (20)     5442 2023-06-15 08:38:31.000000 natia-0.0.2/natia/kb/docdb/mongodb.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432747 natia-0.0.2/natia/kb/document/
--rw-r--r--   0 isaac      (501) staff       (20)      105 2023-06-11 13:20:21.000000 natia-0.0.2/natia/kb/document/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     1169 2023-06-12 14:13:47.000000 natia-0.0.2/natia/kb/document/document.py
--rw-r--r--   0 isaac      (501) staff       (20)     1677 2023-06-12 13:42:17.000000 natia-0.0.2/natia/kb/document/id.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432992 natia-0.0.2/natia/kb/vecdb/
--rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:03:25.000000 natia-0.0.2/natia/kb/vecdb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     1947 2023-06-14 18:33:32.000000 natia-0.0.2/natia/kb/vecdb/base.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.433530 natia-0.0.2/natia/kb/vecdb/doc2vec/
--rw-r--r--   0 isaac      (501) staff       (20)      201 2023-06-13 13:04:22.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)      595 2023-06-13 13:29:12.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/base.py
--rw-r--r--   0 isaac      (501) staff       (20)     1914 2023-06-14 18:06:00.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/doc2text.py
--rw-r--r--   0 isaac      (501) staff       (20)     1354 2023-06-13 07:21:21.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/sentence_transformer.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.433872 natia-0.0.2/natia/kb/vecdb/qdrant/
--rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:02:26.000000 natia-0.0.2/natia/kb/vecdb/qdrant/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)    11304 2023-06-15 09:38:00.000000 natia-0.0.2/natia/kb/vecdb/qdrant/client.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431631 natia-0.0.2/natia.egg-info/
--rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)      677 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/SOURCES.txt
--rw-r--r--   0 isaac      (501) staff       (20)        1 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/dependency_links.txt
--rw-r--r--   0 isaac      (501) staff       (20)       12 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/top_level.txt
--rw-r--r--   0 isaac      (501) staff       (20)      563 2023-06-15 10:01:31.000000 natia-0.0.2/pyproject.toml
--rw-r--r--   0 isaac      (501) staff       (20)       38 2023-06-15 10:01:53.434600 natia-0.0.2/setup.cfg
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.434232 natia-0.0.2/tests/
--rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-11 12:31:34.000000 natia-0.0.2/tests/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)      210 2023-06-14 18:52:53.000000 natia-0.0.2/tests/test_docdb.py
--rw-r--r--   0 isaac      (501) staff       (20)     3730 2023-06-15 09:40:20.000000 natia-0.0.2/tests/test_kb.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.646561 natia-0.0.3/
+-rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 16:54:47.646309 natia-0.0.3/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)       92 2023-06-11 20:41:21.000000 natia-0.0.3/README.md
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.640003 natia-0.0.3/natia/
+-rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-08 18:38:30.000000 natia-0.0.3/natia/__init__.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.641081 natia-0.0.3/natia/kb/
+-rw-r--r--   0 isaac      (501) staff       (20)       81 2023-06-13 12:56:54.000000 natia-0.0.3/natia/kb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     5424 2023-06-15 14:59:41.000000 natia-0.0.3/natia/kb/client.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.641944 natia-0.0.3/natia/kb/docdb/
+-rw-r--r--   0 isaac      (501) staff       (20)       69 2023-06-11 13:40:05.000000 natia-0.0.3/natia/kb/docdb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     3851 2023-06-15 14:51:52.000000 natia-0.0.3/natia/kb/docdb/base.py
+-rw-r--r--   0 isaac      (501) staff       (20)     6652 2023-06-15 15:16:05.000000 natia-0.0.3/natia/kb/docdb/mongodb.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.642759 natia-0.0.3/natia/kb/document/
+-rw-r--r--   0 isaac      (501) staff       (20)      105 2023-06-11 13:20:21.000000 natia-0.0.3/natia/kb/document/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1169 2023-06-12 14:13:47.000000 natia-0.0.3/natia/kb/document/document.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1677 2023-06-12 13:42:17.000000 natia-0.0.3/natia/kb/document/id.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.643359 natia-0.0.3/natia/kb/vecdb/
+-rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:03:25.000000 natia-0.0.3/natia/kb/vecdb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1947 2023-06-14 18:33:32.000000 natia-0.0.3/natia/kb/vecdb/base.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.644557 natia-0.0.3/natia/kb/vecdb/doc2vec/
+-rw-r--r--   0 isaac      (501) staff       (20)      201 2023-06-13 13:04:22.000000 natia-0.0.3/natia/kb/vecdb/doc2vec/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)      595 2023-06-13 13:29:12.000000 natia-0.0.3/natia/kb/vecdb/doc2vec/base.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1914 2023-06-14 18:06:00.000000 natia-0.0.3/natia/kb/vecdb/doc2vec/doc2text.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1354 2023-06-13 07:21:21.000000 natia-0.0.3/natia/kb/vecdb/doc2vec/sentence_transformer.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.645115 natia-0.0.3/natia/kb/vecdb/qdrant/
+-rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:02:26.000000 natia-0.0.3/natia/kb/vecdb/qdrant/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)    11304 2023-06-15 09:38:00.000000 natia-0.0.3/natia/kb/vecdb/qdrant/client.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.640511 natia-0.0.3/natia.egg-info/
+-rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 16:54:47.000000 natia-0.0.3/natia.egg-info/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)      677 2023-06-15 16:54:47.000000 natia-0.0.3/natia.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac      (501) staff       (20)        1 2023-06-15 16:54:47.000000 natia-0.0.3/natia.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac      (501) staff       (20)       12 2023-06-15 16:54:47.000000 natia-0.0.3/natia.egg-info/top_level.txt
+-rw-r--r--   0 isaac      (501) staff       (20)      563 2023-06-15 15:39:49.000000 natia-0.0.3/pyproject.toml
+-rw-r--r--   0 isaac      (501) staff       (20)       38 2023-06-15 16:54:47.646618 natia-0.0.3/setup.cfg
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 16:54:47.645932 natia-0.0.3/tests/
+-rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-11 12:31:34.000000 natia-0.0.3/tests/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)      210 2023-06-14 18:52:53.000000 natia-0.0.3/tests/test_docdb.py
+-rw-r--r--   0 isaac      (501) staff       (20)     4019 2023-06-15 15:38:06.000000 natia-0.0.3/tests/test_kb.py
```

### Comparing `natia-0.0.2/natia/kb/client.py` & `natia-0.0.3/natia/kb/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,20 +98,50 @@
             }
         
         return {
             'doc_db': inserted_document_ids_in_doc_db,
             'vec_db': []
         }
         
+    def update_documents(
+            self, 
+            documents: Iterable[Document],
+            do_insert: bool = True
+        ) -> dict[str, list[DocumentID]]:
+        
+        update_result = {
+            'doc_db': [],
+            'vec_db': []
+        }
+        
+        # update documents in document database
+        document_ids = self._doc_db_client.update_documents(
+            documents=documents, 
+            do_insert=do_insert
+        )
+        update_result['doc_db'] = document_ids
+        
+        # find the corresponding documents
+        documents = self._doc_db_client.find_documents_by_ids(document_ids)
+        
+        # update embedding vectors
+        self.update_document_embeddings(documents)
+        update_result['vec_db'] = document_ids
+        
+        return update_result
+        
     def delete_documents(
             self, 
             documents: Iterable[Document]
         ) -> dict[str, list[DocumentID]]:
         
-        deletion_result = {}
+        deletion_result = {
+            'doc_db': [],
+            'vec_db': []
+        }
         
         # delete from document database
         deleted_document_ids = self._doc_db_client.delete_documents(documents)
         deletion_result['doc_db'] = deleted_document_ids
         
         # delete from vector database
         deleted_document_ids = self._vec_db_client.delete_documents_by_ids(deleted_document_ids)
```

### Comparing `natia-0.0.2/natia/kb/docdb/base.py` & `natia-0.0.3/natia/kb/docdb/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,25 @@
             lambda id: id is None,
             ids
         ))
         
         return ids
     
     @abstractmethod
-    def insert_document(self, document: Document) -> DocumentID:
-        pass
-    
-    @abstractmethod
     def insert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
         pass
     
+    def insert_document(self, document: Document) -> Optional[DocumentID]:
+        
+        document_ids = self.insert_documents([document])
+        if len(document_ids) > 0:
+            return document_ids[0]
+        else:
+            return None
+    
     @abstractmethod
     def find_document(self, *args, **kwargs) -> Optional[Document]:
         """Find one document in the database satisfying some requirements.
 
         Returns
         -------
             Optional[Document]: None if no ducument is found.
@@ -104,14 +108,22 @@
         
         documents = []
         for id in ids:
             document = self.find_document_by_id(id)
             documents.append(document)
         
         return documents
+    
+    @abstractmethod
+    def update_documents(
+            self, 
+            documents: Iterable[Document],
+            do_insert: bool = True
+        ) -> list[DocumentID]:
+        pass
 
     @abstractmethod
     def delete_documents(
             self, 
             documents: Iterable[Document]
         ) -> list[DocumentID]:
         pass
```

### Comparing `natia-0.0.2/natia/kb/docdb/mongodb.py` & `natia-0.0.3/natia/kb/docdb/mongodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import (
     Any, 
     Self,
     Optional,
     Iterable
 )
 from itertools import filterfalse
+from natia.kb.document import DocumentID
 import pymongo
+from pymongo.database import Database
+from pymongo.collection import Collection
 from .base import BaseDocumentDatabaseClient
 from ..document import Document, DocumentID
 
 class MongoDBClient(BaseDocumentDatabaseClient, pymongo.MongoClient):
     
     def __init__(self, *args, **kwargs) -> None:
         
         super().__init__(*args, **kwargs)
         
-        self._database = None
-        self._collection = None
+        self._database: Optional[Database] = None
+        self._collection: Optional[Collection] = None
     
     @property
     def collection_name(self) -> str:
         return self._collection.name
     
     @classmethod
     def connect_to_host_port(cls, host: str, port: int) -> Self:
@@ -59,31 +62,34 @@
         
         if self._database is None:
             raise RuntimeError('no database is opened')
         
         self._collection = self._database.get_collection(collection_name)
         
         return self
-    
-    def insert_document(self, document: Document) -> DocumentID:
-        inserted_result = self._collection.insert_one(document)
-        inserted_id = DocumentID(inserted_result.inserted_id)
-        return inserted_id
         
     def insert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
         
+        # filter out those documents that have IDs
+        # since they are already in the collection
+        documents = self.filter_out_documents_with_ids(documents)
+        
         # stop here if there is no document to insert
         if len(documents) == 0:
             return []
         
-        inserted_result = self._collection.insert_many(documents)
+        # get insertion result from MongoDB
+        insertion_result = self._collection.insert_many(documents)
+        
+        # convert to document IDs
         inserted_ids = list(map(
             DocumentID,
-            inserted_result.inserted_ids
+            insertion_result.inserted_ids
         ))
+        
         return inserted_ids
         
     def find_document(self, filter: Optional[Any] = None) -> Optional[Document]:
         
         # find document in the collection
         document: Optional[dict] = self._collection.find_one(filter)
         
@@ -122,14 +128,15 @@
             document.id = document_id
             
             documents.append(document)
         
         return documents
     
     def find_document_by_id(self, id: DocumentID) -> Optional[Document]:
+        
         return self.find_document(id.to_objectid())
     
     def find_documents_by_ids(self, ids: Iterable[DocumentID]) -> list[Document]:
         
         # use find_many method provided by MongoDB 
         # may not be helpful since the number of documents to find 
         # is not large,
@@ -141,14 +148,47 @@
         for document_id in ids:
             document = self.find_document_by_id(document_id)
             if document is not None:
                 documents.append(document)
         
         return documents
     
+    def update_documents(
+            self, 
+            documents: Iterable[Document],
+            do_insert: bool = True
+        ) -> list[DocumentID]:
+        
+        document_ids: list[DocumentID] = []
+        
+        for document in documents:
+            
+            # the document is not in the collection yet
+            if document.id is None:
+                if do_insert:
+                    document_id = self.insert_document(document)
+                    if document_id is not None:
+                        document_ids.append(document_id)
+                else:
+                    continue
+            
+            # update the document
+            self._collection.update_one(
+                filter={
+                    '_id': document.id.to_objectid()
+                },
+                update={
+                    '$set': document
+                }
+            )
+            
+            document_ids.append(document.id)
+        
+        return document_ids
+    
     def delete_documents(
             self, 
             documents: Iterable[Document]
         ) -> list[DocumentID]:
         
         # extract docuemnt IDs
         document_ids = list(map(
```

### Comparing `natia-0.0.2/natia/kb/document/document.py` & `natia-0.0.3/natia/kb/document/document.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/document/id.py` & `natia-0.0.3/natia/kb/document/id.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/vecdb/base.py` & `natia-0.0.3/natia/kb/vecdb/base.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/vecdb/doc2vec/base.py` & `natia-0.0.3/natia/kb/vecdb/doc2vec/base.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/vecdb/doc2vec/doc2text.py` & `natia-0.0.3/natia/kb/vecdb/doc2vec/doc2text.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/vecdb/doc2vec/sentence_transformer.py` & `natia-0.0.3/natia/kb/vecdb/doc2vec/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia/kb/vecdb/qdrant/client.py` & `natia-0.0.3/natia/kb/vecdb/qdrant/client.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/natia.egg-info/SOURCES.txt` & `natia-0.0.3/natia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `natia-0.0.2/pyproject.toml` & `natia-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ['.']
 exclude = ['playground']  # empty by default
 namespaces = false  # true by default
 
 [project]
 name = 'natia'
-version = '0.0.2'
+version = '0.0.3'
 authors = [
     {name = 'Isaac Fei', email = 'isaac.omega.fei@gmail.com'},
 ]
 description = 'Natia stands for NATural IterAction. We aim to build a toolkit that leverages LLMs.'
 readme = 'README.md'
 requires-python = '>=3.11'
```

### Comparing `natia-0.0.2/tests/test_kb.py` & `natia-0.0.3/tests/test_kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,24 +96,31 @@
             n_similar_documents=2
         )
         print('Similar documents:')
         pprint(documents)
         print()
         
         # udpate documents
+        documents[0]['value'] = 100
+        update_result = knowledge_base_client.update_documents(documents)
+        print('Update result:')
+        pprint(update_result)
+        pprint(knowledge_base_client._doc_db_client.find_documents_by_ids(update_result['doc_db']))
+        print()
+        
         updated_document_ids = knowledge_base_client.update_document_embeddings(documents)
         pprint(updated_document_ids)
         
         # clean up
         
         doc_db_client.drop_collection(
             collection_name='test-document-collection'
         )
         
         vec_db_client.drop_collection(
             collection_name='test-vector-database-collection'
         )
-        
-        
 
 if __name__ == '__main__':
-    unittest.main()
+    
+    unittest.main()
+
```

