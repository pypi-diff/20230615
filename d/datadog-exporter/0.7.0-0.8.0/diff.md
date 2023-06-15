# Comparing `tmp/datadog_exporter-0.7.0-py3-none-any.whl.zip` & `tmp/datadog_exporter-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 15986 bytes, number of entries: 19
+Zip file size: 15990 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-10 11:05 datadog_export/__init__.py
 -rw-r--r--  2.0 unx       44 b- defN 20-Mar-16 16:39 datadog_export/__main__.py
--rw-r--r--  2.0 unx      520 b- defN 20-Mar-18 15:25 datadog_export/cli.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jun-15 08:24 datadog_export/cli.py
 -rw-r--r--  2.0 unx     2207 b- defN 20-Mar-18 15:25 datadog_export/config.py
 -rw-r--r--  2.0 unx     4947 b- defN 20-Mar-18 16:38 datadog_export/events.py
--rw-r--r--  2.0 unx     4102 b- defN 20-Mar-18 16:52 datadog_export/exporter.py
+-rw-r--r--  2.0 unx     4141 b- defN 23-Jun-15 08:23 datadog_export/exporter.py
 -rw-r--r--  2.0 unx      253 b- defN 20-Mar-18 15:23 datadog_export/logger.py
--rw-r--r--  2.0 unx     3694 b- defN 20-Mar-18 16:45 datadog_export/metrics.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jun-15 08:20 datadog_export/metrics.py
 -rw-r--r--  2.0 unx     2221 b- defN 20-Mar-18 16:52 datadog_export/names.py
 -rw-r--r--  2.0 unx      105 b- defN 20-Mar-10 13:27 datadog_export/click_argument_types/__init__.py
--rw-r--r--  2.0 unx     1385 b- defN 20-Mar-17 12:49 datadog_export/click_argument_types/click_datetime.py
+-rw-r--r--  2.0 unx     1393 b- defN 23-Jun-15 08:53 datadog_export/click_argument_types/click_datetime.py
 -rw-r--r--  2.0 unx      598 b- defN 20-Mar-17 12:50 datadog_export/click_argument_types/click_duration.py
 -rw-r--r--  2.0 unx      553 b- defN 20-Mar-17 12:53 datadog_export/click_argument_types/click_regex.py
--rw-------  2.0 unx    11357 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1940 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1689 b- defN 22-Dec-19 16:01 datadog_exporter-0.7.0.dist-info/RECORD
-19 files, 35788 bytes uncompressed, 13170 bytes compressed:  63.2%
+-rw-------  2.0 unx    11357 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1940 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1689 b- defN 23-Jun-15 09:04 datadog_exporter-0.8.0.dist-info/RECORD
+19 files, 35672 bytes uncompressed, 13174 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: datadog_export/click_argument_types/click_duration.py
 Comment: 
 
 Filename: datadog_export/click_argument_types/click_regex.py
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/LICENSE
+Filename: datadog_exporter-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/METADATA
+Filename: datadog_exporter-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/WHEEL
+Filename: datadog_exporter-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/entry_points.txt
+Filename: datadog_exporter-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/top_level.txt
+Filename: datadog_exporter-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: datadog_exporter-0.7.0.dist-info/RECORD
+Filename: datadog_exporter-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datadog_export/cli.py

```diff
@@ -1,9 +1,9 @@
 from datadog_export.logger import log
-
+import logging
 import click
 import os
 
 from datadog_export.events import main as export_events
 from datadog_export.metrics import main as export_metrics
 from datadog_export.names import main as export_names
```

## datadog_export/exporter.py

```diff
@@ -31,14 +31,15 @@
         self,
         account: str,
         start_time: Optional[datetime],
         end_time: datetime,
         window: Duration,
     ):
         super(Exporter, self).__init__()
+        self.ratelimit = RateLimit({})
         self.account: str = account if account else "DEFAULT"
         self.window: Duration = window
         self.end_time: datetime = end_time
         self.start_time: datetime = start_time
         self.iso_date_formats = False
         self.pretty_print = False
         self.metrics = []
```

## datadog_export/metrics.py

```diff
@@ -24,19 +24,14 @@
         self.query = None
 
     def export_started(self):
         log.info(
             f"exporting {self.query} from {self.start_time} to {self.end_time} in {self.window.representation} steps"
         )
 
-    def export_started(self):
-        log.info(
-            f"exporting {self.query} from {self.start_time} to {self.end_time} in {self.window.representation} steps"
-        )
-
     def _get(self, st: datetime, et: datetime) -> requests.Response:
         return requests.get(
             "https://api.datadoghq.com/api/v1/query",
             headers=self.get_headers(),
             params={
                 "from": int(st.timestamp()),
                 "to": int(et.timestamp()),
```

## datadog_export/click_argument_types/click_datetime.py

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self):
         self.tz = get_localzone()
 
     def to_utc(self, dt: datetime):
         result = dt
         if not result.tzinfo:
-            result = self.tz.localize(result)
+            result = result.astimezone(result.tzinfo)
         return result.astimezone(pytz.UTC)
 
     def convert(self, value, param, ctx) -> Optional[datetime]:
         if value is None:
             return value
 
         if isinstance(value, datetime):
```

## Comparing `datadog_exporter-0.7.0.dist-info/LICENSE` & `datadog_exporter-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `datadog_exporter-0.7.0.dist-info/METADATA` & `datadog_exporter-0.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-exporter
-Version: 0.7.0
+Version: 0.8.0
 Summary: CLI for exporting datadog metrics
 Home-page: https://github.com/binxio/datadog-exporter
 Author: Mark van Holsteijn
 Author-email: mark@binx.io
 License: Apache2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `datadog_exporter-0.7.0.dist-info/RECORD` & `datadog_exporter-0.8.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 datadog_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datadog_export/__main__.py,sha256=KdMI7zDM0H5DErLkgmS-UanoehcYk2nCvoiR_KCaVxw,44
-datadog_export/cli.py,sha256=u3Wuz_b4uczRn13gHwTSFvliZ-aeGQ-W3UpGOK-EYik,520
+datadog_export/cli.py,sha256=AbohxqkuEOGGbe4zynCrHK8vnPss2YjIZFnR1AKYm1g,534
 datadog_export/config.py,sha256=Rk9fZbVW51Pj2Pt6YzNFE2qkCpEeDtjMOWZKzdWjuyY,2207
 datadog_export/events.py,sha256=qGF2gayM_qFLOllK1Sb6kVvT0SVG-0oNodhXKMdOxgQ,4947
-datadog_export/exporter.py,sha256=W6K5tjsFte0bsdIrQWLFVzU4chhDpyFwrq3519LlqvI,4102
+datadog_export/exporter.py,sha256=l3KI20bIaDl7g6msZmXxzfjKz7CQ-n9Q3WV52rkwZzY,4141
 datadog_export/logger.py,sha256=1dOModbv8dzzyaUlQYstVSmbwEGa6nz5e3ikm7NdLP4,253
-datadog_export/metrics.py,sha256=Ftk-XVZZSqQL5F4voaamzprBbI5QDAvcVDYaGkJ3ao8,3694
+datadog_export/metrics.py,sha256=x0vusSOX5xp8UI0FyuNih16smd9tM4oiLvycH2l5T1g,3517
 datadog_export/names.py,sha256=0MavYpW8h2cxWbzkTcQ_6fPHYAIY_S7lEiTfBK4HvZI,2221
 datadog_export/click_argument_types/__init__.py,sha256=gWqHcFdMsoViGTfFx2gdfLzdWgeA9gfzwN44qXmNFEU,105
-datadog_export/click_argument_types/click_datetime.py,sha256=nC1AP1iU-tDD5Oh2h1fveKfKRd48tgRHuAAMosmTzdU,1385
+datadog_export/click_argument_types/click_datetime.py,sha256=xKpNQ6NoL08-o3oC7MXRDZ6zbIoUr-4d65gPM49FQY4,1393
 datadog_export/click_argument_types/click_duration.py,sha256=ujnuUDNXhEnSn3rE9G70Gk-xc8Yw_Mg9QMVibcVG0F8,598
 datadog_export/click_argument_types/click_regex.py,sha256=xzWQInqRnztZDwoSSik_QObsKJRxO8sy4n7fqjuPrq4,553
-datadog_exporter-0.7.0.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-datadog_exporter-0.7.0.dist-info/METADATA,sha256=W5NURIbmvlKMRLgdnZXy5CEkaNkXjVJF1BLTJQbT9pY,1940
-datadog_exporter-0.7.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-datadog_exporter-0.7.0.dist-info/entry_points.txt,sha256=EdkWdHccAaPqwq2nV_rNwKQH7rlIEaEOfHgv2_NrKe8,66
-datadog_exporter-0.7.0.dist-info/top_level.txt,sha256=Qj0GsIj204dnLGGcYayxMffI6MeI_Xbh_6si4hhcDps,15
-datadog_exporter-0.7.0.dist-info/RECORD,,
+datadog_exporter-0.8.0.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+datadog_exporter-0.8.0.dist-info/METADATA,sha256=mwMr6WDnA1oTb9WeMPFqbIelhmo_vtRnvAAcKCmSKKc,1940
+datadog_exporter-0.8.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datadog_exporter-0.8.0.dist-info/entry_points.txt,sha256=EdkWdHccAaPqwq2nV_rNwKQH7rlIEaEOfHgv2_NrKe8,66
+datadog_exporter-0.8.0.dist-info/top_level.txt,sha256=Qj0GsIj204dnLGGcYayxMffI6MeI_Xbh_6si4hhcDps,15
+datadog_exporter-0.8.0.dist-info/RECORD,,
```

