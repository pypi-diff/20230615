# Comparing `tmp/numalogic_prometheus-0.4.5.tar.gz` & `tmp/numalogic_prometheus-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.4.5.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.4.6.tar", max compression
```

## Comparing `numalogic_prometheus-0.4.5.tar` & `numalogic_prometheus-0.4.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/LICENSE
--rw-r--r--   0        0        0     1894 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/__init__.py
--rw-r--r--   0        0        0     1400 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3603 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1291 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2519 2023-06-14 20:34:45.594565 numalogic_prometheus-0.4.5/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4496 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/factory.py
--rw-r--r--   0        0        0     7169 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      720 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4687 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/inference.py
--rw-r--r--   0        0        0     7309 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     3270 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     4744 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4217 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     7399 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udsink/train.py
--rw-r--r--   0        0        0     8543 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     6016 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/numaprom/watcher.py
--rw-r--r--   0        0        0     1537 2023-06-14 20:34:45.598565 numalogic_prometheus-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 00:42:16.032019 numalogic_prometheus-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1894 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/__init__.py
+-rw-r--r--   0        0        0     1400 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1291 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2519 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4496 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/factory.py
+-rw-r--r--   0        0        0     7169 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      720 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4687 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     7309 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     3270 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     4744 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4217 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     7399 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     8543 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     6016 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/numaprom/watcher.py
+-rw-r--r--   0        0        0     1537 2023-06-15 00:42:16.036019 numalogic_prometheus-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 numalogic_prometheus-0.4.6/PKG-INFO
```

### Comparing `numalogic_prometheus-0.4.5/LICENSE` & `numalogic_prometheus-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/__init__.py` & `numalogic_prometheus-0.4.6/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/_config.py` & `numalogic_prometheus-0.4.6/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/_constants.py` & `numalogic_prometheus-0.4.6/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.4.6/numaprom/clients/prometheus.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,72 +25,76 @@
             query = metric_name + "{" + ",".join(label_list) + "}"
 
         LOGGER.debug("Prometheus Query: {query}", query=query)
 
         if end < start:
             raise ValueError("end_time must not be before start_time")
 
-        result = self.query_range(query, start, end, step)
+        results = self.query_range(query, start, end, step)
 
-        arr = np.array(result["values"])
-        df = pd.DataFrame(arr, columns=["timestamp", metric_name])
-        df = df.astype(float)
-
-        data = result["metric"]
-        if return_labels:
-            for label in return_labels:
-                if label in data:
-                    df[label] = data[label]
-
-        if not df.empty:
-            df.set_index("timestamp", inplace=True)
-            df.index = pd.to_datetime(df.index.astype(int), unit="s")
+        frames = []
+        for result in results:
+            LOGGER.debug(
+                "Prometheus query has returned {total} values for {metric}.",
+                total=len(result["values"]),
+                metric=result["metric"],
+            )
+            arr = np.array(result["values"], dtype=float)
+            _df = pd.DataFrame(arr, columns=["timestamp", metric_name])
+
+            data = result["metric"]
+            if return_labels:
+                for label in return_labels:
+                    if label in data:
+                        _df[label] = data[label]
+            frames.append(_df)
+
+        df = pd.DataFrame()
+        if frames:
+            df = pd.concat(frames, ignore_index=True)
+            df.sort_values(by=["timestamp"], inplace=True)
+            df["timestamp"] = pd.to_datetime(df["timestamp"], unit="s")
+            df.reset_index(drop=True, inplace=True)
         return df
 
-    def query_range(self, query: str, start: float, end: float, step: int = 30) -> Optional[dict]:
-        results = {}
+    def query_range(self, query: str, start: float, end: float, step: int = 30) -> Optional[list]:
+        results = []
         data_points = (end - start) / step
         temp_start = start
         while data_points > 11000:
             temp_end = temp_start + 11000 * step
             response = self.query_range_limit(query, temp_start, temp_end, step)
-            if results:
-                results["values"] = results["values"] + response["values"]
-            else:
-                results = response
+            for res in response:
+                results.append(res)
             temp_start = temp_end
             data_points = (end - temp_start) / step
 
         if data_points > 0:
             response = self.query_range_limit(query, temp_start, end)
-            if results:
-                LOGGER.debug("Prometheus query returned results.")
-                results["values"] = results["values"] + response["values"]
-            else:
-                LOGGER.debug("Prometheus query has returned empty results.")
-                results = response
-
+            for res in response:
+                results.append(res)
         return results
 
-    def query_range_limit(
-        self, query: str, start: float, end: float, step: int = 30
-    ) -> Optional[dict]:
+    def query_range_limit(self, query: str, start: float, end: float, step: int = 30) -> list:
+        results = []
         data_points = (end - start) / step
 
         if data_points > 11000:
             LOGGER.info("Limit query only supports 11,000 data points")
-            return None
-
-        results = None
+            return results
         try:
             response = requests.get(
                 self.PROMETHEUS_SERVER + "/api/v1/query_range",
                 params={"query": query, "start": start, "end": end, "step": f"{step}s"},
             )
-            results = response.json()["data"]["result"][0]
+            results = response.json()["data"]["result"]
+            LOGGER.debug(
+                "Prometheus query has returned results for {results} metric series.",
+                results=len(results),
+            )
         except Exception as ex:
             LOGGER.exception("Prometheus error: {err}", err=ex)
         return results
 
     def query(self, query: str) -> Optional[dict]:
         results = []
         try:
```

### Comparing `numalogic_prometheus-0.4.5/numaprom/clients/redis.py` & `numalogic_prometheus-0.4.6/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.4.6/numaprom/clients/sentinel.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/configs/config.yaml` & `numalogic_prometheus-0.4.6/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.4.6/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/entities.py` & `numalogic_prometheus-0.4.6/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/factory.py` & `numalogic_prometheus-0.4.6/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/tools.py` & `numalogic_prometheus-0.4.6/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/filter.py` & `numalogic_prometheus-0.4.6/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/inference.py` & `numalogic_prometheus-0.4.6/numaprom/udf/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.4.6/numaprom/udf/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.4.6/numaprom/udf/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/threshold.py` & `numalogic_prometheus-0.4.6/numaprom/udf/threshold.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udf/window.py` & `numalogic_prometheus-0.4.6/numaprom/udf/window.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udsink/train.py` & `numalogic_prometheus-0.4.6/numaprom/udsink/train.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.4.6/numaprom/udsink/train_rollout.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/numaprom/watcher.py` & `numalogic_prometheus-0.4.6/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.4.5/pyproject.toml` & `numalogic_prometheus-0.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.4.5"
+version = "0.4.6"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
```

### Comparing `numalogic_prometheus-0.4.5/PKG-INFO` & `numalogic_prometheus-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.4.5
+Version: 0.4.6
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```

