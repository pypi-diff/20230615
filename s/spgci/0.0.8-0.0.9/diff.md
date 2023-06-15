# Comparing `tmp/spgci-0.0.8.tar.gz` & `tmp/spgci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spgci-0.0.8.tar", max compression
+gzip compressed data, was "spgci-0.0.9.tar", max compression
```

## Comparing `spgci-0.0.8.tar` & `spgci-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1088 2023-02-27 00:45:39.438840 spgci-0.0.8/LICENSE
--rw-r--r--   0        0        0      700 2023-03-24 00:59:26.201013 spgci-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5373 2023-03-24 00:58:10.153394 spgci-0.0.8/README.md
--rw-r--r--   0        0        0      971 2023-03-22 20:46:14.355760 spgci-0.0.8/spgci/__init__.py
--rw-r--r--   0        0        0     3855 2023-02-27 00:52:23.013608 spgci-0.0.8/spgci/api_client.py
--rw-r--r--   0        0        0     1779 2023-02-27 00:45:39.495372 spgci-0.0.8/spgci/auth.py
--rw-r--r--   0        0        0     1262 2023-03-24 00:59:07.593166 spgci-0.0.8/spgci/config.py
--rw-r--r--   0        0        0    29245 2023-02-27 01:00:26.195877 spgci-0.0.8/spgci/epf.py
--rw-r--r--   0        0        0    10253 2023-02-27 01:07:13.166157 spgci-0.0.8/spgci/ewindow_md.py
--rw-r--r--   0        0        0      101 2023-02-27 00:45:39.500695 spgci-0.0.8/spgci/exceptions.py
--rw-r--r--   0        0        0    12948 2023-02-27 00:53:40.333522 spgci-0.0.8/spgci/forward_curves.py
--rw-r--r--   0        0        0    25393 2023-03-24 00:51:49.527036 spgci-0.0.8/spgci/insights.py
--rw-r--r--   0        0        0    23884 2023-03-05 17:10:05.981615 spgci-0.0.8/spgci/market_data.py
--rw-r--r--   0        0        0     3312 2023-02-27 00:54:49.571097 spgci-0.0.8/spgci/utilities.py
--rw-r--r--   0        0        0    29936 2023-02-27 00:57:48.402378 spgci-0.0.8/spgci/wos.py
--rw-r--r--   0        0        0    37028 2023-03-22 13:50:17.243776 spgci-0.0.8/spgci/wrd.py
--rw-r--r--   0        0        0     6167 1970-01-01 00:00:00.000000 spgci-0.0.8/setup.py
--rw-r--r--   0        0        0     5960 1970-01-01 00:00:00.000000 spgci-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-02-27 00:45:39.438840 spgci-0.0.9/LICENSE
+-rw-r--r--   0        0        0      700 2023-03-25 01:01:00.538273 spgci-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5698 2023-03-25 01:00:22.169911 spgci-0.0.9/README.md
+-rw-r--r--   0        0        0      971 2023-03-22 20:46:14.355760 spgci-0.0.9/spgci/__init__.py
+-rw-r--r--   0        0        0     4144 2023-03-25 00:45:47.311258 spgci-0.0.9/spgci/api_client.py
+-rw-r--r--   0        0        0     1779 2023-02-27 00:45:39.495372 spgci-0.0.9/spgci/auth.py
+-rw-r--r--   0        0        0     1262 2023-03-25 01:01:25.371531 spgci-0.0.9/spgci/config.py
+-rw-r--r--   0        0        0    29245 2023-02-27 01:00:26.195877 spgci-0.0.9/spgci/epf.py
+-rw-r--r--   0        0        0    10253 2023-02-27 01:07:13.166157 spgci-0.0.9/spgci/ewindow_md.py
+-rw-r--r--   0        0        0      101 2023-02-27 00:45:39.500695 spgci-0.0.9/spgci/exceptions.py
+-rw-r--r--   0        0        0    12948 2023-02-27 00:53:40.333522 spgci-0.0.9/spgci/forward_curves.py
+-rw-r--r--   0        0        0    25393 2023-03-24 00:51:49.527036 spgci-0.0.9/spgci/insights.py
+-rw-r--r--   0        0        0    23884 2023-03-05 17:10:05.981615 spgci-0.0.9/spgci/market_data.py
+-rw-r--r--   0        0        0     3312 2023-02-27 00:54:49.571097 spgci-0.0.9/spgci/utilities.py
+-rw-r--r--   0        0        0    29936 2023-02-27 00:57:48.402378 spgci-0.0.9/spgci/wos.py
+-rw-r--r--   0        0        0    48745 2023-03-25 00:46:16.729387 spgci-0.0.9/spgci/wrd.py
+-rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 spgci-0.0.9/setup.py
+-rw-r--r--   0        0        0     6275 1970-01-01 00:00:00.000000 spgci-0.0.9/PKG-INFO
```

### Comparing `spgci-0.0.8/LICENSE` & `spgci-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/pyproject.toml` & `spgci-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spgci"
-version = "0.0.8"
+version = "0.0.9"
 description = "SPGCI is an API Client for the S&P Commodity Insights REST API"
 authors = ["S&P Global Commodity Insights <pl_api_support@spglobal.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
```

### Comparing `spgci-0.0.8/README.md` & `spgci-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 import spgci as ci
 
 wrd = ci.WorldRefineryDatabase()
 
 wrd.get_yields(year=2020, owner="BP")
 # DataFrame of yields for the year "2020" where "BP" is the refinery owner.
 
+ref = wrd.get_reference_data(type=wrd.RefTypes.Refineries)
+# DataFrame of all refineries.
+
+az = ref[ref['Name'].str.contains("Al-Zour")]
+wrd.get_runs(refinery_id=az["Id"])
+# DataFrame of runs for the refineries with "Al-Zour" in the name.
+
+wrd.get_outages(refineryId=245)
+# DataFrame of outages for refineryId 245
+
 ```
 
 ### Insights
 
 ```python
 import spgci as ci
```

### Comparing `spgci-0.0.8/spgci/__init__.py` & `spgci-0.0.9/spgci/__init__.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/api_client.py` & `spgci-0.0.9/spgci/api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,34 +34,40 @@
 logger = logging.getLogger("spgci")
 
 
 @retry(tries=2, exceptions=AuthError)
 def _get(
     url: str,
     params: Dict[Any, Any],
+    include_auth_header: bool = True
     # token_fn: Callable[[str, str, str, str], str] = get_token,
 ) -> requests.Response:
-    token = get_token(spgci.config.username, spgci.config.password, spgci.config.appkey)
     headers = {
         "User-Agent": f"spgci-py/{spgci.config.version}",
-        "Authorization": f"Bearer {token}",
+        # "Authorization": f"Bearer {token}",
         "appkey": spgci.config.appkey,
     }
 
+    if include_auth_header:
+        token = get_token(
+            spgci.config.username, spgci.config.password, spgci.config.appkey
+        )
+        headers["Authorization"] = f"Bearer {token}"
+
     sleep(spgci.config.sleep_time)
 
     response: requests.Response = requests.get(
         url=url,
         params=params,
         headers=headers,
         verify=spgci.config.verify_ssl,
         proxies=spgci.config.proxies,
     )
 
-    # print(f"[{response.status_code}] - {response.url}")
+    # print(f"[{response.status_code}] - {response.url} - {response.request.headers}")
 
     # clear token cache and retry once if its a 401/403. shouldn't be hit unless token is expired..
     if response.status_code in [401, 403]:
         get_token.cache_clear()
         raise AuthError("Invalid Username, Password or Appkey")
 
     if response.status_code != 200:
@@ -74,17 +80,18 @@
 def get_data(
     path: str,
     params: Dict[Any, Any],
     df_fn: Callable[[requests.Response], DataFrame] = _to_df,
     paginate_fn: Callable[[requests.Response], Paginator] = _paginate,
     raw: bool = False,
     paginate: bool = False,
+    include_auth_header: bool = True,
 ) -> Union[DataFrame, requests.Response]:
     url = f"{spgci.config.base_url}/{path}"
-    response = _get(url, params=params)
+    response = _get(url, params=params, include_auth_header=False)
 
     if raw:
         if paginate:
             warnings.warn(
                 f"\nCannot set `paginate=True` along with `raw=True`. Returning only the page requested."
             )
         return response
@@ -118,13 +125,13 @@
             parsed = urlparse(url)
             qs = dict(parse_qsl(parsed.query))
             qs[pagination.key] = str((i - 1) * int(qs["pageSize"]))
             parsed = parsed._replace(query=urlencode(qs, quote_via=quote))
             resp = _get(url=parsed.geturl(), params={})
         else:
             params[pagination.key] = i
-            resp = _get(url, params=params)
+            resp = _get(url, params=params, include_auth_header=include_auth_header)
 
         new_df = df_fn(resp)
         df: DataFrame = pd.concat(objs=[df, new_df], ignore_index=True)  # type: ignore
 
     return df
```

### Comparing `spgci-0.0.8/spgci/auth.py` & `spgci-0.0.9/spgci/auth.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/config.py` & `spgci-0.0.9/spgci/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 base_url = "https://api.platts.com"
 #: Set `verify` to `False` when making HTTP calls
 verify_ssl = True
 #: Add proxy to HTTP calls
 proxies: Dict[str, str] = {}
 
 #: Version of the SPGCI Pkg
-version = "0.0.8"
+version = "0.0.9"
 
 #: time to sleep between api calls
 sleep_time = 0
 
 
 def set_credentials(un: str, pw: str, apikey: str) -> None:
     """
```

### Comparing `spgci-0.0.8/spgci/epf.py` & `spgci-0.0.9/spgci/epf.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/ewindow_md.py` & `spgci-0.0.9/spgci/ewindow_md.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/forward_curves.py` & `spgci-0.0.9/spgci/forward_curves.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/insights.py` & `spgci-0.0.9/spgci/insights.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/market_data.py` & `spgci-0.0.9/spgci/market_data.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/utilities.py` & `spgci-0.0.9/spgci/utilities.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/wos.py` & `spgci-0.0.9/spgci/wos.py`

 * *Files identical despite different names*

### Comparing `spgci-0.0.8/spgci/wrd.py` & `spgci-0.0.9/spgci/wrd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from typing import Union, Optional
 from requests import Response
 from pandas import Series, DataFrame, to_datetime, json_normalize  # type: ignore
 from spgci.api_client import get_data, Paginator
-from spgci.utilities import odata_list_to_filter
+from spgci.utilities import odata_list_to_filter, list_to_filter
 from urllib.parse import urlencode, quote, parse_qs, urlparse
 from datetime import date
 from enum import Enum
 
 
 class WorldRefineryData:
     """
@@ -102,14 +102,16 @@
         year_lte: Optional[int] = None,
         quarter: Optional[Union[int, list[int], "Series[int]"]] = None,
         refinery_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         owner: Optional[Union[str, list[str], "Series[str]"]] = None,
         capacity_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         capacity_status_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         process_unit: Optional[Union[str, list[str], "Series[str]"]] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        region: Optional[Union[str, list[str], "Series[str]"]] = None,
         filter_exp: Optional[str] = None,
         skip: int = 0,
         page_size: int = 1000,
         paginate: bool = False,
         raw: bool = False,
     ) -> Union[Response, DataFrame]:
         """
@@ -135,14 +137,18 @@
             filter by Owner/Name, by default None
         capacity_id : Optional[Union[int, list[int], Series[int]]], optional
             filter by capacityId, by default None
         capacity_status_id : Optional[Union[int, list[int], Series[int]]], optional
             filter by capacityStatusId, by default None
         process_unit : Optional[Union[str, list[str], Series[str]]], optional
             filter by ProcessUnit/Name, by default None
+        country : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Country/Name, by default None
+        region : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Region/Name, by default None
         filter_exp : Optional[str], optional
             pass-thru ``$filter`` query param to use a handcrafted filter expression, by default None
         skip : int, optional
             pass-thru ``$skip`` query param to skip a certain number of records, by default 0
         page_size : int, optional
             pass-thru ``pageSize`` query param to request a particular page size, by default 1000
         paginate : bool, optional
@@ -178,14 +184,16 @@
         filter_params.append(odata_list_to_filter("RefineryId", refinery_id))
         filter_params.append(odata_list_to_filter("Owner/Name", owner))
         filter_params.append(odata_list_to_filter("CapacityId", capacity_id))
         filter_params.append(
             odata_list_to_filter("CapacityStatusId", capacity_status_id)
         )
         filter_params.append(odata_list_to_filter("ProcessUnit/Name", process_unit))
+        filter_params.append(odata_list_to_filter("Refinery/Country/Name", country))
+        filter_params.append(odata_list_to_filter("Refinery/Region/Name", region))
 
         if year_gt:
             filter_params.append(f"year gt {year_gt}")
         if year_gte:
             filter_params.append(f"year ge {year_gte}")
         if year_lt:
             filter_params.append(f"year lt {year_lt}")
@@ -231,14 +239,16 @@
         year_lt: Optional[int] = None,
         year_lte: Optional[int] = None,
         quarter: Optional[Union[int, list[int], "Series[int]"]] = None,
         refinery_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         owner: Optional[Union[str, list[str], "Series[int]"]] = None,
         capacity_status_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         process_unit: Optional[Union[str, list[str], "Series[str]"]] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        region: Optional[Union[str, list[str], "Series[str]"]] = None,
         filter_exp: Optional[str] = None,
         skip: int = 0,
         page_size: int = 1000,
         paginate: bool = False,
         raw: bool = False,
     ) -> Union[Response, DataFrame]:
         """
