# Comparing `tmp/mfhpo_simulator-1.0.2-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 17667 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      483 b- defN 23-Jun-10 22:24 benchmark_simulator/__init__.py
+Zip file size: 18041 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      483 b- defN 23-Jun-14 20:07 benchmark_simulator/__init__.py
 -rw-rw-r--  2.0 unx     2845 b- defN 23-Jun-10 22:16 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx     9472 b- defN 23-Jun-10 22:21 benchmark_simulator/_secure_proc.py
--rw-rw-r--  2.0 unx     1846 b- defN 23-May-25 06:25 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    28375 b- defN 23-Jun-10 22:13 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      871 b- defN 23-Jun-10 22:25 mfhpo_simulator-1.0.2.dist-info/RECORD
-10 files, 55071 bytes uncompressed, 16167 bytes compressed:  70.6%
+-rw-rw-r--  2.0 unx    10604 b- defN 23-Jun-14 17:27 benchmark_simulator/_secure_proc.py
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
+-rw-rw-r--  2.0 unx    29922 b- defN 23-Jun-14 19:51 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      872 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/RECORD
+10 files, 57677 bytes uncompressed, 16541 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-1.0.2.dist-info/LICENSE
+Filename: mfhpo_simulator-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.0.2.dist-info/METADATA
+Filename: mfhpo_simulator-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.0.2.dist-info/WHEEL
+Filename: mfhpo_simulator-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.0.2.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.0.2.dist-info/RECORD
+Filename: mfhpo_simulator-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import ObjectiveFuncType
 from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import fcntl
 import os
 import time
 import warnings
 
-from _io import TextIOWrapper
-
 from benchmark_simulator._constants import (
     _SharedDataLocations,
     _StateType,
     _TIME_VALUES,
     _TimeStampDictType,
 )
-from benchmark_simulator._utils import secure_edit, secure_read
+from benchmark_simulator._utils import _SecureLock
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
 
 def _init_simulator(dir_name: str) -> None:
@@ -31,197 +29,211 @@
                 f.seek(0)
                 f.truncate()
                 f.write("{}")
 
             fcntl.flock(f.fileno(), fcntl.LOCK_UN)
 
 
