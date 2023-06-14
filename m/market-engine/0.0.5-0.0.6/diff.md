# Comparing `tmp/market-engine-0.0.5.tar.gz` & `tmp/market-engine-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.5.tar", last modified: Fri May 26 22:45:43 2023, max compression
+gzip compressed data, was "market-engine-0.0.6.tar", last modified: Wed Jun 14 23:36:07 2023, max compression
```

## Comparing `market-engine-0.0.5.tar` & `market-engine-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.736065 market-engine-0.0.5/
--rw-rw-rw-   0        0        0      216 2023-05-26 22:45:43.736065 market-engine-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.730561 market-engine-0.0.5/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.5/market_engine/__init__.py
--rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.5/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.734561 market-engine-0.0.5/market_engine/modules/
--rw-rw-rw-   0        0        0    14007 2023-05-26 19:26:37.000000 market-engine-0.0.5/market_engine/modules/MarketAPI.py
--rw-rw-rw-   0        0        0     6989 2023-05-26 19:26:52.000000 market-engine-0.0.5/market_engine/modules/MarketDB.py
--rw-rw-rw-   0        0        0    15043 2023-05-26 22:45:19.000000 market-engine-0.0.5/market_engine/modules/MarketData.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.5/market_engine/modules/__init__.py
--rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.5/market_engine/modules/categories.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:45:43.733561 market-engine-0.0.5/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 22:45:43.000000 market-engine-0.0.5/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 22:45:43.736065 market-engine-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-26 22:45:35.000000 market-engine-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:36:07.534800 market-engine-0.0.6/
+-rw-rw-rw-   0        0        0      216 2023-06-14 23:36:07.534800 market-engine-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 23:36:07.530800 market-engine-0.0.6/market_engine/
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.6/market_engine/__init__.py
+-rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.6/market_engine/common.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:36:07.533801 market-engine-0.0.6/market_engine/modules/
+-rw-rw-rw-   0        0        0    13868 2023-06-13 16:05:31.000000 market-engine-0.0.6/market_engine/modules/MarketAPI.py
+-rw-rw-rw-   0        0        0     7054 2023-06-14 23:34:47.000000 market-engine-0.0.6/market_engine/modules/MarketDB.py
+-rw-rw-rw-   0        0        0    15043 2023-05-26 22:45:19.000000 market-engine-0.0.6/market_engine/modules/MarketData.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.6/market_engine/modules/__init__.py
+-rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.6/market_engine/modules/categories.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:36:07.531801 market-engine-0.0.6/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-06-14 23:36:07.000000 market-engine-0.0.6/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-14 23:36:07.000000 market-engine-0.0.6/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:36:07.000000 market-engine-0.0.6/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-14 23:36:07.000000 market-engine-0.0.6/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-14 23:36:07.000000 market-engine-0.0.6/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:36:07.534800 market-engine-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-06-14 23:35:38.000000 market-engine-0.0.6/setup.py
```

### Comparing `market-engine-0.0.5/market_engine/common.py` & `market-engine-0.0.6/market_engine/common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.5/market_engine/modules/MarketAPI.py` & `market-engine-0.0.6/market_engine/modules/MarketAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from json import JSONDecodeError
 from typing import Dict, Any, List, Tuple
 
 from aiohttp import ClientResponseError, ServerDisconnectedError
 from aiolimiter import AsyncLimiter
 from bs4 import BeautifulSoup
 
-import ..common
+from ..common import logger, session_manager, cache_manager
 
 MANIFEST_URL = "https://content.warframe.com/PublicExport/index_en.txt.lzma"
 API_BASE_URL = "https://api.warframe.market/v1"
 ITEMS_ENDPOINT = "/items"
 STATISTICS_ENDPOINT = "/items/{}/statistics"
 
 rate_limiter = AsyncLimiter(3, 1)  # 3 requests per 1 second
 
 
 def get_cached_data(cache, url: str) -> Any | None:
     data = cache.get(url)
     if data is not None:
-        common.logger.debug(f"Using cached data for {url}")
+        logger.debug(f"Using cached data for {url}")
         return data
 
     return None
 
 
 async def fetch_api_data(cache, session, url: str) -> Dict[str, Any]:
     # Check if the data is in the cache
