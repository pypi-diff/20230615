# Comparing `tmp/citrusdb-0.3.3.tar.gz` & `tmp/citrusdb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.3.3.tar", last modified: Tue Jun  6 08:47:19 2023, max compression
+gzip compressed data, was "citrusdb-0.4.0.tar", last modified: Thu Jun 15 19:17:20 2023, max compression
```

## Comparing `citrusdb-0.3.3.tar` & `citrusdb-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.551436 citrusdb-0.3.3/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.3.3/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-06 08:47:19.551316 citrusdb-0.3.3/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1666 2023-06-01 13:10:08.000000 citrusdb-0.3.3/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.548664 citrusdb-0.3.3/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      166 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549589 citrusdb-0.3.3/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     6257 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.547635 citrusdb-0.3.3/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549817 citrusdb-0.3.3/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550268 citrusdb-0.3.3/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3056 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1469 2023-06-06 08:43:11.000000 citrusdb-0.3.3/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550576 citrusdb-0.3.3/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.3.3/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.550907 citrusdb-0.3.3/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-01 13:09:38.000000 citrusdb-0.3.3/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.549238 citrusdb-0.3.3/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2249 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      649 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-06 08:47:19.000000 citrusdb-0.3.3/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-06 08:47:19.551137 citrusdb-0.3.3/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.3.3/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.3.3/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)      672 2023-06-06 08:47:02.000000 citrusdb-0.3.3/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-06 08:47:19.551468 citrusdb-0.3.3/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      894 2023-06-06 08:47:10.000000 citrusdb-0.3.3/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.323471 citrusdb-0.4.0/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.4.0/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2341 2023-06-15 19:17:20.323342 citrusdb-0.4.0/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1758 2023-06-15 19:08:11.000000 citrusdb-0.4.0/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.320189 citrusdb-0.4.0/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321187 citrusdb-0.4.0/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     6648 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321320 citrusdb-0.4.0/citrusdb/db/
+-rw-r--r--   0 debabrata   (501) staff       (20)     1039 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321522 citrusdb-0.4.0/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321890 citrusdb-0.4.0/citrusdb/db/postgres/
+-rw-r--r--   0 debabrata   (501) staff       (20)     3888 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1479 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1445 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322389 citrusdb-0.4.0/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     3101 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1472 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322616 citrusdb-0.4.0/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322952 citrusdb-0.4.0/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.320819 citrusdb-0.4.0/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2341 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      770 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.323173 citrusdb-0.4.0/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.4.0/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.4.0/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-15 19:16:46.000000 citrusdb-0.4.0/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-15 19:17:20.323501 citrusdb-0.4.0/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-15 19:14:39.000000 citrusdb-0.4.0/setup.py
```

### Comparing `citrusdb-0.3.3/LICENSE` & `citrusdb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/PKG-INFO` & `citrusdb-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: citrusdb
-Version: 0.3.3
-Summary: open-source vector database. store and retrieve embeddings for your next project!
-Home-page: https://github.com/0xDebabrata/citrus
-Author: Debabrata Mondal
-Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
-Project-URL: Homepage, https://github.com/0xDebabrata/citrus
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🍋 citrus.
 ### open-source (distributed) vector database
 
 <p align="center">
   Special thanks to
 </p>
 <p align="center">
@@ -41,33 +26,36 @@
 import citrusdb
 
 # Initialize client
 citrus = citrusdb.Client()
 
 # Create index
 citrus.create_index(
+  name="example",
   max_elements=1000,            # increases dynamically as you insert more vectors
-  persist_directory="db"       # save data and load index from disk
 )
 ```
 
 #### 2. Insert elements
 ```py
 ids = [1, 2, 3]
 documents = [
   "Your time is limited, so don't waste it living someone else's life",
   "I'd rather be optimistic and wrong than pessimistic and right.",
   "Running a start-up is like chewing glass and staring into the abyss."
 ]
 