-@secure_edit
-def _allocate_proc_to_worker(f: TextIOWrapper, pid: int) -> None:
-    cur_alloc = json.load(f)
-    cur_alloc[pid] = 0
-    f.seek(0)
-    json.dump(cur_alloc, f, indent=4)
+def _allocate_proc_to_worker(path: str, pid: int, lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        cur_alloc = json.load(f)
+        cur_alloc[pid] = 0
+        f.seek(0)
+        json.dump(cur_alloc, f, indent=4)
+
 
+def _complete_proc_allocation(path: str, lock: _SecureLock) -> dict[int, int]:
+    with lock.edit(path) as f:
+        alloc = json.load(f)
+        sorted_pids = np.sort([int(pid) for pid in alloc.keys()])
+        alloc = {pid: idx for idx, pid in enumerate(sorted_pids)}
+        f.seek(0)
+        json.dump(alloc, f, indent=4)
 
-@secure_edit
-def _complete_proc_allocation(f: TextIOWrapper) -> dict[int, int]:
-    alloc = json.load(f)
-    sorted_pids = np.sort([int(pid) for pid in alloc.keys()])
-    alloc = {pid: idx for idx, pid in enumerate(sorted_pids)}
-    f.seek(0)
-    json.dump(alloc, f, indent=4)
     return alloc
 
 
-@secure_edit
-def _record_cumtime(f: TextIOWrapper, worker_id: str, cumtime: float) -> None:
-    record = json.load(f)
-    prev_cumtime = record.get(worker_id, 0.0)
-    record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TIME_VALUES.crashed)
-    f.seek(0)
-    json.dump(record, f, indent=4)
-
-
-@secure_edit
-def _record_timestamp(f: TextIOWrapper, worker_id: str, prev_timestamp: float, waited_time: float) -> None:
-    record = json.load(f)
-    record[worker_id] = dict(prev_timestamp=prev_timestamp, waited_time=waited_time)
-    f.seek(0)
-    json.dump(record, f, indent=4)
-
-
-@secure_edit
-def _cache_state(f: TextIOWrapper, config_hash: int, new_state: _StateType, update_index: int | None = None) -> None:
-    config_hash_str = str(config_hash)
-    cache = json.load(f)
-    _new_state = [new_state.runtime, new_state.cumtime, new_state.fidel, new_state.seed]
-    if config_hash_str not in cache:
-        cache[config_hash_str] = [_new_state]
-    elif update_index is not None:
-        cache[config_hash_str][update_index] = _new_state
-    else:
-        cache[config_hash_str].append(_new_state)
-
-    f.seek(0)
-    json.dump(cache, f, indent=4)
-
-
-@secure_edit
-def _delete_state(f: TextIOWrapper, config_hash: int, index: int) -> None:
-    cache = json.load(f)
-    config_hash_str = str(config_hash)
-    cache[config_hash_str].pop(index)
-    if len(cache[config_hash_str]) == 0:
-        cache.pop(config_hash_str)
-
-    f.seek(0)
-    json.dump(cache, f, indent=4)
-
-
-@secure_read
-def _fetch_cache_states(f: TextIOWrapper, config_hash: int) -> list[_StateType]:
-    states = json.load(f).get(str(config_hash), [])
+def _record_cumtime(path: str, worker_id: str, cumtime: float, lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        record = json.load(f)
+        prev_cumtime = record.get(worker_id, 0.0)
+        record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TIME_VALUES.crashed)
+        f.seek(0)
+        json.dump(record, f, indent=4)
+
+
+def _record_timestamp(path: str, worker_id: str, prev_timestamp: float, waited_time: float, lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        record = json.load(f)
+        record[worker_id] = dict(prev_timestamp=prev_timestamp, waited_time=waited_time)
+        f.seek(0)
+        json.dump(record, f, indent=4)
+
+
+def _cache_state(
+    path: str, config_hash: int, new_state: _StateType, lock: _SecureLock, update_index: int | None = None
+) -> None:
+    with lock.edit(path) as f:
+        config_hash_str = str(config_hash)
+        cache = json.load(f)
+        _new_state = [new_state.runtime, new_state.cumtime, new_state.fidel, new_state.seed]
+        if config_hash_str not in cache:
+            cache[config_hash_str] = [_new_state]
+        elif update_index is not None:
+            cache[config_hash_str][update_index] = _new_state
+        else:
+            cache[config_hash_str].append(_new_state)
+
+        f.seek(0)
+        json.dump(cache, f, indent=4)
+
+
+def _delete_state(path: str, config_hash: int, index: int, lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        cache = json.load(f)
+        config_hash_str = str(config_hash)
+        cache[config_hash_str].pop(index)
+        if len(cache[config_hash_str]) == 0:
+            cache.pop(config_hash_str)
+
+        f.seek(0)
+        json.dump(cache, f, indent=4)
+
+
+def _fetch_cache_states(path: str, config_hash: int, lock: _SecureLock) -> list[_StateType]:
+    with lock.read(path) as f:
+        states = json.load(f).get(str(config_hash), [])
+
     return [_StateType(runtime=state[0], cumtime=state[1], fidel=state[2], seed=state[3]) for state in states]
 
 
-@secure_read
-def _fetch_cumtimes(f: TextIOWrapper) -> dict[str, float]:
-    cumtimes = json.load(f)
+def _fetch_cumtimes(path: str, lock: _SecureLock) -> dict[str, float]:
+    with lock.read(path) as f:
+        cumtimes = json.load(f)
+
     return cumtimes
 
 
-@secure_read
-def _fetch_timestamps(f: TextIOWrapper) -> dict[str, _TimeStampDictType]:
-    timestamps = {th: _TimeStampDictType(**ts_dict) for th, ts_dict in json.load(f).items()}
+def _fetch_timestamps(path: str, lock: _SecureLock) -> dict[str, _TimeStampDictType]:
+    with lock.read(path) as f:
+        timestamps = {th: _TimeStampDictType(**ts_dict) for th, ts_dict in json.load(f).items()}
+
     return timestamps
 
 
-def _fetch_proc_alloc(path: str) -> dict[int, int]:
-    return _complete_proc_allocation(path=path)
+def _fetch_proc_alloc(path: str, lock: _SecureLock) -> dict[int, int]:
+    return _complete_proc_allocation(path=path, lock=lock)
 
 
-@secure_edit
-def _record_result(f: TextIOWrapper, results: dict[str, float], fixed: bool = True) -> None:
-    record = json.load(f)
-    n_observations = len(record.get("cumtime", []))
-    keys = list(set(list(record.keys()) + list(results.keys()))) if not fixed else results.keys()
-    for key in keys:
-        val = results.get(key, None)
-        if n_observations == 0:
-            record[key] = [val]
-        elif key not in record:
-            record[key] = [None] * n_observations + [val]
-        else:
-            record[key].append(val)
+def _record_result(path: str, results: dict[str, float], lock: _SecureLock, fixed: bool = True) -> None:
+    with lock.edit(path) as f:
+        record = json.load(f)
+        n_observations = len(record.get("cumtime", []))
+        keys = list(set(list(record.keys()) + list(results.keys()))) if not fixed else results.keys()
+        for key in keys:
+            val = results.get(key, None)
+            if n_observations == 0:
+                record[key] = [val]
+            elif key not in record:
+                record[key] = [None] * n_observations + [val]
+            else:
+                record[key].append(val)
 
-    f.seek(0)
-    json.dump(record, f, indent=4)
+        f.seek(0)
+        json.dump(record, f, indent=4)
 
 
-@secure_read
-def _is_simulator_terminated(f: TextIOWrapper, max_evals: int) -> bool:
-    return len(json.load(f)["cumtime"]) >= max_evals
+def _is_simulator_terminated(path: str, max_evals: int, lock: _SecureLock) -> bool:
+    with lock.read(path) as f:
+        result = len(json.load(f)["cumtime"]) >= max_evals
 
+    return result
 
-@secure_read
-def _is_simulator_ready(f: TextIOWrapper, n_workers: int) -> bool:
-    return len(json.load(f)) == n_workers
 
+def _is_simulator_ready(path: str, n_workers: int, lock: _SecureLock) -> bool:
+    with lock.read(path) as f:
+        result = len(json.load(f)) == n_workers
 
-@secure_read
-def _is_allocation_ready(f: TextIOWrapper, n_workers: int) -> bool:
-    return len(json.load(f)) == n_workers
+    return result
 
 
-@secure_read
-def _get_worker_id_to_idx(f: TextIOWrapper) -> dict[str, int]:
-    return {worker_id: idx for idx, worker_id in enumerate(json.load(f).keys())}
+def _is_allocation_ready(path: str, n_workers: int, lock: _SecureLock) -> bool:
+    with lock.read(path) as f:
+        result = len(json.load(f)) == n_workers
 
+    return result
 
-def _is_min_cumtime(path: str, worker_id: str) -> bool:
-    cumtimes = _fetch_cumtimes(path=path)
+
+def _get_worker_id_to_idx(path: str, lock: _SecureLock) -> dict[str, int]:
+    with lock.read(path) as f:
+        result = {worker_id: idx for idx, worker_id in enumerate(json.load(f).keys())}
+
+    return result
+
+
+def _is_min_cumtime(path: str, worker_id: str, lock: _SecureLock) -> bool:
+    cumtimes = _fetch_cumtimes(path=path, lock=lock)
     proc_cumtime = cumtimes[worker_id]
     return min(cumtime for cumtime in cumtimes.values()) == proc_cumtime
 
 
-def _start_timestamp(path: str, worker_id: str, prev_timestamp: float) -> None:
-    _record_timestamp(path=path, worker_id=worker_id, prev_timestamp=time.time(), waited_time=0.0)
+def _start_timestamp(path: str, worker_id: str, prev_timestamp: float, lock: _SecureLock) -> None:
+    _record_timestamp(path=path, worker_id=worker_id, prev_timestamp=time.time(), waited_time=0.0, lock=lock)
 
 
-def _start_worker_timer(path: str, worker_id: str) -> None:
-    _record_cumtime(path=path, worker_id=worker_id, cumtime=0.0)
+def _start_worker_timer(path: str, worker_id: str, lock: _SecureLock) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=0.0, lock=lock)
 
 
-def _finish_worker_timer(path: str, worker_id: str) -> None:
-    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.terminated)
+def _finish_worker_timer(path: str, worker_id: str, lock: _SecureLock) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.terminated, lock=lock)
 
 
-def _kill_worker_timer(path: str, worker_id: str) -> None:
-    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.crashed)
+def _kill_worker_timer(path: str, worker_id: str, lock: _SecureLock) -> None:
+    _record_cumtime(path=path, worker_id=worker_id, cumtime=_TIME_VALUES.crashed, lock=lock)
 
 
-def _kill_worker_timer_with_min_cumtime(path: str) -> None:
-    cumtimes = _fetch_cumtimes(path=path)
-    worker_id = min(cumtimes, key=cumtimes.get)
-    _kill_worker_timer(path=path, worker_id=worker_id)
+def _kill_worker_timer_with_min_cumtime(path: str, lock: _SecureLock) -> None:
+    cumtimes = _fetch_cumtimes(path=path, lock=lock)
+    worker_id = min(cumtimes, key=cumtimes.get)  # type: ignore[arg-type]
+    _kill_worker_timer(path=path, worker_id=worker_id, lock=lock)
 
 
 def _get_timeout_message(cause: str, path: str) -> str:
     dir_name = os.path.join(*path.split("/")[:-1])
     msg = f"Timeout in {cause}. There could be two possible reasons:\n"
     msg += f"(1) The path {dir_name} already existed before the execution of the program.\n"
     msg += "(2) n_workers specified in your optimizer and that in the simulator might be different."
     return msg
 
 
 def _wait_proc_allocation(
-    path: str, n_workers: int, waiting_time: float = 1e-2, time_limit: float = 10.0
+    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-2, time_limit: float = 10.0
 ) -> dict[int, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
-    while not _is_allocation_ready(path, n_workers=n_workers):
+    while not _is_allocation_ready(path, n_workers=n_workers, lock=lock):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="the allocation of procs", path=path))
 
