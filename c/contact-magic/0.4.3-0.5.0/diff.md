# Comparing `tmp/contact_magic-0.4.3.tar.gz` & `tmp/contact_magic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.4.3.tar", max compression
+gzip compressed data, was "contact_magic-0.5.0.tar", max compression
```

## Comparing `contact_magic-0.4.3.tar` & `contact_magic-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.4.3/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.4.3/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.4.3/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.4.3/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.4.3/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.4.3/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.4.3/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-13 06:14:51.344787 contact_magic-0.4.3/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.4.3/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1638 2023-06-13 07:39:32.822031 contact_magic-0.4.3/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.4.3/contact_magic/logger.py
--rw-r--r--   0        0        0    12297 2023-06-11 23:14:52.374634 contact_magic-0.4.3/contact_magic/models.py
--rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.4.3/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.4.3/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.4.3/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.4.3/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.4.3/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.4.3/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.4.3/contact_magic/utils.py
--rw-r--r--   0        0        0     1903 2023-06-13 08:14:13.348239 contact_magic-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.0/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.0/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.0/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.0/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.5.0/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2336 2023-06-14 20:44:43.846650 contact_magic-0.5.0/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.5.0/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.0/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2499 2023-06-14 21:27:06.608482 contact_magic-0.5.0/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1678 2023-06-14 21:25:23.127407 contact_magic-0.5.0/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1638 2023-06-13 07:39:32.822031 contact_magic-0.5.0/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.0/contact_magic/logger.py
+-rw-r--r--   0        0        0    13609 2023-06-14 21:27:07.154508 contact_magic-0.5.0/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.0/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.0/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.5.0/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.0/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.0/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.5.0/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.0/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-06-14 22:00:28.797252 contact_magic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.0/PKG-INFO
```

### Comparing `contact_magic-0.4.3/README.md` & `contact_magic-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/asyncio.py` & `contact_magic-0.5.0/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/conf/settings.py` & `contact_magic-0.5.0/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/helpers.py` & `contact_magic-0.5.0/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.0/contact_magic/integrations/copyfactory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import logging
 
 import httpx
 
 from contact_magic.conf.settings import SETTINGS
-from contact_magic.utils import find_item
+from contact_magic.dict_utils import get_values_in_object_by_key
+from contact_magic.logger import logger
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 endpoint = "https://app.copyfactory.io/api/v2/generate/"
 
 
@@ -38,30 +39,36 @@
     try:
         session = httpx.AsyncClient(timeout=90)
         retries = 0
         while retries < max_retries:
             res = await session.request(
                 method="POST", url=endpoint, headers=headers, json=data
             )
+            # authorization error so can break
+            if res.status_code == 403:
+                logger.warning("copyfactory_error", message=res.text)
+                break
             if res.status_code == 429:
                 await asyncio.sleep(_get_rate_limit_sleep_time(res))
                 retries += 1
                 continue
 
             if res.status_code == 200:
                 response_data = res.json()["data"]
                 if response_data["status"] == "success":
                     return response_data
                 if response_data["status"] == "error":
                     required_variables = response_data["meta_data"]["sentence_premise"][
                         "required_variables"
                     ]
                     for req_var in required_variables:
-                        if item := find_item(variables, req_var):
-                            data["variables"][req_var] = str(item)
+                        if item := list(
+                            get_values_in_object_by_key(variables, req_var)
+                        ):
+                            data["variables"][req_var] = str(item[0])
                     if not data["variables"].get("company_organization_name"):
                         data["variables"]["company_organization_name"] = ""
 
             retries += 1
         return None
     except Exception:
         return None
```

### Comparing `contact_magic-0.4.3/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.0/contact_magic/integrations/sales_scrapers.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     try:
         session = httpx.AsyncClient(timeout=120)
         retries = 0
         while retries < max_retries:
             res = await session.request(
                 method="get", url=url, headers=headers, params=data
             )
+            # authorization error so can break
+            if res.status_code == 401:
+                logger.warning("sales_scraper_error", message=res.text)
+                break
             if res.status_code == 400:
                 logger.warning("proxy_error", message=res.text)
             if res.status_code == 200:
                 return res.json()
             if res.status_code == 422:
                 validation_errors = res.json().get("detail")
                 for error in validation_errors:
```

### Comparing `contact_magic-0.4.3/contact_magic/integrations/sheets.py` & `contact_magic-0.5.0/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/models.py` & `contact_magic-0.5.0/contact_magic/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 import numpy as np
 import pandas as pd
 from pydantic import AnyUrl, BaseModel, Field, validator
 
 from contact_magic.asyncio import do_bulk
 from contact_magic.conf.settings import SETTINGS
