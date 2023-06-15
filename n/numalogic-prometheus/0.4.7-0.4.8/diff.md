# Comparing `tmp/numalogic_prometheus-0.4.7.tar.gz` & `tmp/numalogic_prometheus-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.4.7.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.8.tar", max compression
```

## Comparing `numalogic_prometheus-0.4.7.tar` & `numalogic_prometheus-0.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/LICENSE
--rw-r--r--   0        0        0     1894 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/__init__.py
--rw-r--r--   0        0        0     1400 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3866 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1291 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2519 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4496 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/factory.py
--rw-r--r--   0        0        0     7169 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      720 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4687 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/inference.py
--rw-r--r--   0        0        0     7309 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     3443 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     4917 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4217 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     7399 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udsink/train.py
--rw-r--r--   0        0        0     8543 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     6016 2023-06-15 16:51:53.998039 numalogic_prometheus-0.4.7/numaprom/watcher.py
--rw-r--r--   0        0        0     1537 2023-06-15 16:51:54.002040 numalogic_prometheus-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1894 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/__init__.py
+-rw-r--r--   0        0        0     1400 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3832 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1260 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2488 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4503 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/entities.py
+-rw-r--r--   0        0        0      950 2023-06-15 18:21:24.050009 numalogic_prometheus-0.4.8/numaprom/factory.py
+-rw-r--r--   0        0        0     7169 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4702 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     7339 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     3473 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4932 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4184 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     7399 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8541 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5979 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/numaprom/watcher.py
+-rw-r--r--   0        0        0     1661 2023-06-15 18:21:24.054010 numalogic_prometheus-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.8/PKG-INFO
```

### Comparing `numalogic_prometheus-0.4.7/LICENSE` & `numalogic_prometheus-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/__init__.py` & `numalogic_prometheus-0.4.8/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/_config.py` & `numalogic_prometheus-0.4.8/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/_constants.py` & `numalogic_prometheus-0.4.8/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.8/numaprom/clients/prometheus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import numpy as np
 import pandas as pd
-from typing import Optional
 
 from numaprom import LOGGER
 
 
 class Prometheus:
     def __init__(self, prometheus_server: str):
         self.PROMETHEUS_SERVER = prometheus_server
@@ -52,15 +51,15 @@
         if frames:
             df = pd.concat(frames, ignore_index=True)
             df.sort_values(by=["timestamp"], inplace=True)
             df["timestamp"] = pd.to_datetime(df["timestamp"], unit="s")
             df.reset_index(drop=True, inplace=True)
         return df
 
-    def query_range(self, query: str, start: float, end: float, step: int = 30) -> Optional[list]:
+    def query_range(self, query: str, start: float, end: float, step: int = 30) -> list | None:
         results = []
         data_points = (end - start) / step
         temp_start = start
         while data_points > 11000:
             temp_end = temp_start + 11000 * step
             response = self.query_range_limit(query, temp_start, temp_end, step)
             for res in response:
@@ -91,15 +90,15 @@
                 "Prometheus query has returned results for {results} metric series.",
                 results=len(results),
             )
         except Exception as ex:
             LOGGER.exception("Prometheus error: {err}", err=ex)
         return results
 
-    def query(self, query: str) -> Optional[dict]:
+    def query(self, query: str) -> dict | None:
         results = []
         try:
             response = requests.get(
                 self.PROMETHEUS_SERVER + "/api/v1/query", params={"query": query}
             )
             if response:
                 results = response.json()["data"]["result"]
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.8/numaprom/clients/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
-from typing import Optional
 
 from redis.cluster import RedisCluster
 from redis.backoff import ExponentialBackoff
 from redis.exceptions import RedisClusterException, RedisError
 from redis.retry import Retry
 
 from numaprom import LOGGER
 from numaprom.tools import is_host_reachable
 
 
