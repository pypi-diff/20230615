# Comparing `tmp/ever_playground-0.7.1.tar.gz` & `tmp/ever_playground-0.7.3.tar.gz`

## Comparing `ever_playground-0.7.1.tar` & `ever_playground-0.7.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ever_playground-0.7.1/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.7.1/.gitignore
--rw-rw-r--   0     1000     1000      230 2023-06-07 13:28:48.000000 ever_playground-0.7.1/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.7.1/README.md
--rw-rw-r--   0     1000     1000     1062 2023-05-24 15:04:04.000000 ever_playground-0.7.1/create-param8.py
--rw-rw-r--   0     1000     1000     6298 2023-06-07 22:03:10.000000 ever_playground-0.7.1/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     9717 2023-06-07 22:10:09.000000 ever_playground-0.7.1/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     2226 2023-06-07 22:10:35.000000 ever_playground-0.7.1/examples/basics.py
--rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.7.1/examples/highload/generate.fif
--rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.7.1/examples/highload/highload-wallet-v2.fif
--rw-rw-r--   0     1000     1000     4667 2023-06-06 14:21:08.000000 ever_playground-0.7.1/examples/highload/highload-wallet-v2.py
--rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/order-list-fift
--rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.7.1/examples/highload/order-list-py
--rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/sample.pk
--rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/sample27172.addr
--rw-rw-r--   0     1000     1000     1540 2023-06-07 22:07:40.000000 ever_playground-0.7.1/examples/ifjmp-perf-eval.py
--rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.7.1/examples/recover-stake.fif
--rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.7.1/examples/recover-stake.py
--rw-rw-r--   0     1000     1000     2371 2023-06-07 22:00:21.000000 ever_playground-0.7.1/examples/runvm.py
--rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.7.1/examples/testgiver.fif
--rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.7.1/examples/testgiver.py
--rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.7.1/examples/validator-elect-req.fif
--rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.7.1/examples/validator-elect-req.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.7.1/pyproject.toml
--rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.7.1/run-examples.py
--rw-rw-r--   0     1000     1000     6460 2023-06-07 21:45:48.000000 ever_playground-0.7.1/src/continuations.rs
--rw-rw-r--   0     1000     1000     1791 2023-06-07 20:27:47.000000 ever_playground-0.7.1/src/crypto.rs
--rw-rw-r--   0     1000     1000    11665 2023-06-07 22:09:29.000000 ever_playground-0.7.1/src/lib.rs
--rw-rw-r--   0     1000     1000      997 2023-06-07 09:59:08.000000 ever_playground-0.7.1/src/tests.rs
--rw-rw-r--   0     1000     1000     5901 2023-06-07 20:27:22.000000 ever_playground-0.7.1/src/utils.rs
--rw-rw-r--   0     1000     1000     4193 2023-06-07 21:56:26.000000 ever_playground-0.7.1/src/vm.rs
--rw-rw-r--   0     1000     1000     3036 2023-06-02 16:56:59.000000 ever_playground-0.7.1/try-catch.py
--rw-rw-r--   0     1000     1000     3613 2023-06-06 15:33:22.000000 ever_playground-0.7.1/ttt.py
--rw-rw-r--   0     1000     1000    24799 2023-06-07 22:15:09.000000 ever_playground-0.7.1/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ever_playground-0.7.3/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.7.3/.gitignore
+-rw-rw-r--   0     1000     1000      230 2023-06-07 13:28:48.000000 ever_playground-0.7.3/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.7.3/README.md
+-rw-rw-r--   0     1000     1000     1062 2023-05-24 15:04:04.000000 ever_playground-0.7.3/create-param8.py
+-rw-rw-r--   0     1000     1000     6697 2023-06-14 15:00:43.000000 ever_playground-0.7.3/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000    10884 2023-06-14 15:14:59.000000 ever_playground-0.7.3/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2226 2023-06-07 22:10:35.000000 ever_playground-0.7.3/examples/basics.py
+-rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.7.3/examples/highload/generate.fif
+-rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.7.3/examples/highload/highload-wallet-v2.fif
+-rw-rw-r--   0     1000     1000     4667 2023-06-06 14:21:08.000000 ever_playground-0.7.3/examples/highload/highload-wallet-v2.py
+-rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.7.3/examples/highload/order-list-fift
+-rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.7.3/examples/highload/order-list-py
+-rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.7.3/examples/highload/sample.pk
+-rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.7.3/examples/highload/sample27172.addr
+-rw-rw-r--   0     1000     1000     1540 2023-06-07 22:07:40.000000 ever_playground-0.7.3/examples/ifjmp-perf-eval.py
+-rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.7.3/examples/recover-stake.fif
+-rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.7.3/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     1097 2023-06-14 22:24:52.000000 ever_playground-0.7.3/examples/runcont.py
+-rw-rw-r--   0     1000     1000     2362 2023-06-07 22:18:55.000000 ever_playground-0.7.3/examples/runvm.py
+-rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.7.3/examples/testgiver.fif
+-rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.7.3/examples/testgiver.py
+-rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.7.3/examples/validator-elect-req.fif
+-rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.7.3/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.7.3/pyproject.toml
+-rwxrwxr-x   0     1000     1000     3108 2023-06-14 22:27:26.000000 ever_playground-0.7.3/run-examples.py
+-rw-rw-r--   0     1000     1000     2098 2023-06-13 20:07:11.000000 ever_playground-0.7.3/runvm-generic.py
+-rw-rw-r--   0     1000     1000     9369 2023-06-14 22:23:25.000000 ever_playground-0.7.3/src/continuations.rs
+-rw-rw-r--   0     1000     1000     1791 2023-06-07 20:27:47.000000 ever_playground-0.7.3/src/crypto.rs
+-rw-rw-r--   0     1000     1000    12075 2023-06-14 16:53:59.000000 ever_playground-0.7.3/src/lib.rs
+-rw-rw-r--   0     1000     1000      997 2023-06-07 09:59:08.000000 ever_playground-0.7.3/src/tests.rs
+-rw-rw-r--   0     1000     1000     6075 2023-06-14 16:24:32.000000 ever_playground-0.7.3/src/utils.rs
+-rw-rw-r--   0     1000     1000     4330 2023-06-14 17:34:02.000000 ever_playground-0.7.3/src/vm.rs
+-rw-rw-r--   0     1000     1000     3036 2023-06-02 16:56:59.000000 ever_playground-0.7.3/try-catch.py
+-rw-rw-r--   0     1000     1000     3613 2023-06-06 15:33:22.000000 ever_playground-0.7.3/ttt.py
+-rw-rw-r--   0     1000     1000    24799 2023-06-14 22:22:53.000000 ever_playground-0.7.3/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.7.3/PKG-INFO
```

### Comparing `ever_playground-0.7.1/Cargo.toml` & `ever_playground-0.7.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ever-playground"
-version = "0.7.1"
+version = "0.7.3"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `ever_playground-0.7.1/README.md` & `ever_playground-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/create-param8.py` & `ever_playground-0.7.3/create-param8.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/ever_playground/__init__.py` & `ever_playground-0.7.3/ever_playground/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from enum import Enum
 from typing import Optional, Tuple
 from fractions import Fraction
 
-from .ever_playground import Cell, Builder, Slice, Dictionary, Gas, Continuation, ContinuationType, SaveList, VmState, VmResult, assemble, runvm_generic
+from .ever_playground import Cell, Builder, Slice, Dictionary, NaN, Gas, Continuation, ContinuationType, SaveList, VmState, VmResult, assemble, runvm_generic
 from .ever_playground import ed25519_new_keypair, ed25519_secret_to_public, ed25519_sign, ed25519_check_signature
 
 __all__ = [
     "Cell",
     "Builder",
     "Slice",
     "Dictionary",
+    "NaN",
     "ExceptionCode",
     "StateInit",
     "assemble",
+    "Gas",
+    "ContinuationType",
+    "Continuation",
+    "SaveList",
     "VmState",
     "VmResult",
     "runvm_generic",
     "runvm",
     "parse_smc_addr",
     "load_address",
     "parse_load_address",
@@ -24,27 +29,41 @@
     "ed25519_new_keypair",
     "ed25519_secret_to_public",
     "ed25519_sign",
     "ed25519_check_signature",
 ]
 
 def runvm(code, stack, **kwargs) -> VmResult:
+    """
+    Invokes TVM with the current continuation cc initialized from the ``code`` slice and
+    the ``stack`` of values.
+
+    Optional parameters:
+     - capabilities: int
+     - c4: Cell
+     - c7: list
+     - gas_limit: int
+     - gas_credit: int
+     - trace: bool
+
+    Returns VmResult.    
+    """
     cc = Continuation(
         ContinuationType.create_ordinary(),
         code,
         stack,
         SaveList(),
         -1
     )
 
     regs = SaveList()
     capabilities = 0
     trace = False
-    gas_limit = 1000000000
-    gas_credit = 10000
+    gas_limit = 1_000_000_000
+    gas_credit = 10_000
     for key, value in kwargs.items():
         if key == "capabilities":
             capabilities = int(value)
         elif key == "trace":
             trace = bool(value)
         elif key == "c4":
             regs.put(4, value)
```