@@ -44,15 +44,15 @@
     sleep_time = 0
     while True:
         # Make the API request
         try:
             async with session.get(url) as response:
                 response.raise_for_status()
                 data = await response.json()
-                common.logger.debug(f"Fetched data for {url}")
+                logger.debug(f"Fetched data for {url}")
 
                 # Store the data in the cache with a 24-hour expiration
                 cache.set(url, json.dumps(data), ex=24 * 60 * 60)
 
                 return data
         except ClientResponseError:
             sleep_time += 1
@@ -82,20 +82,20 @@
 async def fix(cache, session):
     data = get_cached_data(cache, MANIFEST_URL)
     if data is None:
         try:
             async with session.get(MANIFEST_URL) as response:
                 response.raise_for_status()
                 data = await response.content.read()
-                common.logger.debug(f"Fetched data for {MANIFEST_URL}")
+                logger.debug(f"Fetched data for {MANIFEST_URL}")
 
                 # Store the data in the cache with a 24-hour expiration
                 cache.set(MANIFEST_URL, data, ex=24 * 60 * 60)
         except ClientResponseError:
-            common.logger.error("Failed to fetch manifest index")
+            logger.error("Failed to fetch manifest index")
             return
 
     byt = bytes(data)
     length = len(data)
     stay = True
     while stay:
         stay = False
@@ -111,38 +111,38 @@
 def save_manifest(manifest_dict):
     for item in manifest_dict:
         with open(f"data/manifest_{item}.json", "w") as f:
             json.dump(manifest_dict, f)
 
 
 async def get_manifest():
-    async with common.session_manager() as session, common.cache_manager() as cache:
+    async with session_manager() as session, cache_manager() as cache:
         wf_manifest = await fix(cache, session)
         wf_manifest = wf_manifest.split('\r\n')
         manifest_dict = {}
         for item in wf_manifest:
             try:
                 url = f"http://content.warframe.com/PublicExport/Manifest/{item}"
                 data = get_cached_data(cache, url)
                 if data is None:
                     async with session.get(url) as response:
                         response.raise_for_status()
                         data = await response.text()
-                        common.logger.debug(f"Fetched data for {url}")
+                        logger.debug(f"Fetched data for {url}")
 
                         # Store the data in the cache with a 24-hour expiration
                         cache.set(url, data, ex=24 * 60 * 60)
 
                 json_file = json.loads(data, strict=False)
 
                 manifest_dict[item.split("_en")[0]] = json_file
             except JSONDecodeError:
                 pass
             except ClientResponseError:
-                common.logger.error(f"Failed to fetch manifest {item}")
+                logger.error(f"Failed to fetch manifest {item}")
 
         save_manifest(manifest_dict)
 
         return manifest_dict
 
 
 async def get_price_history_dates(cache, session) -> set:
@@ -151,15 +151,15 @@
     # Check if the data is in the cache
     data = get_cached_data(cache, url)
     if data is None:
         # Make the API request
         async with session.get(url) as response:
             response.raise_for_status()
             data = await response.text()
-            common.logger.debug(f"Fetched data for {url}")
+            logger.debug(f"Fetched data for {url}")
 
             # Store the data in the cache with a 24-hour expiration
             cache.set(url, data, ex=24 * 60 * 60)
 
     soup = BeautifulSoup(data, 'html.parser')
 
     urls = set()
@@ -192,27 +192,27 @@
     async def fetch_data(date):
         url = f"https://relics.run/history/{date}"
 
         try:
             async with session.get(url) as response:
                 response.raise_for_status()
                 data = await response.json()
-                common.logger.debug(f"Fetched data for {url}")
+                logger.debug(f"Fetched data for {url}")
         except ClientResponseError:
-            common.logger.error(f"Failed to fetch data for {date}")
+            logger.error(f"Failed to fetch data for {date}")
             return
         except ServerDisconnectedError:
-            common.logger.error(f"Failed to fetch data for {date}")
+            logger.error(f"Failed to fetch data for {date}")
             return
 
         with open(os.path.join('output', date), 'w') as f:
             json.dump(data, f)
 