-redis_client: Optional[RedisCluster] = None
+redis_client: RedisCluster | None = None
 
 
 def get_redis_client(
     host: str, port: str, password: str = None, decode_responses: bool = True, recreate=False
 ) -> RedisCluster:
     global redis_client
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.8/numaprom/clients/sentinel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
-from typing import Optional
 
 from numalogic.tools.types import redis_client_t
 from redis.backoff import ExponentialBackoff
 from redis.exceptions import RedisClusterException, RedisError
 from redis.retry import Retry
 from redis.sentinel import Sentinel, MasterNotFoundError
 
 from numaprom import LOGGER
 from numaprom._config import RedisConf
 from numaprom.watcher import ConfigManager
 
 
-SENTINEL_MASTER_CLIENT: Optional[redis_client_t] = None
+SENTINEL_MASTER_CLIENT: redis_client_t | None = None
 
 
 def get_redis_client(
     host: str,
     port: int,
     password: str,
     mastername: str,
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.8/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.8/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/entities.py` & `numalogic_prometheus-0.4.8/numaprom/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from copy import copy
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Optional, Any, Union, TypeVar
+from typing import Any, TypeVar
 from collections import OrderedDict
 
 import numpy as np
 import numpy.typing as npt
 import orjson
 from typing_extensions import Self
 
 Vector = list[float]
-Matrix = Union[Vector, list[Vector], npt.NDArray[float]]
+Matrix = Vector | list[Vector] | npt.NDArray[float]
 
 
 class Status(str, Enum):
     RAW = "raw"
     EXTRACTED = "extracted"
     PRE_PROCESSED = "pre_processed"
     INFERRED = "inferred"
@@ -28,29 +28,29 @@
 class Header(str, Enum):
     STATIC_INFERENCE = "static_threshold"
     MODEL_INFERENCE = "model_inference"
     TRAIN_REQUEST = "request_training"
     MODEL_STALE = "model_stale"
 
 
-@dataclass
+@dataclass(slots=True)
 class _BasePayload:
     uuid: str
     composite_keys: OrderedDict[str, str]
 
 
 PayloadType = TypeVar("PayloadType", bound=_BasePayload)
 
 
-@dataclass
+@dataclass(slots=True)
 class TrainerPayload(_BasePayload):
     header: Header = Header.TRAIN_REQUEST
 
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class StreamPayload(_BasePayload):
     win_raw_arr: Matrix
     win_arr: Matrix
     win_ts_arr: list[str]
     status: Status = Status.RAW
     metadata: dict[str, Any] = field(default_factory=dict)
     header: Header = Header.MODEL_INFERENCE
@@ -61,16 +61,16 @@
 
     @property
     def end_ts(self) -> str:
         return self.win_ts_arr[-1]
 
     def get_stream_array(self, original=False) -> npt.NDArray[float]:
         if original:
-            return np.asarray(self.win_raw_arr)
-        return np.asarray(self.win_arr)
+            return np.array(self.win_raw_arr)
+        return np.array(self.win_arr)
 
     def get_metadata(self, key: str) -> dict[str, Any]:
         return copy(self.metadata[key])
 
     def set_win_arr(self, arr: Matrix) -> None:
         self.win_arr = arr
 
@@ -102,29 +102,29 @@
         Header.MODEL_INFERENCE: StreamPayload,
         Header.TRAIN_REQUEST: TrainerPayload,
         Header.STATIC_INFERENCE: StreamPayload,
         Header.MODEL_STALE: StreamPayload,
     }
 
     @classmethod
-    def from_json(cls, json_data: Union[bytes, str]) -> PayloadType:
+    def from_json(cls, json_data: bytes | str) -> PayloadType:
         data = orjson.loads(json_data)
         header = data.get("header")
         if not header:
             raise RuntimeError(f"Header not present in json: {json_data}")
         payload_cls = cls.__HEADER_MAP[header]
         return payload_cls(**data)
 
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class PrometheusPayload:
     timestamp_ms: int
     name: str
     namespace: str
