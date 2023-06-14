# Comparing `tmp/mfhpo_simulator-1.0.1-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17634 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      483 b- defN 23-Jun-07 06:50 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     2797 b- defN 23-May-28 09:29 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx     9482 b- defN 23-May-27 16:40 benchmark_simulator/_secure_proc.py
+Zip file size: 17667 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      483 b- defN 23-Jun-10 22:24 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     2845 b- defN 23-Jun-10 22:16 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx     9472 b- defN 23-Jun-10 22:21 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1846 b- defN 23-May-25 06:25 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    28381 b- defN 23-May-28 09:34 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      871 b- defN 23-Jun-07 06:50 mfhpo_simulator-1.0.1.dist-info/RECORD
-10 files, 55039 bytes uncompressed, 16134 bytes compressed:  70.7%
+-rw-rw-r--  2.0 unx    28375 b- defN 23-Jun-10 22:13 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      871 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/RECORD
+10 files, 55071 bytes uncompressed, 16167 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-1.0.1.dist-info/LICENSE
+Filename: mfhpo_simulator-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.0.1.dist-info/METADATA
+Filename: mfhpo_simulator-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.0.1.dist-info/WHEEL
+Filename: mfhpo_simulator-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.0.1.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.0.1.dist-info/RECORD
+Filename: mfhpo_simulator-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import ObjectiveFuncType
 from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -37,19 +37,23 @@
     proc_alloc: str = "proc_alloc.json"
     result: str = "results.json"
     state_cache: str = "state_cache.json"
     worker_cumtime: str = "simulated_cumtime.json"
     timestamp: str = "timestamp.json"
 
 
-class _TimeValue(Enum):
+@dataclass(frozen=True)
+class _TimeValue:
     terminated: float = float(1 << 40)
     crashed: float = float(1 << 41)
 
 
+_TIME_VALUES = _TimeValue()
+
+
 class ObjectiveFuncType(Protocol):
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         seed: int | None = None,
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -6,16 +6,16 @@
 import warnings
 
 from _io import TextIOWrapper
 
 from benchmark_simulator._constants import (
     _SharedDataLocations,
     _StateType,
+    _TIME_VALUES,
     _TimeStampDictType,
-    _TimeValue,
 )
 from benchmark_simulator._utils import secure_edit, secure_read
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
@@ -53,15 +53,15 @@
     return alloc
 
 
 @secure_edit
 def _record_cumtime(f: TextIOWrapper, worker_id: str, cumtime: float) -> None:
     record = json.load(f)
     prev_cumtime = record.get(worker_id, 0.0)
-    record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TimeValue.crashed.value)
+    record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TIME_VALUES.crashed)
     f.seek(0)
     json.dump(record, f, indent=4)
 
 
 @secure_edit
 def _record_timestamp(f: TextIOWrapper, worker_id: str, prev_timestamp: float, waited_time: float) -> None:
     record = json.load(f)
@@ -169,19 +169,19 @@
 
 
 def _start_worker_timer(path: str, worker_id: str) -> None:
     _record_cumtime(path=path, worker_id=worker_id, cumtime=0.0)
 
 
 def _finish_worker_timer(path: str, worker_id: str) -> None:
-    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TimeValue.terminated.value)
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.terminated)
 
 
 def _kill_worker_timer(path: str, worker_id: str) -> None:
-    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TimeValue.crashed.value)
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.crashed)
 
 
 def _kill_worker_timer_with_min_cumtime(path: str) -> None:
     cumtimes = _fetch_cumtimes(path=path)
     worker_id = min(cumtimes, key=cumtimes.get)
     _kill_worker_timer(path=path, worker_id=worker_id)
```

## benchmark_simulator/simulator.py

```diff
@@ -77,16 +77,16 @@
 from typing import Any
 
 from benchmark_simulator._constants import (
     DIR_NAME,
     INF,
     ObjectiveFuncType,
     _StateType,
+    _TIME_VALUES,
     _TimeStampDictType,
-    _TimeValue,
     _get_file_paths,
 )
 from benchmark_simulator._secure_proc import (
     _allocate_proc_to_worker,
     _cache_state,
     _delete_state,
     _fetch_cache_states,
@@ -488,16 +488,16 @@
             _start_timestamp(
                 path=self._paths.timestamp, worker_id=worker_id, prev_timestamp=init_timestamp.prev_timestamp
             )
             return init_timestamp
 
         timestamp = timestamp_dict[worker_id]
         self._cumtime = _fetch_cumtimes(self._paths.worker_cumtime)[worker_id]
-        self._terminated = self._cumtime >= _TimeValue.terminated.value - 1e-5
-        self._crashed = self._cumtime >= _TimeValue.crashed.value - 1e-5
+        self._terminated = self._cumtime >= _TIME_VALUES.terminated - 1e-5
+        self._crashed = self._cumtime >= _TIME_VALUES.crashed - 1e-5
         return timestamp
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
```

## Comparing `mfhpo_simulator-1.0.1.dist-info/LICENSE` & `mfhpo_simulator-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