-    async with common.cache_manager() as cache:
-        async with common.session_manager() as session:
+    async with cache_manager() as cache:
+        async with session_manager() as session:
             date_list = await get_dates_to_fetch(cache, session)
 
             await asyncio.gather(*[fetch_data(date) for date in date_list])
 
 
 async def fetch_set_data(url_name, cache, session):
     url = f"{API_BASE_URL}/items/{url_name}"
@@ -225,15 +225,15 @@
     for item in items:
         item_ids[item['item_name']] = item['id']
 
     for file in os.listdir('output'):
         if not file.endswith('.json'):
             continue
 
-        common.logger.info(f"Processing {file}")
+        logger.info(f"Processing {file}")
         with open(os.path.join('output', file), 'r') as f:
             history_file = json.load(f)
 
         for item in history_file:
             for order_type in history_file[item]:
                 if item not in translation_dict:
                     fixed_item = item
@@ -259,16 +259,16 @@
     with open('data/item_info.json', 'w') as f:
         json.dump(item_info, f)
 
 
 async def fetch_and_save_statistics(items, item_ids) -> tuple[
     defaultdict[Any, defaultdict[Any, list] | defaultdict[str, list]] | defaultdict[
         str, defaultdict[Any, list] | defaultdict[str, list]], dict[Any, Any]]:
-    async with common.cache_manager() as cache:
-        async with common.session_manager() as session:
+    async with cache_manager() as cache:
+        async with session_manager() as session:
             with open('data/translation_dict.json', 'r') as f:
                 translation_dict = json.load(f)
 
             price_history_dict, item_info = await process_price_history(cache, session, items, translation_dict,
                                                                         item_ids)
             save_price_history(price_history_dict)
             save_item_info(item_info)
@@ -305,15 +305,15 @@
             str, defaultdict[Any, list] | defaultdict[str, list]], dict[Any, Any]]:
     price_history_dict = defaultdict(lambda: defaultdict(list))
     item_info = {}
 
     async def fetch_and_process_item_statistics(item):
         api_data = await fetch_item_statistics(cache, session, item["url_name"])
         price_history = api_data["payload"]
-        common.logger.info(f"Processing {item['item_name']}")
+        logger.info(f"Processing {item['item_name']}")
         item_info[item['id']] = parse_item_info(api_data["include"]["item"])
 
         for ph in [price_history["statistics_closed"]["90days"], price_history["statistics_live"]["90days"]]:
             for price_history_day in ph:
                 date = price_history_day["datetime"].split("T")[0]
                 item_name = item["item_name"]
                 if item_name in translation_dict:
@@ -328,32 +328,32 @@
 
     await asyncio.gather(*[fetch_and_process_item_statistics(item) for item in items])
 
     return price_history_dict, item_info
 
 
 async def fetch_all_items() -> List[Dict[str, Any]]:
-    async with common.session_manager() as session, common.cache_manager() as cache:
+    async with session_manager() as session, cache_manager() as cache:
         url = f"{API_BASE_URL}{ITEMS_ENDPOINT}"
         return (await fetch_api_data(cache, session, url))["payload"]["items"]
 
 
 async def fetch_and_save_items_and_ids():
     items = await fetch_all_items()
-    async with common.cache_manager() as cache:
+    async with cache_manager() as cache:
         item_ids = get_cached_data(cache, 'data/item_ids.json')
         if item_ids is None:
-            common.logger.info("Building Item IDs")
+            logger.info("Building Item IDs")
             with open('data/translation_dict.json', 'r') as f:
                 translation_dict = json.load(f)
 
             item_ids = build_item_ids(items, translation_dict)
             cache.set('data/item_ids.json', json.dumps(item_ids), ex=60 * 60 * 24 * 7)
         else:
-            common.logger.info("Loaded Item IDs from cache")
+            logger.info("Loaded Item IDs from cache")
             item_ids = json.loads(item_ids)
 
     with open('data/item_ids.json', 'w') as f:
         json.dump(item_ids, f)
 
     with open('data/items.json', 'w') as f:
         json.dump(items, f)
