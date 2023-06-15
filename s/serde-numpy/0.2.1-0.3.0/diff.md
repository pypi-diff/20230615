# Comparing `tmp/serde_numpy-0.2.1.tar.gz` & `tmp/serde_numpy-0.3.0.tar.gz`

## Comparing `serde_numpy-0.2.1.tar` & `serde_numpy-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,33 @@
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 serde_numpy-0.2.1/Cargo.toml
--rw-rw-r--   0     1000     1000       59 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/.gitignore
--rw-rw-r--   0     1000     1000     1062 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/LICENSE
--rw-rw-r--   0     1000     1000     4094 2023-02-10 16:08:35.000000 serde_numpy-0.2.1/README.md
--rw-rw-r--   0     1000     1000    15288 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/poetry.lock
--rw-rw-r--   0     1000     1000   145331 2023-02-10 16:08:20.000000 serde_numpy-0.2.1/profile/2darr_profile.png
--rw-rw-r--   0     1000     1000     6600 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/profile/profile.py
--rw-rw-r--   0     1000     1000    20967 2023-02-10 16:09:04.000000 serde_numpy-0.2.1/profile/transpose_profile.png
--rw-rw-r--   0     1000     1000     1174 2023-02-10 16:03:54.000000 serde_numpy-0.2.1/pyproject.toml
--rw-rw-r--   0     1000     1000       43 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/pytest.ini
--rw-rw-r--   0     1000     1000      494 2023-02-10 16:10:44.000000 serde_numpy-0.2.1/release.py
--rw-rw-r--   0     1000     1000     2305 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/src/lib.rs
--rw-rw-r--   0     1000     1000     9901 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/src/parsing/array_types.rs
--rw-rw-r--   0     1000     1000     1289 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/src/parsing/python_types.rs
--rw-rw-r--   0     1000     1000     6822 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/src/parsing/transpose_types.rs
--rw-rw-r--   0     1000     1000    25619 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/src/parsing.rs
--rw-rw-r--   0     1000     1000        0 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/tests/__init__.py
--rw-rw-r--   0     1000     1000     2384 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/tests/fixtures.py
--rw-rw-r--   0     1000     1000     5734 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/tests/test_errors.py
--rw-rw-r--   0     1000     1000     9043 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/tests/test_successes.py
--rw-rw-r--   0     1000     1000     2204 2023-02-10 15:36:34.000000 serde_numpy-0.2.1/tests/utils.py
--rw-rw-r--   0     1000     1000    11609 2023-02-10 16:06:22.000000 serde_numpy-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 serde_numpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 serde_numpy-0.3.0/Cargo.toml
+-rw-rw-r--   0     1000     1000       72 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/.gitignore
+-rw-rw-r--   0     1000     1000     1062 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/LICENSE
+-rw-rw-r--   0     1000     1000     5830 2023-06-15 15:11:30.000000 serde_numpy-0.3.0/README.md
+-rw-rw-r--   0     1000     1000    15288 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/poetry.lock
+-rw-rw-r--   0     1000     1000   135495 2023-06-15 15:07:35.000000 serde_numpy-0.3.0/profile/2darr_profile.png
+-rw-rw-r--   0     1000     1000        0 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/profile/__init__.py
+-rw-rw-r--   0     1000     1000      622 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/profile/img_util.py
+-rw-rw-r--   0     1000     1000    18211 2023-06-15 15:08:20.000000 serde_numpy-0.3.0/profile/jpeg_profile.png
+-rw-rw-r--   0     1000     1000     1955 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/profile/json_util.py
+-rw-rw-r--   0     1000     1000    19180 2023-06-15 15:08:34.000000 serde_numpy-0.3.0/profile/png_profile.png
+-rw-rw-r--   0     1000     1000     7393 2023-06-15 15:07:52.000000 serde_numpy-0.3.0/profile/profile.py
+-rw-rw-r--   0     1000     1000    20988 2023-06-15 15:08:16.000000 serde_numpy-0.3.0/profile/transpose_profile.png
+-rw-rw-r--   0     1000     1000     1211 2023-06-15 15:15:59.000000 serde_numpy-0.3.0/pyproject.toml
+-rw-rw-r--   0     1000     1000       43 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/pytest.ini
+-rw-rw-r--   0     1000     1000      494 2023-02-10 16:10:44.000000 serde_numpy-0.3.0/release.py
+-rw-rw-r--   0     1000     1000     1813 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/src/img.rs
+-rw-rw-r--   0     1000     1000     3584 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     9901 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/src/parsing/array_types.rs
+-rw-rw-r--   0     1000     1000     1289 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/src/parsing/python_types.rs
+-rw-rw-r--   0     1000     1000     6822 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/src/parsing/transpose_types.rs
+-rw-rw-r--   0     1000     1000    25630 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/src/parsing.rs
+-rw-rw-r--   0     1000     1000        0 2023-02-10 15:36:34.000000 serde_numpy-0.3.0/tests/__init__.py
+-rw-rw-r--   0     1000     1000        0 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/img/__init__.py
+-rw-rw-r--   0     1000     1000     2578 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/img/fixtures.py
+-rw-rw-r--   0     1000     1000     2308 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/img/test_sucesses.py
+-rw-rw-r--   0     1000     1000        0 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/json/__init__.py
+-rw-rw-r--   0     1000     1000     2384 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/json/fixtures.py
+-rw-rw-r--   0     1000     1000     5734 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/json/test_errors.py
+-rw-rw-r--   0     1000     1000     9043 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/json/test_successes.py
+-rw-rw-r--   0     1000     1000     2204 2023-06-15 14:59:49.000000 serde_numpy-0.3.0/tests/json/utils.py
+-rw-rw-r--   0     1000     1000    14563 2023-06-15 15:13:15.000000 serde_numpy-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     6973 1970-01-01 00:00:00.000000 serde_numpy-0.3.0/PKG-INFO
```

### Comparing `serde_numpy-0.2.1/LICENSE` & `serde_numpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/poetry.lock` & `serde_numpy-0.3.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/profile/profile.py` & `serde_numpy-0.3.0/profile/profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,178 +1,253 @@
-from typing import Callable, List, Mapping, Sequence, Type, Tuple, Any
-import json
+from typing import Mapping, Sequence, Type
 import time
 
 import numpy as np
