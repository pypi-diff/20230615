# Comparing `tmp/floodgate_rs-0.1.1.tar.gz` & `tmp/floodgate_rs-0.1.2.tar.gz`

## Comparing `floodgate_rs-0.1.1.tar` & `floodgate_rs-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 floodgate_rs-0.1.1/Cargo.toml
--rw-r--r--   0     1001      122     2009 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/.github/workflows/release.yml
--rw-r--r--   0     1001      122      685 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/.gitignore
--rw-r--r--   0     1001      122     1068 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/LICENSE
--rw-r--r--   0     1001      122      516 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/README.md
--rw-r--r--   0     1001      122      187 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/floodgate/__init__.py
--rw-r--r--   0     1001      122     1499 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/floodgate/floodgate.pyi
--rw-r--r--   0     1001      122        0 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/floodgate/py.typed
--rw-r--r--   0     1001      122     1094 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/pyproject.toml
--rw-r--r--   0     1001      122     2323 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/src/dynamic_mapping.rs
--rw-r--r--   0     1001      122     1837 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/src/fixed_mapping.rs
--rw-r--r--   0     1001      122     1235 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/src/jumping_window.rs
--rw-r--r--   0     1001      122      374 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/src/lib.rs
--rw-r--r--   0     1001      122      755 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/src/traits.rs
--rw-r--r--   0     1001      122    15606 2022-12-04 23:01:44.000000 floodgate_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 floodgate_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 floodgate_rs-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2009 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      685 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/.gitignore
+-rw-r--r--   0     1001      123     1068 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/LICENSE
+-rw-r--r--   0     1001      123      516 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/README.md
+-rw-r--r--   0     1001      123      186 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/__init__.py
+-rw-r--r--   0     1001      123    11914 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/floodgate.pyi
+-rw-r--r--   0     1001      123        0 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/floodgate/py.typed
+-rw-r--r--   0     1001      123     1094 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     2323 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/dynamic_mapping.rs
+-rw-r--r--   0     1001      123     1837 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/fixed_mapping.rs
+-rw-r--r--   0     1001      123     1235 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/jumping_window.rs
+-rw-r--r--   0     1001      123      374 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123      755 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/src/traits.rs
+-rw-r--r--   0     1001      123    15606 2023-06-14 22:08:12.000000 floodgate_rs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 floodgate_rs-0.1.2/PKG-INFO
```

### Comparing `floodgate_rs-0.1.1/.github/workflows/release.yml` & `floodgate_rs-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/.gitignore` & `floodgate_rs-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/LICENSE` & `floodgate_rs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/README.md` & `floodgate_rs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/pyproject.toml` & `floodgate_rs-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "floodgate-rs"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 description = "Python bindings for, a ratelimiting library written in Rust."
```

### Comparing `floodgate_rs-0.1.1/src/dynamic_mapping.rs` & `floodgate_rs-0.1.2/src/dynamic_mapping.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/src/fixed_mapping.rs` & `floodgate_rs-0.1.2/src/fixed_mapping.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/src/jumping_window.rs` & `floodgate_rs-0.1.2/src/jumping_window.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/src/traits.rs` & `floodgate_rs-0.1.2/src/traits.rs`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/Cargo.lock` & `floodgate_rs-0.1.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `floodgate_rs-0.1.1/PKG-INFO` & `floodgate_rs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floodgate-rs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for, a ratelimiting library written in Rust.
 Keywords: cooldown,ratelimit,rate limit,rust,pyo3
 License: MIT
```