@@ -262,14 +272,18 @@
             filter by refineryId, by default None
         owner : Optional[Union[str, list[str], Series[str]]], optional
             filter by Owner/Name, by default None
         capacity_status_id : Optional[Union[int, list[int], Series[int]]], optional
             filter by CapacityStatusId, by default None
         process_unit : Optional[Union[str, list[str], Series[str]]], optional
             filter by ProcessUnit/Name, by default None
+        country : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Country/Name, by default None
+        region : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Region/Name, by default None
         filter_exp : Optional[str], optional
             pass-thru ``$filter`` query param to use a handcrafted filter expression, by default None
         skip : int, optional
             pass-thru ``$skip`` query param to skip a certain number of records, by default 0
         page_size : int, optional
             pass-thru ``pageSize`` query param to request a particular page size, by default 1000
         paginate : bool, optional
@@ -304,14 +318,16 @@
         filter_params.append(odata_list_to_filter("Quarter", quarter))
         filter_params.append(odata_list_to_filter("RefineryId", refinery_id))
         filter_params.append(odata_list_to_filter("Owner/Name", owner))
         filter_params.append(
             odata_list_to_filter("CapacityStatusId", capacity_status_id)
         )
         filter_params.append(odata_list_to_filter("ProcessUnit/Name", process_unit))