-import orjson
-import json
-import string
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 
-from serde_numpy import NumpyDeserializer
+from serde_numpy import NumpyDeserializer, decode_jpeg, decode_png
+from img_util import (
+    get_random_img,
+    get_jpeg_bytes,
+    get_png_bytes,
+    decode_pillow
+)
+from json_util import (
+    make_data,
+    make_transposed_data,
+    orjson_then_numpy,
+    orjson_then_numpy_tranpose,
+)
 
 PLOT_COLS = 3
 np.random.seed(33)
 
 
-def make_array(shape: Tuple[int, ...], dtype: Type) -> List[Any]:
-    if dtype in [int, np.int16, np.int32, np.int64]:
-        return np.random.randint(-2**15, 2**15, size=shape).tolist()
-    elif dtype in [np.uint16, np.uint32, np.uint64]:
-        return np.random.randint(0, 2**16, size=shape).tolist()
-    elif dtype in [float, np.float16, np.float32, np.float64]:
-        return (np.random.randn(np.prod(shape)).reshape(shape) * 2**8).tolist()
-    elif dtype in [bool, np.bool_]:
-        return (np.random.rand(np.prod(shape)).reshape(shape) < 0.5).tolist()
-    elif dtype == str:
-        return np.random.choice(list(string.ascii_letters), np.prod(shape), replace=True).reshape(shape).tolist()
-    else:
-        raise ValueError(f"dtype: {dtype} not recognised.")
-
-
-def make_data(shape: Tuple[int, ...], dtype: Type) -> bytes:
-    return str.encode(json.dumps(dict(key=make_array(shape, dtype))))
-
-
-def tranpose_lol(lol: List[List[Any]]) -> List[List[Any]]:
-    return [list(row) for row in zip(*lol)]
-
-
-def make_transposed_data(n_rows: int, dtypes: Sequence[Type]) -> bytes:
-    data = [ make_array((n_rows,), dtype) for dtype in dtypes]
-    data = tranpose_lol(data)
-    return str.encode(json.dumps(dict(key=data)))
-
-
-def orjson_then_numpy(json_str: bytes, dtype: Type) -> Mapping[str, np.ndarray]:
-    out = orjson.loads(json_str)
-    out["key"] = np.array(out["key"], dtype)
-    return out
-
-
-def orjson_then_numpy_tranpose(json_str: bytes, dtypes: Sequence[Type]) -> Mapping[str, np.ndarray]:
-    out = orjson.loads(json_str)
-    out["key"] = tranpose_lol(out["key"])
-    out["key"] = [np.array(out["key"][i], dtype) for i, dtype in enumerate(dtypes)]
-    return out
-
-
-def serde_numpy(json_str: bytes, deserialize: Callable) -> Mapping[str, List[np.ndarray]]:
-    return deserialize(json_str, )
-
-
 def _get_dtype(name: str) -> type:
     try:
         return eval(name)
     except NameError:
         return getattr(np, name)
 
 
