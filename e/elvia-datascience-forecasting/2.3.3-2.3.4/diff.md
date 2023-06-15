# Comparing `tmp/elvia-datascience-forecasting-2.3.3.tar.gz` & `tmp/elvia-datascience-forecasting-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elvia-datascience-forecasting-2.3.3.tar", last modified: Thu Jun  1 14:34:53 2023, max compression
+gzip compressed data, was "elvia-datascience-forecasting-2.3.4.tar", last modified: Thu Jun 15 12:15:08 2023, max compression
```

## Comparing `elvia-datascience-forecasting-2.3.3.tar` & `elvia-datascience-forecasting-2.3.4.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.277194 elvia-datascience-forecasting-2.3.3/
--rw-rw-rw-   0        0        0      146 2023-06-01 14:34:53.276191 elvia-datascience-forecasting-2.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.193653 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/
--rw-rw-rw-   0        0        0      146 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1422 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.201647 elvia-datascience-forecasting-2.3.3/forecast_dataprep/
--rw-rw-rw-   0        0        0       71 2023-06-01 14:33:20.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.231664 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/__init__.py
--rw-rw-rw-   0        0        0     2037 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/cyclical_features.py
--rw-rw-rw-   0        0        0     1246 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/delayed_features.py
--rw-rw-rw-   0        0        0     2926 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/national_holiday.py
--rw-rw-rw-   0        0        0      845 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/prices.py
--rw-rw-rw-   0        0        0     4397 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/school_holiday.py
--rw-rw-rw-   0        0        0     1757 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/temperature.py
--rw-rw-rw-   0        0        0      180 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/time_constants.py
--rw-rw-rw-   0        0        0     1290 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/weekly_average.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.252192 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/
--rw-rw-rw-   0        0        0     2745 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/__init__.py
--rw-rw-rw-   0        0        0      259 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/bq_auth.py
--rw-rw-rw-   0        0        0     4940 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/common.py
--rw-rw-rw-   0        0        0      577 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/data_models.py
--rw-rw-rw-   0        0        0     3196 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/meteringpoints.py
--rw-rw-rw-   0        0        0     3277 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/substations.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.264199 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/__init__.py
--rw-rw-rw-   0        0        0     2034 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/prediction.py
--rw-rw-rw-   0        0        0     3083 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/shared.py
--rw-rw-rw-   0        0        0     7296 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/training.py
--rw-rw-rw-   0        0        0     3367 2023-05-30 13:30:49.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_models.py
--rw-rw-rw-   0        0        0     8506 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.273196 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/data_models.py
--rw-rw-rw-   0        0        0     8404 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/wrapper.py
--rw-rw-rw-   0        0        0      230 2023-01-18 21:23:05.000000 elvia-datascience-forecasting-2.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:34:53.278195 elvia-datascience-forecasting-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-01-23 21:07:35.000000 elvia-datascience-forecasting-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:08.100088 elvia-datascience-forecasting-2.3.4/
+-rw-rw-rw-   0        0        0      146 2023-06-15 12:15:08.094157 elvia-datascience-forecasting-2.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:07.848179 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/
+-rw-rw-rw-   0        0        0      146 2023-06-15 12:15:07.000000 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2023-06-15 12:15:07.000000 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 12:15:07.000000 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      239 2023-06-15 12:15:07.000000 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-15 12:15:07.000000 elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:07.872795 elvia-datascience-forecasting-2.3.4/forecast_dataprep/
+-rw-rw-rw-   0        0        0       71 2023-06-15 11:39:20.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:07.958513 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/__init__.py
+-rw-rw-rw-   0        0        0     2037 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/cyclical_features.py
+-rw-rw-rw-   0        0        0     1246 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/delayed_features.py
+-rw-rw-rw-   0        0        0     2926 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/national_holiday.py
+-rw-rw-rw-   0        0        0      845 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/prices.py
+-rw-rw-rw-   0        0        0     4397 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/school_holiday.py
+-rw-rw-rw-   0        0        0     1757 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/temperature.py
+-rw-rw-rw-   0        0        0      180 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/time_constants.py
+-rw-rw-rw-   0        0        0     1290 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/weekly_average.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:08.010841 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/
+-rw-rw-rw-   0        0        0     2763 2023-06-15 11:54:51.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/bq_auth.py
+-rw-rw-rw-   0        0        0     4964 2023-06-15 11:55:26.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/common.py
+-rw-rw-rw-   0        0        0      577 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/data_models.py
+-rw-rw-rw-   0        0        0     3196 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/meteringpoints.py
+-rw-rw-rw-   0        0        0     3277 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/substations.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:08.042903 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/__init__.py
+-rw-rw-rw-   0        0        0     2034 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/prediction.py
+-rw-rw-rw-   0        0        0     3083 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/shared.py
+-rw-rw-rw-   0        0        0     7296 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/training.py
+-rw-rw-rw-   0        0        0     4856 2023-06-15 11:54:13.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_models.py
+-rw-rw-rw-   0        0        0     8506 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:08.062135 elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/data_models.py
+-rw-rw-rw-   0        0        0     8404 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/wrapper.py
+-rw-rw-rw-   0        0        0      251 2023-06-15 10:41:04.000000 elvia-datascience-forecasting-2.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 12:15:08.101651 elvia-datascience-forecasting-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-01-23 21:07:35.000000 elvia-datascience-forecasting-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 12:15:08.079155 elvia-datascience-forecasting-2.3.4/test/
+-rw-rw-rw-   0        0        0        0 2023-06-15 10:07:54.000000 elvia-datascience-forecasting-2.3.4/test/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-06-15 12:09:43.000000 elvia-datascience-forecasting-2.3.4/test/constants.py
```

### Comparing `elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/SOURCES.txt` & `elvia-datascience-forecasting-2.3.4/elvia_datascience_forecasting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 forecast_dataprep/data_fetching/substations.py
 forecast_dataprep/data_ingestion/__init__.py
 forecast_dataprep/data_ingestion/prediction.py
 forecast_dataprep/data_ingestion/shared.py
 forecast_dataprep/data_ingestion/training.py
 forecast_dataprep/weather_api/__init__.py
 forecast_dataprep/weather_api/data_models.py