+        filter_params.append(odata_list_to_filter("Refinery/Country/Name", country))
+        filter_params.append(odata_list_to_filter("Refinery/Region/Name", region))
 
         if year_gt:
             filter_params.append(f"year gt {year_gt}")
         if year_gte:
             filter_params.append(f"year ge {year_gte}")
         if year_lt:
             filter_params.append(f"year lt {year_lt}")
@@ -357,14 +373,16 @@
         year_lt: Optional[int] = None,
         year_lte: Optional[int] = None,
         quarter: Optional[Union[int, list[int], "Series[int]"]] = None,
         refinery_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         owner: Optional[Union[str, list[str], "Series[str]"]] = None,
         capacity_status_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         process_unit: Optional[Union[str, list[str], "Series[str]"]] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        region: Optional[Union[str, list[str], "Series[str]"]] = None,
         filter_exp: Optional[str] = None,
         skip: int = 0,
         page_size: int = 1000,
         paginate: bool = False,
         raw: bool = False,
     ) -> Union[Response, DataFrame]:
         """
@@ -388,14 +406,18 @@
             filter by refineryId, by default None
         owner : Optional[Union[str, list[str], Series[str]]], optional
             filter by Owner/Name, by default None
         capacity_status_id : Optional[Union[int, list[int], Series[int]]], optional
             filter by CapacityStatusId, by default None
         process_unit : Optional[Union[str, list[str], Series[str]]], optional
             filter by ProcessUnit/Name, by default None
+        country : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Country/Name, by default None
+        region : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Region/Name, by default None
         filter_exp : Optional[str], optional
             pass-thru ``$filter`` query param to use a handcrafted filter expression, by default None
         skip : int, optional
             pass-thru ``$skip`` query param to skip a certain number of records, by default 0
         page_size : int, optional
             pass-thru ``pageSize`` query param to request a particular page size, by default 1000
         paginate : bool, optional
@@ -430,14 +452,16 @@
         filter_params.append(odata_list_to_filter("Quarter", quarter))
         filter_params.append(odata_list_to_filter("RefineryId", refinery_id))
         filter_params.append(odata_list_to_filter("Owner/Name", owner))
         filter_params.append(
             odata_list_to_filter("CapacityStatusId", capacity_status_id)
         )
         filter_params.append(odata_list_to_filter("ProcessUnit/Name", process_unit))
+        filter_params.append(odata_list_to_filter("Refinery/Country/Name", country))
+        filter_params.append(odata_list_to_filter("Refinery/Region/Name", region))
 
         if year_gt:
             filter_params.append(f"year gt {year_gt}")
         if year_gte:
             filter_params.append(f"year ge {year_gte}")
         if year_lt:
             filter_params.append(f"year lt {year_lt}")
@@ -470,14 +494,215 @@
             # params=params,
             paginate=paginate,
             raw=raw,
             df_fn=self._to_df,
             paginate_fn=self._paginate,
         )
 
+    @staticmethod
+    def _outage_alert_pg_fn(resp: Response) -> Paginator:
+        j = resp.json()
+
+        count: int = j["metadata"]["count"]
+        page_size: int = j["metadata"]["pageSize"]
+
+        if not page_size:
+            return Paginator(False, "page", 0)
+
+        remainder = count % int(page_size)
+        quotient = count // int(page_size)
+        total_pages = quotient + (1 if remainder > 0 else 0)
+
+        if total_pages <= 1:
+            return Paginator(False, "page", total_pages)
+
+        return Paginator(True, "page", total_pages)
+
+    @staticmethod
+    def _outage_alerts_to_df(resp: Response) -> DataFrame:
+        j = resp.json()
+
+        df = json_normalize(
+            j["results"],
+            meta=[
+                "outageId",
+                "refineryId",
+                "operatorname",
+                "countryName",
+                "cityName",
+                "latitude",
+                "longitude",
+                "createdDate",
+            ],
+            record_path="alerts",
+        )
+        df["createdDate"] = to_datetime(df["createdDate"], utc=True)
+        df["modifiedDate"] = to_datetime(df["modifiedDate"], utc=True)
+        df["startDate"] = to_datetime(df["startDate"])
+        df["endDate"] = to_datetime(df["endDate"])
+        return df
+
+    def get_outage_alerts(
+        self,
+        *,
+        outage_id: Optional[Union[int, list[int], "Series[int]"]] = None,
+        created_date: Optional[Union[date, list[date], "Series[date]"]] = None,
+        created_date_gt: Optional[date] = None,
+        created_date_gte: Optional[date] = None,
+        created_date_lt: Optional[date] = None,
+        created_date_lte: Optional[date] = None,
+        refinery_id: Optional[Union[int, list[int], "Series[int]"]] = None,
+        operator: Optional[Union[str, list[str], "Series[str]"]] = None,
+        planning_status: Optional[Union[str, list[str], "Series[str]"]] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        process_unit: Optional[Union[str, list[str], "Series[str]"]] = None,
+        outage_vol: Optional[Union[float, list[float], "Series[float]"]] = None,
+        outage_vol_gt: Optional[float] = None,
+        outage_vol_gte: Optional[float] = None,
+        outage_vol_lt: Optional[float] = None,
+        outage_vol_lte: Optional[float] = None,
+        # modified_date: Optional[Union[date, list[date], "Series[date]"]] = None,
+        # modified_date_gt: Optional[date] = None,
+        # modified_date_gte: Optional[date] = None,
+        # modified_date_lt: Optional[date] = None,
+        # modified_date_lte: Optional[date] = None,
+        filter_exp: Optional[str] = None,
+        page: int = 1,
+        page_size: int = 1000,
+        paginate: bool = False,
+        raw: bool = False,
+    ) -> Union[Response, DataFrame]:
+        """_summary_
+
+        Parameters
+        ----------
+        outage_id : Optional[Union[int, list[int], &quot;Series[int]&quot;]], optional
+            filter by outageId, by default None
+        created_date : Optional[Union[date, list[date], &quot;Series[date]&quot;]], optional
+            _description_, by default None
+        created_date_gt : Optional[date], optional
+            _description_, by default None
+        created_date_gte : Optional[date], optional
+            _description_, by default None
+        created_date_lt : Optional[date], optional
+            _description_, by default None
+        created_date_lte : Optional[date], optional
+            _description_, by default None
+        refinery_id : Optional[Union[int, list[int], &quot;Series[int]&quot;]], optional
+            filter by refineryId, by default None
+        operator : Optional[Union[str, list[str], &quot;Series[str]&quot;]], optional
+            filter by operatorname, by default None
+        planning_status : Optional[Union[str, list[str], &quot;Series[str]&quot;]], optional
+            filter by planningStatus, by default None
+        country : Optional[Union[str, list[str], &quot;Series[str]&quot;]], optional
+            filter by countryName, by default None
+        process_unit : Optional[Union[str, list[str], &quot;Series[str]&quot;]], optional
+            filter by processUnitName, by default None
+        outage_vol : Optional[Union[float, list[float], Series[float]]], optional
+            filter by ``OutageVol_MBD = x`` , by default None
+        outage_vol_gt : Optional[float], optional
+            filter by ``OutageVol_MBD > x`` , by default None
+        outage_vol_gte : Optional[float], optional
+            filter by ``OutageVol_MBD >= x`` , by default None
+        outage_vol_lt : Optional[float], optional
+            filter by ``OutageVol_MBD < x`` , by default None
+        outage_vol_lte : Optional[float], optional
+            filter by ``OutageVol_MBD <= x`` , by default None
+        filter_exp : Optional[str], optional
+            pass-thru ``filter`` query param to use a handcrafted filter expression, by default None
+        page : int, optional
+            pass-thru ``page`` query param to skip a certain number of records, by default 1
+        page_size : int, optional
+            pass-thru ``pageSize`` query param to request a particular page size, by default 1000
+        paginate : bool, optional
+            whether to auto-paginate the response, by default False
+        raw : bool, optional
+            return a ``requests.Response`` instead of a ``DataFrame, by default False
+
+        Returns
+        -------
+        Union[pd.DataFrame, Response]
+            DataFrame
+              DataFrame of the ``response.json()``
+            Response
+              Raw ``requests.Response`` object
+        Examples
+        --------
+        **Simple**
+        >>> WorldRefineryData().get_outage_alerts(refineryId=245)
+
+        **Using Lists**
+        >>> WorldRefineryData().get_outage_alerts(process_unit=["Coker", "CDU"])
+        """
+        endpoint = "outage-alerts"
+
+        filter_params: list[str] = []
+
+        filter_params.append(list_to_filter("outageId", outage_id))
+        filter_params.append(list_to_filter("refineryId", refinery_id))
+        filter_params.append(list_to_filter("operatorname", operator))
+        filter_params.append(list_to_filter("countryName", country))
+        filter_params.append(list_to_filter("planningStatus", planning_status))
+        filter_params.append(list_to_filter("processUnitName", process_unit))
+        filter_params.append(list_to_filter("outageVol_MBD", outage_vol))
+        # filter_params.append(list_to_filter("modifiedDate", modified_date))
+        filter_params.append(list_to_filter("createdDate", created_date))
+
+        if created_date_gt:
+            filter_params.append(f'createdDate > "{created_date_gt}"')
+        if created_date_gte:
+            filter_params.append(f'createdDate >= "{created_date_gte}"')
+        if created_date_lt:
+            filter_params.append(f'createdDate < "{created_date_lt}"')
+        if created_date_lte:
+            filter_params.append(f'createdDate <= "{created_date_lte}"')
+
+        # if modified_date_gt:
+        #     filter_params.append(f'modifiedDate > "{modified_date_gt}"')
+        # if modified_date_gte:
+        #     filter_params.append(f'modifiedDate >= "{modified_date_gte}"')
+        # if modified_date_lt:
+        #     filter_params.append(f'modifiedDate < "{modified_date_lt}"')
+        # if modified_date_lte:
+        #     filter_params.append(f'modifiedDate <= "{modified_date_lte}"')
+
+        if outage_vol_gt:
+            filter_params.append(f"OutageVol_MBD > {outage_vol_gt}")
+        if outage_vol_gte:
+            filter_params.append(f"OutageVol_MBD >= {outage_vol_gte}")
+        if outage_vol_lt:
+            filter_params.append(f"OutageVol_MBD < {outage_vol_lt}")
+        if outage_vol_lte:
+            filter_params.append(f"OutageVol_MBD <= {outage_vol_lte}")
+
+        filter_params = [fp for fp in filter_params if fp != ""]
+
+        if filter_exp is None:
+            filter_exp = " AND ".join(filter_params)
+        else:
+            filter_exp += " AND " + " AND ".join(filter_params)
+
+        params: dict[str, Union[str, int]] = {
+            "page": page,
+            "pageSize": page_size,
+        }
+
+        if filter_exp:
+            params["filter"] = filter_exp
+
+        return get_data(
+            path=f"refinery-data/v1/{endpoint}",
+            params=params,
+            paginate=paginate,
+            raw=raw,
+            df_fn=self._outage_alerts_to_df,
+            paginate_fn=self._outage_alert_pg_fn,
+            include_auth_header=False,
+        )
+
     def get_outages(
         self,
         *,
         year: Optional[Union[int, list[int], "Series[int]"]] = None,
         year_gt: Optional[int] = None,
         year_gte: Optional[int] = None,
         year_lt: Optional[int] = None,
@@ -494,14 +719,16 @@
         planning_status: Optional[Union[str, list[str], "Series[str]"]] = None,
         outage_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         outage_vol: Optional[Union[float, list[float], "Series[float]"]] = None,
         outage_vol_gt: Optional[float] = None,
         outage_vol_gte: Optional[float] = None,
         outage_vol_lt: Optional[float] = None,
         outage_vol_lte: Optional[float] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        region: Optional[Union[str, list[str], "Series[str]"]] = None,
         filter_exp: Optional[str] = None,
         skip: int = 0,
         page_size: int = 1000,
         paginate: bool = False,
         raw: bool = False,
     ) -> Union[Response, DataFrame]:
         """