+from contact_magic.dict_utils import (
+    delete_key_in_object,
+    get_values_in_object_by_key,
+    replace_keys_in_object,
+    replace_values_in_object,
+)
 from contact_magic.integrations import (
     make_copyfactory_request,
     make_sales_scraper_request,
 )
 from contact_magic.logger import logger
-from contact_magic.utils import (
-    find_item,
-    get_id_from_url,
-    is_valid_premise_url,
-    replace_keys,
-    replace_values,
-)
+from contact_magic.utils import get_id_from_url, is_valid_premise_url
 
 
 class DataRow(BaseModel):
     """
     A class to hold a row of data and it's index number
     to sort by after. Converts set data to a dict.
     """
@@ -82,14 +82,16 @@
         "If any of the fields fail validation "
         "Copyfactory will not be called.",
         default={},
     )
 
     @validator("premise_url")
     def validate_premise_url(cls, url):
+        if not isinstance(url, str):
+            return url
         return f"{url}/" if not url.endswith("/") else url
 
     @validator("scraper_name")
     def validate_scraper_name(cls, value):
         if value is None:
             return value
         if not SETTINGS.ALLOWED_SCRAPER_NAMES:
@@ -108,42 +110,43 @@
     def fill_fallback(self, row: DataRow) -> str:
         """
         Fills in the template with row data.
         either returns the filled in template or an empty string.
         """
         list_pot_keys = re.findall(r"\{(.*?)\}", self.fallback_template)
         copy_of_template = self.fallback_template
-        filled_all = True
         for key in list_pot_keys:
-            value = find_item(row.data, key)
+            value = get_values_in_object_by_key(row.data, key)
             if not value:
-                filled_all = False
-                continue
-            copy_of_template = copy_of_template.replace("{" + key + "}", value)
-        return copy_of_template if filled_all else ""
+                return ""
+            copy_of_template = copy_of_template.replace("{" + key + "}", value[0])
+        return copy_of_template
 
     async def run_sales_scraper(self, row: DataRow, col_prefix: str, overwrite=False):
         """
         Runs the scraping and extends the row by adding
         the column name + scraper as a prefix to ensure uniqueness.
         """
         if not self.scraper_name:
             return row
         if not self.scraper_mapping and SETTINGS.SCRAPER_MAPPING:
             self.scraper_mapping = SETTINGS.SCRAPER_MAPPING
 
         data = (
-            replace_keys(row.data, self.scraper_mapping)
+            replace_keys_in_object(row.data, self.scraper_mapping)
             if self.scraper_mapping
             else row.data
         )
         if scrape := await make_sales_scraper_request(self.scraper_name, data=data):
             for key, value in scrape.items():
                 if key in row.data and not overwrite:
                     continue