-    return _complete_proc_allocation(path)
+    return _complete_proc_allocation(path, lock=lock)
 
 
 def _wait_all_workers(
-    path: str, n_workers: int, waiting_time: float = 1e-2, time_limit: float = 10.0
+    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-2, time_limit: float = 10.0
 ) -> dict[str, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
-    while not _is_simulator_ready(path, n_workers=n_workers):
+    while not _is_simulator_ready(path, n_workers=n_workers, lock=lock):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="creating a simulator", path=path))
 
-    return _get_worker_id_to_idx(path)
+    return _get_worker_id_to_idx(path, lock=lock)
 
 
 def _raise_unexpected_timeout_error(max_waiting_time: float) -> None:
     raise TimeoutError(
         f"The simulation was terminated due to too long waiting time (> {max_waiting_time} seconds). \n"
         "You can avoid this error by setting `max_waiting_time=np.inf`,\nbut this is not recommended because "
         "n_workers may not be consistent throughout the simulation without setting max_waiting_time.\n"
@@ -234,37 +246,40 @@
         "\t1. Your OS and its version,\n"
         "\t2. Python version,\n"
         "\t3. Your optimizer package name and its internal distributed computation module, and\n"
         "\t4. Your benchmark details.\n"
     )
 
 
-def _terminate_with_unexpected_timeout(path: str, worker_id: str, max_waiting_time: float) -> None:
-    _kill_worker_timer(path=path, worker_id=worker_id)
+def _terminate_with_unexpected_timeout(path: str, worker_id: str, max_waiting_time: float, lock: _SecureLock) -> None:
+    _kill_worker_timer(path=path, worker_id=worker_id, lock=lock)
     # The worker with minimum cumlative time may be able to evaluate several HPs during the wait,
     # but it does not matter because the timeout happens due to too long wait.
     time.sleep(1.0)