-forecast_dataprep/weather_api/wrapper.py
+forecast_dataprep/weather_api/wrapper.py
+test/__init__.py
+test/constants.py
```

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/cyclical_features.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/cyclical_features.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/delayed_features.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/delayed_features.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/national_holiday.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/national_holiday.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/prices.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/prices.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/school_holiday.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/school_holiday.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/temperature.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/temperature.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/weekly_average.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_enrichment/weekly_average.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/__init__.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from typing import Optional, Tuple
 
 import pandas as pd
 
 from forecast_dataprep.data_fetching.data_models import BigQueryBundle
-from forecast_dataprep.data_models import Dataframes, EnrichmentFeaturesBundle, ModelTargetList, ModelTargetLevel
+from forecast_dataprep.data_models import Dataframes, EnrichmentFeaturesBundle, ForecastTargetList, ForecastTargetLevel
 from forecast_dataprep.data_fetching.common import get_hourly_data, get_national_holidays, get_prices, get_school_holidays, get_weekly_data
 from forecast_dataprep.data_fetching.meteringpoints import get_meteringpoint_metadata
 from forecast_dataprep.data_fetching.substations import get_substation_metadata
 
 
-def get_dataframes(bq: BigQueryBundle, targets: ModelTargetList,
+def get_dataframes(bq: BigQueryBundle, targets: ForecastTargetList,
                    timespan: Tuple[datetime,
                                    datetime], use_prices: bool) -> Dataframes:
     """
     Query Edna tables and fetch data, returned as dataframes.
     The substation/meteringpoint metadata is not part of this group of queries, in order to 
     optimise the overall execution order.
 
@@ -43,19 +43,19 @@
     dfnh = dfnh.result()
     dfsh = dfsh.result()
 
     return Dataframes(dfh, EnrichmentFeaturesBundle(dfw, dfsh, dfnh, dfp))
 
 
 def get_metadata(bq: BigQueryBundle,
-                 targets: ModelTargetList) -> Optional[pd.DataFrame]:
+                 targets: ForecastTargetList) -> Optional[pd.DataFrame]:
     """
     Get meteringpoint/substation metadata. 
     The result contains columns latitude and longitude that are needed to get the right forecast
     data from Weather API. It also contains column postalCode, which is needed to enrich with the
     location-dependant school holidays feature.
     """
-    if targets.level == ModelTargetLevel.METERING_POINT:
+    if targets.level == ForecastTargetLevel.METERING_POINT:
         return get_meteringpoint_metadata(bq, targets.identifiers)
-    elif targets.level == ModelTargetLevel.SUBSTATION:
+    elif targets.level == ForecastTargetLevel.SUBSTATION:
         return get_substation_metadata(bq, targets.identifiers)
     return None
```

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/common.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 from typing import Optional, Tuple
 
 from google.cloud import bigquery
 from google.cloud.bigquery.job import QueryJob
 import pandas as pd
 
 from forecast_dataprep.data_fetching.data_models import BigQueryBundle