@@ -547,14 +774,18 @@
             filter by ``OutageVol_MBD > x`` , by default None
         outage_vol_gte : Optional[float], optional
             filter by ``OutageVol_MBD >= x`` , by default None
         outage_vol_lt : Optional[float], optional
             filter by ``OutageVol_MBD < x`` , by default None
         outage_vol_lte : Optional[float], optional
             filter by ``OutageVol_MBD <= x`` , by default None
+        country : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Country/Name, by default None
+        region : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Region/Name, by default None
         filter_exp : Optional[str], optional
             pass-thru ``$filter`` query param to use a handcrafted filter expression, by default None
         skip : int, optional
             pass-thru ``$skip`` query param to skip a certain number of records, by default 0
         page_size : int, optional
             pass-thru ``pageSize`` query param to request a particular page size, by default 1000
         paginate : bool, optional
@@ -591,14 +822,16 @@
         filter_params.append(odata_list_to_filter("OutageVol_MBD", outage_vol))
         filter_params.append(odata_list_to_filter("Quarter", quarter))
         filter_params.append(odata_list_to_filter("RefineryId", refinery_id))
         filter_params.append(odata_list_to_filter("Owner/Name", owner))
         filter_params.append(odata_list_to_filter("ProcessUnit/Name", process_unit))
         filter_params.append(odata_list_to_filter("PlanningStatus", planning_status))
         filter_params.append(odata_list_to_filter("OutageId", outage_id))