-    _kill_worker_timer_with_min_cumtime(path=path)
+    _kill_worker_timer_with_min_cumtime(path=path, lock=lock)
     _raise_unexpected_timeout_error(max_waiting_time=max_waiting_time)
 
 
 def _wait_until_next(
     path: str,
     worker_id: str,
-    waiting_time: float = 1e-4,
+    lock: _SecureLock,
+    waiting_time: float,
     warning_interval: int = 10,
     max_waiting_time: float = np.inf,
 ) -> None:
     start = time.time()
     waiting_time *= 1 + np.random.random()
-    while not _is_min_cumtime(path, worker_id=worker_id):
+    while not _is_min_cumtime(path, worker_id=worker_id, lock=lock):
         time.sleep(waiting_time)
         curtime = time.time()
         if int(curtime - start + 1) % warning_interval == 0:
             warnings.warn(
                 "Workers might be hanging. Please consider setting `max_waiting_time` (< np.inf).\n"
                 "Note that if samplers or the objective function need long time (> 10 seconds), "
                 "please ignore this warning."
             )
 
         if curtime - start > max_waiting_time:
-            _terminate_with_unexpected_timeout(path=path, worker_id=worker_id, max_waiting_time=max_waiting_time)
+            _terminate_with_unexpected_timeout(
+                path=path, worker_id=worker_id, max_waiting_time=max_waiting_time, lock=lock
+            )
```

## benchmark_simulator/_utils.py

```diff
@@ -1,57 +1,55 @@
 import fcntl
 import hashlib
 import time
