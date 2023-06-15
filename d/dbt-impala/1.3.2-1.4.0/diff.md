# Comparing `tmp/dbt-impala-1.3.2.tar.gz` & `tmp/dbt-impala-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-impala-1.3.2.tar", last modified: Thu May 11 04:58:01 2023, max compression
+gzip compressed data, was "dbt-impala-1.4.0.tar", last modified: Thu Jun 15 00:26:53 2023, max compression
```

## Comparing `dbt-impala-1.3.2.tar` & `dbt-impala-1.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/
--rw-r--r--   0 jenkins   (1001) users      (100)    10837 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     2433 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.629726 dbt-impala-1.3.2/dbt/adapters/impala/
--rw-------   0 jenkins   (1001) users      (100)      227 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt/adapters/impala/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1062 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      596 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8443 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2771 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15342 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15388 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2406 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/adapters/impala/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.625726 dbt-impala-1.3.2/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.629726 dbt-impala-1.3.2/dbt/include/impala/
--rw-r--r--   0 jenkins   (1001) users      (100)      630 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      651 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.633726 dbt-impala-1.3.2/dbt/include/impala/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    15268 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1591 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/apply_grants.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      676 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/catalog.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6282 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1899 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/insertoverwrite.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1877 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/seed.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.633726 dbt-impala-1.3.2/dbt/include/impala/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      721 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      157 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      155 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      159 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      751 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      672 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      750 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     5905 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      696 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      825 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1208 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1106 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      727 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      863 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      779 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/dbt/include/impala/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/dbt_impala.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1544 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) users      (100)       50 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2023-05-11 04:58:01.000000 dbt-impala-1.3.2/dbt_impala.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2023-05-11 04:58:01.637726 dbt-impala-1.3.2/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3118 2023-05-11 04:57:29.000000 dbt-impala-1.3.2/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.460251 dbt-impala-1.4.0/
+-rw-r--r--   0 jenkins   (1001) users      (100)    10837 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-06-15 00:26:53.460251 dbt-impala-1.4.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     2433 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.452251 dbt-impala-1.4.0/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.452251 dbt-impala-1.4.0/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.456251 dbt-impala-1.4.0/dbt/adapters/impala/
+-rw-------   0 jenkins   (1001) users      (100)      227 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt/adapters/impala/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1062 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      596 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2771 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15338 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15344 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2431 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/adapters/impala/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.452251 dbt-impala-1.4.0/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.456251 dbt-impala-1.4.0/dbt/include/impala/
+-rw-r--r--   0 jenkins   (1001) users      (100)      630 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      651 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.456251 dbt-impala-1.4.0/dbt/include/impala/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    15259 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1591 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/apply_grants.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      676 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/catalog.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6282 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1899 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/insertoverwrite.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1877 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/seed.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.460251 dbt-impala-1.4.0/dbt/include/impala/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      721 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      157 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      155 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      159 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      751 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      672 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      750 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     5905 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      696 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      825 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1106 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      727 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      863 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      779 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/dbt/include/impala/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-06-15 00:26:53.460251 dbt-impala-1.4.0/dbt_impala.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     3101 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1544 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) users      (100)       50 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2023-06-15 00:26:53.000000 dbt-impala-1.4.0/dbt_impala.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2023-06-15 00:26:53.460251 dbt-impala-1.4.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3118 2023-06-15 00:26:22.000000 dbt-impala-1.4.0/setup.py
```

### Comparing `dbt-impala-1.3.2/LICENSE` & `dbt-impala-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/PKG-INFO` & `dbt-impala-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.3.2
+Version: 1.4.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-impala-1.3.2/README.md` & `dbt-impala-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/__init__.py` & `dbt-impala-1.4.0/dbt/adapters/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/__version__.py` & `dbt-impala-1.4.0/dbt/adapters/impala/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.3.2"
+version = "1.4.0"
```

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/cloudera_tracking.py` & `dbt-impala-1.4.0/dbt/adapters/impala/cloudera_tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/column.py` & `dbt-impala-1.4.0/dbt/adapters/impala/column.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/connections.py` & `dbt-impala-1.4.0/dbt/adapters/impala/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if "database" not in data:
             data["database"] = None
         return data
 
     def __post_init__(self):
         # impala classifies database and schema as the same thing
         if self.database is not None and self.database != self.schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Impala, database must be omitted or have the same value as"
                 f" schema."
             )
         self.database = None
 
@@ -165,28 +165,28 @@
 
     @contextmanager
     def exception_handler(self, sql: str):
         try:
             yield
         except HttpError as httpError:
             logger.debug(f"Authorization error: {httpError}")
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "HTTP Authorization error: " + str(httpError) + ", please check your credentials"
             )
         except HiveServer2Error as servError:
             logger.debug(f"Server connection error: {servError}")
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "Unable to establish connection to Impala server: " + str(servError)
             )
         except DatabaseError as dbError:
             logger.debug(f"Database connection error: {str(dbError)}")
             raise dbt.exceptions.DatabaseException("Database Connection error: " + str(dbError))
         except Exception as exc:
             logger.debug(f"Error running SQL: {sql}")
-            raise dbt.exceptions.RuntimeException(str(exc))
+            raise dbt.exceptions.DbtRuntimeError(str(exc))
 
     @classmethod
     def open(cls, connection):
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
```

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/impl.py` & `dbt-impala-1.4.0/dbt/adapters/impala/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import agate
 import dbt.exceptions
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.sql import SQLAdapter
 from dbt.clients import agate_helper
 from dbt.clients.agate_helper import ColumnTypeBuilder, NullableAgateType, _NullMarker
 from dbt.events import AdapterLogger