+        filter_params.append(odata_list_to_filter("Refinery/Country/Name", country))
+        filter_params.append(odata_list_to_filter("Refinery/Region/Name", region))
 
         if year_gt:
             filter_params.append(f"year gt {year_gt}")
         if year_gte:
             filter_params.append(f"year ge {year_gte}")
         if year_lt:
             filter_params.append(f"year lt {year_lt}")
@@ -660,14 +893,16 @@
         year_gt: Optional[int] = None,
         year_gte: Optional[int] = None,
         year_lt: Optional[int] = None,
         year_lte: Optional[int] = None,
         quarter: Optional[Union[int, list[int], "Series[int]"]] = None,
         refinery_id: Optional[Union[int, list[int], "Series[int]"]] = None,
         owner: Optional[Union[str, list[str], "Series[str]"]] = None,
+        country: Optional[Union[str, list[str], "Series[str]"]] = None,
+        region: Optional[Union[str, list[str], "Series[str]"]] = None,
         filter_exp: Optional[str] = None,
         skip: int = 0,
         page_size: int = 1000,
         paginate: bool = False,
         raw: bool = False,
     ) -> Union[Response, DataFrame]:
         """_summary_
@@ -686,14 +921,18 @@
             filter by ``year <= x`` , by default None
         quarter : Optional[Union[int, list[int], Series[int]]], optional
             filter by quarter, by default None
         refinery_id : Optional[Union[int, list[int], Series[int]]], optional
             filter by refineryId, by default None
         owner : Optional[Union[str, list[str], Series[str]]], optional
             filter by Owner/Name, by default None
+        country : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Country/Name, by default None
+        region : Optional[Union[str, list[str], Series[str]]], optional
+            filter by Refinery/Region/Name, by default None
         filter_exp : Optional[str], optional
             pass-thru ``$filter`` query param to use a handcrafted filter expression, by default None
         skip : int, optional
             pass-thru ``$skip`` query param to skip a certain number of records, by default 0
         page_size : int, optional
             pass-thru ``pageSize`` query param to request a particular page size, by default 1000
         paginate : bool, optional
@@ -725,14 +964,16 @@
 
         filter_params: list[str] = []
 
         filter_params.append(odata_list_to_filter("Year", year))
         filter_params.append(odata_list_to_filter("Quarter", quarter))
         filter_params.append(odata_list_to_filter("RefineryId", refinery_id))
         filter_params.append(odata_list_to_filter("Owner/Name", owner))
+        filter_params.append(odata_list_to_filter("Refinery/Country/Name", country))
+        filter_params.append(odata_list_to_filter("Refinery/Region/Name", region))
 
         if year_gt:
             filter_params.append(f"year gt {year_gt}")
         if year_gte:
             filter_params.append(f"year ge {year_gte}")
         if year_lt:
             filter_params.append(f"year lt {year_lt}")
```

### Comparing `spgci-0.0.8/setup.py` & `spgci-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'requests>=2.28.2,<3.0.0',
  'retry>=0.9.2,<0.10.0',
  'tqdm>=4.64.1,<5.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spgci',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'SPGCI is an API Client for the S&P Commodity Insights REST API',
-    'long_description': '# SPGCI\n\nPython Client for the [S&P Global Commodity Insights API](https://developer.platts.com).\n\n## Installation\n\nRequires Python >= 3.8.10.\n\n```bash\npip install spgci\n```\n\n## Getting Started\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/achristie/images/blob/master/readme.ipynb)\n\n```python\n    import spgci as ci\n\n    ci.set_credentials(<username>, <password>, <appkey>)\n    mdd = ci.MarketData()\n\n    symbols = ["PCAAS00", "PCAAT00"]\n    mdd.get_assessments_by_symbol_current(symbol=symbols)\n```\n\n## ![SPGCI](https://raw.githubusercontent.com/achristie/images/master/getting_started.gif)\n\n---\n\nAlternatively, you can set your credentials via Environment Variables and _omit_ the `set_credentials` call:\n| Environment Variable | Description |\n| :------------------- | :----------------|\n| SPGCI_USERNAME | Your Username |\n| SPGCI_PASSWORD | Your Password |\n| SPGCI_APPKEY | Your AppKey |\n\n## Features\n\n- Automatically generates token prior to making request.\n- Returns data as a pandas DataFrame (set `raw=False` to get the raw `request.response` object).\n- Can auto-paginate response and concatenates into a single DataFrame (set `paginate=True` to enable).\n- Sets datatype for `date` and `datetime` fields in DataFrame.\n- Composes nicely with native python/pandas types. Arguments support `lists` and `pd.Series` which are automatically converted into filter expressions.\n\n## Datasets Supported\n\n### Market Data\n\n```python\nimport spgci as ci\n\nmdd = ci.MarketData()\n\nmdd.get_symbols(commodity="Crude oil")\n# DataFrame of symbols with commodity = "Crude oil"\n\nmdd.get_mdcs(subscribed_only=True)\n# DataFrame of all Market Data Categories you are subscribed to\n\nmdd.get_assessments_by_mdc_current(mdc="ET")\n# DataFrame of current assessments for all symbols in the Market Data Category "ET"\n```\n\n### Forward Curves\n\n```python\nimport spgci as ci\n\nfc = ci.ForwardCurves()\n\nfc.get_curves(\n    commodity=["Benzene", "Crude oil"],\n    derivative_maturity_frequency="Month"\n    )\n# DataFrame of all curves with commodity in ("Benzene", "Crude Oil") and have a Monthly frequency\n\nfc.get_assessments(curve_code=["CN003", "CN006"])\n# DataFrame of the latest assessments for all symbols in the curves ("CN003", "CN006")\n```\n\n### Energy Price Forecast\n\n```python\nimport spgci as ci\n\nepf = ci.EnergyPriceForecast()\n\nepf.get_prices_shortterm(symbol="PCAAS00", month=[10, 11, 12])\n# DataFrame of monthly forecasts for the symbol "PCAAS00" in the last 3 months of the year\n\nepf.get_prices_longterm(year=[2020, 2021], sector="Energy Transition", delivery_region="Europe")\n# DataFrame of the annual forecasts for the years in ("2020", "2021"), where the sector is "Energy Transition" and the delivery region is "Europe"\n```\n\n### EWindow Market Data\n\n```python\nimport spgci as ci\nfrom datetime import date\n\newmd = ci.EWindowMarketData()\n\newmd.get_markets()\n# DataFrame of Markets\n\nd = date(2023,2,13)\newmd.get_botes(market=["EU BFOE", "US MidWest"], order_time=d)\n# DataFrame of all BOTes in the markets ("EU BFOE", "US MidWest") on Feb 13, 2023\n\n```\n\n### World Oil Supply\n\n```python\nimport spgci as ci\n\nwos = ci.WorldOilSupply()\n\ncountries = wos.get_reference_data(type=wos.RefType.Countries)\n# DataFrame of all countries\n\nwos.get_ownership(country=countries[\'countryName\'][:3], year=2040)\n# DataFrame of Ownership for the first three countries from the countries endpoint and year "2040"\n\n```\n\n### World Refinery Database\n\n```python\nimport spgci as ci\n\nwrd = ci.WorldRefineryDatabase()\n\nwrd.get_yields(year=2020, owner="BP")\n# DataFrame of yields for the year "2020" where "BP" is the refinery owner.\n\n```\n\n### Insights\n\n```python\nimport spgci as ci\n\nni = ci.Insights()\n\nni.get_stories(q="Suez", content_type=ni.ContentType.MarketCommentary)\n# DataFrame of articles related to "Suez" where the content type is "Market Commentary"\n\nni.get_subscriber_notes(q="Naptha")\n# DataFrame of all subscriber notes related to "Naptha"\n\nni.get_heards(q="Steel", content_type=ni.HeardsContentType.Heard, geography=[\'Europe\', \'Middle East\'], strip_html=True)\n# DataFrame of all Heards related to "Steel" where the geography is in ("Europe", "Middle East") with HTML Tags removed from the headline and body.\n```\n\n## Disclaimer\n\nPlease note that by using this Alpha offering, you agree that you are participating in a prototype to develop these software development kits (“Alpha SDKs”) and that your participation and use of the Alpha SDKs is at your own risk. You will be liable for all activities by anyone using your application in connection with the Alpha SDKs.\n\nIf you are dissatisfied with the Alpha SDKs, your sole remedy is to stop using it, and S&P Global Commodity Insights (“SPGCI”) will not pay you any damages (direct, indirect, special, or consequential) in connection with your use of the Alpha SDKs. Commodity Insights SPGCI disclaims any and all representations and warranties, express or implied, including but not limited to any warranties of merchantability or fitness for a particular purpose or use as to the Alpha SDKs, and does not guarantee the adequacy, accuracy, timeliness or completeness of the Alpha SDKs or any component of them.\n',
+    'long_description': '# SPGCI\n\nPython Client for the [S&P Global Commodity Insights API](https://developer.platts.com).\n\n## Installation\n\nRequires Python >= 3.8.10.\n\n```bash\npip install spgci\n```\n\n## Getting Started\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/achristie/images/blob/master/readme.ipynb)\n\n```python\n    import spgci as ci\n\n    ci.set_credentials(<username>, <password>, <appkey>)\n    mdd = ci.MarketData()\n\n    symbols = ["PCAAS00", "PCAAT00"]\n    mdd.get_assessments_by_symbol_current(symbol=symbols)\n```\n\n## ![SPGCI](https://raw.githubusercontent.com/achristie/images/master/getting_started.gif)\n\n---\n\nAlternatively, you can set your credentials via Environment Variables and _omit_ the `set_credentials` call:\n| Environment Variable | Description |\n| :------------------- | :----------------|\n| SPGCI_USERNAME | Your Username |\n| SPGCI_PASSWORD | Your Password |\n| SPGCI_APPKEY | Your AppKey |\n\n## Features\n\n- Automatically generates token prior to making request.\n- Returns data as a pandas DataFrame (set `raw=False` to get the raw `request.response` object).\n- Can auto-paginate response and concatenates into a single DataFrame (set `paginate=True` to enable).\n- Sets datatype for `date` and `datetime` fields in DataFrame.\n- Composes nicely with native python/pandas types. Arguments support `lists` and `pd.Series` which are automatically converted into filter expressions.\n\n## Datasets Supported\n\n### Market Data\n\n```python\nimport spgci as ci\n\nmdd = ci.MarketData()\n\nmdd.get_symbols(commodity="Crude oil")\n# DataFrame of symbols with commodity = "Crude oil"\n\nmdd.get_mdcs(subscribed_only=True)\n# DataFrame of all Market Data Categories you are subscribed to\n\nmdd.get_assessments_by_mdc_current(mdc="ET")\n# DataFrame of current assessments for all symbols in the Market Data Category "ET"\n```\n\n### Forward Curves\n\n```python\nimport spgci as ci\n\nfc = ci.ForwardCurves()\n\nfc.get_curves(\n    commodity=["Benzene", "Crude oil"],\n    derivative_maturity_frequency="Month"\n    )\n# DataFrame of all curves with commodity in ("Benzene", "Crude Oil") and have a Monthly frequency\n\nfc.get_assessments(curve_code=["CN003", "CN006"])\n# DataFrame of the latest assessments for all symbols in the curves ("CN003", "CN006")\n```\n\n### Energy Price Forecast\n\n```python\nimport spgci as ci\n\nepf = ci.EnergyPriceForecast()\n\nepf.get_prices_shortterm(symbol="PCAAS00", month=[10, 11, 12])\n# DataFrame of monthly forecasts for the symbol "PCAAS00" in the last 3 months of the year\n\nepf.get_prices_longterm(year=[2020, 2021], sector="Energy Transition", delivery_region="Europe")\n# DataFrame of the annual forecasts for the years in ("2020", "2021"), where the sector is "Energy Transition" and the delivery region is "Europe"\n```\n\n### EWindow Market Data\n\n```python\nimport spgci as ci\nfrom datetime import date\n\newmd = ci.EWindowMarketData()\n\newmd.get_markets()\n# DataFrame of Markets\n\nd = date(2023,2,13)\newmd.get_botes(market=["EU BFOE", "US MidWest"], order_time=d)\n# DataFrame of all BOTes in the markets ("EU BFOE", "US MidWest") on Feb 13, 2023\n\n```\n\n### World Oil Supply\n\n```python\nimport spgci as ci\n\nwos = ci.WorldOilSupply()\n\ncountries = wos.get_reference_data(type=wos.RefType.Countries)\n# DataFrame of all countries\n\nwos.get_ownership(country=countries[\'countryName\'][:3], year=2040)\n# DataFrame of Ownership for the first three countries from the countries endpoint and year "2040"\n\n```\n\n### World Refinery Database\n\n```python\nimport spgci as ci\n\nwrd = ci.WorldRefineryDatabase()\n\nwrd.get_yields(year=2020, owner="BP")\n# DataFrame of yields for the year "2020" where "BP" is the refinery owner.\n\nref = wrd.get_reference_data(type=wrd.RefTypes.Refineries)\n# DataFrame of all refineries.\n\naz = ref[ref[\'Name\'].str.contains("Al-Zour")]\nwrd.get_runs(refinery_id=az["Id"])\n# DataFrame of runs for the refineries with "Al-Zour" in the name.\n\nwrd.get_outages(refineryId=245)\n# DataFrame of outages for refineryId 245\n\n```\n\n### Insights\n\n```python\nimport spgci as ci\n\nni = ci.Insights()\n\nni.get_stories(q="Suez", content_type=ni.ContentType.MarketCommentary)\n# DataFrame of articles related to "Suez" where the content type is "Market Commentary"\n\nni.get_subscriber_notes(q="Naptha")\n# DataFrame of all subscriber notes related to "Naptha"\n\nni.get_heards(q="Steel", content_type=ni.HeardsContentType.Heard, geography=[\'Europe\', \'Middle East\'], strip_html=True)\n# DataFrame of all Heards related to "Steel" where the geography is in ("Europe", "Middle East") with HTML Tags removed from the headline and body.\n```\n\n## Disclaimer\n\nPlease note that by using this Alpha offering, you agree that you are participating in a prototype to develop these software development kits (“Alpha SDKs”) and that your participation and use of the Alpha SDKs is at your own risk. You will be liable for all activities by anyone using your application in connection with the Alpha SDKs.\n\nIf you are dissatisfied with the Alpha SDKs, your sole remedy is to stop using it, and S&P Global Commodity Insights (“SPGCI”) will not pay you any damages (direct, indirect, special, or consequential) in connection with your use of the Alpha SDKs. Commodity Insights SPGCI disclaims any and all representations and warranties, express or implied, including but not limited to any warranties of merchantability or fitness for a particular purpose or use as to the Alpha SDKs, and does not guarantee the adequacy, accuracy, timeliness or completeness of the Alpha SDKs or any component of them.\n',
     'author': 'S&P Global Commodity Insights',
     'author_email': 'pl_api_support@spglobal.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `spgci-0.0.8/PKG-INFO` & `spgci-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spgci
-Version: 0.0.8
+Version: 0.0.9
 Summary: SPGCI is an API Client for the S&P Commodity Insights REST API
 License: MIT
 Author: S&P Global Commodity Insights
 Author-email: pl_api_support@spglobal.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -151,14 +151,24 @@
 import spgci as ci
 
 wrd = ci.WorldRefineryDatabase()
 
 wrd.get_yields(year=2020, owner="BP")
 # DataFrame of yields for the year "2020" where "BP" is the refinery owner.
 
+ref = wrd.get_reference_data(type=wrd.RefTypes.Refineries)
+# DataFrame of all refineries.
+
+az = ref[ref['Name'].str.contains("Al-Zour")]
+wrd.get_runs(refinery_id=az["Id"])
+# DataFrame of runs for the refineries with "Al-Zour" in the name.
+
+wrd.get_outages(refineryId=245)
+# DataFrame of outages for refineryId 245
+
 ```
 
 ### Insights
 
 ```python
 import spgci as ci
```