-from typing import Any, Callable
+from contextlib import contextmanager
+from dataclasses import dataclass
+from typing import Iterator, TextIO
 
 import numpy as np
 
 
 def _generate_time_hash() -> str:
     hash = hashlib.sha1()
     hash.update(str(time.time()).encode("utf-8"))
     return hash.hexdigest()
 
 
-def secure_read(func: Callable) -> Callable:
-    def _inner(path: str, waiting_time: float = 1e-4, time_limit: float = 10.0, **kwargs: Any) -> Any:
+@dataclass(frozen=True)
+class _SecureLock:
+    waiting_time: float = 1e-4
+    time_limit: float = 10.0
+
+    @contextmanager
+    def read(self, path: str) -> Iterator[TextIO]:
         start = time.time()
-        waiting_time *= 1 + np.random.random()
-        fetched, output = False, None
+        waiting_time = self.waiting_time * (1 + np.random.random())
+        fetched = False
         while not fetched:
             with open(path, "r") as f:
                 try:
                     fcntl.flock(f, fcntl.LOCK_SH | fcntl.LOCK_NB)
-                    output = func(f, **kwargs)
+                    yield f
                     fetched = True
                 except IOError:
                     time.sleep(waiting_time)
-                    if time.time() - start >= time_limit:
+                    if time.time() - start >= self.time_limit:
                         raise TimeoutError("Timeout during secure read. Try again.")
 
-        return output
-
-    return _inner
-
-
-def secure_edit(func: Callable) -> Callable:
-    def _inner(path: str, waiting_time: float = 1e-4, time_limit: float = 10.0, **kwargs: Any) -> Any:
+    @contextmanager
+    def edit(self, path: str) -> Iterator[TextIO]:
         start = time.time()
-        waiting_time *= 1 + np.random.random()
-        fetched, output = False, None
+        waiting_time = self.waiting_time * (1 + np.random.random())
+        fetched = False
         while not fetched:
             with open(path, "r+") as f:
                 try:
                     fcntl.flock(f, fcntl.LOCK_EX)
-                    output = func(f, **kwargs)
+                    yield f
                     f.truncate()
                     fetched = True
                 except IOError:
                     time.sleep(waiting_time)
-                    if time.time() - start >= time_limit:
+                    if time.time() - start >= self.time_limit:
                         raise TimeoutError("Timeout during secure edit. Try again.")
                 finally:
                     fcntl.flock(f, fcntl.LOCK_UN)
-
-        return output
-
-    return _inner
```

## benchmark_simulator/simulator.py

```diff
@@ -102,15 +102,15 @@
     _record_timestamp,
     _start_timestamp,
     _start_worker_timer,
     _wait_all_workers,
     _wait_proc_allocation,
     _wait_until_next,
 )
-from benchmark_simulator._utils import _generate_time_hash
+from benchmark_simulator._utils import _SecureLock, _generate_time_hash
 
 import numpy as np
 
 
 @dataclass(frozen=True)
 class _WrapperVars:
     subdir_name: str
@@ -120,14 +120,15 @@
     n_evals: int
     obj_keys: list[str]
     runtime_key: str
     fidel_keys: list[str] | None
     seed: int | None
     continual_max_fidel: int | None
     max_waiting_time: float
+    check_interval_time: float
     store_config: bool
 
 
 @dataclass(frozen=True)
 class _WorkerVars:
     continual_eval: bool
     worker_id: str
@@ -156,19 +157,20 @@
         self,
         subdir_name: str,
         n_workers: int,
         obj_func: ObjectiveFuncType,
         n_actual_evals_in_opt: int,
         n_evals: int,
         fidel_keys: list[str] | None = None,
-        obj_keys: list[str] = ["loss"][:],
+        obj_keys: list[str] | None = None,
         runtime_key: str = "runtime",
         seed: int | None = None,
         continual_max_fidel: int | None = None,
         max_waiting_time: float = np.inf,
