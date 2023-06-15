# Comparing `tmp/talkytrend-1.3.0.tar.gz` & `tmp/talkytrend-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.3.0.tar", max compression
+gzip compressed data, was "talkytrend-1.3.1.tar", max compression
```

## Comparing `talkytrend-1.3.0.tar` & `talkytrend-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-15 09:28:48.081838 talkytrend-1.3.0/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-15 09:28:48.081838 talkytrend-1.3.0/README.md
--rw-r--r--   0        0        0     1720 2023-06-15 09:29:08.918063 talkytrend-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-15 09:29:08.918063 talkytrend-1.3.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      628 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/config.py
--rw-r--r--   0        0        0      842 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6465 2023-06-15 09:28:48.081838 talkytrend-1.3.0/talkytrend/main.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-15 19:54:26.676061 talkytrend-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-15 19:54:26.676061 talkytrend-1.3.1/README.md
+-rw-r--r--   0        0        0     1720 2023-06-15 19:54:41.769239 talkytrend-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-15 19:54:41.769239 talkytrend-1.3.1/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/config.py
+-rw-r--r--   0        0        0      951 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6121 2023-06-15 19:54:26.676061 talkytrend-1.3.1/talkytrend/main.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.3.1/PKG-INFO
```

### Comparing `talkytrend-1.3.0/LICENSE` & `talkytrend-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.0/README.md` & `talkytrend-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.0/pyproject.toml` & `talkytrend-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.3.0"
+version = "1.3.1"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.3.0/talkytrend/config.py` & `talkytrend-1.3.1/talkytrend/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 settings = Dynaconf(
     envvar_prefix="TT",
     # Set the root path of the project
     root_path=os.path.dirname(ROOT),
     # Load the default settings file
     settings_files=[
         os.path.join(ROOT, "default_settings.toml"),
+        'talky_settings.toml',
         'settings.toml',
         '.secrets.toml'
     ],
     # Load the.env file
     load_dotenv=True,
+    # merge=True,
+    # merge_enabled=True,
     # Set the environments to True
     environments=True,
     # Set the default environment
     default_env="default",)
+
```

### Comparing `talkytrend-1.3.0/talkytrend/default_settings.toml` & `talkytrend-1.3.1/talkytrend/default_settings.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 [default]
 talkytrend_enabled = true
+talkytrend_mode = "scanner"
+talkytrend_scanner = false
+talkytrend_scheduler = false
 scanner_frequency = 86400
 enable_signals = true
 assets = [
     { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
     { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
     #use https://tvdb.brianthe.dev/ to get details
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
@@ -11,11 +14,11 @@
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 enable_news = true
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
-live_tv_url = "http://sc2022.stream-link.org/list.php?id=e007"
+live_tv_url = "https://bloomberg-bloombergtv-1.samsung.wurl.com/manifest/playlist.m3u8"
 
 [testing]
 VALUE = "On Testing"
```

### Comparing `talkytrend-1.3.0/talkytrend/main.py` & `talkytrend-1.3.1/talkytrend/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 from prettytable import PrettyTable, MARKDOWN
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from talkytrend.config import settings
 
 class TalkyTrend:
     def __init__(self):
-        self.logger = logging.getLogger("TalkyTrend")
-        self.enabled = settings.talkytrend_enabled
-        if not self.enabled:
-            return
-        #self.mode = settings_talkytrend_mode
-        self.assets = settings.assets
-        self.asset_signals = {}
-        self.economic_calendar = settings.economic_calendar
-        self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
-        self.live_tv = settings.live_tv_url
+        try:
+            self.logger = logging.getLogger("TalkyTrend")
+            self.enabled = settings.talkytrend_enabled
+            if not self.enabled:
+                return
+            self.mode = settings.talkytrend_mode
+            self.assets = settings.assets
+            self.asset_signals = {}
+            self.economic_calendar = settings.economic_calendar
+            self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
+            self.live_tv = settings.live_tv_url
+        except Exception as error:
+            self.logger.error("TalkyTrend init error %s",error)
 
     async def fetch_analysis(
         self,
         asset_id,
         exchange,
         screener,
         interval):
@@ -34,15 +37,14 @@
             handler = TA_Handler(
                 symbol=asset_id,
                 exchange=exchange,
                 screener=screener,
                 interval=interval
             )
             analysis = handler.get_analysis()
-            self.logger.debug("fetch_analysis summary %s",analysis.summary)
             return analysis.summary["RECOMMENDATION"]
         except Exception as error:
             self.logger.error("event %s",error)
 
     async def check_signal(self):
         try:
             signals = []
@@ -51,31 +53,26 @@
             for asset in self.assets:
                 current_signal = await self.fetch_analysis(
                     asset_id=asset["id"],
                     exchange=asset["exchange"],
                     screener=asset["screener"],
                     interval=asset["interval"]
                 )
-                self.logger.debug("fetch_analysis summary %s", current_signal)
                 if self.is_new_signal(asset["id"], asset["interval"], current_signal):
                     signal_item = {
                         "symbol": asset["id"],
                         "interval": asset["interval"],
                         "signal": current_signal
                     }
-                    self.logger.debug("signal message %s", signal_item)
-                    print(asset["id"], current_signal)
                     self.update_signal(asset["id"], asset["interval"], current_signal)
                     table.add_row([asset["id"], current_signal])
-                    self.logger.debug("table %s", table)
                     signals.append(signal_item)
-                self.logger.debug("asset_signals %s", self.asset_signals)
-                self.logger.debug("signals %s", signals)
             #return signals
             #return str(table)
+            # table.border = False
             table.set_style(MARKDOWN)
 
             table_text = table.get_string()
             return table_text
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
@@ -123,40 +120,39 @@
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
                     key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
-                    self.logger.debug("key_news %s", key_news)
                     last_item = key_news[-1]
                     return f"{last_item['title']} {last_item['url']}"
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
 
     async def scanner(self):
         while True:
             try:
                 if settings.enable_events:
                     key_events = await self.fetch_key_events()
                     if key_events is not None:
-                        self.logger.debug("Key event %s", key_events)
+                        self.logger.debug("Key event\n%s", key_events)
                         yield key_events
                 if settings.enable_news:
                     key_news = await self.fetch_key_news()
                     if key_news is not None:
-                        self.logger.debug("Key news %s", key_news)
+                        self.logger.debug("Key news\n%s", key_news)
                         yield key_news
 
                 if settings.enable_signals:
                     signals = await self.check_signal()
                     if signals is not None:
-                        self.logger.debug("Signals %s", signals)
+                        self.logger.debug("Signals\n%s", signals)
                         yield signals
 
             except Exception as error:
                 self.logger.error("scanner %s", error)
 
             await asyncio.sleep(settings.scanner_frequency)
```

### Comparing `talkytrend-1.3.0/PKG-INFO` & `talkytrend-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.3.0
+Version: 1.3.1
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

