# Comparing `tmp/arrow_json-0.7.1.tar.gz` & `tmp/arrow_json-0.7.2.tar.gz`

## Comparing `arrow_json-0.7.1.tar` & `arrow_json-0.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 arrow_json-0.7.1/Cargo.toml
--rw-r--r--   0      501       20      149 2023-03-31 16:27:18.000000 arrow_json-0.7.1/.vscode/settings.json
--rw-r--r--   0      501       20      453 2023-03-31 16:27:18.000000 arrow_json-0.7.1/README.md
--rw-r--r--   0      501       20     1111 2023-03-31 16:27:18.000000 arrow_json-0.7.1/pyproject.toml
--rw-r--r--   0      501       20      101 2023-03-31 16:27:18.000000 arrow_json-0.7.1/python/arrow_json/__init__.py
--rw-r--r--   0      501       20      171 2023-03-31 16:27:18.000000 arrow_json-0.7.1/python/arrow_json/_arrow_json.pyi
--rw-r--r--   0      501       20        0 2023-03-31 16:27:18.000000 arrow_json-0.7.1/python/arrow_json/py.typed
--rw-r--r--   0      501       20     1004 2023-03-31 16:27:18.000000 arrow_json-0.7.1/src/lib.rs
--rw-r--r--   0      501       20        0 2023-03-31 16:27:18.000000 arrow_json-0.7.1/test_arrow_json/__init__.py
--rw-r--r--   0      501       20     1101 2023-03-31 16:27:18.000000 arrow_json-0.7.1/test_arrow_json/test_array_to_json.py
--rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 arrow_json-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 arrow_json-0.7.2/Cargo.toml
+-rw-r--r--   0      501       20       99 2023-06-15 04:55:37.000000 arrow_json-0.7.2/.gitignore
+-rw-r--r--   0      501       20      453 2023-06-15 04:55:37.000000 arrow_json-0.7.2/README.md
+-rw-r--r--   0      501       20     1112 2023-06-15 04:55:37.000000 arrow_json-0.7.2/pyproject.toml
+-rw-r--r--   0      501       20      583 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/__init__.py
+-rw-r--r--   0      501       20      165 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/_arrow_json.pyi
+-rw-r--r--   0      501       20        0 2023-06-15 04:55:37.000000 arrow_json-0.7.2/python/arrow_json/py.typed
+-rw-r--r--   0      501       20     1474 2023-06-15 04:55:37.000000 arrow_json-0.7.2/src/lib.rs
+-rw-r--r--   0      501       20        0 2023-06-15 04:55:37.000000 arrow_json-0.7.2/tests/__init__.py
+-rw-r--r--   0      501       20     1480 2023-06-15 04:55:37.000000 arrow_json-0.7.2/tests/test_array_to_json.py
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 arrow_json-0.7.2/PKG-INFO
```

### Comparing `arrow_json-0.7.1/pyproject.toml` & `arrow_json-0.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 [project.urls]
 homepage = "https://github.com/adriangb/pgpq"
 documentation = "https://github.com/adriangb/pgpq/README.md"
 repository = "https://github.com/adriangb/pgpq"
 
 [build-system]
-requires = ["maturin>=0.13.0<14"]
+requires = ["maturin>=0.14.0,<15"]
 build-backend = "maturin"
 
 [tool.maturin]
 sdist-include = ["Cargo.lock"]
 strip = true
 python-source = "python"
 profile = "release"
```

### Comparing `arrow_json-0.7.1/src/lib.rs` & `arrow_json-0.7.2/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+use arrow::array::StringBuilder;
 use pyo3::prelude::*;
 use pyo3::Python;
 
 use arrow::array::{make_array, Array, ArrayData, LargeStringBuilder};
 use arrow::json::writer::array_to_json_array;
 use arrow::pyarrow::PyArrowConvert;
 use serde_json::{to_string, Value};
 
 #[pyfunction]
-#[pyo3(signature = (array))]
-fn array_to_utf8_json_array(py: Python, array: &PyAny) -> PyResult<PyObject> {
+#[pyo3(signature = (array, large))]
+fn array_to_utf8_json_array(py: Python, array: &PyAny, large: bool) -> PyResult<PyObject> {
     // This is super inefficient, leaving optimization as a TODO
     let array = make_array(ArrayData::from_pyarrow(array)?);
     let json = array_to_json_array(&array).unwrap();
-    let mut builder = LargeStringBuilder::new();
-    for value in json.into_iter() {
-        match value {
-            Value::Null => builder.append_null(),
-            value => builder.append_value(to_string(&value).unwrap()),
+    if large {
+        let mut builder = LargeStringBuilder::new();
+        for value in json.into_iter() {
+            match value {
+                Value::Null => builder.append_null(),
+                value => builder.append_value(to_string(&value).unwrap()),
+            }
         }
+        let json_arr = builder.finish();
+        json_arr.data().to_pyarrow(py)
+    } else {
+        let mut builder = StringBuilder::new();
+        for value in json.into_iter() {
+            match value {
+                Value::Null => builder.append_null(),
+                value => builder.append_value(to_string(&value).unwrap()),
+            }
+        }
+        let json_arr = builder.finish();
+        json_arr.data().to_pyarrow(py)
     }
-    let json_arr = builder.finish();
-    json_arr.data().to_pyarrow(py)
 }
 
 #[pymodule]
 fn _arrow_json(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(array_to_utf8_json_array, m)?)?;
     Ok(())
 }
```

### Comparing `arrow_json-0.7.1/PKG-INFO` & `arrow_json-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: arrow-json
-Version: 0.7.1
+Version: 0.7.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pyarrow>=11
 Requires-Dist: typing-extensions>=3; python_version < '3.8'
 Requires-Dist: pytest >=7.0.0; extra == 'test'
 Requires-Dist: maturin >= 0.14.0; extra == 'test'
 Requires-Dist: pre-commit>=2.16.0; extra == 'test'
 Requires-Dist: pyarrow >= 11.0.0; extra == 'test'
 Requires-Dist: polars >= 0.16.1; extra == 'test'
-Provides-Extra: bench
 Provides-Extra: test
+Provides-Extra: bench
 Summary: Arrow -> JSON encoder
 Author: Adrian Garcia Badaracco
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/adriangb/pgpq
 Project-URL: homepage, https://github.com/adriangb/pgpq
```