+        check_interval_time: float = 1e-4,
         store_config: bool = False,
     ):
         """The initialization of a wrapper class.
 
         Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
 
         Args:
@@ -195,29 +197,36 @@
             n_evals (int):
                 How many configurations we would like to collect.
                 More specifically, how many times we call the objective function during the optimization.
                 We can guarantee that `results.json` has at least this number of evaluations.
             fidel_keys (list[str] | None):
                 The fidelity names to be used in the objective function.
                 If None, we assume that no fidelity is used.
-            obj_keys (list[str]):
+            obj_keys (list[str] | None):
                 The keys of the objective metrics used in `results` returned by func.
             runtime_key (str):
                 The key of the runtime metric used in `results` returned by func.
             seed (int | None):
                 The random seed to be used to allocate random seed to each call.
             continual_max_fidel (int | None):
                 The maximum fidelity to used in continual evaluations.
                 This is valid only if we use a single fidelity.
                 If not None, each call is a continuation from the call with the same eval_config and lower fidel.
                 For example, when we already trained the objective with configA and training_epoch=10,
                 we probably would like to continue the training from epoch 10 rather than from scratch
                 for call with configA and training_epoch=30.
                 continual_eval=True calculates the runtime considers this.
                 If False, each call is considered to be processed from scratch.
+            check_interval_time (float):
+                How often each worker should check whether they could be assigned a new job.
+                For example, if 1e-2 is specified, each worker check whether they can get a new job every 1e-2 seconds.
+                If there are many workers, too small check_interval_time may cause a big bottleneck.
+                On the other hand, a big check_interval_time spends more time for waiting.
+                By default, check_interval_time is set to a relatively small number, so users might rather want to
+                increase the number to avoid the bottleneck for many workers.
             max_waiting_time (float):
                 The maximum waiting time to judge hang.
                 If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
             store_config (bool):
                 Whether to store all config/fidel information.
                 The information is sorted chronologically.
                 When you do large-scale experiments, this may incur too much storage consumption.
@@ -225,24 +234,26 @@
         self._wrapper_vars = _WrapperVars(
             subdir_name=subdir_name,
             n_workers=n_workers,
             obj_func=obj_func,
             n_actual_evals_in_opt=n_actual_evals_in_opt,
             n_evals=n_evals,
             fidel_keys=fidel_keys,
-            obj_keys=obj_keys,
+            obj_keys=obj_keys if obj_keys is not None else ["loss"],
             runtime_key=runtime_key,
             seed=seed,
             continual_max_fidel=continual_max_fidel,
             max_waiting_time=max_waiting_time,
+            check_interval_time=check_interval_time,
             store_config=store_config,
         )
+        self._lock = _SecureLock()
         self._dir_name = os.path.join(DIR_NAME, subdir_name)
         self._paths = _get_file_paths(self.dir_name)
-        self._obj_keys, self._runtime_key = obj_keys[:], runtime_key
+        self._obj_keys, self._runtime_key = self._wrapper_vars.obj_keys, runtime_key
         self._fidel_keys = [] if fidel_keys is None else fidel_keys[:]
         self._init_wrapper()
 
     @property
     def dir_name(self) -> str:
         return self._dir_name
 
@@ -291,18 +302,20 @@
             raise ValueError(
                 f"continual_max_fidel is valid only if fidel_keys has only one element, but got {self._fidel_keys}"
             )
 
     def _init_worker(self, worker_id: str) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         _init_simulator(dir_name=self.dir_name)
-        _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id)
+        _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id, lock=self._lock)
 
     def _alloc_index(self, worker_id: str) -> int:
-        worker_id_to_index = _wait_all_workers(path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers)
+        worker_id_to_index = _wait_all_workers(
+            path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers, lock=self._lock
+        )
         time.sleep(1e-2)  # buffer before the optimization
         return worker_id_to_index[worker_id]
 
     def _init_wrapper(self) -> None:
         continual_eval = self._wrapper_vars.continual_max_fidel is not None
         worker_id = _generate_time_hash()
         self._guarantee_no_hang()
@@ -360,15 +373,15 @@
             raise ValueError(f"Fidelity for continual evaluation must be integer, but got {fidel}")
         if fidel < 0:
             raise ValueError(f"Fidelity for continual evaluation must be non-negative, but got {fidel}")
 
         return fidel
 
     def _get_cached_state_and_index(self, config_hash: int, fidel: int) -> tuple[_StateType, int | None]:
-        cached_states = _fetch_cache_states(self._paths.state_cache, config_hash=config_hash)
+        cached_states = _fetch_cache_states(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
         intermediate_avail = [state.cumtime <= self._cumtime and state.fidel < fidel for state in cached_states]
         cached_state_index = intermediate_avail.index(True) if any(intermediate_avail) else None
         if cached_state_index is None:
             # initial seed, note: 1 << 30 is a huge number that fits 32bit.
             init_state = _StateType(seed=self._worker_vars.rng.randint(1 << 30))
             return init_state, None
         else:
@@ -378,35 +391,42 @@
         self,
         config_hash: int,
         fidel: int,
         total_runtime: float,
         seed: int | None,
         cached_state_index: int | None,
     ) -> None:
-        kwargs = dict(path=self._paths.state_cache, config_hash=config_hash)
+        kwargs = dict(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
         if fidel != self._wrapper_vars.continual_max_fidel:  # update the cache data
             new_state = _StateType(runtime=total_runtime, cumtime=self._cumtime, fidel=fidel, seed=seed)
-            _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)
+            _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)  # type: ignore[arg-type]
         elif cached_state_index is not None:  # if None, newly start and train till the end, so no need to delete.
-            _delete_state(index=cached_state_index, **kwargs)
+            _delete_state(index=cached_state_index, **kwargs)  # type: ignore[arg-type]
 
     def _wait_other_workers(self) -> None:
         """
         Wait until the worker's cumulative runtime becomes the smallest.
         The smallest cumulative runtime implies that the order in the record will not disturbed
         even if the worker reports its results now.
         """
         wait_start, worker_id = time.time(), self._worker_vars.worker_id
         max_waiting_time = self._wrapper_vars.max_waiting_time
-        _wait_until_next(path=self._paths.worker_cumtime, worker_id=worker_id, max_waiting_time=max_waiting_time)
+        _wait_until_next(
+            path=self._paths.worker_cumtime,
+            worker_id=worker_id,
+            max_waiting_time=max_waiting_time,
+            waiting_time=self._wrapper_vars.check_interval_time,
+            lock=self._lock,
+        )
         _record_timestamp(
             path=self._paths.timestamp,
             worker_id=worker_id,
             prev_timestamp=time.time(),
             waited_time=time.time() - wait_start,
+            lock=self._lock,
         )
 
     def _query_obj_func(
         self,
         eval_config: dict[str, Any],
         fidels: dict[str, int | float] | None,
         seed: int | None,
@@ -461,41 +481,52 @@
 
         # Otherwise, we try the continual evaluation
         fidel = self._validate_provided_fidels(fidels)
         return self._proc_output_from_existing_state(eval_config=eval_config, fidel=fidel, **data_to_scatter)
 
     def _post_proc(self, results: dict[str, float]) -> None:
         # First, record the simulated cumulative runtime after calling the objective
-        _record_cumtime(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id, cumtime=self._cumtime)
+        _record_cumtime(
+            path=self._paths.worker_cumtime,
+            worker_id=self._worker_vars.worker_id,
+            cumtime=self._cumtime,
+            lock=self._lock,
+        )
         # Wait till the cumulative runtime becomes the smallest
         self._wait_other_workers()
 
         row = dict(
             cumtime=self._cumtime,
             worker_index=self._worker_vars.worker_index,
             **{k: results[k] for k in self._obj_keys},
             **self._used_config,
         )
         # Record the results to the main database when the cumulative runtime is the smallest
-        _record_result(self._paths.result, results=row, fixed=bool(not self._wrapper_vars.store_config))
+        _record_result(
+            self._paths.result, results=row, fixed=bool(not self._wrapper_vars.store_config), lock=self._lock
+        )
         self._used_config = {}  # Make it empty
-        if _is_simulator_terminated(self._paths.result, max_evals=self._wrapper_vars.n_evals):
+        if _is_simulator_terminated(self._paths.result, max_evals=self._wrapper_vars.n_evals, lock=self._lock):
             self._finish()
 
     def _load_timestamps(self) -> _TimeStampDictType:
-        timestamp_dict, worker_id = _fetch_timestamps(self._paths.timestamp), self._worker_vars.worker_id
+        timestamp_dict = _fetch_timestamps(self._paths.timestamp, lock=self._lock)
+        worker_id = self._worker_vars.worker_id
         if worker_id not in timestamp_dict:  # Initialize the timestamp
             init_timestamp = _TimeStampDictType(prev_timestamp=time.time(), waited_time=0.0)
             _start_timestamp(
-                path=self._paths.timestamp, worker_id=worker_id, prev_timestamp=init_timestamp.prev_timestamp
+                path=self._paths.timestamp,
+                worker_id=worker_id,
+                prev_timestamp=init_timestamp.prev_timestamp,
+                lock=self._lock,
             )
             return init_timestamp
 
         timestamp = timestamp_dict[worker_id]
-        self._cumtime = _fetch_cumtimes(self._paths.worker_cumtime)[worker_id]
+        self._cumtime = _fetch_cumtimes(self._paths.worker_cumtime, lock=self._lock)[worker_id]
         self._terminated = self._cumtime >= _TIME_VALUES.terminated - 1e-5
         self._crashed = self._cumtime >= _TIME_VALUES.crashed - 1e-5
         return timestamp
 
     def __call__(
         self,
         eval_config: dict[str, Any],
@@ -541,15 +572,15 @@
         return results
 
     def _finish(self) -> None:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang.
         """