-def get_times_2d_array(n_rows: Sequence[int], n_cols: Sequence[int], dtype: Type, n_iters: int = 10) -> Mapping[str, np.ndarray]:
+def get_times_2d_array(
+    n_rows: Sequence[int], n_cols: Sequence[int], dtype: Type, n_iters: int = 10
+) -> Mapping[str, np.ndarray]:
     times_orjson = []
     times_serde_numpy = []
     n_rows_ = []
     n_cols_ = []
     deserializer = NumpyDeserializer.from_dict(dict(key=dtype))
     for rows in n_rows:
         for cols in n_cols:
             data = make_data((rows, cols), dtype)
             n_rows_.append(rows)
             n_cols_.append(cols)
             orjson_times_ = []
             serde_np_times_ = []
             for _ in range(n_iters):
-                
                 time0 = time.time()
                 _ = orjson_then_numpy(data, dtype)
                 orjson_times_.append(time.time() - time0)
 
                 time0 = time.time()
                 _ = deserializer.deserialize_json(data)
                 serde_np_times_.append(time.time() - time0)
-                
+
             times_orjson.append(np.median(orjson_times_))
             times_serde_numpy.append(np.median(serde_np_times_))
 
-    return dict(n_rows=np.array(n_rows_), 
-                n_cols=np.array(n_cols_), 
-                orjson_plus_numpy_time=np.array(times_orjson), 
-                serde_numpy_time=np.array(times_serde_numpy))
+    return dict(
+        n_rows=np.array(n_rows_),
+        n_cols=np.array(n_cols_),
+        orjson_plus_numpy_time=np.array(times_orjson),
+        serde_numpy_time=np.array(times_serde_numpy),
+    )
 
 
-def get_times_transposed_arrays(n_rows: Sequence[int], dtypes: Sequence[Type], n_iters: int = 10) -> Mapping[str, np.ndarray]:
+def get_times_transposed_arrays(
+    n_rows: Sequence[int], dtypes: Sequence[Type], n_iters: int = 10
+) -> Mapping[str, np.ndarray]:
     times_orjson = []
     times_serde_numpy = []
     n_rows_ = []
     deserializer = NumpyDeserializer.from_dict(dict(key=[dtypes]))
     for rows in n_rows:
         data = make_transposed_data(rows, dtypes)
         n_rows_.append(rows)
         orjson_times_ = []
         serde_np_times_ = []
         for _ in range(n_iters):
-            
             time0 = time.time()
             _ = orjson_then_numpy_tranpose(data, dtypes)
             orjson_times_.append(time.time() - time0)
 
             time0 = time.time()
             _ = deserializer.deserialize_json(data)
             serde_np_times_.append(time.time() - time0)
-            
+
         times_orjson.append(np.median(orjson_times_))
         times_serde_numpy.append(np.median(serde_np_times_))
 