-    subsystem: Optional[str]
+    subsystem: str | None
     type: str
     value: float
     labels: dict[str, str]
 
     def as_json(self) -> bytes:
         return orjson.dumps(
             {
@@ -135,15 +135,15 @@
                 "Type": self.type,
                 "Value": self.value,
                 "Labels": self.labels,
             }
         )
 
     @classmethod
-    def from_json(cls, json_obj: Union[bytes, str]) -> Self:
+    def from_json(cls, json_obj: bytes | str) -> Self:
         obj = orjson.loads(json_obj)
         return cls(
             timestamp_ms=obj["TimestampMs"],
             name=obj["Name"],
             namespace=obj["Namespace"],
             subsystem=obj["Subsystem"],
             type=obj["Type"],
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/factory.py` & `numalogic_prometheus-0.4.8/numaprom/factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Callable, Union
+from collections.abc import Callable
 
 from pynumaflow.function import Messages
 from pynumaflow.sink import Responses
 
 from numaprom.udf import preprocess, postprocess, window, metric_filter, inference, threshold
 from numaprom.udsink import train, train_rollout
 
 
 class HandlerFactory:
     @classmethod
-    def get_handler(cls, step: str) -> Callable[..., Union[Messages, Responses]]:
+    def get_handler(cls, step: str) -> Callable[..., Messages | Responses]:
         if step == "metric_filter":
             return metric_filter
 
         if step == "window":
             return window
 
         if step == "preprocess":
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/tools.py` & `numalogic_prometheus-0.4.8/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.8/numaprom/udf/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import json
-from typing import Optional
 
 from pynumaflow.function import Messages, Datum
 
 from numaprom import LOGGER
 from numaprom.tools import catch_exception, msg_forward
 
 
 @catch_exception
 @msg_forward
-def metric_filter(_: list[str], datum: Datum) -> Optional[Messages]:
+def metric_filter(_: list[str], datum: Datum) -> Messages | None:
     """UDF to filter metrics by labels."""
     LOGGER.debug("Received Msg: {value} ", value=datum.value)
 
     msg = datum.value.decode("utf-8")
     data = json.loads(msg)
 
     label = os.getenv("LABEL")
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.8/numaprom/udf/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     if not artifact_data:
         LOGGER.info(
-            "{uuid} - Inference artifact not found, forwarding for static thresholding. Keys: {keys}",
+            "{uuid} - Inference artifact not found, "
+            "forwarding for static thresholding. Keys: {keys}",
             uuid=payload.uuid,
             keys=payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.ARTIFACT_NOT_FOUND)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.8/numaprom/udf/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 
     LOGGER.debug("{uuid} - Received all metrics, generating unified anomaly", uuid=payload.uuid)
     unified_weights = unified_config.unified_weights
     if unified_weights:
         weighted_anomalies = np.multiply(anomalies, unified_weights)
         unified_anomaly = float(np.sum(weighted_anomalies) / np.sum(unified_weights))
         LOGGER.info(
-            "{uuid} - Generating unified anomaly, using unified weights. Unified Anomaly: {anomaly}",
+            "{uuid} - Generating unified anomaly, using unified weights. "
+            "Unified Anomaly: {anomaly}",
             uuid=payload.uuid,
             anomaly=unified_anomaly,
         )
     else:
         unified_anomaly = max(anomalies)
         LOGGER.info(
             "{uuid} - Generated unified anomaly, using max strategy. Unified Anomaly: {anomaly}",
@@ -193,15 +194,16 @@
             keys=payload.composite_keys,
         )
 
     # Compute ensemble score otherwise
     else:
         final_score = winscorer.get_final_winscore(payload)
         LOGGER.info(
-            "{uuid} - Final ensemble score: {ensemble_score}, static thresh wt: {thresh}, keys: {keys}",
+            "{uuid} - Final ensemble score: {ensemble_score}, "
+            "static thresh wt: {thresh}, keys: {keys}",
             uuid=payload.uuid,
             ensemble_score=final_score,
             thresh=metric_config.static_threshold_wt,
             keys=payload.composite_keys,
         )
 
     payload.set_status(Status.POST_PROCESSED)
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.8/numaprom/udf/preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,26 +54,28 @@
             err=err,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
     except Exception as ex:
         LOGGER.exception(
-            "{uuid} - Unhandled exception while fetching preproc artifact, keys: {keys}, err: {err}",
+            "{uuid} - Unhandled exception while fetching preproc artifact, "
+            "keys: {keys}, err: {err}",
             uuid=payload.uuid,
             keys=payload.composite_keys,
             err=ex,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     if not preproc_artifact:
         LOGGER.info(
-            "{uuid} - Preprocess artifact not found, forwarding for static thresholding. Keys: {keys}",
+            "{uuid} - Preprocess artifact not found, forwarding for static thresholding. "
+            "Keys: {keys}",
             uuid=payload.uuid,
             keys=payload.composite_keys,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.ARTIFACT_NOT_FOUND)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/threshold.py` & `numalogic_prometheus-0.4.8/numaprom/udf/threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             err=err,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
     except Exception as ex:
         LOGGER.exception(
-            "{uuid} - Unhandled exception while fetching threshold artifact, keys: {keys}, err: {err}",
+            "{uuid} - Unhandled exception while fetching threshold artifact, "
+            "keys: {keys}, err: {err}",
             uuid=payload.uuid,
             keys=payload.composite_keys,
             err=ex,
         )
         payload.set_header(Header.STATIC_INFERENCE)
         payload.set_status(Status.RUNTIME_ERROR)
         return [
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udf/window.py` & `numalogic_prometheus-0.4.8/numaprom/udf/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import time
 import uuid
-from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 
@@ -52,15 +51,15 @@
     if not _is_new:
         return []
     _window = list(map(lambda x: (float(x[0].decode().split("::")[0]), x[1]), _window))
     return _window
 
 
 @msg_forward
-def window(_: list[str], datum: Datum) -> Optional[bytes]:
+def window(_: list[str], datum: Datum) -> bytes | None:
     """UDF to construct windowing of the streaming input data, required by ML models."""
     LOGGER.debug("Received Msg: {data} ", data=datum.value)
 
     _start_time = time.perf_counter()
     msg = orjson.loads(datum.value)
 
     metric_config = ConfigManager.get_metric_config(
@@ -94,15 +93,15 @@
         return None
 
     # Construct payload object
     _uuid = uuid.uuid4().hex
     win_list = [float(_val) for _val, _ in elements]
 
     # Store win_arr as a matrix with columns representing features
-    win_arr = np.asarray(win_list).reshape(-1, 1)
+    win_arr = np.array(win_list).reshape(-1, 1)
     win_arr = _clean_arr(_uuid, composite_keys, win_arr)
 
     payload = StreamPayload(
         uuid=uuid.uuid4().hex,
         header=Header.MODEL_INFERENCE,
         composite_keys=composite_keys,
         status=Status.EXTRACTED,
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.8/numaprom/udsink/train.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.7/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.8/numaprom/udsink/train_rollout.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     x_reconerr, anomaly_model, trainer = _train_model(payload.uuid, x_train, model_cfg, trainer_cfg)
 
     thresh_cfg = metric_config.numalogic_conf.threshold
     thresh_clf = _find_threshold(x_reconerr, thresh_cfg)
 
     skeys = [payload.composite_keys["namespace"], payload.composite_keys["name"]]
 
-    # TODO if one of the models fail to save, delete the previously saved models and transition stage
+    # TODO if one of the models fail to save, delete the previously saved models & transition stage
     # Save main model
     model_registry = RedisRegistry(client=redis_client)
     try:
         version = model_registry.save(
             skeys=skeys,
             dkeys=[model_cfg.name],
             artifact=anomaly_model,
```

### Comparing `numalogic_prometheus-0.4.7/numaprom/watcher.py` & `numalogic_prometheus-0.4.8/numaprom/watcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import time
 from functools import lru_cache
-from typing import Optional
 
 from omegaconf import OmegaConf
 from watchdog.observers import Observer
 from numalogic.config import NumalogicConf
 from watchdog.events import FileSystemEventHandler
 
 from numaprom._config import PipelineConf, RedisConf, PrometheusConf, RegistryConf
@@ -49,15 +48,15 @@
         cls.config["pipeline_config"] = pipeline_config
 
         LOGGER.info("Successfully updated configs - {config}", config=cls.config)
         return cls.config
 
     @classmethod
     @lru_cache(maxsize=100)
-    def get_app_config(cls, metric: str, namespace: str) -> Optional[AppConf]:
+    def get_app_config(cls, metric: str, namespace: str) -> AppConf | None:
         if not cls.config:
             cls.update_configs()
 
         app_config = None
 
         # search and load from app configs
         if namespace in cls.config["app_configs"]:
@@ -78,27 +77,27 @@
         for metric_config in app_config.metric_configs:
             if OmegaConf.is_missing(metric_config, "numalogic_conf"):
                 metric_config.numalogic_conf = cls.config["default_numalogic"]
 
         return app_config
 
     @classmethod
-    def get_metric_config(cls, composite_keys: dict) -> Optional[MetricConf]:
+    def get_metric_config(cls, composite_keys: dict) -> MetricConf | None:
         app_config = cls.get_app_config(
             metric=composite_keys["name"], namespace=composite_keys["namespace"]
         )
         metric_config = list(
             filter(lambda conf: (conf.metric == composite_keys["name"]), app_config.metric_configs)
         )
         if not metric_config:
             return app_config.metric_configs[0]
         return metric_config[0]
 
     @classmethod
-    def get_unified_config(cls, composite_keys: dict) -> Optional[UnifiedConf]:
+    def get_unified_config(cls, composite_keys: dict) -> UnifiedConf | None:
         app_config = cls.get_app_config(
             metric=composite_keys["name"], namespace=composite_keys["namespace"]
         )
         unified_config = list(
             filter(
                 lambda conf: (composite_keys["name"] in conf.unified_metrics),
                 app_config.unified_configs,
```

### Comparing `numalogic_prometheus-0.4.7/pyproject.toml` & `numalogic_prometheus-0.4.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.4.7"
+version = "0.4.8"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
@@ -23,31 +23,26 @@
 pynumaflow = "~0.4.1"
 numalogic = {version = "~0.4", extras = ["redis"]}
 orjson = "^3.8.4"
 omegaconf = "^2.3.0"
 watchdog = "^3.0.0"
 loguru = "^0.7.0"
 
-[tool.poetry.group.mlflowserver]
-optional = true
-
-[tool.poetry.group.mlflowserver.dependencies]
-mlflow = "^2.2"
-
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.3"
 black = "^23.1"
 fakeredis = "^2.11"
-flake8 = "^5.0"
+ruff = "^0.0.264"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 freezegun = "^1.2.2"
+pre-commit = "^3.3.1"
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
@@ -60,10 +55,23 @@
   | buck-out
   | build
   | dist
   | tests/.*/setup.py
 )/
 '''
 
+[tool.ruff]
+line-length = 100
+src = ["numaprom", "tests"]
+select = ["E", "F", "UP"]
+target-version = "py310"
+show-fixes = true
+show-source = true
+extend-exclude = [
+    "*_pb2.py",
+    "*_pb2*.py",
+    "*.pyi"
+]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `numalogic_prometheus-0.4.7/PKG-INFO` & `numalogic_prometheus-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.4.7
+Version: 0.4.8
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```