-        _finish_worker_timer(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id)
+        _finish_worker_timer(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id, lock=self._lock)
         self._terminated = True
 
 
 class CentralWorkerManager(_BaseWrapperInterface):
     """A central worker manager class.
     This class is supposed to be instantiated if the optimizer module uses multiprocessing.
     For example, Dask, multiprocessing, and joblib would need this class.
@@ -574,19 +605,21 @@
 
         pool.close()
         pool.join()
         self._workers = [result.get() for result in results]
 
     def _init_alloc(self, pid: int) -> None:
         path = self._paths.proc_alloc
-        if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers):
-            _allocate_proc_to_worker(path=path, pid=pid)
-            self._pid_to_index = _wait_proc_allocation(path=path, n_workers=self._wrapper_vars.n_workers)
+        if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock):
+            _allocate_proc_to_worker(path=path, pid=pid, lock=self._lock)
+            self._pid_to_index = _wait_proc_allocation(
+                path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock
+            )
         else:
-            self._pid_to_index = _fetch_proc_alloc(path=path)
+            self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         **data_to_scatter: Any,
```

## Comparing `mfhpo_simulator-1.0.2.dist-info/LICENSE` & `mfhpo_simulator-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.0.2.dist-info/RECORD` & `mfhpo_simulator-1.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-benchmark_simulator/__init__.py,sha256=H_YjPoh2Z7pvTclJebrHXih2nWujZT6HKoh-TTH-fzg,483
+benchmark_simulator/__init__.py,sha256=TxeWE17qgGghk7_PtnFtAmqRUnX0qTwN5VDMKAh6k2Y,483
 benchmark_simulator/_constants.py,sha256=l68ir_HRUoVkKvEYqBXb1nf0LjUSlZvDb-Hft6Q0aio,2845
-benchmark_simulator/_secure_proc.py,sha256=bdCroF9mVq1u_cy2AvYe2KFignG7V-frA3hXP9I3O-M,9472
-benchmark_simulator/_utils.py,sha256=SBu3r9mAYgwgB2CLo4YVxGcSthUZOO8quyX7cGbikks,1846
-benchmark_simulator/simulator.py,sha256=v_h_LPI0n1qali7WJB-tAdPhQEdfA37VwulxusK8k7I,28375
-mfhpo_simulator-1.0.2.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.0.2.dist-info/METADATA,sha256=rElJ-Bc85bfSi9Gi__j71FI5TdLfrJbzT4PCTSiZh1U,307
-mfhpo_simulator-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-1.0.2.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
-mfhpo_simulator-1.0.2.dist-info/RECORD,,
+benchmark_simulator/_secure_proc.py,sha256=lr8Uxudvmw3Ed7jR5_lpHxcA-9y-ztgtjX0WTECMYYM,10604
+benchmark_simulator/_utils.py,sha256=s2kwhhHIJbrT0VbNglmq-rlm0oE8OrqUBvDpCLEAsXk,1772
+benchmark_simulator/simulator.py,sha256=TXiCJ4OatZze_vUqr8bKlV7mNrI17JL1J4NyXUXe81M,29922
+mfhpo_simulator-1.1.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.1.0.dist-info/METADATA,sha256=kB4vYlefEEKMWTn9wOKrAp8N7Py3tVCefsJpZTPxjKc,307
+mfhpo_simulator-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_simulator-1.1.0.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
+mfhpo_simulator-1.1.0.dist-info/RECORD,,
```

