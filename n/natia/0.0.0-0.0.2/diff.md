# Comparing `tmp/natia-0.0.0.tar.gz` & `tmp/natia-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natia-0.0.0.tar", last modified: Wed Jun 14 19:51:41 2023, max compression
+gzip compressed data, was "natia-0.0.2.tar", last modified: Thu Jun 15 10:01:53 2023, max compression
```

## Comparing `natia-0.0.0.tar` & `natia-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.190854 natia-0.0.0/
--rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-14 19:51:41.190679 natia-0.0.0/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)       92 2023-06-11 20:41:21.000000 natia-0.0.0/README.md
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.184414 natia-0.0.0/natia/
--rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-08 18:38:30.000000 natia-0.0.0/natia/__init__.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.185555 natia-0.0.0/natia/kb/
--rw-r--r--   0 isaac      (501) staff       (20)       81 2023-06-13 12:56:54.000000 natia-0.0.0/natia/kb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     3943 2023-06-14 19:27:25.000000 natia-0.0.0/natia/kb/client.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.186434 natia-0.0.0/natia/kb/docdb/
--rw-r--r--   0 isaac      (501) staff       (20)       69 2023-06-11 13:40:05.000000 natia-0.0.0/natia/kb/docdb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     2148 2023-06-14 14:17:40.000000 natia-0.0.0/natia/kb/docdb/base.py
--rw-r--r--   0 isaac      (501) staff       (20)     4385 2023-06-14 19:26:07.000000 natia-0.0.0/natia/kb/docdb/mongodb.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.187381 natia-0.0.0/natia/kb/document/
--rw-r--r--   0 isaac      (501) staff       (20)      105 2023-06-11 13:20:21.000000 natia-0.0.0/natia/kb/document/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     1169 2023-06-12 14:13:47.000000 natia-0.0.0/natia/kb/document/document.py
--rw-r--r--   0 isaac      (501) staff       (20)     1677 2023-06-12 13:42:17.000000 natia-0.0.0/natia/kb/document/id.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.187996 natia-0.0.0/natia/kb/vecdb/
--rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:03:25.000000 natia-0.0.0/natia/kb/vecdb/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     1947 2023-06-14 18:33:32.000000 natia-0.0.0/natia/kb/vecdb/base.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.189114 natia-0.0.0/natia/kb/vecdb/doc2vec/
--rw-r--r--   0 isaac      (501) staff       (20)      201 2023-06-13 13:04:22.000000 natia-0.0.0/natia/kb/vecdb/doc2vec/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)      595 2023-06-13 13:29:12.000000 natia-0.0.0/natia/kb/vecdb/doc2vec/base.py
--rw-r--r--   0 isaac      (501) staff       (20)     1914 2023-06-14 18:06:00.000000 natia-0.0.0/natia/kb/vecdb/doc2vec/doc2text.py
--rw-r--r--   0 isaac      (501) staff       (20)     1354 2023-06-13 07:21:21.000000 natia-0.0.0/natia/kb/vecdb/doc2vec/sentence_transformer.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.189661 natia-0.0.0/natia/kb/vecdb/qdrant/
--rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:02:26.000000 natia-0.0.0/natia/kb/vecdb/qdrant/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)    10840 2023-06-14 18:42:20.000000 natia-0.0.0/natia/kb/vecdb/qdrant/client.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.184965 natia-0.0.0/natia.egg-info/
--rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-14 19:51:41.000000 natia-0.0.0/natia.egg-info/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)      677 2023-06-14 19:51:41.000000 natia-0.0.0/natia.egg-info/SOURCES.txt
--rw-r--r--   0 isaac      (501) staff       (20)        1 2023-06-14 19:51:41.000000 natia-0.0.0/natia.egg-info/dependency_links.txt
--rw-r--r--   0 isaac      (501) staff       (20)       12 2023-06-14 19:51:41.000000 natia-0.0.0/natia.egg-info/top_level.txt
--rw-r--r--   0 isaac      (501) staff       (20)      581 2023-06-14 19:51:22.000000 natia-0.0.0/pyproject.toml
--rw-r--r--   0 isaac      (501) staff       (20)       38 2023-06-14 19:51:41.190909 natia-0.0.0/setup.cfg
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-14 19:51:41.190333 natia-0.0.0/tests/
--rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-11 12:31:34.000000 natia-0.0.0/tests/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)      210 2023-06-14 18:52:53.000000 natia-0.0.0/tests/test_docdb.py
--rw-r--r--   0 isaac      (501) staff       (20)     3029 2023-06-14 19:39:35.000000 natia-0.0.0/tests/test_kb.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.434562 natia-0.0.2/
+-rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 10:01:53.434421 natia-0.0.2/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)       92 2023-06-11 20:41:21.000000 natia-0.0.2/README.md
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431172 natia-0.0.2/natia/
+-rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-08 18:38:30.000000 natia-0.0.2/natia/__init__.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431879 natia-0.0.2/natia/kb/
+-rw-r--r--   0 isaac      (501) staff       (20)       81 2023-06-13 12:56:54.000000 natia-0.0.2/natia/kb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     4545 2023-06-15 09:17:24.000000 natia-0.0.2/natia/kb/client.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432338 natia-0.0.2/natia/kb/docdb/
+-rw-r--r--   0 isaac      (501) staff       (20)       69 2023-06-11 13:40:05.000000 natia-0.0.2/natia/kb/docdb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     3509 2023-06-15 08:41:14.000000 natia-0.0.2/natia/kb/docdb/base.py
+-rw-r--r--   0 isaac      (501) staff       (20)     5442 2023-06-15 08:38:31.000000 natia-0.0.2/natia/kb/docdb/mongodb.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432747 natia-0.0.2/natia/kb/document/
+-rw-r--r--   0 isaac      (501) staff       (20)      105 2023-06-11 13:20:21.000000 natia-0.0.2/natia/kb/document/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1169 2023-06-12 14:13:47.000000 natia-0.0.2/natia/kb/document/document.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1677 2023-06-12 13:42:17.000000 natia-0.0.2/natia/kb/document/id.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.432992 natia-0.0.2/natia/kb/vecdb/
+-rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:03:25.000000 natia-0.0.2/natia/kb/vecdb/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1947 2023-06-14 18:33:32.000000 natia-0.0.2/natia/kb/vecdb/base.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.433530 natia-0.0.2/natia/kb/vecdb/doc2vec/
+-rw-r--r--   0 isaac      (501) staff       (20)      201 2023-06-13 13:04:22.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)      595 2023-06-13 13:29:12.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/base.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1914 2023-06-14 18:06:00.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/doc2text.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1354 2023-06-13 07:21:21.000000 natia-0.0.2/natia/kb/vecdb/doc2vec/sentence_transformer.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.433872 natia-0.0.2/natia/kb/vecdb/qdrant/
+-rw-r--r--   0 isaac      (501) staff       (20)       67 2023-06-13 13:02:26.000000 natia-0.0.2/natia/kb/vecdb/qdrant/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)    11304 2023-06-15 09:38:00.000000 natia-0.0.2/natia/kb/vecdb/qdrant/client.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.431631 natia-0.0.2/natia.egg-info/
+-rw-r--r--   0 isaac      (501) staff       (20)      422 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)      677 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac      (501) staff       (20)        1 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac      (501) staff       (20)       12 2023-06-15 10:01:53.000000 natia-0.0.2/natia.egg-info/top_level.txt
+-rw-r--r--   0 isaac      (501) staff       (20)      563 2023-06-15 10:01:31.000000 natia-0.0.2/pyproject.toml
+-rw-r--r--   0 isaac      (501) staff       (20)       38 2023-06-15 10:01:53.434600 natia-0.0.2/setup.cfg
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-06-15 10:01:53.434232 natia-0.0.2/tests/
+-rw-r--r--   0 isaac      (501) staff       (20)        0 2023-06-11 12:31:34.000000 natia-0.0.2/tests/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)      210 2023-06-14 18:52:53.000000 natia-0.0.2/tests/test_docdb.py
+-rw-r--r--   0 isaac      (501) staff       (20)     3730 2023-06-15 09:40:20.000000 natia-0.0.2/tests/test_kb.py
```

### Comparing `natia-0.0.0/natia/kb/client.py` & `natia-0.0.2/natia/kb/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,14 +97,31 @@
                 'vec_db': inserted_document_ids_in_vec_db
             }
         
         return {
             'doc_db': inserted_document_ids_in_doc_db,
             'vec_db': []
         }