-from forecast_dataprep.data_models import ModelTargetLevel, ModelTargetList
+from forecast_dataprep.data_models import ForecastTargetLevel, ForecastTargetList
 from forecast_dataprep.data_fetching.meteringpoints import get_meteringpoint_hourly_data, get_meteringpoint_weekly_data
 from forecast_dataprep.data_fetching.substations import get_substation_hourly_data, get_substation_weekly_data
 
 
 def get_hourly_data(
     bq: BigQueryBundle,
-    targets: ModelTargetList,
+    targets: ForecastTargetList,
     timespan: Optional[Tuple[datetime, datetime]] = None
 ) -> Optional[pd.DataFrame]:
 
-    if targets.level == ModelTargetLevel.METERING_POINT:
+    if targets.level == ForecastTargetLevel.METERING_POINT:
         return get_meteringpoint_hourly_data(bq, targets.identifiers, timespan)
-    elif targets.level == ModelTargetLevel.SUBSTATION:
+    elif targets.level == ForecastTargetLevel.SUBSTATION:
         return get_substation_hourly_data(bq, targets.identifiers, timespan)
     return None
 
 
 def get_weekly_data(bq: BigQueryBundle,
-                    targets: ModelTargetList) -> pd.DataFrame:
+                    targets: ForecastTargetList) -> pd.DataFrame:
 
-    if targets.level == ModelTargetLevel.METERING_POINT:
+    if targets.level == ForecastTargetLevel.METERING_POINT:
         return get_meteringpoint_weekly_data(bq, targets.identifiers)
