# Comparing `tmp/arrow_json-0.7.2.tar.gz` & `tmp/arrow_json-0.7.3.tar.gz`

## Comparing `arrow_json-0.7.2.tar` & `arrow_json-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 arrow_json-0.7.2/Cargo.toml
--rw-r--r--   0      501       20       99 2023-06-15 04:55:37.000000 arrow_json-0.7.2/.gitignore
--rw-r--r--   0      501       20      453 2023-06-15 04:55:37.000000 arrow_json-0.7.2/README.md
--rw-r--r--   0      501       20     1112 2023-06-15 04:55:37.000000 arrow_json-0.7.2/pyproject.toml
--rw-r--r--   0      501       20      583 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/__init__.py
--rw-r--r--   0      501       20      165 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/_arrow_json.pyi
--rw-r--r--   0      501       20        0 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/py.typed
--rw-r--r--   0      501       20     1474 2023-06-15 04:55:37.000000 arrow_json-0.7.2/src/lib.rs
--rw-r--r--   0      501       20        0 2023-06-15 04:55:37.000000 arrow_json-0.7.2/tests/__init__.py
--rw-r--r--   0      501       20     1480 2023-06-15 04:55:37.000000 arrow_json-0.7.2/tests/test_array_to_json.py
--rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 arrow_json-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 arrow_json-0.7.3/Cargo.toml
+-rw-r--r--   0      501       20       99 2023-06-15 15:23:24.000000 arrow_json-0.7.3/.gitignore
+-rw-r--r--   0      501       20      453 2023-06-15 15:23:24.000000 arrow_json-0.7.3/README.md
+-rw-r--r--   0      501       20     1112 2023-06-15 15:23:24.000000 arrow_json-0.7.3/pyproject.toml
+-rw-r--r--   0      501       20      100 2023-06-15 15:23:24.000000 arrow_json-0.7.3/python/arrow_json/__init__.py
+-rw-r--r--   0      501       20      449 2023-06-15 15:23:24.000000 arrow_json-0.7.3/python/arrow_json/_arrow_json.pyi
+-rw-r--r--   0      501       20        0 2023-06-15 15:23:24.000000 arrow_json-0.7.3/python/arrow_json/py.typed
+-rw-r--r--   0      501       20     1481 2023-06-15 15:23:24.000000 arrow_json-0.7.3/src/lib.rs
+-rw-r--r--   0      501       20        0 2023-06-15 15:23:24.000000 arrow_json-0.7.3/tests/__init__.py
+-rw-r--r--   0      501       20     1480 2023-06-15 15:23:24.000000 arrow_json-0.7.3/tests/test_array_to_json.py
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 arrow_json-0.7.3/PKG-INFO
```

### Comparing `arrow_json-0.7.2/pyproject.toml` & `arrow_json-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arrow_json-0.7.2/src/lib.rs` & `arrow_json-0.7.3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 use arrow::array::{make_array, Array, ArrayData, LargeStringBuilder};
 use arrow::json::writer::array_to_json_array;
 use arrow::pyarrow::PyArrowConvert;
 use serde_json::{to_string, Value};
 
 #[pyfunction]
-#[pyo3(signature = (array, large))]
+#[pyo3(signature = (array, large = true))]
 fn array_to_utf8_json_array(py: Python, array: &PyAny, large: bool) -> PyResult<PyObject> {
     // This is super inefficient, leaving optimization as a TODO
     let array = make_array(ArrayData::from_pyarrow(array)?);
     let json = array_to_json_array(&array).unwrap();
     if large {
         let mut builder = LargeStringBuilder::new();
         for value in json.into_iter() {
```

### Comparing `arrow_json-0.7.2/tests/test_array_to_json.py` & `arrow_json-0.7.3/tests/test_array_to_json.py`

 * *Files identical despite different names*

### Comparing `arrow_json-0.7.2/PKG-INFO` & `arrow_json-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrow-json
-Version: 0.7.2
+Version: 0.7.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pyarrow>=11
@@ -17,17 +17,17 @@
 Provides-Extra: test
 Provides-Extra: bench
 Summary: Arrow -> JSON encoder
 Author: Adrian Garcia Badaracco
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/adriangb/pgpq
-Project-URL: homepage, https://github.com/adriangb/pgpq
 Project-URL: documentation, https://github.com/adriangb/pgpq/README.md
+Project-URL: homepage, https://github.com/adriangb/pgpq
+Project-URL: repository, https://github.com/adriangb/pgpq
 
 # arrow-json
 
 Encode an arrow array into an array of json strings:
 
 ```python
 import json
```