@@ -363,30 +363,30 @@
 
 async def fetch_item_statistics(cache, session, item_url_name: str) -> Dict[str, Any]:
     url = f"{API_BASE_URL}{STATISTICS_ENDPOINT.format(item_url_name)}?include=item"
     return await fetch_api_data(cache, session, url)
 
 
 def save_price_history(price_history_dict: Dict[str, Dict[str, List[Dict[str, Any]]]],
-                       directory: str = common.OUTPUT_DIRECTORY):
+                       directory: str = "output"):
     for day, history in price_history_dict.items():
         filename = f"{directory}/price_history_{day}.json"
         if not os.path.isfile(filename):
             with open(filename, "w") as fp:
                 json.dump(history, fp)
 
 
 async def fetch_premade_item_data():
     urls = [
         "https://relics.run/market_data/items.json",
         "https://relics.run/market_data/item_ids.json",
         "https://relics.run/market_data/item_info.json"
     ]
 
-    async with common.session_manager() as session:
+    async with session_manager() as session:
         # Create a list of tasks for each URL
         tasks = [session.get(url) for url in urls]
 
         # Wait for all tasks to complete and store the responses in a list
         responses = await asyncio.gather(*tasks)
 
         # Convert each response to JSON data and store them in a list
```

### Comparing `market-engine-0.0.5/market_engine/modules/MarketDB.py` & `market-engine-0.0.6/market_engine/modules/MarketDB.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,26 @@
 import os
 from datetime import datetime
 from typing import Dict, List, Any
 
 import pymysql
 from pytz import timezone
 
-import ..common
-from common import managed_transaction
-from modules import categories
+from ..common import managed_transaction
+import categories
 
 
-def connect_to_database():
-    return pymysql.connect(user='market', password='38NwWvkvZXiWV3', host='localhost', database='market')
+def connect_to_database(user, password, host, database):
+    return pymysql.connect(user=user, password=password, host=host, database=database)
 
 
-connection = connect_to_database()
-
-
-def save_items(items, item_ids, item_info):
+def save_items(connection, items, item_ids, item_info):
     if items is None or item_ids is None:
         return
 
-    type(item_info)
-
     data_list = [(item['id'], item['item_name'], item['url_name'], item['thumb'], item_info[item['id']]['mod_max_rank'])
                  for item in items]
 
     new_item_ids = {}
     for item, item_id in item_ids.items():
         if item_id not in [x['id'] for x in items]:
             new_item_ids[item] = item_id
@@ -40,70 +34,70 @@
 
     with connection.cursor() as cursor:
         cursor.executemany(insert_query, data_list)
 
     connection.commit()
 
 
-def get_sub_type_data():
+def get_sub_type_data(connection):
     with connection.cursor() as cursor:
         cursor.execute("""SELECT i.item_name, GROUP_CONCAT(DISTINCT s.sub_type) as subtypes
                           FROM item_subtypes s
                           JOIN items i ON s.item_id = i.id
                           GROUP BY i.item_name""")
         sub_type_data = cursor.fetchall()
 
         return {row[0]: row[1].split(',') for row in sub_type_data}
 
 
-def get_mod_rank_data():
+def get_mod_rank_data(connection):
     with connection.cursor() as cursor:
         cursor.execute("""SELECT i.item_name, GROUP_CONCAT(DISTINCT s.mod_rank) as modrank
                           FROM item_mod_ranks s
                           JOIN items i ON s.item_id = i.id
                           GROUP BY i.item_name""")
         sub_type_data = cursor.fetchall()
 
         return {row[0]: row[1].split(',') for row in sub_type_data}
 
 
-def get_item_data():
+def get_item_data(connection):
     with connection.cursor() as cursor:
         cursor.execute("""SELECT item_name, id FROM items""")
 
     return dict(cursor.fetchall())
 
 