-    elif targets.level == ModelTargetLevel.SUBSTATION:
+    elif targets.level == ForecastTargetLevel.SUBSTATION:
         return get_substation_weekly_data(bq, targets.identifiers)
     return None
 
 
 def get_national_holidays(bq: BigQueryBundle, from_time: datetime,
                           to_time: datetime):
     query = (
```

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/data_models.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/data_models.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/meteringpoints.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/meteringpoints.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/substations.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_fetching/substations.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/prediction.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/prediction.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/shared.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/shared.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/training.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_ingestion/training.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_models.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/data_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,75 +4,102 @@
 import re
 from typing import List, Optional, Union
 
 import pandas as pd
 
 
 ### Abstractions to represent (a list of) either meteringpoints or substations
-class ModelTargetLevel(Enum):
+class ForecastTargetLevel(Enum):
 
     METERING_POINT = 1
     SUBSTATION = 2
 
 
-class ModelTargetList:
+class ForecastTarget:
 
-    def __init__(self,
-                 identifiers: Optional[List[Union[str, int]]] = None,
-                 allow_duplicates: bool = False) -> None:
+    def __init__(self, identifier: Union[int, str]):
+        if ForecastTargetList.get_type(identifier) is not None:
+            self.identifier = identifier
+        else:
+            raise ValueError
+
+    @property
+    def level(self)->ForecastTargetLevel:
+        return ForecastTargetList.get_type(self.identifier)
+    
+
+class ForecastTargetList:
 
+    def __init__(self,
+                 identifiers: List[Union[str, int, ForecastTarget]],
+                 allow_duplicates: bool = False,
+                 enforce_int_meteringpoints:bool=True,
+                 enforce_str_substations:bool=True) -> None:
+        """
+        Mixing strings and ints when instantiating is allowed, but the identifiers must all belong to the same ForecastTargetLevel
+        """
         self.identifiers: list = []
         self.allow_duplicates = allow_duplicates
+        self.enforce_int_meteringpoints = enforce_int_meteringpoints
+        self.enforce_str_substations = enforce_str_substations
 
-        if identifiers:
-            for i in identifiers:
-                self.put(i)
+        if not identifiers:
+            raise ValueError
+        for i in identifiers:
+            self.put(i)
 
-    def put(self, identifier: Union[int, str]) -> None:
+    def put(self, identifier: Union[int, str, ForecastTarget]) -> None:
         level = self.get_type(identifier)
         if level is None:
             raise ValueError('The identifier does not look right')
-        if level == ModelTargetLevel.METERING_POINT:
-            self._add_if_match_existing(int(identifier))
-        if level == ModelTargetLevel.SUBSTATION:
-            self._add_if_match_existing(str(identifier).upper())
+        if level == ForecastTargetLevel.METERING_POINT:
+            self._add_if_match_existing(identifier if not isinstance(identifier, ForecastTarget) else identifier.identifier)
+        if level == ForecastTargetLevel.SUBSTATION:
+            self._add_if_match_existing(identifier if not isinstance(identifier, ForecastTarget) else identifier.identifier)
 
-    def _add_if_match_existing(self, identifier):
+    def _add_if_match_existing(self, identifier: Union[str, int]):
         if not self.identifiers or self.get_type(identifier) == self.get_type(
                 self.identifiers[0]):
             if self.allow_duplicates or identifier not in set(
                     self.identifiers):
-                self.identifiers.append(identifier)
+                if self.enforce_int_meteringpoints and self.get_type(identifier) == ForecastTargetLevel.METERING_POINT:
+                    self.identifiers.append(int(identifier))
+                elif self.enforce_str_substations and self.get_type(identifier) == ForecastTargetLevel.SUBSTATION:
+                    self.identifiers.append(str(identifier))
+                else:
+                    self.identifiers.append(identifier)
             else:
-                raise ValueError('Duplicates not allowed')
+                raise ValueError(f'Duplicates were not allowed in this {__class__.__name__} instance')
         else:
             raise ValueError(
-                'Model targets must all be either substation or meteringpoint')
+                'Forecast targets must all be either substation or meteringpoint')
 
     @staticmethod
-    def get_type(identifier: Union[str, int]) -> Optional[ModelTargetLevel]:
-        if isinstance(
+    def get_type(identifier: Union[str, int, ForecastTarget]) -> Optional[ForecastTargetLevel]:
+        if isinstance(identifier, ForecastTarget):
+            return identifier.level        
+        elif isinstance(
                 identifier, int
         ) and identifier > 707057500014300000 and identifier < 707057500087400700:
-            return ModelTargetLevel.METERING_POINT
+            return ForecastTargetLevel.METERING_POINT
         elif isinstance(identifier, str) and re.fullmatch(
                 r"7070575000[\d]{8}", identifier):
-            return ModelTargetLevel.METERING_POINT
+            return ForecastTargetLevel.METERING_POINT
         elif isinstance(identifier, str) and re.fullmatch(
-                r"[A-ZÆØÅ\d\-]+", identifier.upper()):
-            return ModelTargetLevel.SUBSTATION
+                r"[A-ZÆØÅ\d\- ]+", identifier.upper()):
+            return ForecastTargetLevel.SUBSTATION
         return None
 
     @property
-    def level(self) -> Optional[ModelTargetLevel]:
-        return self.get_type(self.identifiers[0]) if self.identifiers else None
+    def level(self) -> ForecastTargetLevel:
+        return self.get_type(self.identifiers[0])
 
     @staticmethod
-    def from_json(target_model_list: str) -> 'ModelTargetList':
-        return ModelTargetList(json.loads(target_model_list))
+    def from_json(target_model_list: str) -> 'ForecastTargetList':
+        return ForecastTargetList(json.loads(target_model_list))
 
     def to_json(self) -> str:
         return json.dumps(self.identifiers)
 
 
 ### Dataframe groupings
```

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/functions.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/functions.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/data_models.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/data_models.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/wrapper.py` & `elvia-datascience-forecasting-2.3.4/forecast_dataprep/weather_api/wrapper.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.3/setup.py` & `elvia-datascience-forecasting-2.3.4/setup.py`

 * *Files identical despite different names*