-from dbt.exceptions import warn_or_error
 from dbt.utils import executor
 
 import dbt.adapters.impala.cloudera_tracking as tracker
 from dbt.adapters.impala import ImpalaConnectionManager
 from dbt.adapters.impala.column import ImpalaColumn
 from dbt.adapters.impala.relation import ImpalaRelation
 
@@ -99,27 +98,27 @@
     def list_relations_without_caching(
         self, schema_relation: ImpalaRelation
     ) -> List[ImpalaRelation]:
         kwargs = {"schema_relation": schema_relation}
 
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
-        except dbt.exceptions.RuntimeException as e:
+        except dbt.exceptions.DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
             if f"Database '{schema_relation}' not found" in errmsg:
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 return []
 
         relations = []
         for row in results:
             if len(row) != 2:
-                raise dbt.exceptions.RuntimeException(
+                raise dbt.exceptions.DbtRuntimeError(
                     f'Invalid value from "show table extended ...", '
                     f"got {len(row)} values, expected 4"
                 )
             _identifier = row[0]
             _rel_type = row[1]
 
             relation = self.Relation.create(
@@ -148,15 +147,15 @@
             columns = self.parse_columns_from_information(cached_relation)
 
         # execute the macro and parse the data
         if not columns:
             try:
                 rows: List[agate.Row] = super().get_columns_in_relation(relation)
                 columns = self.parse_describe_extended(relation, rows)
-            except dbt.exceptions.RuntimeException as e:
+            except dbt.exceptions.DbtRuntimeError as e:
                 # impala would throw error when table doesn't exist
                 errmsg = getattr(e, "msg", "")
                 if (
                     "Table or view not found" in errmsg
                     or "NoSuchTableException" in errmsg
                     or "Could not resolve path" in errmsg
                 ):
```

### Comparing `dbt-impala-1.3.2/dbt/adapters/impala/relation.py` & `dbt-impala-1.4.0/dbt/adapters/impala/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.exceptions import RuntimeException
 
 import dbt.adapters.impala.cloudera_tracking as tracker
 
 
 @dataclass
 class ImpalaQuotePolicy(Policy):
     database: bool = False
@@ -32,16 +31,16 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class ImpalaRelation(BaseRelation):
-    quote_policy: ImpalaQuotePolicy = ImpalaQuotePolicy()
-    include_policy: ImpalaIncludePolicy = ImpalaIncludePolicy()
+    quote_policy: ImpalaQuotePolicy = field(default_factory=lambda: ImpalaQuotePolicy())
+    include_policy: ImpalaIncludePolicy = field(default_factory=lambda: ImpalaIncludePolicy())
     quote_character: str = None
     information: str = None
 
     def __post_init__(self):
         if self.type:
             tracker.track_usage(
                 {
```

### Comparing `dbt-impala-1.3.2/dbt/include/impala/__init__.py` & `dbt-impala-1.4.0/dbt/include/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/dbt_project.yml` & `dbt-impala-1.4.0/dbt/include/impala/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/adapters.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -167,30 +167,28 @@
     {%- if table_type == 'iceberg' -%} STORED BY ICEBERG {%- endif -%}
     {{ ct_option_stored_as(label="stored as") }}
     {{ ct_option_location_clause(label="location") }}
     {{ ct_option_cached_in(label="cached in") }}
     {{ ct_option_tbl_properties(label="tblproperties") }}
   as
     {{ sql }}
-  ;
 {%- endmacro %}
 
 {% macro impala__create_view_as(relation, sql) -%}
 
   {%- set sql_header = config.get('sql_header', none) -%}
   {%- set backup = config.get('backup') -%}
 
   {{ sql_header if sql_header is not none }}
 
   create view
     {{ relation.include(schema=True) }}
     {{ ct_option_comment_relation(label="comment") }}
   as
     {{ sql }}
-  ;
 {%- endmacro %}
 
 {% macro impala__create_schema(relation) -%}
   {%- call statement('create_schema') -%}
     create schema if not exists {{ relation }}
   {% endcall %}
 {% endmacro %}
@@ -253,15 +251,15 @@
 {% macro impala__rename_relation(from_relation, to_relation) -%}
   {% set from_rel_type = get_relation_type(from_relation) %}
 
   {% call statement('drop_relation_if_exists_table') %}
     drop table if exists {{ to_relation }}
   {% endcall %}
   {% call statement('drop_relation_if_exists_view') %}
-    drop view if exists {{ to_relation }};
+    drop view if exists {{ to_relation }}
   {% endcall %}
   {% call statement('rename_relation') -%}
     {% if not from_rel_type %}
       {% do exceptions.raise_database_error("Cannot rename a relation with a blank type: " ~ from_relation.identifier) %}
     {% elif from_rel_type == 'table' %}
         alter table {{ from_relation }} rename to {{ to_relation }}
     {% elif from_rel_type == 'view' %}
```

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/apply_grants.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/catalog.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/incremental.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/insertoverwrite.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/insertoverwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/seed.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/any_value.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/bool_or.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/concat.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/dateadd.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/datediff.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/escape_single_quotes.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/escape_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/hash.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/last_day.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/listagg.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/position.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/split_part.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/macros/utils/timestamps.sql` & `dbt-impala-1.4.0/dbt/include/impala/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt/include/impala/sample_profiles.yml` & `dbt-impala-1.4.0/dbt/include/impala/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/dbt_impala.egg-info/PKG-INFO` & `dbt-impala-1.4.0/dbt_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.3.2
+Version: 1.4.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-impala-1.3.2/dbt_impala.egg-info/SOURCES.txt` & `dbt-impala-1.4.0/dbt_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.3.2/setup.py` & `dbt-impala-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-impala"
 # make sure this always matches dbt/adapters/dbt_impala/__version__.py
-package_version = "1.3.2"
+package_version = "1.4.0"
 description = """The Impala adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
```

