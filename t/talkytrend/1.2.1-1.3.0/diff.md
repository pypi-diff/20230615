# Comparing `tmp/talkytrend-1.2.1.tar.gz` & `tmp/talkytrend-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.2.1.tar", max compression
+gzip compressed data, was "talkytrend-1.3.0.tar", max compression
```

## Comparing `talkytrend-1.2.1.tar` & `talkytrend-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-14 19:23:58.809130 talkytrend-1.2.1/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-14 19:23:58.809130 talkytrend-1.2.1/README.md
--rw-r--r--   0        0        0     1720 2023-06-14 19:24:17.305615 talkytrend-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-14 19:24:17.305615 talkytrend-1.2.1/talkytrend/__init__.py
--rw-r--r--   0        0        0      628 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/config.py
--rw-r--r--   0        0        0      842 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6295 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/main.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-15 09:28:48.081838 talkytrend-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-15 09:28:48.081838 talkytrend-1.3.0/README.md
+-rw-r--r--   0        0        0     1720 2023-06-15 09:29:08.918063 talkytrend-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-15 09:29:08.918063 talkytrend-1.3.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/config.py
+-rw-r--r--   0        0        0      842 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6465 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/main.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.0/PKG-INFO
```

### Comparing `talkytrend-1.2.1/LICENSE` & `talkytrend-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.1/README.md` & `talkytrend-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.1/pyproject.toml` & `talkytrend-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.2.1"
+version = "1.3.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.2.1/talkytrend/config.py` & `talkytrend-1.3.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.1/talkytrend/default_settings.toml` & `talkytrend-1.3.0/talkytrend/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [default]
 talkytrend_enabled = true
-scanner_frequency = 7200
+scanner_frequency = 86400
 enable_signals = true
 assets = [
     { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
     { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
     #use https://tvdb.brianthe.dev/ to get details
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
-enable_news = false
+enable_news = true
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
 live_tv_url = "http://sc2022.stream-link.org/list.php?id=e007"
 
 [testing]
 VALUE = "On Testing"
```

### Comparing `talkytrend-1.2.1/talkytrend/main.py` & `talkytrend-1.3.0/talkytrend/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,26 @@
  talky trend Main
 """
 
 import asyncio
 import logging
 from datetime import date
 import aiohttp
-from prettytable import PrettyTable
+from prettytable import PrettyTable, MARKDOWN
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from talkytrend.config import settings
 
 class TalkyTrend:
     def __init__(self):
         self.logger = logging.getLogger("TalkyTrend")
         self.enabled = settings.talkytrend_enabled
         if not self.enabled:
             return
+        #self.mode = settings_talkytrend_mode
         self.assets = settings.assets
         self.asset_signals = {}
         self.economic_calendar = settings.economic_calendar
         self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
         self.live_tv = settings.live_tv_url
 
     async def fetch_analysis(
@@ -66,15 +67,19 @@
                     self.update_signal(asset["id"], asset["interval"], current_signal)
                     table.add_row([asset["id"], current_signal])
                     self.logger.debug("table %s", table)
                     signals.append(signal_item)
                 self.logger.debug("asset_signals %s", self.asset_signals)
                 self.logger.debug("signals %s", signals)
             #return signals
-            return str(table)
+            #return str(table)
+            table.set_style(MARKDOWN)
+
+            table_text = table.get_string()
+            return table_text
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
 
 
     def is_new_signal(self, asset_id, interval, current_signal):
```

### Comparing `talkytrend-1.2.1/PKG-INFO` & `talkytrend-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.2.1
+Version: 1.3.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

