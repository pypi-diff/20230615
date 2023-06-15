# Comparing `tmp/pgpq-0.7.2.tar.gz` & `tmp/pgpq-0.7.3.tar.gz`

## Comparing `pgpq-0.7.2.tar` & `pgpq-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pgpq-0.7.2/local_dependencies/pgpq/Cargo.toml
--rw-r--r--   0      501       20      104 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/README.md
--rw-r--r--   0      501       20    10455 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/benches/experiments.rs
--rw-r--r--   0      501       20     2765 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/benches/yellow_cab_dataset.rs
--rw-r--r--   0      501       20    40799 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/encoders.rs
--rw-r--r--   0      501       20     2495 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/error.rs
--rw-r--r--   0      501       20     7733 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/lib.rs
--rw-r--r--   0      501       20     3516 2023-06-15 05:00:42.000000 pgpq-0.7.2/local_dependencies/pgpq/src/pg_schema.rs
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 pgpq-0.7.2/Cargo.toml
--rw-r--r--   0      501       20     2191 2023-06-15 05:00:42.000000 pgpq-0.7.2/README.md
--rw-r--r--   0      501       20     3034 2023-06-15 05:00:42.000000 pgpq-0.7.2/benches/encode.ipynb
--rw-r--r--   0      501       20     2136 2023-06-15 05:00:42.000000 pgpq-0.7.2/example.py
--rw-r--r--   0      501       20     1362 2023-06-15 05:00:42.000000 pgpq-0.7.2/pyproject.toml
--rw-r--r--   0      501       20      139 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/__init__.py
--rw-r--r--   0      501       20     6078 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/_pgpq.pyi
--rw-r--r--   0      501       20     1770 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/encoders.py
--rw-r--r--   0      501       20        0 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/py.typed
--rw-r--r--   0      501       20      581 2023-06-15 05:00:42.000000 pgpq-0.7.2/python/pgpq/schema.py
--rw-r--r--   0      501       20    39649 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/encoders.rs
--rw-r--r--   0      501       20     5784 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/lib.rs
--rw-r--r--   0      501       20    13436 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/pg_schema.rs
--rw-r--r--   0      501       20     1876 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/template.py
--rw-r--r--   0      501       20       96 2023-06-15 05:00:42.000000 pgpq-0.7.2/src/utils.rs
--rw-r--r--   0      501       20        0 2023-06-15 05:00:42.000000 pgpq-0.7.2/test_pgpq/__init__.py
--rw-r--r--   0      501       20     7253 2023-06-15 05:00:42.000000 pgpq-0.7.2/test_pgpq/test_pgpq.py
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 pgpq-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pgpq-0.7.3/local_dependencies/pgpq/Cargo.toml
+-rw-r--r--   0      501       20      104 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/README.md
+-rw-r--r--   0      501       20    10455 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/benches/experiments.rs
+-rw-r--r--   0      501       20     2765 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/benches/yellow_cab_dataset.rs
+-rw-r--r--   0      501       20    40799 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/src/encoders.rs
+-rw-r--r--   0      501       20     2495 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/src/error.rs
+-rw-r--r--   0      501       20     7733 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/src/lib.rs
+-rw-r--r--   0      501       20     3516 2023-06-15 15:17:16.000000 pgpq-0.7.3/local_dependencies/pgpq/src/pg_schema.rs
+-rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 pgpq-0.7.3/Cargo.toml
+-rw-r--r--   0      501       20     2191 2023-06-15 15:17:16.000000 pgpq-0.7.3/README.md
+-rw-r--r--   0      501       20     3034 2023-06-15 15:17:16.000000 pgpq-0.7.3/benches/encode.ipynb
+-rw-r--r--   0      501       20     2136 2023-06-15 15:17:16.000000 pgpq-0.7.3/example.py
+-rw-r--r--   0      501       20     1362 2023-06-15 15:17:16.000000 pgpq-0.7.3/pyproject.toml
+-rw-r--r--   0      501       20      139 2023-06-15 15:17:16.000000 pgpq-0.7.3/python/pgpq/__init__.py
+-rw-r--r--   0      501       20     6078 2023-06-15 15:17:16.000000 pgpq-0.7.3/python/pgpq/_pgpq.pyi
+-rw-r--r--   0      501       20     1770 2023-06-15 15:17:16.000000 pgpq-0.7.3/python/pgpq/encoders.py
+-rw-r--r--   0      501       20        0 2023-06-15 15:17:16.000000 pgpq-0.7.3/python/pgpq/py.typed
+-rw-r--r--   0      501       20      581 2023-06-15 15:17:16.000000 pgpq-0.7.3/python/pgpq/schema.py
+-rw-r--r--   0      501       20    39649 2023-06-15 15:17:16.000000 pgpq-0.7.3/src/encoders.rs
+-rw-r--r--   0      501       20     5784 2023-06-15 15:17:16.000000 pgpq-0.7.3/src/lib.rs
+-rw-r--r--   0      501       20    13436 2023-06-15 15:17:16.000000 pgpq-0.7.3/src/pg_schema.rs
+-rw-r--r--   0      501       20     1876 2023-06-15 15:17:16.000000 pgpq-0.7.3/src/template.py
+-rw-r--r--   0      501       20       96 2023-06-15 15:17:16.000000 pgpq-0.7.3/src/utils.rs
+-rw-r--r--   0      501       20        0 2023-06-15 15:17:16.000000 pgpq-0.7.3/test_pgpq/__init__.py
+-rw-r--r--   0      501       20     7253 2023-06-15 15:17:16.000000 pgpq-0.7.3/test_pgpq/test_pgpq.py
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 pgpq-0.7.3/PKG-INFO
```

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/Cargo.toml` & `pgpq-0.7.3/local_dependencies/pgpq/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pgpq"
-version = "0.7.2"
+version = "0.7.3"
 edition = "2021"
 description = "Encode Apache Arrow `RecordBatch`es to Postgres' native binary format"
 license = "MIT"
 readme = "README.md"
 exclude = ["/tests"]
 homepage = "https://github.com/adriangb/pgpq"
 repository = "https://github.com/adriangb/pgpq"
```

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/benches/experiments.rs` & `pgpq-0.7.3/local_dependencies/pgpq/benches/experiments.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/benches/yellow_cab_dataset.rs` & `pgpq-0.7.3/local_dependencies/pgpq/benches/yellow_cab_dataset.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/src/encoders.rs` & `pgpq-0.7.3/local_dependencies/pgpq/src/encoders.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/src/error.rs` & `pgpq-0.7.3/local_dependencies/pgpq/src/error.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/src/lib.rs` & `pgpq-0.7.3/local_dependencies/pgpq/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/local_dependencies/pgpq/src/pg_schema.rs` & `pgpq-0.7.3/local_dependencies/pgpq/src/pg_schema.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/README.md` & `pgpq-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/benches/encode.ipynb` & `pgpq-0.7.3/benches/encode.ipynb`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/example.py` & `pgpq-0.7.3/example.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/pyproject.toml` & `pgpq-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/python/pgpq/_pgpq.pyi` & `pgpq-0.7.3/python/pgpq/_pgpq.pyi`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/python/pgpq/encoders.py` & `pgpq-0.7.3/python/pgpq/encoders.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/python/pgpq/schema.py` & `pgpq-0.7.3/python/pgpq/schema.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/src/encoders.rs` & `pgpq-0.7.3/src/encoders.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/src/lib.rs` & `pgpq-0.7.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/src/pg_schema.rs` & `pgpq-0.7.3/src/pg_schema.rs`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/src/template.py` & `pgpq-0.7.3/src/template.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/test_pgpq/test_pgpq.py` & `pgpq-0.7.3/test_pgpq/test_pgpq.py`

 * *Files identical despite different names*

### Comparing `pgpq-0.7.2/PKG-INFO` & `pgpq-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pgpq
-Version: 0.7.2
+Version: 0.7.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pyarrow>=11
 Requires-Dist: typing-extensions>=3; python_version < '3.8'
-Requires-Dist: jupyter >=1.0.0; extra == 'bench'
-Requires-Dist: requests; extra == 'bench'
 Requires-Dist: pytest >=7.0.0; extra == 'test'
 Requires-Dist: maturin >= 0.14.0; extra == 'test'
 Requires-Dist: pre-commit>=2.16.0; extra == 'test'
 Requires-Dist: testing.postgresql >= 1.3.0; extra == 'test'
 Requires-Dist: psycopg[binary] >= 3.1.8; extra == 'test'
 Requires-Dist: pyarrow >= 11.0.0; extra == 'test'
-Provides-Extra: bench
+Requires-Dist: jupyter >=1.0.0; extra == 'bench'
+Requires-Dist: requests; extra == 'bench'
 Provides-Extra: test
+Provides-Extra: bench
 Summary: Arrow -> PostgreSQL encoder
 Author: Adrian Garcia Badaracco
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/adriangb/pgpq
 Project-URL: documentation, https://github.com/adriangb/pgpq/README.md
```