### Comparing `ever_playground-0.7.1/examples/basics.py` & `ever_playground-0.7.3/examples/basics.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/highload/generate.fif` & `ever_playground-0.7.3/examples/highload/generate.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/highload/highload-wallet-v2.fif` & `ever_playground-0.7.3/examples/highload/highload-wallet-v2.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/highload/highload-wallet-v2.py` & `ever_playground-0.7.3/examples/highload/highload-wallet-v2.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/ifjmp-perf-eval.py` & `ever_playground-0.7.3/examples/ifjmp-perf-eval.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/recover-stake.fif` & `ever_playground-0.7.3/examples/recover-stake.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/recover-stake.py` & `ever_playground-0.7.3/examples/recover-stake.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/runvm.py` & `ever_playground-0.7.3/examples/runvm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 from ever_playground import Cell as C
 from ever_playground import Slice as S
 from ever_playground import ExceptionCode
-from ever_playground import StateInit, VmState, runvm, assemble
+from ever_playground import StateInit, runvm, assemble
 
 def expect(expected, v):
     if not expected == v:
         raise Exception("{} != {}".format(expected, v))
 
 add = assemble("""
     ADD
```

### Comparing `ever_playground-0.7.1/examples/testgiver.fif` & `ever_playground-0.7.3/examples/testgiver.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/testgiver.py` & `ever_playground-0.7.3/examples/testgiver.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/validator-elect-req.fif` & `ever_playground-0.7.3/examples/validator-elect-req.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/examples/validator-elect-req.py` & `ever_playground-0.7.3/examples/validator-elect-req.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/pyproject.toml` & `ever_playground-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/run-examples.py` & `ever_playground-0.7.3/run-examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,18 @@
     assert(p == f)
 
     os.chdir(curdir)
 
 def test_ifjmp_perf_eval():
     run(["python3", "examples/ifjmp-perf-eval.py"])
 
+def run_runcont():
+    run(["python3", "examples/runcont.py"])
+
 run_basics()
 run_runvm()
+run_runcont()
 test_recover_stake()
 test_testgiver()
 test_validator_elect_req()
 test_highload_wallet_v2()
 test_ifjmp_perf_eval()
```

### Comparing `ever_playground-0.7.1/src/crypto.rs` & `ever_playground-0.7.3/src/crypto.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/src/lib.rs` & `ever_playground-0.7.3/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         for arg in args.iter() {
             let cell = arg.extract::<PyCell>()?;
             b.checked_append_reference(cell.cell).map_err(runtime_err)?;
         }
         let cell = b.into_cell().map_err(runtime_err)?;
         Ok(Self::new(cell))
     }
+    #[staticmethod]
+    fn empty() -> Self {
+        Self::new(Cell::default())
+    }
     fn reference(&self, index: usize) -> PyResult<Self> {
         self.cell.reference(index)
             .map(|cell| Self::new(cell))
             .map_err(runtime_err)
     }
     fn write<'a>(&'a self, py: Python<'a>, flags: usize) -> PyResult<&PyBytes> {
         if flags > 3 {
@@ -89,27 +93,27 @@
                     stack.push(cell.reference(i).unwrap())
                 }
             }
         }
         Ok(unique_count)
     }
     fn __str__(&self) -> PyResult<String> {
-        PyResult::Ok(dump_cell(self.cell.clone()))
+        Ok(dump_cell(self.cell.clone()))
     }
     fn __richcmp__(&self, other: Self, op: CompareOp, py: Python<'_>) -> PyObject {
         match op {
             CompareOp::Eq => self.cell.eq(&other.cell).into_py(py),
             CompareOp::Ne => self.cell.ne(&other.cell).into_py(py),
             _ => py.NotImplemented(),
         }
     }
 }
 
 #[pyclass(name = "Slice")]
-#[derive(Clone)]
+#[derive(Clone, Default)]
 struct PySlice {
     slice: SliceData,
 }
 
 impl PySlice {
     fn new(slice: SliceData) -> Self {
         Self { slice }
@@ -326,29 +330,38 @@
 #[pyfunction]
 fn assemble(code: String) -> PyResult<PyCell> {
     let slice = ton_labs_assembler::compile_code(&code)
         .map_err(|err| PyRuntimeError::new_err(err.to_string()))?;
     Ok(PyCell::new(slice.cell().clone()))
 }
 
+#[derive(Clone)]
 #[pyclass(name = "NaN")]
 struct PyNaN {
 }
 
 impl PyNaN {
     fn new() -> Self {
         Self { }
     }
 }
 
 #[pymethods]
 impl PyNaN {
     #[new]
     fn create() -> Self {
-        Self::new()
+        PyNaN::new()
+    }
+    // TODO consider making PyNaN a singleton instead
+    fn __richcmp__(&self, _other: Self, op: CompareOp, py: Python<'_>) -> PyObject {
+        match op {
+            CompareOp::Eq => true.into_py(py),
+            CompareOp::Ne => false.into_py(py),
+            _ => py.NotImplemented(),
+        }
     }
 }
 
 #[pymodule]
 fn ever_playground(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PyNaN>()?;
     m.add_class::<PyCell>()?;
```

### Comparing `ever_playground-0.7.1/src/tests.rs` & `ever_playground-0.7.3/src/tests.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/src/utils.rs` & `ever_playground-0.7.3/src/utils.rs`

 * *Files 9% similar despite different names*

```diff
@@ -141,53 +141,55 @@
 pub(crate) fn convert_to_vm(value: &PyAny) -> PyResult<StackItem> {
     if value.is_none() {
         Ok(StackItem::None)
     } else if let Ok(v) = value.downcast::<PyLong>() {
         let integer = IntegerData::from(v.extract::<BigInt>()?)
             .map_err(runtime_err)?;
         Ok(StackItem::Integer(Arc::new(integer)))
+    } else if let Ok(_) = value.extract::<crate::PyNaN>() {
+        Ok(StackItem::Integer(Arc::new(IntegerData::nan())))
     } else if let Ok(v) = value.downcast::<PyList>() {
         let mut tuple = Vec::new();
         for item in v {
             tuple.push(convert_to_vm(item)?)
         }
         Ok(StackItem::Tuple(Arc::new(tuple)))
     } else if let Ok(v) = value.extract::<PyCell>() {
         Ok(StackItem::Cell(v.cell))
     } else if let Ok(v) = value.extract::<PySlice>() {
         Ok(StackItem::Slice(v.slice))
     } else if let Ok(v) = value.extract::<PyBuilder>() {
         Ok(StackItem::Builder(Arc::new(v.builder)))
     } else if let Ok(v) = value.extract::<PyContinuation>() {
-        Ok(StackItem::Continuation(Arc::new(v.cont)))
+        Ok(StackItem::Continuation(Arc::new(v.cont(value.py())?)))
     } else {
         return err!("unsupported value {}", value)
     }
 }
 
-pub(crate) fn convert_from_vm(py: Python<'_>, item: &StackItem) -> PyObject {
+pub(crate) fn convert_from_vm(py: Python<'_>, item: &StackItem) -> PyResult<PyObject> {
     match item {
         StackItem::None =>
-            py.None(),
+            Ok(py.None()),
         StackItem::Builder(v) =>
-            PyBuilder::new(v.as_ref().clone()).into_py(py),
+            Ok(PyBuilder::new(v.as_ref().clone()).into_py(py)),
         StackItem::Cell(v) =>
-            crate::PyCell::new(v.clone()).into_py(py),
+            Ok(crate::PyCell::new(v.clone()).into_py(py)),
         StackItem::Continuation(cont) =>
-            PyContinuation::new(cont.as_ref().clone()).into_py(py),
+            Ok(PyContinuation::new(py, cont.as_ref())?.into_py(py)),
         StackItem::Integer(v) => {
             match process_value(v.as_ref(), |v| Ok(v.clone())) {
-                Err(_) => PyNaN::new().into_py(py),
-                Ok(v) => v.into_py(py),
+                Err(_) => Ok(PyNaN::new().into_py(py)),
+                Ok(v) => Ok(v.into_py(py)),
             }
         }
         StackItem::Slice(v) =>
-            PySlice::new(v.clone()).into_py(py),
+            Ok(PySlice::new(v.clone()).into_py(py)),
         StackItem::Tuple(v) => {
             let mut list = Vec::new();
             for item in v.iter() {
-                list.push(convert_from_vm(py, item))
+                list.push(convert_from_vm(py, item)?)
             }
-            PyList::new(py, list).into_py(py)
+            Ok(PyList::new(py, list).into_py(py))
         }
     }
 }
```

### Comparing `ever_playground-0.7.1/src/vm.rs` & `ever_playground-0.7.3/src/vm.rs`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     }
     #[getter]
     fn credit(&self) -> i64 {
         self.gas.get_gas_credit()
     }
 }
 
-#[derive(Clone, Default)]
+#[derive(Clone)]
 #[pyclass(get_all, name = "VmState")]
 pub(crate) struct PyVmState {
     cc: PyContinuation,
     regs: PySaveList,
     steps: u32,
     gas: PyGas,
     committed_c4: Option<crate::PyCell>,
@@ -78,39 +78,41 @@
         regs: PySaveList,
         gas: PyGas,
     ) -> Self {
         Self::new(cc, regs, 0, gas, None, None)
     }
 }
 
-#[derive(Default)]
 #[pyclass(get_all, name = "VmResult")]
 pub(crate) struct PyVmResult {
     state: PyVmState,
     exit_code: i32,
     exception_value: Option<PyObject>,
 }
 
 #[pyfunction]
+#[pyo3(signature = (state, capabilities = 0, trace = false))]
 pub(crate) fn runvm_generic(py: Python<'_>, state: PyVmState, capabilities: u64, trace: bool) -> PyResult<PyObject> {
+    let cc = state.cc.cont(py)?;
     let mut engine = Engine::with_capabilities(capabilities).setup(
-        state.cc.cont.code().clone(),
+        cc.code().clone(),
         Some(state.regs.savelist),
-        Some(state.cc.cont.stack),
+        Some(cc.stack),
         Some(state.gas.gas)
     );
     if trace {
         engine.set_trace_callback(trace_callback);
     }
-    let mut result = PyVmResult::default();
+    let exit_code;
+    let mut exception_value = None;
     match engine.execute() {
-        Ok(exit_code) => result.exit_code = exit_code,
+        Ok(code) => exit_code = code,
         Err(err) => if let Some(exception) = tvm_exception_full(&err) {
-            result.exit_code = exception.exception_or_custom_code();
-            result.exception_value = Some(convert_from_vm(py, &exception.value));
+            exit_code = exception.exception_or_custom_code();
+            exception_value = Some(convert_from_vm(py, &exception.value)?);
         } else {
             return Err(PyRuntimeError::new_err(format!("execution failed: {}", err)))
         }
     }
 
     let committed_state = engine.get_committed_state();
     let (committed_c4, committed_c5) = if committed_state.is_committed() {
@@ -119,22 +121,27 @@
         let c4 = c4.as_cell().map_err(runtime_err)?.clone();
         let c5 = c5.as_cell().map_err(runtime_err)?.clone();
         (Some(crate::PyCell::new(c4)), Some(crate::PyCell::new(c5)))
     } else {
         (None, None)
     };
 
-    result.state = PyVmState::new(
-        PyContinuation::new(engine.cc().clone()),
+    let result_state = PyVmState::new(
+        PyContinuation::new(py, engine.cc())?,
         PySaveList::new(engine.ctrls().clone()),
         engine.steps(),
         PyGas::new(engine.get_gas().clone()),
         committed_c4,
         committed_c5,
     );
+    let result = PyVmResult {
+        state: result_state,
+        exit_code,
+        exception_value,
+    };
     Ok(result.into_py(py))
 }
 
 fn trace_callback(_engine: &Engine, info: &EngineTraceInfo) {
     use ton_vm::executor::EngineTraceInfoType::*;
     match &info.info_type {
         Start => { }
```

### Comparing `ever_playground-0.7.1/try-catch.py` & `ever_playground-0.7.3/try-catch.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/ttt.py` & `ever_playground-0.7.3/ttt.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.7.1/Cargo.lock` & `ever_playground-0.7.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.7.1"
+version = "0.7.3"
 dependencies = [
  "ed25519-dalek",
  "num-bigint",
  "pyo3",
  "rand",
  "ton_block 1.9.74",
  "ton_labs_assembler",
```

### Comparing `ever_playground-0.7.1/PKG-INFO` & `ever_playground-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.7.1
+Version: 0.7.3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