+        
+    def delete_documents(
+            self, 
+            documents: Iterable[Document]
+        ) -> dict[str, list[DocumentID]]:
+        
+        deletion_result = {}
+        
+        # delete from document database
+        deleted_document_ids = self._doc_db_client.delete_documents(documents)
+        deletion_result['doc_db'] = deleted_document_ids
+        
+        # delete from vector database
+        deleted_document_ids = self._vec_db_client.delete_documents_by_ids(deleted_document_ids)
+        deletion_result['vec_db'] = deleted_document_ids
+        
+        return deletion_result
 
     def retrieve_similar_documents(
             self, 
             query: str,
             n_similar_documents: int
         ) -> list[Document]:
```

### Comparing `natia-0.0.0/natia/kb/docdb/base.py` & `natia-0.0.2/natia/kb/vecdb/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,70 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
+from itertools import filterfalse
 from ..document import Document, DocumentID
 
-class BaseDocumentDatabaseClient(ABC):
+class BaseVectorDatabaseClient(ABC):
     
     @property
     @abstractmethod
     def collection_name(self) -> str:
         pass
     
-    @abstractmethod
-    def insert_document(self, document: Document) -> DocumentID:
-        pass
-    
-    @abstractmethod
-    def insert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
-        pass
+    @staticmethod
+    def filter_out_documents_without_ids(documents: Iterable[Document]) -> list[Document]:
+        
+        return list(filterfalse(
+            lambda document: document.id is None,
+            documents
+        ))
+        
     
     @abstractmethod