-def build_and_save_category_info(manifest_dict):
+def build_and_save_category_info(connection, manifest_dict):
     wf_parser = categories.build_parser(manifest_dict)
     item_categories = categories.get_wfm_item_categorized(get_item_data(), manifest_dict, wf_parser)
 
     query = """UPDATE items SET item_type = %s WHERE id = %s"""
 
     with connection.cursor() as cursor:
         for item_type in item_categories:
             cursor.executemany(query, [(item_type, item_id) for item_id in item_categories[item_type].values()])
 
 
 
-def get_all_sets():
+def get_all_sets(connection):
     with connection.cursor() as cursor:
         cursor.execute("""select id, url_name from items where item_name like '%Set'""")
 
     return dict(cursor.fetchall())
 
 
 def get_last_saved_date(date_to_fetch):
     if date_to_fetch == "NEW":
         return get_date()
     elif date_to_fetch == "ALL":
         return None
 
 
-def insert_item_statistics(last_save_date):
+def insert_item_statistics(connection, last_save_date):
     file_list = get_file_list(last_save_date)
     data_list = get_data_list(file_list)
 
     # Get the union of all keys in the data_list
     all_columns = set().union(*(data.keys() for data in data_list))
     columns_str = ', '.join(all_columns)
     placeholders = ', '.join(['%s'] * len(all_columns))
@@ -141,15 +135,15 @@
     for item in price_history:
         for statistic_type in price_history[item]:
             data_list.append(statistic_type)
 
     return data_list
 
 
-def get_date():
+def get_date(connection):
     query = "SELECT MAX(datetime) FROM item_statistics"
 
     with connection.cursor() as cursor:
         cursor.execute(query)
         most_recent_datetime = cursor.fetchone()[0]
 
     if most_recent_datetime is not None:
@@ -158,65 +152,65 @@
         most_recent_date = utc_datetime.date()
     else:
         most_recent_date = None
 
     return most_recent_date
 
 
-def get_file_list(date):
+def get_file_list(date, output_directory='output'):
     file_list = []
-    for file in os.listdir(common.OUTPUT_DIRECTORY):
+    for file in os.listdir(output_directory):
         if file.endswith(".json"):
             if date is not None:
                 file_date = datetime.strptime(file, "price_history_%Y-%m-%d.json").date()
                 if file_date <= date:
                     continue
 
-            file_list.append(os.path.join(common.OUTPUT_DIRECTORY, file))
+            file_list.append(os.path.join(output_directory, file))
 
     return file_list
 
 
 def get_data_list(file_list):
     data_list = []
 
     for file in file_list:
         data_list.extend(parse_price_history(open_price_history_file(file)))
 
     return data_list
 
 
-def commit_data():
+def commit_data(connection):
     with connection.cursor() as cursor:
         cursor.execute("COMMIT")
 
 
-def save_items_in_set(item_info):
+def save_items_in_set(connection, item_info):
     data_list = []
     for item in item_info:
         for item_in_set in item_info[item]['set_items']:
             data_list.append((item, item_in_set))
 
     query = """INSERT IGNORE INTO items_in_set (set_id, item_id) VALUES (%s, %s)"""
     with connection.cursor() as cursor:
         cursor.executemany(query, data_list)
 
 
-def save_item_tags(item_info):
+def save_item_tags(connection, item_info):
     data_list = []
     for item in item_info:
         for tag in item_info[item]['tags']:
             data_list.append((item, tag))
 
     query = """INSERT IGNORE INTO item_tags (item_id, tag) VALUES (%s, %s)"""
     with connection.cursor() as cursor:
         cursor.executemany(query, data_list)
 
 
-def save_item_subtypes(item_info):
+def save_item_subtypes(connection, item_info):
     data_list = []
     for item in item_info:
         for subtype in item_info[item]['subtypes']:
             data_list.append((item, subtype))
 
     query = """INSERT IGNORE INTO item_subtypes (item_id, sub_type) VALUES (%s, %s)"""
     with connection.cursor() as cursor:
```

### Comparing `market-engine-0.0.5/market_engine/modules/MarketData.py` & `market-engine-0.0.6/market_engine/modules/MarketData.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.5/market_engine/modules/categories.py` & `market-engine-0.0.6/market_engine/modules/categories.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.0.5/setup.py` & `market-engine-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.5',
+    version='0.0.6',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