+                # Remove output schema since don't want
+                # to pass schema values to Copyfactory
+                value = delete_key_in_object(value, "output_schema")
                 unique_key = f"{col_prefix}__{self.scraper_name}__{key}"
                 row.data[unique_key] = value
             return row
         return row
 
     async def run_copyfactory(
         self, row: DataRow, content_col_name: str, source_col_name: str
@@ -161,15 +164,15 @@
             self.copyfactory_mapping = SETTINGS.COPYFACTORY_MAPPING
 
         row, is_valid = self.run_processors(row)
         if not is_valid:
             return row, False
 
         data = (
-            replace_keys(row.data, self.copyfactory_mapping)
+            replace_keys_in_object(row.data, self.copyfactory_mapping)
             if self.copyfactory_mapping
             else row.data
         )
         if cf := await make_copyfactory_request(self.premise_id, variables=data):
             row.data[content_col_name] = cf["content"]
             source = row.data.get(
                 f"{content_col_name}__{self.scraper_name}__scraper_info", {}
@@ -185,39 +188,45 @@
 
         if not self.field_processors:
             return row, True
 
         from contact_magic.preprocessors import processors
 
         for key, processor in self.field_processors.items():
-            item = find_item(row.data, key)
-            if item is not None:
+            if item := get_values_in_object_by_key(row.data, key):
                 if validation_model := processors.get(
                     processor.get("type", None), None
                 ):
-                    value, is_value_valid = validation_model(
-                        processor=processor, value=item, scraper=self, row_data=row.data
-                    ).process()
-                    if is_value_valid is False:
+                    # If Pydantic fails validation/init just move on.
+                    try:
+                        value, is_value_valid = validation_model(
+                            processor=processor,
+                            value=item[0],
+                            wizard=self,
+                            row_data=row.data,
+                        ).process()
+                        row.data = replace_values_in_object(row.data, key, value)
+                    except Exception:
+                        is_value_valid = False
+                    if not is_value_valid:
                         return row, False
-                    row.data = replace_values(row.data, {key: value})
         return row, True
 
     async def execute(
         self, row: DataRow, content_col_name: str, source_col_name: str
     ) -> tuple[DataRow, bool]:
         """
         Executes the scraper and extends the DataRow as it moves along to
         allow for exploding the DF with more
         datapoints from the scraping + personalization.
         """
         if self.scraper_name == "FALLBACK" and self.fallback_template:
             row.data[content_col_name] = self.fill_fallback(row)
             row.data[source_col_name] = "-"
-            return row, row.data[content_col_name] is not None
+            return row, row.data[content_col_name] != ""
         row = await self.run_sales_scraper(row, col_prefix=content_col_name)
         row, success = await self.run_copyfactory(
             row, content_col_name, source_col_name
         )
         return row, success
 
     def __init__(self, **data: Any):
@@ -245,36 +254,41 @@
     def get_col_name_as_source(self) -> str:
         return f"source__{self.col_name}"
 
     async def build_datapoint(self, row: DataRow):
         for scraper in self.sentence_wizards:
             logger.info(
                 "processing_row",
-                row_number=row.index + 2,
+                row_number=row.index,
                 scraper_name=scraper.scraper_name,
+                premise_id=scraper.premise_id or get_id_from_url(scraper.premise_url),
                 column_name=self.col_name,
                 status="STARTING",
             )
             row, did_succeed = await scraper.execute(
                 row, self.col_name, self.get_col_name_as_source
             )
             if did_succeed:
                 logger.info(
                     "processing_row",
-                    row_number=row.index + 2,
+                    row_number=row.index,
                     scraper_name=scraper.scraper_name,
+                    premise_id=scraper.premise_id
+                    or get_id_from_url(scraper.premise_url),
                     column_name=self.col_name,
                     status="SUCCESS",
                 )
                 break
             else:
                 logger.info(
                     "processing_row",
-                    row_number=row.index + 2,
+                    row_number=row.index,
                     scraper_name=scraper.scraper_name,
+                    premise_id=scraper.premise_id
+                    or get_id_from_url(scraper.premise_url),
                     column_name=self.col_name,
                     status="FAILED",
                 )
         return row
 
 
 class PersonalizationSettings(BaseModel):
@@ -283,14 +297,25 @@
     """
 
     name: str = ""
     datapoints: list[DataPoint]
     uid: UUID = Field(default_factory=uuid4)
     created: datetime = Field(default_factory=datetime.utcnow)
 
+    @validator("datapoints")
+    def validate_datapoints(cls, datapoints):
+        seen_names = {}
+        for dp in datapoints:
+            if dp.col_name in seen_names:
+                seen_names[dp.col_name] += 1
+                dp.col_name = f"{dp.col_name}__{seen_names[dp.col_name]}"
+            else:
+                seen_names[dp.col_name] = 1
+        return datapoints
+
     @property
     def get_datapoint_column_names(self) -> list:
         """
         Returns a list of column names and a source field.
         """
         return [dp.col_name for dp in self.datapoints] + [
             dp.get_col_name_as_source for dp in self.datapoints
@@ -315,14 +340,16 @@
         the row from the dataframe to filter on.
         This function must resolve to a boolean and rows that are
         True are not processed.
         """
         df = self.extend_dataframe_with_settings_columns(df)
         untouched_rows = []
         jobs = []
+        # Set to 1 based index for logging
+        df.index = df.index + 1
         for i, row in df.iterrows():
             if exclude_filter_func and exclude_filter_func(row):
                 untouched_rows.append(DataRow(data=row, index=i))
                 continue
             jobs.append(DataRow(data=row, index=i))
         return pd.DataFrame(
             data=[
```

### Comparing `contact_magic-0.4.3/contact_magic/preprocessors.py` & `contact_magic-0.5.0/contact_magic/preprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class BaseProcessor(BaseModel):
     """
     Base validator to inherit from. Define the 'validate' method to return a boolean.
     """
 
     value: Any = None
     processor: dict
-    scraper: SentenceWizard
+    wizard: SentenceWizard
     row_data: dict
 
     _is_valid: bool = True
 
     def process(self) -> tuple[Any, bool]:
         if not self._is_valid:
             return self.value, self._is_valid
```

### Comparing `contact_magic-0.4.3/contact_magic/scripts/agency.py` & `contact_magic-0.5.0/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.0/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.0/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.3/pyproject.toml` & `contact_magic-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.4.3"
+version = "0.5.0"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
@@ -50,11 +50,12 @@
 contact-magic = "contact_magic.scripts.agency:app"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
+mkdocs-material = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contact_magic-0.4.3/PKG-INFO` & `contact_magic-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.4.3
+Version: 0.5.0
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