-    def find_document(self, *args, **kwargs) -> Optional[Document]:
-        """Find one document in the database satisfying some requirements.
-
-        Returns
-        -------
-            Optional[Document]: None if no ducument is found.
-        """
+    def upsert_document(self, document: Document) -> Optional[DocumentID]:
         pass
     
-    @abstractmethod
-    def find_documents(self, *args, **kwargs) -> list[Document]:
-        """Find all documents in the databae satisfying some requirements.
-
-        Returns
-        -------
-            list[Document]: An empty list if no ducument is found.
-        """
-        pass
+    def upsert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
+        
+        document_ids = []
+        for document in documents:
+            document_id = self.upsert_document(document)
+            if document_id is not None:
+                document_ids.append(document_id)
+        
+        return document_ids
     
     @abstractmethod
-    def find_document_by_id(self, id: DocumentID) -> Optional[Document]:
-        """Find one document in the databae by its ID.
-
-        Parameters
-        ----------
-            id (DocumentID): Document ID.
+    def delete_document_by_id(self, id: DocumentID) -> None:
+        """Delete the vector embedding of the document specified by its ID.
 
-        Returns
-        -------
-            Optional[Document]: None if no ducument is found.
+        Paramerters
+        -----------
+            id (DocumentID): ID of the document to delete.
         """
+        
         pass
     
-    def find_documents_by_ids(self, ids: Iterable[DocumentID]) -> list[Document]:
-        """Find one document in the databae by its ID.
-
-        Parameters
-        ----------
-            ids (Iterable[DocumentID]): Document IDs.
-            If a list of IDs is passed in,
-            then the documents to find will be returned in the same order.
+    def delete_documents_by_ids(self, ids: Iterable[DocumentID]) -> None:
+        """Delete all vector embeddings of the documents specified by their IDs.
 
-        Returns
-        -------
-            list[Document]: An empty list if no ducument is found.
+        Paramerters
+        -----------
+            ids (Iterable[DocumentID]): IDs of the documents to delete.
         """
         
-        documents = []
         for id in ids:
-            document = self.find_document_by_id(id)
-            documents.append(document)
+            self.delete_document_by_id(id)
         
-        return documents
+    @abstractmethod
+    def retrieve_similar_document_ids(
+            self, 
+            query: str, 
+            n_similar_documents: int
+        ) -> list[DocumentID]:
+        pass
     
     @abstractmethod
     def drop_collection(self, collection_name: str) -> None:
         pass
+        
+
```

### Comparing `natia-0.0.0/natia/kb/docdb/mongodb.py` & `natia-0.0.2/natia/kb/docdb/mongodb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import (
     Any, 
     Self,
     Optional,
     Iterable
 )
+from itertools import filterfalse
 import pymongo
 from .base import BaseDocumentDatabaseClient
 from ..document import Document, DocumentID
 
 class MongoDBClient(BaseDocumentDatabaseClient, pymongo.MongoClient):
     
     def __init__(self, *args, **kwargs) -> None:
@@ -140,14 +141,53 @@
         for document_id in ids:
             document = self.find_document_by_id(document_id)
             if document is not None:
                 documents.append(document)
         
         return documents
     
+    def delete_documents(
+            self, 
+            documents: Iterable[Document]
+        ) -> list[DocumentID]:
+        
+        # extract docuemnt IDs
+        document_ids = list(map(
+            lambda document: document.id, 
+            documents
+        ))
+        
+        # get deleted document IDs
+        deleted_document_ids = self.delete_documents_by_ids(document_ids)
+        
+        return deleted_document_ids
+        
+    def delete_documents_by_ids(
+            self, 
+            ids: Iterable[DocumentID]
+        ) -> list[DocumentID]:
+        
+        # get nonempty IDs
+        ids = self.filter_out_empty_document_ids(ids)
+        
+        # convert each ID to ObjectId instance
+        document_ids_as_objectids = list(map(
+            lambda id: id.to_objectid(),
+            ids
+        ))
+        
+        # delete documents
+        self._collection.delete_many({
+            '_id': {
+                '$in': document_ids_as_objectids
+            }
+        })
+        
+        return ids
+    
     def drop_collection(self, collection_name: str) -> None:
         
         if self._database is None:
             raise RuntimeError('no database is opened')
         
         self._database.drop_collection(collection_name)
```

### Comparing `natia-0.0.0/natia/kb/document/document.py` & `natia-0.0.2/natia/kb/document/document.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/natia/kb/document/id.py` & `natia-0.0.2/natia/kb/document/id.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/natia/kb/vecdb/base.py` & `natia-0.0.2/natia/kb/docdb/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,133 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
 from itertools import filterfalse
 from ..document import Document, DocumentID
 
-class BaseVectorDatabaseClient(ABC):
+class BaseDocumentDatabaseClient(ABC):
     
     @property
     @abstractmethod
     def collection_name(self) -> str:
         pass
     
     @staticmethod
-    def filter_out_documents_without_ids(documents: Iterable[Document]) -> list[Document]:
+    def filter_out_documents_with_ids(
+            documents: Iterable[Document]
+        ) -> list[Document]:
         