-    return dict(n_rows=np.array(n_rows_),
-                orjson_plus_numpy_time=np.array(times_orjson), 
-                serde_numpy_time=np.array(times_serde_numpy))
+    return dict(
+        n_rows=np.array(n_rows_),
+        orjson_plus_numpy_time=np.array(times_orjson),
+        serde_numpy_time=np.array(times_serde_numpy),
+    )
 
 
-def plot_times_2d_array(times_rows: Mapping[str, np.ndarray], times_cols: Mapping[str, np.ndarray], ax: plt.Axes, title: str):
-    ax.plot(times_rows["n_rows"], times_rows["orjson_plus_numpy_time"] / times_rows["serde_numpy_time"], alpha=0.5)
-    ax.plot(times_cols["n_cols"], times_cols["orjson_plus_numpy_time"] / times_cols["serde_numpy_time"], alpha=0.5)
+def get_times_jpeg() -> Mapping[str, np.ndarray]:
+    sizes = [2**i for i in range(2, 14)]
+    times_pillow = []
+    times_serde_numpy = []
+    for size in sizes:
+        img = get_random_img(size)
+        jpeg_bytes = get_jpeg_bytes(img)
+        time0 = time.time()
+        _ = decode_pillow(jpeg_bytes)
+        times_pillow.append(time.time() - time0)
+
+        time0 = time.time()
+        _ = decode_jpeg(
+            jpeg_bytes
+        )
+        times_serde_numpy.append(time.time() - time0)
+    return dict(
+        sizes=np.array(sizes),
+        pillow_time=np.array(times_pillow),
+        serde_numpy_time=np.array(times_serde_numpy),
+    )
+
+
+def get_times_png() -> Mapping[str, np.ndarray]:
+    sizes = [2**i for i in range(2, 14)]
+    times_pillow = []
+    times_serde_numpy = []
+    for size in sizes:
+        img = get_random_img(size)
+        png_bytes = get_png_bytes(img)
+        time0 = time.time()
+        _ = decode_pillow(png_bytes)
+        times_pillow.append(time.time() - time0)
+
+        time0 = time.time()
+        _ = decode_png(
+            png_bytes
+        )
+        times_serde_numpy.append(time.time() - time0)
+    return dict(
+        sizes=np.array(sizes),
+        pillow_time=np.array(times_pillow),
+        serde_numpy_time=np.array(times_serde_numpy),
+    )
+
+
+def plot_times_2d_array(
+    times_rows: Mapping[str, np.ndarray],
+    times_cols: Mapping[str, np.ndarray],
+    ax: plt.Axes,
+    title: str,
+):
+    ax.plot(
+        times_rows["n_rows"],
+        times_rows["orjson_plus_numpy_time"] / times_rows["serde_numpy_time"],
+        alpha=0.5,
+    )
+    ax.plot(
+        times_cols["n_cols"],
+        times_cols["orjson_plus_numpy_time"] / times_cols["serde_numpy_time"],
+        alpha=0.5,
+    )
     ax.grid()
     ax.set_xscale("log")
     ax.legend(["n_rows", "n_cols"])
     ax.set_title(title)
     ax.set_ylabel("speed up")
 
 
 def run_profile_2d_array(dtypes: Sequence[type]):
     print("Profiling 2D array deserialization...")
-    n_rows = (2**np.arange(0, 20, 2)).astype(int)
-    n_cols = (2**np.arange(0, 20, 2)).astype(int)
+    n_rows = (2 ** np.arange(0, 20, 2)).astype(int)
+    n_cols = (2 ** np.arange(0, 20, 2)).astype(int)
     plot_rows = int(np.ceil(len(dtypes) / PLOT_COLS))