-citrus.add(ids, documents=documents)
+citrus.add(index="example", ids=ids, documents=documents)
 ```
 You can directly pass vector embeddings as well. If you're passing a list of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate the embeddings. Please reach out if you're looking for support from a different provider!
 
 #### 3. Search
 ```py
-result, distances = citrus.query("What is it like to launch a startup", k=1)
+result, distances = citrus.query(index="example", documents=["What is it like to launch a startup"], k=1)
 ```
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
+
+## Facing issues?
+Feel free to open issues on this repository! Discord server coming soon!
```

#### html2text {}

```diff
@@ -1,31 +1,23 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.3 Summary: open-source vector
-database. store and retrieve embeddings for your next project! Home-page:
-https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
-Debabrata Mondal
-js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # ð citrus. ### open-source (distributed) vector
-database
+# ð citrus. ### open-source (distributed) vector database
                                Special thanks to
                                    [DevKit]
                    DevKit_-_The_Essential_Developer_Toolkit
                                    DSoC 2023
 ## Installation ``` pip install citrusdb ``` ## Getting started #### 1. Create
 index ```py import citrusdb # Initialize client citrus = citrusdb.Client() #
-Create index citrus.create_index( max_elements=1000, # increases dynamically as
-you insert more vectors persist_directory="db" # save data and load index from
-disk ) ``` #### 2. Insert elements ```py ids = [1, 2, 3] documents = [ "Your
-time is limited, so don't waste it living someone else's life", "I'd rather be
-optimistic and wrong than pessimistic and right.", "Running a start-up is like
-chewing glass and staring into the abyss." ] citrus.add(ids,
-documents=documents) ``` You can directly pass vector embeddings as well. If
-you're passing a list of strings like we have done here, ensure you have your
-`OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate
-the embeddings. Please reach out if you're looking for support from a different
-provider! #### 3. Search ```py result, distances = citrus.query("What is it
-like to launch a startup", k=1) ``` Go launch a repl on [Replit](https://
-replit.com) and see what result you get after running the query! `result` will
+Create index citrus.create_index( name="example", max_elements=1000, #
+increases dynamically as you insert more vectors ) ``` #### 2. Insert elements
+```py ids = [1, 2, 3] documents = [ "Your time is limited, so don't waste it
+living someone else's life", "I'd rather be optimistic and wrong than
+pessimistic and right.", "Running a start-up is like chewing glass and staring
+into the abyss." ] citrus.add(index="example", ids=ids, documents=documents)
+``` You can directly pass vector embeddings as well. If you're passing a list
+of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the
+environment. By default we use OpenAI to to generate the embeddings. Please
+reach out if you're looking for support from a different provider! #### 3.
+Search ```py result, distances = citrus.query(index="example", documents=["What
+is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
+/replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
-(https://replit.com/@debabratajr/pokedex-search)
+(https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
+open issues on this repository! Discord server coming soon!
```

### Comparing `citrusdb-0.3.3/README.md` & `citrusdb-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: citrusdb
+Version: 0.4.0
+Summary: open-source vector database. store and retrieve embeddings for your next project!
+Home-page: https://github.com/0xDebabrata/citrus
+Author: Debabrata Mondal
+Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
+Project-URL: Homepage, https://github.com/0xDebabrata/citrus
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🍋 citrus.
 ### open-source (distributed) vector database
 
 <p align="center">
   Special thanks to
 </p>
 <p align="center">
@@ -26,33 +41,36 @@
 import citrusdb
 
 # Initialize client
 citrus = citrusdb.Client()
 
 # Create index
 citrus.create_index(
+  name="example",
   max_elements=1000,            # increases dynamically as you insert more vectors
-  persist_directory="db"       # save data and load index from disk
 )
 ```
 
 #### 2. Insert elements
 ```py
 ids = [1, 2, 3]
 documents = [
   "Your time is limited, so don't waste it living someone else's life",
   "I'd rather be optimistic and wrong than pessimistic and right.",
   "Running a start-up is like chewing glass and staring into the abyss."
 ]
 
-citrus.add(ids, documents=documents)
+citrus.add(index="example", ids=ids, documents=documents)
 ```
 You can directly pass vector embeddings as well. If you're passing a list of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate the embeddings. Please reach out if you're looking for support from a different provider!
 
 #### 3. Search
 ```py
-result, distances = citrus.query("What is it like to launch a startup", k=1)
+result, distances = citrus.query(index="example", documents=["What is it like to launch a startup"], k=1)
 ```
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
+
+## Facing issues?
+Feel free to open issues on this repository! Discord server coming soon!
```

#### html2text {}

```diff
@@ -1,22 +1,32 @@
-# ð citrus. ### open-source (distributed) vector database
+Metadata-Version: 2.1 Name: citrusdb Version: 0.4.0 Summary: open-source vector
+database. store and retrieve embeddings for your next project! Home-page:
+https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
+Debabrata Mondal
+js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE # ð citrus. ### open-source (distributed) vector
+database
                                Special thanks to
                                    [DevKit]
                    DevKit_-_The_Essential_Developer_Toolkit
                                    DSoC 2023
 ## Installation ``` pip install citrusdb ``` ## Getting started #### 1. Create
 index ```py import citrusdb # Initialize client citrus = citrusdb.Client() #
-Create index citrus.create_index( max_elements=1000, # increases dynamically as
-you insert more vectors persist_directory="db" # save data and load index from
-disk ) ``` #### 2. Insert elements ```py ids = [1, 2, 3] documents = [ "Your
-time is limited, so don't waste it living someone else's life", "I'd rather be
-optimistic and wrong than pessimistic and right.", "Running a start-up is like
-chewing glass and staring into the abyss." ] citrus.add(ids,
-documents=documents) ``` You can directly pass vector embeddings as well. If
-you're passing a list of strings like we have done here, ensure you have your
-`OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate
-the embeddings. Please reach out if you're looking for support from a different
-provider! #### 3. Search ```py result, distances = citrus.query("What is it
-like to launch a startup", k=1) ``` Go launch a repl on [Replit](https://
-replit.com) and see what result you get after running the query! `result` will
+Create index citrus.create_index( name="example", max_elements=1000, #
+increases dynamically as you insert more vectors ) ``` #### 2. Insert elements
+```py ids = [1, 2, 3] documents = [ "Your time is limited, so don't waste it
+living someone else's life", "I'd rather be optimistic and wrong than
+pessimistic and right.", "Running a start-up is like chewing glass and staring
+into the abyss." ] citrus.add(index="example", ids=ids, documents=documents)
+``` You can directly pass vector embeddings as well. If you're passing a list
+of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the
+environment. By default we use OpenAI to to generate the embeddings. Please
+reach out if you're looking for support from a different provider! #### 3.
+Search ```py result, distances = citrus.query(index="example", documents=["What
+is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
+/replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
-(https://replit.com/@debabratajr/pokedex-search)
+(https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
+open issues on this repository! Discord server coming soon!
```

### Comparing `citrusdb-0.3.3/citrusdb/api/index.py` & `citrusdb-0.4.0/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/citrusdb/api/local.py` & `citrusdb-0.4.0/citrusdb/api/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 import os
 import json
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from numpy import float32
 from numpy._typing import NDArray
 import shutil
 
 from citrusdb.api.index import Index
-from citrusdb.db.sqlite.db import DB
+from citrusdb.db import BaseDB
+from citrusdb.db.postgres.db import PostgresDB
+from citrusdb.db.sqlite.db import SQLiteDB
 
 
 class LocalAPI:
     _db: Dict[str, Index] 
-    _sqlClient: DB
+    _SQLClient: BaseDB
     persist_directory: Optional[str]
     _TEMP_DIRECTORY = "citrus_temp"
 
-    def __init__(self, persist_directory: Optional[str] = None):
+    def __init__(
+        self,
+        persist_directory: Optional[str] = None,
+        database_type: Optional[str] = "sqlite",
+        **kwargs: Optional[Dict[str, Any]]
+    ):
         self._db = {}
         self.persist_directory = persist_directory
 
         if not(persist_directory) and os.path.isdir(self._TEMP_DIRECTORY):
             # Cleanup previous sqlite data
             shutil.rmtree(self._TEMP_DIRECTORY)
 
-        self._sqlClient = DB(persist_directory if persist_directory else self._TEMP_DIRECTORY)
+        if persist_directory and database_type == "pg":
+            self._SQLClient = PostgresDB(**kwargs)
+        else:
+            self._SQLClient = SQLiteDB(persist_directory if persist_directory else self._TEMP_DIRECTORY)
 
     def create_index(
         self,
         name: str,
         max_elements: int = 1000,
         M: int = 64,
         ef_construction: int = 200,
         allow_replace_deleted: bool = False,
     ):
-        if not(self._sqlClient.get_index_details(name)):
-            self._sqlClient.create_index(
+        if not(self._SQLClient.get_index_details(name)):
+            self._SQLClient.create_index(
                 name,
                 max_elements,
                 M,
                 ef_construction,
                 allow_replace_deleted
             )
 
@@ -67,15 +77,15 @@
         embeddings: List of embeddings to index
         metadatas: Additional metadata for each vector
         """
 
         if embeddings is None and documents is None:
             raise ValueError("Please provide either embeddings or documents.")
 
-        index_details = self._sqlClient.get_index_details(index)
+        index_details = self._SQLClient.get_index_details(index)
         if index_details is None:
             raise ValueError(f"Index with name '{index}' does not exist.")
 
         if (documents is not None) and (embeddings is None):
             from citrusdb.embedding.openai import get_embeddings
 
             embeddings = get_embeddings(documents)
@@ -99,86 +109,87 @@
 
             data = []
             for i in range(len(ids)):
                 row = (
                     ids[i],
                     index_id,
                     None if documents is None else documents[i],
-                    embeddings[i],
+                    json.dumps(embeddings[i].tolist()),
                     None if metadatas is None else json.dumps(metadatas[i])
                 )
                 data.append(row + row)
 
             # Insert data into sqlite
-            self._sqlClient.insert_to_index(data)
+            self._SQLClient.insert_to_index(data)
 
             # Index vectors
             self._db[index].add(
                 ids=ids,
                 embeddings=embeddings,
                 replace_deleted=replace_deleted
             )
 
     def delete_vectors(
         self,
         index: str,
         ids: List[int],
     ):
-        index_details = self._sqlClient.get_index_details(index)
+        index_details = self._SQLClient.get_index_details(index)
         if index_details is None:
             raise ValueError(f"Could not find index: {index}")
 
         index_id = index_details[0]
-        self._sqlClient.delete_vectors_from_index(
+        self._SQLClient.delete_vectors_from_index(
             index_id=index_id,
             ids=ids
         )
 
         self._db[index].delete_vectors(ids)
 
     def reload_indices(self):
         """
         Load all indices from disk to memory
         """
 
-        indices = self._sqlClient.get_indices()
+        indices = self._SQLClient.get_indices()
+        print("Indices: ", indices)
         for index in indices:
             index_name = index[1]
             # Load index
             self.create_index(
                 name=index_name,
                 max_elements=index[3],
                 M=index[4],
                 ef_construction=index[6],
                 allow_replace_deleted=index[7]
             )
             # Set ef value
             self._db[index_name].set_ef(index[5])
 
     def set_ef(self, index: str, ef: int):
-        index_details = self._sqlClient.get_index_details(index)
+        index_details = self._SQLClient.get_index_details(index)
         if index_details is None:
             raise ValueError(f"Could not find index: {index}")
 
-        self._sqlClient.update_ef(index, ef)
+        self._SQLClient.update_ef(index, ef)
         self._db[index].set_ef(ef)
 
     def query(
         self,
         index: str,
         documents: Optional[List[str]] = None,
         query_embeddings: Optional[NDArray[float32]] = None,
         k=1,
         filters: Optional[List[Dict]] = None
     ):
         allowed_ids = []
         if filters is not None:
-            allowed_ids = self._sqlClient.filter_vectors(index, filters)
+            allowed_ids = self._SQLClient.filter_vectors(index, filters)
 
-        filter_function = lambda label: str(label) in allowed_ids
+        filter_function = lambda label: label in allowed_ids
 
         flag = 1
         for key in self._db.keys():
             if key == index:
                 flag = 0
                 return self._db[key].query(
                     documents=documents,
```

### Comparing `citrusdb-0.3.3/citrusdb/db/index/hnswlib.py` & `citrusdb-0.4.0/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/citrusdb/db/sqlite/db.py` & `citrusdb-0.4.0/citrusdb/db/sqlite/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import sqlite3
 from typing import Dict, List, Optional, Tuple
 
+from citrusdb.db import BaseDB
 from citrusdb.utils.utils import ensure_valid_path
 import citrusdb.db.sqlite.queries as queries
 from citrusdb.db.sqlite.query_builder import QueryBuilder
 
 
-class DB:
+class SQLiteDB(BaseDB):
     _con: sqlite3.Connection
 
     def __init__(
         self,
         persist_directory: str,
     ):
         ensure_valid_path(persist_directory)
```

### Comparing `citrusdb-0.3.3/citrusdb/db/sqlite/queries.py` & `citrusdb-0.4.0/citrusdb/db/sqlite/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ef_construction INTEGER NOT NULL,
     allow_replace_deleted INTEGER NOT NULL
 );
 '''
 
 CREATE_INDEX_DATA_TABLE = '''
 CREATE TABLE IF NOT EXISTS index_data (
-    id TEXT,
+    id INTEGER,
     index_id INTEGER,
     text TEXT,
     embedding BLOB NOT NULL,
     metadata TEXT,
     PRIMARY KEY(id, index_id),
     FOREIGN KEY(index_id) REFERENCES index_manager(index_id) ON DELETE CASCADE
 );
```

### Comparing `citrusdb-0.3.3/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.4.0/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/citrusdb/utils/utils.py` & `citrusdb-0.4.0/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.4.0/citrusdb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.3.3
+Version: 0.4.0
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,33 +41,36 @@
 import citrusdb
 
 # Initialize client
 citrus = citrusdb.Client()
 
 # Create index
 citrus.create_index(
+  name="example",
   max_elements=1000,            # increases dynamically as you insert more vectors
-  persist_directory="db"       # save data and load index from disk
 )
 ```
 
 #### 2. Insert elements
 ```py
 ids = [1, 2, 3]
 documents = [
   "Your time is limited, so don't waste it living someone else's life",
   "I'd rather be optimistic and wrong than pessimistic and right.",
   "Running a start-up is like chewing glass and staring into the abyss."
 ]
 
-citrus.add(ids, documents=documents)
+citrus.add(index="example", ids=ids, documents=documents)
 ```
 You can directly pass vector embeddings as well. If you're passing a list of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate the embeddings. Please reach out if you're looking for support from a different provider!
 
 #### 3. Search
 ```py
-result, distances = citrus.query("What is it like to launch a startup", k=1)
+result, distances = citrus.query(index="example", documents=["What is it like to launch a startup"], k=1)
 ```
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
+
+## Facing issues?
+Feel free to open issues on this repository! Discord server coming soon!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.3.3 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.4.0 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -10,22 +10,23 @@
 database
                                Special thanks to
                                    [DevKit]
                    DevKit_-_The_Essential_Developer_Toolkit
                                    DSoC 2023
 ## Installation ``` pip install citrusdb ``` ## Getting started #### 1. Create
 index ```py import citrusdb # Initialize client citrus = citrusdb.Client() #
-Create index citrus.create_index( max_elements=1000, # increases dynamically as
-you insert more vectors persist_directory="db" # save data and load index from
-disk ) ``` #### 2. Insert elements ```py ids = [1, 2, 3] documents = [ "Your
-time is limited, so don't waste it living someone else's life", "I'd rather be
-optimistic and wrong than pessimistic and right.", "Running a start-up is like
-chewing glass and staring into the abyss." ] citrus.add(ids,
-documents=documents) ``` You can directly pass vector embeddings as well. If
-you're passing a list of strings like we have done here, ensure you have your
-`OPENAI_API_KEY` in the environment. By default we use OpenAI to to generate
-the embeddings. Please reach out if you're looking for support from a different
-provider! #### 3. Search ```py result, distances = citrus.query("What is it
-like to launch a startup", k=1) ``` Go launch a repl on [Replit](https://
-replit.com) and see what result you get after running the query! `result` will
+Create index citrus.create_index( name="example", max_elements=1000, #
+increases dynamically as you insert more vectors ) ``` #### 2. Insert elements
+```py ids = [1, 2, 3] documents = [ "Your time is limited, so don't waste it
+living someone else's life", "I'd rather be optimistic and wrong than
+pessimistic and right.", "Running a start-up is like chewing glass and staring
+into the abyss." ] citrus.add(index="example", ids=ids, documents=documents)
+``` You can directly pass vector embeddings as well. If you're passing a list
+of strings like we have done here, ensure you have your `OPENAI_API_KEY` in the
+environment. By default we use OpenAI to to generate the embeddings. Please
+reach out if you're looking for support from a different provider! #### 3.
+Search ```py result, distances = citrus.query(index="example", documents=["What
+is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
+/replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
-(https://replit.com/@debabratajr/pokedex-search)
+(https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
+open issues on this repository! Discord server coming soon!
```

### Comparing `citrusdb-0.3.3/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.4.0/citrusdb.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 citrusdb.egg-info/SOURCES.txt
 citrusdb.egg-info/dependency_links.txt
 citrusdb.egg-info/requires.txt
 citrusdb.egg-info/top_level.txt
 citrusdb/api/__init__.py
 citrusdb/api/index.py
 citrusdb/api/local.py
+citrusdb/db/__init__.py
 citrusdb/db/index/__init__.py
 citrusdb/db/index/hnswlib.py
+citrusdb/db/postgres/db.py
+citrusdb/db/postgres/queries.py
+citrusdb/db/postgres/query_builder.py
 citrusdb/db/sqlite/__init__.py
 citrusdb/db/sqlite/db.py
 citrusdb/db/sqlite/queries.py
 citrusdb/db/sqlite/query_builder.py
 citrusdb/embedding/__init__.py
 citrusdb/embedding/openai.py
 citrusdb/utils/__init__.py
```

### Comparing `citrusdb-0.3.3/cloud-temp/index.py` & `citrusdb-0.4.0/cloud-temp/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.3.3/pyproject.toml` & `citrusdb-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.3.3"
+version = "0.4.0"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -13,14 +13,16 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'hnswlib >= 0.7',
   'numpy >= 1.21.6',
   'openai >= 0.27',
+  'psycopg[c] >= 3.1.9',
+  'psycopg[pool] >= 3.1.7'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/0xDebabrata/citrus"
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

### Comparing `citrusdb-0.3.3/setup.py` & `citrusdb-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.3.3",
+    version="0.4.0",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
         find_packages(
             exclude=["demo"]
         ) +
-        ["citrusdb.db.index", "citrusdb.db.sqlite"]
+        ["citrusdb.db.index", "citrusdb.db.sqlite", "citrusdb.db.postgres"]
     ),
     include_package_data=True,
     install_requires=[
         "numpy",
         "hnswlib",
         "openai",
+        "psycopg[c]",
+        "psycopg[pool]"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