-        return list(filterfalse(
+        documents = list(filter(
             lambda document: document.id is None,
             documents
         ))
         
+        return documents
     
-    @abstractmethod
-    def upsert_document(self, document: Document) -> Optional[DocumentID]:
-        pass
+    @staticmethod
+    def filter_out_documents_without_ids(
+            documents: Iterable[Document]
+        ) -> list[Document]:
+        
+        documents = list(filterfalse(
+            lambda document: document.id is None,
+            documents
+        ))
+        
+        return documents
     
-    def upsert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
+    @staticmethod
+    def filter_out_empty_document_ids(
+            ids: Iterable[DocumentID]
+        ) -> list[DocumentID]:
         
-        document_ids = []
-        for document in documents:
-            document_id = self.upsert_document(document)
-            if document_id is not None:
-                document_ids.append(document_id)
+        ids = list(filterfalse(
+            lambda id: id is None,
+            ids
+        ))
         
-        return document_ids
+        return ids
+    
+    @abstractmethod
+    def insert_document(self, document: Document) -> DocumentID:
+        pass
     
     @abstractmethod
-    def delete_document_by_id(self, id: DocumentID) -> None:
-        """Delete the vector embedding of the document specified by its ID.
+    def insert_documents(self, documents: Iterable[Document]) -> list[DocumentID]:
+        pass
+    
+    @abstractmethod
+    def find_document(self, *args, **kwargs) -> Optional[Document]:
+        """Find one document in the database satisfying some requirements.
 
-        Paramerters
-        -----------
-            id (DocumentID): ID of the document to delete.
+        Returns
+        -------
+            Optional[Document]: None if no ducument is found.
         """
-        
         pass
     
-    def delete_documents_by_ids(self, ids: Iterable[DocumentID]) -> None:
-        """Delete all vector embeddings of the documents specified by their IDs.
+    @abstractmethod
+    def find_documents(self, *args, **kwargs) -> list[Document]:
+        """Find all documents in the databae satisfying some requirements.
+
+        Returns
+        -------
+            list[Document]: An empty list if no ducument is found.
+        """
+        pass
+    
+    @abstractmethod
+    def find_document_by_id(self, id: DocumentID) -> Optional[Document]:
+        """Find one document in the databae by its ID.
+
+        Parameters
+        ----------
+            id (DocumentID): Document ID.
+
+        Returns
+        -------
+            Optional[Document]: None if no ducument is found.
+        """
+        pass
+    
+    def find_documents_by_ids(self, ids: Iterable[DocumentID]) -> list[Document]:
+        """Find one document in the databae by its ID.
+
+        Parameters
+        ----------
+            ids (Iterable[DocumentID]): Document IDs.
+            If a list of IDs is passed in,
+            then the documents to find will be returned in the same order.
 
-        Paramerters
-        -----------
-            ids (Iterable[DocumentID]): IDs of the documents to delete.
+        Returns
+        -------
+            list[Document]: An empty list if no ducument is found.
         """
         
+        documents = []
         for id in ids:
-            self.delete_document_by_id(id)
+            document = self.find_document_by_id(id)
+            documents.append(document)
         
+        return documents
+
     @abstractmethod
-    def retrieve_similar_document_ids(
+    def delete_documents(
             self, 
-            query: str, 
-            n_similar_documents: int
+            documents: Iterable[Document]
         ) -> list[DocumentID]:
         pass
     
+    def delete_document(
+            self, 
+            document: Document
+        ) -> Optional[DocumentID]:
+        
+        deleted_document_ids = self.delete_documents([document])
+        
+        if len(deleted_document_ids) > 0:
+            return deleted_document_ids[0]
+        else:
+            return None
+    
     @abstractmethod
     def drop_collection(self, collection_name: str) -> None:
         pass
-        
-
```

### Comparing `natia-0.0.0/natia/kb/vecdb/doc2vec/base.py` & `natia-0.0.2/natia/kb/vecdb/doc2vec/base.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/natia/kb/vecdb/doc2vec/doc2text.py` & `natia-0.0.2/natia/kb/vecdb/doc2vec/doc2text.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/natia/kb/vecdb/doc2vec/sentence_transformer.py` & `natia-0.0.2/natia/kb/vecdb/doc2vec/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/natia/kb/vecdb/qdrant/client.py` & `natia-0.0.2/natia/kb/vecdb/qdrant/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -304,29 +304,47 @@
         self.delete(
             collection_name=self.collection_name,
             points_selector=PointIdsList(
                 points=[str(id.to_uuid())]
             )
         )
     
-    def delete_documents_by_ids(self, ids: Iterable[DocumentID]) -> None:
+    def delete_documents_by_ids(self, ids: Iterable[DocumentID]) -> list[DocumentID]:
+        
+        # do nothing
+        if len(ids) == 0:
+            return []
         
         # convert IDs to a list of UUID strings
         document_ids = list(map(
             lambda document_id: str(document_id.to_uuid()),
             ids
         ))
         
+        # find actual records to delete
+        records = self.retrieve(
+            collection_name=self.collection_name,
+            ids=document_ids
+        )
+        
         # delete from database
         self.delete(
             collection_name=self.collection_name,
             points_selector=PointIdsList(
                 points=document_ids
             )
         )
+        
+       # extract IDs
+        deleted_document_ids = list(map(
+            lambda record: DocumentID(UUID(record.id)),
+            records
+        ))
+        
+        return deleted_document_ids
 
     def retrieve_similar_document_ids(
             self, 
             query: str,
             n_similar_documents: int
         ) -> list[DocumentID]:
```

### Comparing `natia-0.0.0/natia.egg-info/SOURCES.txt` & `natia-0.0.2/natia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `natia-0.0.0/pyproject.toml` & `natia-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 [tool.setuptools.packages.find]
 where = ['.']
 exclude = ['playground']  # empty by default
 namespaces = false  # true by default
 
 [project]
 name = 'natia'
-version = '0.0.0'
+version = '0.0.2'
 authors = [
     {name = 'Isaac Fei', email = 'isaac.omega.fei@gmail.com'},
 ]
 description = 'Natia stands for NATural IterAction. We aim to build a toolkit that leverages LLMs.'
 readme = 'README.md'
 requires-python = '>=3.11'
-dependencies = []
 
 [project.urls]
 Homepage = 'https://github.com/Isaac-Fate/natural-interact'
```