-    fig = plt.figure(figsize=(6*PLOT_COLS, 4*plot_rows))
+    fig = plt.figure(figsize=(6 * PLOT_COLS, 4 * plot_rows))
     gs = gridspec.GridSpec(plot_rows, PLOT_COLS)
     for i, dtype in enumerate(dtypes):
         times_rows = get_times_2d_array(n_rows, [10], dtype)
         times_cols = get_times_2d_array([10], n_cols, dtype)
         ax = fig.add_subplot(gs[i // PLOT_COLS, i % PLOT_COLS])
         plot_times_2d_array(times_rows, times_cols, ax, dtype.__name__)
-    plt.savefig("profile/2darr_profile.png", pad_inches = 0) 
+    plt.savefig("./2darr_profile.png", pad_inches=0, bbox_inches='tight')
 
 
 def run_profile_transposed_arrays(dtypes: Sequence[type]):
-    print("Profiling tranposed arrays deserialization...")
-    n_rows = (2**np.arange(0, 22, 2)).astype(int)
+    print("Profiling transposed arrays deserialization...")
+    n_rows = (2 ** np.arange(0, 22, 2)).astype(int)
     times = get_times_transposed_arrays(n_rows, dtypes)
     fig = plt.figure(figsize=(6, 4))
-    plt.plot(times["n_rows"], times["orjson_plus_numpy_time"] / times["serde_numpy_time"], alpha=0.5)
+    plt.plot(
+        times["n_rows"],
+        times["orjson_plus_numpy_time"] / times["serde_numpy_time"],
+        alpha=0.5,
+    )
     plt.grid()
     plt.xscale("log")
     plt.legend(["n_rows"])
     plt.title([dtype.__name__ for dtype in dtypes], fontsize=10)
     plt.ylabel("speed up")
-    plt.savefig("profile/transpose_profile.png", pad_inches = 0)
+    plt.savefig("./transpose_profile.png", pad_inches=0, bbox_inches='tight')
+
+
+def run_profile_jpeg():
+    print("Profiling JPEG decoding...")
+    times = get_times_jpeg()
+    fig = plt.figure(figsize=(6, 4))
+    plt.plot(
+        times["sizes"],
+        times["pillow_time"] / times["serde_numpy_time"],
+        alpha=0.5,
+    )
+    plt.grid()
+    plt.xscale("log")
+    plt.xlabel("image size (n x n)")
+    plt.title("JPEG decoding", fontsize=10)
+    plt.ylabel("speed up")
+    plt.savefig("./jpeg_profile.png", pad_inches=0, bbox_inches='tight')
+
+
+def run_profile_png():
+    print("Profiling PNG decoding...")
+    times = get_times_png()
+    fig = plt.figure(figsize=(6, 4))
+    plt.plot(
+        times["sizes"],
+        times["pillow_time"] / times["serde_numpy_time"],
+        alpha=0.5,
+    )
+    plt.grid()
+    plt.xscale("log")
+    plt.xlabel("image size (n x n)")
+    plt.title("PNG decoding", fontsize=10)
+    plt.ylabel("speed up")
+    plt.savefig("./png_profile.png", pad_inches=0, bbox_inches='tight')
+
 
-        
 if __name__ == "__main__":
     import sys
-    dtypes = [_get_dtype(s) for s in sys.argv[1:]] or [np.int16, np.int32, np.int64, np.uint16, np.uint32, np.uint64, np.float32, np.float64, np.bool_]
+
+    dtypes = [_get_dtype(s) for s in sys.argv[1:]] or [
+        np.int16,
+        np.int32,
+        np.int64,
+        np.uint16,
+        np.uint32,
+        np.uint64,
+        np.float32,
+        np.float64,
+        np.bool_,
+    ]
     run_profile_2d_array(dtypes)
     run_profile_transposed_arrays(dtypes)
+    run_profile_jpeg()
+    run_profile_png()
     print("Done.")
-
-
-
```

### Comparing `serde_numpy-0.2.1/pyproject.toml` & `serde_numpy-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "maturin"
 requires = ["maturin>=0.13"]
 
 [project]
 name = "serde-numpy"
-version = "0.2.1"
+version = "0.3.0"
 description = "A library for deserializing various formats directly into numpy arrays"
 authors = [{name="Will Norcliffe Brown"}]
 dependencies = ["numpy>=1.18"]
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -23,14 +23,16 @@
     "Programming Language :: Python",
     "Programming Language :: Rust",
     "Typing :: Typed",
 ]
 
 [dev-dependencies]
 pytest = "^6.1"
+pillow = "^9.5"
+scikit-image= "^3.0"
 
 [project.urls]
 homepage = "https://github.com/wnorcbrown/serde-numpy"
 documentation = "https://github.com/wnorcbrown/serde-numpy"
 repository = "https://github.com/wnorcbrown/serde-numpy"
 
 [tool.maturin]
```

### Comparing `serde_numpy-0.2.1/src/parsing/array_types.rs` & `serde_numpy-0.3.0/src/parsing/array_types.rs`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/src/parsing/python_types.rs` & `serde_numpy-0.3.0/src/parsing/python_types.rs`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/src/parsing/transpose_types.rs` & `serde_numpy-0.3.0/src/parsing/transpose_types.rs`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/src/parsing.rs` & `serde_numpy-0.3.0/src/parsing.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use serde_json::Value;
 
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::{IntoPy, PyAny, PyErr, PyObject, PyResult, Python};
 use pyo3::types::PyType;
 use pyo3::FromPyObject;
 
-mod array_types;
+pub(crate) mod array_types;
 mod python_types;
 mod transpose_types;
 use array_types::{Array, BoolArray};
 use python_types::PythonType;
 use transpose_types::{TransposeMap, TransposeSeq};
 
 #[derive(Clone, Debug, Deserialize)]
```

### Comparing `serde_numpy-0.2.1/tests/fixtures.py` & `serde_numpy-0.3.0/tests/json/fixtures.py`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/tests/test_errors.py` & `serde_numpy-0.3.0/tests/json/test_errors.py`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/tests/test_successes.py` & `serde_numpy-0.3.0/tests/json/test_successes.py`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/tests/utils.py` & `serde_numpy-0.3.0/tests/json/utils.py`

 * *Files identical despite different names*

### Comparing `serde_numpy-0.2.1/Cargo.lock` & `serde_numpy-0.3.0/Cargo.lock`

 * *Files 21% similar despite different names*

```diff
@@ -11,153 +11,164 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.0.1"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdb031dd78e28731d87d56cc8ffef4a8f36ca26c38fe2de700543e627f8a464a"
+checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6dbe3c979c178231552ecba20214a8272df4e09f232a87aef4320cf06539aded"
+
+[[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+
+[[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "either"
-version = "1.6.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "itertools"
 version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d47946d458e94a1b7bcabbf6521ea7c037062c81f534615abcad76e84d4970d"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "0.4.8"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.5"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712a4d093c9976e24e7dbca41db895dabcbac38eb5f4045393d17a95bdfb1109"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
+ "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
-version = "0.15.4"
+version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec23e6762830658d2b3d385a75aa212af2f67a4586d4442907144f3bb6a1ca8"
+checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.0"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26873667bbbb7c5182d4a37c1add32cdf09f841af72da53318fdb81543c15085"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2cc698a63b549a70bc047073d2949cce27cd1c7b0a4a862d08a8031bc2801db"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a64b1ec5cda2586e284722486d802acf1f7dbdc623e2bfc57e65ca1cd099290"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.17.2"
@@ -171,54 +182,52 @@
  "num-integer",
  "num-traits",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.13.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "074864da206b4973b84eb91683020dbefd6a8c3f0f38e054d93954e891935e4e"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
- "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d76e8e1493bcac0d2766c42737f34458f1c8c50c0d23bcb24ea953affb273216"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "winapi",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
@@ -261,50 +270,50 @@
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.10"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38bc8cc6a5f2e3655e0899c1b848643b2562f853f114bfec7be120678e3ace05"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.10"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8383f39639269cde97d255a32bdb68c047337295414940c68bdd30c2e13203ff"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "rmp"
 version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44519172358fd6d58656c86ab8e7fbc9e1490c3e8f14d35ed78ca0dd07403c9f"
@@ -323,130 +332,224 @@
  "byteorder",
  "rmp",
  "serde",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.5"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71d301d4193d031abdd79ff7e3dd721168a9572ef3fe51a1517aba235bd8f86e"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.71"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "063bf466a64011ac24040a49009724ee60a57da1b437617ceb32e53ad61bfb19"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_numpy"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "itertools",
  "ndarray",
  "num-traits",
  "numpy",
  "pyo3",
  "rmp-serde",
  "serde",
  "serde_json",
+ "zune-jpeg",
+ "zune-png",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
+
+[[package]]
 name = "smallvec"
-version = "1.7.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ecab6c735a6bb4139c0caafd0cc3635748bbb3acf4550e8138122099251f309"
+checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
-version = "0.1.7"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f14ee04d9415b52b3aeab06258a3f07093182b88ba0f9b8d203f211a7a7d41c7"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "zune-core"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29ca36c2e02af0d8d7ee977542bfe33ed1c516be73d3c1faa4420af46e96ceee"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "bitflags 2.3.2",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
+name = "zune-inflate"
+version = "0.2.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
+dependencies = [
+ "simd-adler32",
+]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "zune-jpeg"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "2848e8f4f29dbdcc79910ab3abdff22bb0bacef8556f2a983b5ca950d8b4991e"
+dependencies = [
+ "log",
+ "zune-core",
+]
+
+[[package]]
+name = "zune-png"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee5abc36f78f32bf5ffb5f070a69cb7beffa7cb393817d3a30f9fe7c1ea57655"
+dependencies = [
+ "bytemuck",
+ "log",
+ "zune-core",
+ "zune-inflate",
+]
```

### Comparing `serde_numpy-0.2.1/PKG-INFO` & `serde_numpy-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,106 @@
-Metadata-Version: 2.1
-Name: serde-numpy
-Version: 0.2.1
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Rust
-Classifier: Typing :: Typed
-Requires-Dist: numpy>=1.18
-License-File: LICENSE
-Summary: A library for deserializing various formats directly into numpy arrays
-Author: Will Norcliffe Brown
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/wnorcbrown/serde-numpy
-Project-URL: documentation, https://github.com/wnorcbrown/serde-numpy
-Project-URL: homepage, https://github.com/wnorcbrown/serde-numpy
-
 # serde-numpy
 
-serde-numpy is a library for deserializing various formats directly into numpy arrays
+serde-numpy is a library for efficient deserializing of various file formats directly into numpy arrays. 
+
+See how it works for:
+- [images](img)
+- [json formats](json)
+
+
+## Installation
+Currently only available for linux, python >= 3.7
+
+```bash
+pip install --upgrade pip
+pip install serde-numpy
+```
+
+# [Image formats](img)
+
+## Example usage
+
+```python
+>>> from serde_numpy import decode_jpeg, read_jpeg, decode_png, read_png
+>>> 
+>>> img = read_jpeg("test.jpg")
+>>> img
+array([[[ 75,  29,  82],
+        [ 96,  56, 133],
+        [ 72,  47, 168],
+        [ 63,  56, 179]],
+
+       [[216, 176, 203],
+        [173, 139, 190],
+        [111,  93, 188],
+        [129, 128, 225]],
+
+       [[ 75,  46,  21],
+        [ 73,  51,  48],
+        [ 81,  73, 115],
+        [157, 167, 209]],
+
+       [[165, 142,  99],
+        [181, 165, 144],
+        [169, 169, 188],
+        [185, 203, 222]]], dtype=uint8)
+>>> 
+>>> byte_array = open("test.png", "rb").read()
+>>> img = decode_png(byte_array)
+>>> img
+array([[[ 33,  47, 146],
+        [206,  19, 120],
+        [185,   8,  55],
+        [ 33,  54, 176]],
+
+       [[252, 156, 169],
+        [169, 139, 100],
+        [ 24, 128, 222],
+        [136, 146, 213]],
+
+       [[ 28,  24, 192],
+        [184,  51,  58],
+        [ 39,  61, 252],
+        [237, 165, 113]],
+
+       [[239, 111,  72],
+        [ 30, 242,  38],
+        [165, 161, 223],
+        [ 91, 246, 217]]], dtype=uint8)
+
+```
+
+## Benchmarks
+
+All benchmarks were performed on an AMD Ryzen 9 3950X (Python 3.8.12, numpy 1.23.2, orjson 3.6.4). We compare serde_numpy's `decode_png` and `decode_jpeg` versus pillow's `Image.open` + `np.asarray` (which is the de facto standard for libraries than do a lot of image loading e.g. pytorch's `torchvision`).
+
+### JPEG
+JPEG decoding for square images:
+
+![alt text](profile/jpeg_profile.png "Jpeg profiling")
+
+### PNG
+PNG decoding for square images:
+
+![alt text](profile/png_profile.png "Png profiling")
+
+# [JSON Formats](json)
 
 ## Motivation
 If you've ever done something like this in your code:
 
 ```python
 data = json.load(open("data.json"))
 
 arr = np.array(data["x"])
 ```
 then this library does it faster by using minimal array allocations and less python.
 
 Speed ups are 1.5x - 8x times faster, depending on array sizes (and CPU), when compared to orjson + numpy.
 
-## Installation
-Currently only available for linux, python >= 3.7
-
-```bash
-pip install --upgrade pip
-pip install serde-numpy
-```
 
 ## Usage
 
 
 The user specifies the numpy dtypes within a `structure` corresponding to the data that they want to deserialize.
 
 ### N-dimensional array
@@ -156,8 +206,8 @@
 
 ![alt text](profile/2darr_profile.png "2D Array profiling")
 
 ### Transposed arrays deserialization
 
 For this test we test the speed of deserializing multiple data types which have been serialized in a row-wise fashion and converting it to column-wise arrays during deserializition.
 
-![alt text](profile/transpose_profile.png "Transpose columns profiling")
+![alt text](profile/transpose_profile.png "Transpose columns profiling")
```

