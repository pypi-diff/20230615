# Comparing `tmp/auto-screener-0.0.9.tar.gz` & `tmp/auto-screener-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.0.9.tar", last modified: Thu Apr 27 07:32:22 2023, max compression
+gzip compressed data, was "auto-screener-0.1.0.tar", last modified: Thu Jun 15 16:45:45 2023, max compression
```

## Comparing `auto-screener-0.0.9.tar` & `auto-screener-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.865464 auto-screener-0.0.9/
--rw-rw-rw-   0        0        0      115 2023-04-27 07:32:22.000000 auto-screener-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-27 07:32:22.865464 auto-screener-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.860326 auto-screener-0.0.9/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.9/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.9/auto_screener/base.py
--rw-rw-rw-   0        0        0    20994 2023-04-27 07:13:14.000000 auto-screener-0.0.9/auto_screener/collect.py
--rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.9/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      602 2023-04-27 07:14:09.000000 auto-screener-0.0.9/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.9/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.9/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.9/auto_screener/progress.py
--rw-rw-rw-   0        0        0    35077 2023-04-27 07:31:55.000000 auto-screener-0.0.9/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.9/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.864456 auto-screener-0.0.9/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.9/build.py
--rw-rw-rw-   0        0        0      645 2023-04-27 07:32:22.000000 auto-screener-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 07:32:22.866464 auto-screener-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-27 07:32:18.000000 auto-screener-0.0.9/setup.py
--rw-rw-rw-   0        0        0      850 2023-04-23 18:00:43.000000 auto-screener-0.0.9/test.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:45:45.290802 auto-screener-0.1.0/
+-rw-rw-rw-   0        0        0       98 2023-06-15 16:45:44.000000 auto-screener-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-15 16:45:45.085771 auto-screener-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 16:45:45.080802 auto-screener-0.1.0/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.1.0/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17227 2023-06-15 16:45:21.000000 auto-screener-0.1.0/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.1.0/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.1.0/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.1.0/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    25427 2023-06-15 15:04:45.000000 auto-screener-0.1.0/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.1.0/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.1.0/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    26142 2023-06-15 15:32:24.000000 auto-screener-0.1.0/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    24728 2023-06-13 13:49:29.000000 auto-screener-0.1.0/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.1.0/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:45:45.083803 auto-screener-0.1.0/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-15 16:45:45.000000 auto-screener-0.1.0/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-15 16:45:45.000000 auto-screener-0.1.0/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:45:45.000000 auto-screener-0.1.0/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-15 16:45:45.000000 auto-screener-0.1.0/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 16:45:45.000000 auto-screener-0.1.0/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.1.0/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-15 16:45:44.000000 auto-screener-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-24 20:12:53.000000 auto-screener-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 19:47:16.000000 auto-screener-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:45:45.290802 auto-screener-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-15 16:45:39.000000 auto-screener-0.1.0/setup.py
```

### Comparing `auto-screener-0.0.9/PKG-INFO` & `auto-screener-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.9
+Version: 0.1.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.9/README.md` & `auto-screener-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.9/auto_screener/base.py` & `auto-screener-0.1.0/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.9/auto_screener/document.py` & `auto-screener-0.1.0/auto_screener/document.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # document.py
 
 # noinspection PyUnresolvedReferences
 from auto_screener.interval import *
 # noinspection PyUnresolvedReferences
-from auto_screener.screening import *
+from auto_screener.symbols import *
 # noinspection PyUnresolvedReferences
-from auto_screener.tickers import *
+from auto_screener.dataset import *
 # noinspection PyUnresolvedReferences
-from auto_screener.progress import *
+from auto_screener.feed import *
 # noinspection PyUnresolvedReferences
-from auto_screener.dataset import *
+from auto_screener.screening import *
 # noinspection PyUnresolvedReferences
 from auto_screener.collect import *
+# noinspection PyUnresolvedReferences
+from auto_screener.screener import *
+# noinspection PyUnresolvedReferences
+from auto_screener.exchanges import *
 
 from auto_screener.base import document
 
 class Documentation:
     """"""
 # end Documentation
```

### Comparing `auto-screener-0.0.9/auto_screener/interval.py` & `auto-screener-0.1.0/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.9/auto_screener/screening.py` & `auto-screener-0.1.0/auto_screener/screener.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1260 +1,923 @@
-# screening.py
+# screener.py
 
 import os
-import time
-import asyncio
 import warnings
 import datetime as dt
+import time
+from abc import ABCMeta
 import threading
 from typing import (
     Optional, Union, Dict, Iterable, Any, List
 )
 
 import pandas as pd
-import numpy as np
-import ccxt
-import ccxt.pro as ccxtpro
 
 from represent import BaseModel, Modifiers
 
-from auto_screener.hints import Number
 from auto_screener.dataset import (
-    OPEN, HIGH, LOW, CLOSE, VOLUME, BIDS,
-    ASKS, row_to_dataset, DATE_TIME
-)
-from auto_screener.base import terminate_thread
-from auto_screener.interval import interval_to_total_time
-from auto_screener.dataset import save_dataset, load_dataset
-from auto_screener.collect import (
-    AutoDataCollector, wait_for_initialization,
-    wait_for_update, WaitingState, configure_exchange,
-    ohlcv_to_dataset
+    DATE_TIME, save_dataset, load_dataset
 )
+from auto_screener.hints import Number
+from auto_screener.collect import validate_symbol
 
 __all__ = [
-    "AutoDataset",
-    "AutoScreener",
-    "MultiScreener",
-    "ScreenerSignature",
+    "BaseScreener",
+    "wait_for_update",
+    "wait_for_initialization",
+    "WaitingState",
+    "DataCollector",
+    "collect_screeners",
+    "wait_for_dynamic_update",
+    "wait_for_dynamic_initialization",
+    "BaseMultiScreener",
+    "live_screeners",
+    "create_market_dataframe",
+    "structure_screeners"
 ]
 
-class AutoScreener(BaseModel, AutoDataCollector):
-    """
-    A class to represent an asset price screener.
+class WaitingState(BaseModel):
+    """A class to represent the waiting state of screener objects."""
 
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
+    modifiers = Modifiers(excluded=["create_screeners"])
 
-    Parameters:
+    __slots__ = "screeners", "delay", "count", "canceled", "cancel"
 
-    - ticker:
-        The ticker symbol of an asset to screen.
+    def __init__(
+            self,
+            screeners: Iterable,
+            delay: Number,
+            count: int,
+            canceled: bool,
+            cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+    ) -> None:
+        """
+        Defines the class attributes.
 
-    - source:
-        The name of the exchange platform to screen data from.
+        :param screeners: The screener objects.
+        :param delay: The waiting delay.
+        :param count: The iterations count.
+        :param canceled: The value for the waiting being canceled.
+        :param cancel: The time to cancel the waiting.
+        """
 
-    - delay:
-        The delay to wait between each data fetching.
+        self.screeners: Iterable[Union[BaseScreener, BaseMultiScreener]] = screeners
 
-    - pro:
-        The value to use the pro interface.
+        self.delay = delay
+        self.cancel = cancel
+        self.count = count
 
-    - options:
-        The ccxt options for the backend screening process.
+        self.canceled = canceled
+    # end __init__
 
-    >>> from auto_screener.screening import AutoScreener
-    >>> from auto_screener.collect wait_for_initialization
-    >>>
-    >>> screener = AutoScreener(
-    >>>     ticker="BTC/USD", source="binance"
-    >>> )
-    >>>
-    >>> screener.run(wait=True)
-    >>>
-    >>> while True:
-    >>>     print(screener.market.iloc[-1])
-    >>>
-    >>>     wait_for_update(screener, delay=1)
-    """
+    @property
+    def time(self) -> dt.timedelta:
+        """
+        Returns the amount of waited time.
 
-    modifiers = Modifiers(
-        excluded=[
-            "market", "exchange", "screening_process",
-            "task", 'timeout_process'
+        :return: The waiting time.
+        """
+
+        return dt.timedelta(seconds=self.delay * self.count)
+    # end time
+# end WaitingState
+
+class DataCollector(BaseModel, metaclass=ABCMeta):
+    """A class to represent an abstract parent class of data collectors."""
+
+    modifiers = Modifiers(**BaseModel.modifiers)
+    modifiers.excluded.extend(
+        [
+            'screening_process', 'timeout_process',
+            'saving_process'
         ]
     )
 
-    ASKS = ASKS
-    BIDS = BIDS
+    LOCATION = "datasets"
 
     DELAY = 0.0
-
-    COLUMNS = (
-        OPEN, HIGH, LOW, CLOSE,
-        ASKS, BIDS, VOLUME
-    )
+    CANCEL = 0
 
     def __init__(
             self,
-            ticker: str,
-            source: str,
-            pro: Optional[bool] = True,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            options: Optional[Dict[str, Any]] = None
+            location: Optional[str] = None,
+            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
-        :param ticker: The ticker of the asset.
-        :param source: The exchange to get source data from.
+        :param location: The saving location for the data.
         :param delay: The delay for the process.
-        :param pro: The value for the pro interface.
-        :param options: The ccxt options.
+        :param cancel: The cancel time for the loops.
         """
 
-        self.options = options or {}
-
-        self.exchange = configure_exchange(
-            source=source, pro=pro, options=self.options
-        )
-
+        self.cancel = cancel or self.CANCEL
         self.delay = delay or self.DELAY
 
-        self.pro = pro
-
-        self.source = source
-
-        self.ticker = self.validate_ticker(ticker=ticker)
+        self.location = location or self.LOCATION
 
         self.running = False
         self.block = False
-
-        self.market = pd.DataFrame(
-            {column: [] for column in self.COLUMNS}, index=[]
-        )
-
-        self.market.index.name = DATE_TIME
+        self.saving = False
 
         self.screening_process = None
         self.timeout_process = None
-
-        self.task = None
+        self.saving_process = None
     # end __init__
 
     def __getstate__(self) -> Dict[str, Any]:
         """
         Returns the data of the object.
 
         :return: The state of the object.
         """
 
         data = self.__dict__.copy()
 
-        data["task"] = None
-        data["screening_process"] = None
-        data["timeout_process"] = False
-        data["exchange"] = None
+        for key, value in data.items():
+            if isinstance(value, threading.Thread):
+                data[key] = None
+            # end if
+        # end for
 
         return data
     # end __getstate__
 
-    def __setstate__(self, state: Dict[str, Any]) -> Any:
+    def blocking(self) -> bool:
         """
-        Sets the state of the object.
+        returns the value of the process being blocked.
 
-        :param state: The state to set to the object.
+        :return: The value.
         """
 
-        self.__dict__.update(state)
+        return self.block
+    # end blocking
 
-        self.exchange = configure_exchange(
-            source=self.source, pro=self.pro
-        )
-    # end __setstate__
+    def run_loop(self) -> None:
+        """Runs the process of the price screening."""
+    # end run_loop
 
-    async def async_get_market(self) -> Dict[str, Number]:
-        """
-        Gets the market data.
+    def saving_loop(self) -> None:
+        """Runs the process of the price screening."""
+    # end saving_loop
 
-        :return: The bids and asks.
+    def wait_for_initialization(
+            self,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            once: Optional[bool] = False,
+            stop: Optional[Union[bool, int]] = False,
+            cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState:
         """
+        Waits for all the create_screeners to update.
 
-        if hasattr(self.exchange, "fetch_tickers"):
-            method = self.exchange.fetch_tickers
+        :param delay: The delay for the waiting.
+        :param once: The value to get data only once.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
 
-        elif hasattr(self.exchange, "watch_tickers"):
-            method = self.exchange.watch_tickers
+        :returns: The total delay.
+        """
 
-        else:
-            raise AttributeError(
-                f"Exchange attribute {self.exchange} of "
-                f"{self} must has at least one of the "
-                f"methods 'fetch_tickers', or 'watch_tickers'."
-            )
-        # end if
+        self: Union[BaseScreener, BaseMultiScreener]
 
-        if isinstance(self.exchange, getattr(ccxtpro, self.source)):
-            data = await method(symbols=[self.ticker])
+        return wait_for_initialization(
+            self, delay=delay, once=once,
+            stop=stop, cancel=cancel or self.cancel
+        )
+    # end wait_for_initialization
 
-        elif isinstance(self.exchange, getattr(ccxt, self.source)):
-            data = method(symbols=[self.ticker])
+    def wait_for_update(
+            self,
+            delay: Optional[Union[Number, dt.timedelta]] = None,
+            once: Optional[bool] = False,
+            stop: Optional[Union[bool, int]] = False,
+            cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState:
+        """
+        Waits for all the create_screeners to update.
 
-        else:
-            raise TypeError(
-                f"Exchange object {self.exchange} of "
-                f"{self} must be from ccxt."
-            )
-        # end if
+        :param delay: The delay for the waiting.
+        :param once: The value to get data only once.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
 
-        ticker = list(data.keys())[0]
+        :returns: The total delay.
+        """
 
-        data[ticker][VOLUME.lower()] = data[ticker]["quoteVolume"]
-        data[ticker][self.ASKS.lower()] = data[ticker]["ask"]
-        data[ticker][self.BIDS.lower()] = data[ticker]["bid"]
+        self: Union[BaseScreener, BaseMultiScreener]
 
-        return {
-            key: data[ticker][key.lower()] for key in
-            self.COLUMNS
-        }
-    # end async_get_market
+        return wait_for_update(
+            self, delay=delay, once=once,
+            stop=stop, cancel=cancel or self.cancel
+        )
+    # end wait_for_update
 
-    async def get_market(self) -> Dict[str, Number]:
+    def run(
+            self,
+            save: Optional[bool] = True,
+            block: Optional[bool] = False,
+            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+    ) -> threading.Thread:
         """
-        Gets the market data.
+        Runs the process of the price screening.
 
-        :return: The bids and asks.
+        :param save: The value to save the data.
+        :param wait: The value to wait after starting to run the process.
+        :param block: The value to block the execution.
+        :param timeout: The valur to add a timeout to the process.
         """
 
-        task = self.async_get_market()
-
-        try:
-            loop = asyncio.get_event_loop()
-
-            self.task = loop.create_task(task)
+        if self.running:
+            warnings.warn(f"Screener object {self} is already running.")
 
-            return await self.task
-
-        except RuntimeError:
-            return asyncio.run(task)
-        # end try
-    # end get_market
-
-    async def async_run_loop(self) -> None:
-        """Runs the processes of price screening."""
+            return self.screening_process
+        # end if
 
         self.running = True
 
-        delay = self.delay
+        self.screening_process = threading.Thread(target=self.run_loop)
 
-        if isinstance(delay, dt.timedelta):
-            delay = delay.total_seconds()
-        # end if
+        self.screening_process.start()
 
-        while self.running:
-            start = time.time()
+        if save:
+            self.saving = True
 
-            try:
-                data = await self.async_get_market()
+            self.saving_process = threading.Thread(
+                target=self.saving_loop
+            )
 
-            except Exception as e:
-                self.terminate()
+            self.saving_process.start()
+        # end if
 
-                raise RuntimeError(
-                    f"Could not complete task. {str(e)}"
-                ) from e
-            # end try
+        if timeout:
+            self.timeout(timeout)
+        # end if
 
-            new_data = pd.DataFrame(
-                data, index=pd.to_datetime(
-                    [int(time.time() * 1000)], unit="ms"
-                )
-            )
-            new_data.index.name = DATE_TIME
+        if block:
+            self.block = block
 
-            self.market = pd.concat([self.market, new_data])
-            self.market.index.name = DATE_TIME
+            while self.blocking():
+                pass
+            # end while
+        # end if
 
-            end = time.time()
+        if isinstance(wait, dt.datetime):
+            wait = wait - dt.datetime.now()
+        # end if
 
-            if delay:
-                time.sleep(max([delay - (end - start), 0]))
-            # end if
-        # end while
-    # end async_run
+        if isinstance(wait, dt.timedelta):
+            wait = wait.total_seconds()
+        # end if
 
-    async def async_run(self) -> None:
-        """Runs the processes of price screening."""
+        if isinstance(wait, bool) and wait:
+            self.wait_for_initialization()
 
-        task = self.async_run_loop()
+        elif isinstance(wait, (int, float)):
+            time.sleep(wait)
+        # end if
 
-        try:
-            loop = asyncio.get_event_loop()
+        return self.screening_process
+    # end run
 
-            self.task = loop.create_task(task)
+    def timeout(
+            self, duration: Union[Number, dt.timedelta, dt.datetime]
+    ) -> threading.Thread:
+        """
+        Runs a timeout for the process.
 
-            await self.task
+        :param duration: The duration of the timeout.
 
-        except RuntimeError:
-            asyncio.run(task)
-        # end try
-    # end async_run
+        :return: The timeout process.
+        """
 
-    def run_loop(self) -> None:
-        """Runs the process of the price screening."""
+        if isinstance(duration, dt.datetime):
+            duration = duration - dt.datetime.now()
+        # end if
 
-        asyncio.run(self.async_run())
-    # end run_loop
+        if isinstance(duration, dt.timedelta):
+            duration = duration.total_seconds()
+        # end if
 
-    def stop(self) -> None:
-        """Stops the screening process."""
+        self.timeout_process = threading.Thread(
+            target=lambda: (time.sleep(duration), self.terminate())
+        )
 
-        super().stop()
+        self.timeout_process.start()
 
-        if self.task is not None:
-            self.task.cancel()
-        # end if
-    # end stop
+        return self.timeout_process
+    # end timeout
 
     def terminate(self) -> None:
         """Stops the trading process."""
 
-        super().terminate()
+        self.stop()
     # end terminate
-# end Screener
 
-class ScreenerSignature(BaseModel):
-    """
-    A class to represent a screener signature.
+    def stop(self) -> None:
+        """Stops the screening process."""
 
-    Parameters:
+        if (
+            self.running and
+            isinstance(self.screening_process, threading.Thread) and
+            self.screening_process.is_alive()
+        ):
+            self.screening_process = None
 
-    - ticker:
-        The ticker symbol of an asset to screen.
+            self.running = False
+        # end if
 
-    - source:
-        The name of the exchange platform to screen data from.
+        if (
+            self.saving and
+            isinstance(self.saving_process, threading.Thread) and
+            self.saving_process.is_alive()
+        ):
+            self.saving_process = None
 
-    - delay:
-        The delay to wait between each data fetching.
+            self.saving = False
+        # end if
 
-    - pro:
-        The value to use the pro interface.
-    """
+        if self.block:
+            self.block = False
+        # end if
+    # end stop
+# end DataCollector
 
-    def __init__(
-            self,
-            ticker: str,
-            source: str,
-            pro: bool,
-            delay: Union[Number, dt.timedelta]
-    ) -> None:
-        """
-        Defines the class attributes.
+def create_market_dataframe(columns: Iterable[str]) -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
 
-        :param ticker: The ticker of the asset.
-        :param source: The exchange to get source data from.
-        :param delay: The delay for the process.
-        :param pro: The value for the pro interface.
-        """
+    :param columns: The dataset columns.
 
-        self.ticker = ticker
-        self.source = source
+    :return: The dataframe.
+    """
 
-        self.pro = pro
+    market = pd.DataFrame(
+        {column: [] for column in columns}, index=[]
+    )
+    market.index.name = DATE_TIME
 
-        self.delay = delay
-    # end __init__
-# end ScreenerSignature
+    return market
+# end create_market_dataframe
 
-class AutoDataset(BaseModel, AutoDataCollector):
+class BaseScreener(DataCollector):
     """
-    A class to represent a live asset data builder.
+    A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
-    You can also use it to build real time datasets of Open
-    High Low Close Volume, with Bids and Asks.
-
     Parameters:
 
-    - ticker:
-        The ticker symbol of an asset to screen.
+    - symbol:
+        The symbol of an asset to screen.
 
-    - source:
+    - exchange:
         The name of the exchange platform to screen data from.
 
-    - interval:
-        The interval for the time between data points in the dataset.
+    - location:
+        The saving location for the saved data of the screener.
+
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
-
-    - screener:
-        The screener object to connect to for creating the dataset.
-
-    - length:
-        An initial dataset length to start with.
-
-    - pro:
-        The value to use the pro interface.
-
-    - options:
-        The ccxt options for the backend screening process.
-
-    >>> from auto_screener.screening import AutoDataset
-    >>> from auto_screener.collect wait_for_initialization
-    >>> from auto_screener.interval import interval_to_total_time
-    >>>
-    >>> interval = "1m"
-    >>>
-    >>> dataset = AutoDataset(
-    >>>     ticker="BTC/USD", source="binance", interval=interval
-    >>> )
-    >>>
-    >>> dataset.run(wait=True)
-    >>>
-    >>> print(dataset.market.iloc[-1].splitlines()[0])
-    >>>
-    >>> while True:
-    >>>     print(dataset.market.iloc[-1].splitlines()[-1])
-    >>>
-    >>>     wait_for_update(dataset, delay=interval_to_total_time(interval))
     """
 
-    modifiers = Modifiers(
-        excluded=[
-            "timeout_process", 'market', 'built',
-            'exchange', 'screening_process', "delay"
-        ]
-    )
-
-    screeners: Dict[ScreenerSignature, AutoScreener] = {}
+    modifiers = Modifiers(**DataCollector.modifiers)
+    modifiers.excluded.append("market")
 
-    EXCHANGES = AutoScreener.EXCHANGES
-    COLUMNS = AutoScreener.COLUMNS
-    TICKERS = AutoScreener.TICKERS
+    __slots__ = "symbol", "exchange", "location", "cancel", "delay", "market"
 
     def __init__(
             self,
-            ticker: str,
-            source: str,
-            interval: str,
-            pro: Optional[bool] = True,
-            data: Optional[pd.DataFrame] = None,
-            length: Optional[Union[bool, int]] = None,
+            symbol: str,
+            exchange: str,
+            location: Optional[str] = None,
+            cancel: Optional[Union[Number, dt.timedelta]] = None,
             delay: Optional[Union[Number, dt.timedelta]] = None,
-            screener: Optional[AutoScreener] = None,
-            options: Optional[Dict[str, Any]] = None
+            market: Optional[pd.DataFrame] = None,
     ) -> None:
         """
         Defines the class attributes.
 
-        :param ticker: The ticker of the asset.
-        :param source: The exchange to get source data from.
-        :param interval: The interval for the data.
-        :param data: The base dataset of the asset to add to.
-        :param length: The length of the base dataset.
+        :param symbol: The symbol of the asset.
+        :param exchange: The exchange to get source data from.
+        :param location: The saving location for the data.
         :param delay: The delay for the process.
-        :param screener: The screener object for the dataset.
-        :param pro: The value for the pro interface.
-        :param options: The ccxt options.
+        :param cancel: The cancel time for the loops.
+        :param market: The data for the market.
         """
 
-        self.options = options or {}
-
-        self.source = source
-
-        self.interval = interval
-        self.ticker = ticker
-        self.delay = delay
-
-        self.built = False
-
-        self.pro = pro
-
-        self.signature = ScreenerSignature(
-            ticker=self.ticker, source=self.source,
-            delay=self.delay, pro=self.pro
+        super().__init__(
+            location=location, cancel=cancel, delay=delay
         )
 
-        if self.signature not in self.screeners:
-            if screener is None:
-                self.built = True
-
-                screener = AutoScreener(
-                    ticker=self.ticker, source=self.source,
-                    delay=self.delay, pro=self.pro,
-                    options=self.options
-                )
-            # end if
-
-            self.screeners[self.signature] = screener
-        # end if
-
-        self.screener = self.screeners[self.signature]
-
-        self.market = self.validate_data(data, length=length)
-
-        ccxt.binance()
+        self.exchange = exchange
 
-        self.exchange = getattr(ccxt, self.source)(self.options)
+        self.symbol = self.validate_symbol(exchange=exchange, symbol=symbol)
 
-        self.screening_process = None
-        self.timeout_process = None
+        if market is None:
+            market = create_market_dataframe(())
+        # end if
 
-        self.running = False
-        self.block = False
+        self.market = market
     # end __init__
 
-    def __getstate__(self) -> Dict[str, Any]:
-        """
-        Returns the data of the object.
-
-        :return: The state of the object.
+    @staticmethod
+    def validate_symbol(exchange: str, symbol: Any) -> str:
         """
+        Validates the symbol value.
 
-        data = self.__dict__.copy()
-
-        data["exchange"] = None
+        :param exchange: The exchange name.
+        :param symbol: The name of the symbol.
 
-        return data
-    # end __getstate__
-
-    def __setstate__(self, state: Dict[str, Any]) -> Any:
-        """
-        Sets the state of the object.
-
-        :param state: The state to set to the object.
+        :return: The validates symbol.
         """
 
-        self.__dict__.update(state)
-
-        self.exchange = getattr(ccxt, self.source)()
-    # end __setstate__
+        return validate_symbol(exchange=exchange, symbol=symbol)
+    # end validate_symbol
 
-    def validate_data(self, data: Any, length: Optional[int]) -> pd.DataFrame:
+    def dataset_path(self, location: Optional[str] = None) -> str:
         """
-        Validates the asset data value.
+        Creates the path to the saving file for the screener object.
 
-        :param data: The asset data.
-        :param length: The length of the data to add.
+        :param location: The saving location of the dataset.
 
-        :return: The validates source.
+        :return: The saving path for the dataset.
         """
 
-        if not all(
-                hasattr(self, name) for name in ["source", "interval"]
-        ):
-            raise AttributeError(
-                "Source and interval attributes must be defined "
-                "before attempting to validate the data parameter data."
-            )
-        # end if
+        location = location or self.location
 
-        if (
-            (data is None) and
-            (
-                (length is None) or
-                (length == 0) or
-                (length is False) or
-                (
-                    isinstance(length, int) and
-                    not (0 < length <= 500)
-                )
-            )
-        ):
-            data = pd.DataFrame(
-                {column: [] for column in self.COLUMNS},
-                index=[]
-            )
-
-        elif (data is None) and (isinstance(length, int)):
-            if 0 < length <= 500:
-                data = self.data_to_dataset(
-                    self.exchange.fetch_ohlcv(
-                        symbol=self.ticker,
-                        timeframe=self.interval,
-                        limit=length
-                    )
-                )
-
-            else:
-                raise ValueError(
-                    f"Length must be a positive int between "
-                    f"1 and 500 when data is not defined, "
-                    f"not: {length}."
-                )
-            # end if
-        # end if
-
-        return data
-    # end validate_data
+        return (location + "/" if isinstance(location, str) else "") + (
+            f"{self.exchange.lower()}/{self.symbol.replace('/', '-')}.csv"
+        )
+    # end dataset_path
 
-    def data_to_dataset(self, data: Iterable[Iterable]) -> pd.DataFrame:
+    def save_dataset(self, location: Optional[str] = None) -> None:
         """
-        Adjusts the dataset to an asset Open, High, Low, Close, Bids, Asks, Volume dataset.
-
-        :param data: The data to adjust.
+        Saves the data of the screener.
 
-        :return: The asset dataset.
+        :param location: The saving location of the dataset.
         """
 
-        data = ohlcv_to_dataset(data=data)
-
-        if len(self.screener.market) == 0:
-            asks = [np.nan] * len(data)
-            bids = [np.nan] * len(data)
-
-        else:
-            asks = (
-                self.screener.market[AutoScreener.ASKS].iloc
-                [-len(data):].values[:]
-            )
-            bids = (
-                self.screener.market[AutoScreener.BIDS].iloc
-                [-len(data):].values[:]
-            )
+        if len(self.market) == 0:
+            return
         # end if
 
-        data[AutoScreener.ASKS].values[:] = asks
-        data[AutoScreener.BIDS].values[:] = bids
-
-        return data[list(self.COLUMNS)]
-    # end data_to_dataset
+        save_dataset(
+            dataset=self.market,
+            path=self.dataset_path(location=location)
+        )
+    # end save_dataset
 
-    def run(
-            self,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            block: Optional[bool] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
-    ) -> threading.Thread:
+    def load_dataset(self, location: Optional[str] = None) -> None:
         """
-        Runs the process of the price screening.
+        Saves the data of the screener.
 
-        :param wait: The value to wait after starting to run the process.
-        :param block: The value to block the execution.
-        :param timeout: The valur to add a timeout to the process.
+        :param location: The saving location of the dataset.
         """
 
-        if not self.screener.running:
-            self.screener.run(wait=True, block=False, timeout=timeout)
-        # end if
+        data = load_dataset(path=self.dataset_path(location=location))
 
-        return super().run(wait=wait, block=block, timeout=timeout)
-    # end run
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.market.loc[index] = data
+        # end for
+    # end load_dataset
 
-    def run_loop(self) -> None:
+    def saving_loop(self) -> None:
         """Runs the process of the price screening."""
 
-        self.running = True
-
-        delay = interval_to_total_time(self.interval).seconds
+        self.saving = True
 
-        while self.running:
-            start = time.time()
+        delay = self.delay
 
-            data = row_to_dataset(self.screener.market, index=-1)
+        if isinstance(self.delay, dt.timedelta):
+            delay = delay.total_seconds()
+        # end if
 
-            # noinspection PyBroadException
-            try:
-                prices = self.validate_data(data=None, length=1)
-                prices[AutoScreener.BIDS].values[:] = (
-                    data[AutoScreener.BIDS].values[:]
-                )
-                prices[AutoScreener.ASKS].values[:] = (
-                    data[AutoScreener.ASKS].values[:]
-                )
-                data = prices
+        while self.saving:
+            start = time.time()
 
-            except Exception as e:
-                warnings.warn(str(e))
-            # end try
+            self.save_dataset()
 
             end = time.time()
 
-            self.market = pd.concat([self.market, data])
-            self.market = self.market[
-                ~self.market.index.duplicated(keep='first')
-            ]
-
-            time.sleep(max([delay - (end - start), 0]))
+            time.sleep(max(delay - (end - start), 0) or 1)
         # end while
     # end run_loop
+# end BaseScreener
 
-    def terminate(self) -> None:
-        """Stops the trading process."""
-
-        super().terminate()
-
-        if self.built:
-            self.screener.terminate()
-        # end if
-    # end terminate
-
-    def stop(self) -> None:
-        """Stops the screening process."""
-
-        super().stop()
-
-        if self.built:
-            self.screener.stop()
-        # end if
-    # end stop
-# end LiveAssetData
-
-class MultiScreener(BaseModel):
+class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
     Parameters:
 
-    - exchanges:
-        The data of exchanges and their tickers to screen.
+    - location:
+        The saving location for the saved data of the screener.
 
-    - interval:
-        The interval for the time between data points in the dataset.
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
-
-    - length:
-        An initial dataset length to start with.
-
-    >>> from auto_screener.screening import MultiScreener
-    >>> from auto_screener.collect wait_for_initialization
-    >>>
-    >>> screener = MultiScreener(
-    >>>     exchanges={
-    >>>         "binance": ["BTC/USDT", "AAVE/EUR"],
-    >>>         "bittrex": ["GRT/USD", "BTC/USD"]
-    >>>     }
-    >>> )
-    >>>
-    >>> screener.run(wait=True)
-    >>>
-    >>> while True:
-    >>>     screener.wait_for_update(delay=1)
     """
 
-    modifiers = Modifiers(
-        excluded=[
-            "exchange", "screening_process",
-            "timeout_process", "screeners"
-        ]
-    )
-
-    LOCATION = "datasets"
-    INTERVAL = "1m"
+    modifiers = Modifiers(**DataCollector.modifiers)
+    modifiers.excluded.append("market")
 
-    DELAY = 1
-    CANCEL = 60
+    screeners: List[BaseScreener]
 
-    PRO = False
-
-    OPTIONS = {}
+    __slots__ = "screeners", "location", "cancel", "delay"
 
     def __init__(
             self,
-            exchanges: Dict[str, Iterable[str]],
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            interval: Optional[Union[bool, str]] = None,
-            length: Optional[Union[int, bool]] = None,
+            screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
-            pro: Optional[bool] = None,
-            options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[int] = None
+            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[Number, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
-        :param interval: The interval of the data to load.
-        :param exchanges: The data of exchanges and their tickers.
-        :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
-        :param delay: The delay between each data fetching request.
-        :param length: The length of the data to get in each request.
-        :param options: The ccxt options.
-        """
-
-        if isinstance(interval, bool) and interval:
-            interval = self.INTERVAL
-
-        elif isinstance(interval, bool):
-            interval = None
-        # end if
-
-        self.options = options or self.OPTIONS
-
-        self.interval = interval
-        self.location = location or self.LOCATION
-
-        self.delay = delay or self.DELAY
-        self.cancel = cancel or self.CANCEL
-        self.length = length
-
-        self.pro = pro or self.PRO
-
-        self.exchanges = self.validate_exchanges(exchanges)
-
-        self.running = False
-        self.block = False
-        self.saving = False
-
-        self.market: Dict[str, Dict[str, Optional[AutoDataCollector]]] = {}
-        self.invalid: Dict[str, List[str]] = {}
-        self.screeners: List[AutoDataCollector] = []
-        self.stopped: List[AutoDataCollector] = []
-
-        self.saving_process = None
-        self.timeout_process = None
-    # end Screener
-
-    @staticmethod
-    def validate_exchanges(data: Any) -> Dict[str, List[str]]:
-        """
-        Validates the data.
-
-        :param data: The data to validate.
-
-        :return: The valid data.
-        """
-
-        if data is None:
-            return {}
-        # end if
-
-        try:
-            if not isinstance(data, dict):
-                raise ValueError
-            # end if
-
-            new_data = {}
-
-            for key, values in data.items():
-                values = list(values)
-
-                if not (
-                    isinstance(key, str) and
-                    all(isinstance(value, str) for value in values)
-                ):
-                    raise ValueError
-                # end if
-
-                new_data[key] = values
-            # end for
-
-        except (TypeError, ValueError):
-            raise ValueError(
-                f"Exchanges data must be a dictionary of "
-                f"exchange names as keys and iterables of "
-                f"ticker names as values, not {data}."
-            )
-        # end try
-
-        return new_data
-    # end validate_data
-
-    @staticmethod
-    def dataset_path(screener: AutoDataCollector, location: Optional[str] = None) -> str:
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
         """
-        Creates the path to the saving file for the screener object.
 
-        :param screener: The screener object.
-        :param location: The saving location of the dataset.
-
-        :return: The saving path for the dataset.
-        """
+        super().__init__(location=location, cancel=cancel, delay=delay)
 
-        return (location + "/" if isinstance(location, str) else "") + (
-            f"{screener.source}/{screener.ticker.replace('/', '-')}.csv"
-        )
-    # end dataset_path
+        self.screeners = list(screeners or [])
+    # end __init__
 
-    def create_screener(
-            self,
-            container: Dict[str, Optional[AutoDataCollector]],
-            ticker: str,
-            source: str
-    ) -> None:
+    def load_datasets(self, location: Optional[str] = None) -> None:
         """
-        Creates the screener and inserts it into the container.
+        Loads the datasets of the create_screeners.
 
-        :param container: The container to contain the new screener.
-        :param ticker: The ticker of the screener.
-        :param source: The source of the data.
+        :param location: The saving or loading path for the dataset.
         """
 
-        try:
-            if isinstance(self.interval, str):
-                container[ticker] = AutoDataset(
-                    ticker=ticker, source=source, options=self.options,
-                    interval=self.interval, pro=self.pro, delay=self.delay
-                )
+        for screener in self.screeners:
+            if os.path.exists(screener.dataset_path() or location):
+                try:
+                    screener.load_dataset(
+                        location=location or self.location or screener.location
+                    )
 
-            else:
-                container[ticker] = AutoScreener(
-                    ticker=ticker, source=source, options=self.options,
-                    pro=self.pro, delay=self.delay
-                )
+                except Exception as e:
+                    warnings.warn(str(e))
+                # end try
             # end if
+        # end for
+    # end load_datasets
 
-        except ValueError:
-            container[ticker] = None
-
-            self.invalid.setdefault(source, []).append(ticker)
-        # end try
-    # end create_screener
-
-    @staticmethod
-    def configure_screener_dataset(
-            screener: AutoDataCollector, path: str, length: Optional[int] = None
-    ) -> None:
+    def save_datasets(self, location: Optional[str] = None) -> None:
         """
-        Configures the dataset of the screener.
+        Saves the datasets of the create_screeners.
 
-        :param screener: The screener object to configure the dataset for.
-        :param path: The saving or loading path for the dataset.
-        :param length: The length of the dataset to fetch.
+        :param location: The saving or loading path for the dataset.
         """
 
-        if os.path.exists(path):
+        for screener in self.screeners:
             try:
-                screener.market = load_dataset(path=path)
+                screener.save_dataset(
+                    location=location or self.location or screener.location
+                )
 
             except Exception as e:
                 warnings.warn(str(e))
             # end try
+        # end for
+    # end load_datasets
+# end BaseScreener
 
-        else:
-            if isinstance(screener, AutoDataset):
-                screener.market = screener.validate_data(
-                    data=None, length=length
-                )
-            # end if
-
-            if len(screener.market) > 0:
-                save_dataset(dataset=screener.market, path=path)
-            # end if
-        # end if
-    # end configure_screener_dataset
-
-    def wait_for_initialization(
-            self,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            once: Optional[bool] = False,
-            stop: Optional[Union[bool, int]] = False
-    ) -> WaitingState:
-        """
-        Waits for all the screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param once: The value to get data only once.
-        :param stop: The value to stop the screener objects.
-
-        :returns: The total delay.
-        """
+def collect_screeners(
+        symbol: str,
+        exchange: str,
+        screeners: Iterable[BaseScreener]
+) -> List[BaseScreener]:
+    """
+    Finds the create_screeners with the given source exchange and symbol.
 
-        return wait_for_initialization(
-            *[
-                screener.screener
-                if isinstance(screener, AutoDataset)
-                else screener
-                for screener in self.screeners
-            ], delay=delay, once=once, stop=stop
-        )
-    # end wait_for_initialization
+    :param symbol: The symbol of the screener.
+    :param exchange: The exchange name of the screener.
+    :param screeners: The create_screeners to search in.
 
-    def wait_for_update(
-            self,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            once: Optional[bool] = False,
-            stop: Optional[Union[bool, int]] = False
-    ) -> WaitingState:
-        """
-        Waits for all the screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param once: The value to get data only once.
-        :param stop: The value to stop the screener objects.
+    :return: A list of the matching create_screeners.
+    """
 
-        :returns: The total delay.
-        """
+    found = []
 
-        return wait_for_update(
-            *self.screeners, delay=delay, once=once, stop=stop
-        )
-    # end wait_for_update
-
-    def initialize_screeners(self) -> None:
-        """Initializes the screeners."""
+    for screener in screeners:
+        if (screener.exchange == exchange) and (screener.symbol == symbol):
+            found.append(screener)
+        # end if
+    # end for
+
+    return found
+# end collect_screeners
+
+def wait_for_dynamic_initialization(
+        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]],
+        delay: Optional[Union[Number, dt.timedelta]] = None,
+        once: Optional[bool] = False,
+        stop: Optional[Union[bool, int]] = False,
+        cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
 
-        self.market.clear()
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param once: The value to get data only once.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
 
-        for exchange, tickers in self.exchanges.items():
-            self.market[exchange] = {}
+    :returns: The total delay.
+    """
 
-            for ticker in tickers:
-                threading.Thread(
-                    target=self.create_screener,
-                    kwargs=dict(
-                        container=self.market[exchange],
-                        ticker=ticker, source=exchange
-                    )
-                ).start()
-            # end for
-        # end for
+    if cancel == 0:
+        cancel = None
+    # end if
 
-        while (
-            sum(len(screeners) for screeners in self.market.values()) <
-            sum(len(tickers) for tickers in self.exchanges.values())
-        ):
-            time.sleep(3)
-        # end while
+    if isinstance(cancel, (int, float)):
+        cancel = dt.timedelta(seconds=cancel)
+    # end if
 
-        self.screeners.clear()
+    current_time = dt.datetime.now()
 
-        for exchange in self.market.values():
-            for ticker, screener in exchange.copy().items():
-                if isinstance(screener, (AutoScreener, AutoDataset)):
-                    self.screeners.append(screener)
+    if isinstance(cancel, dt.timedelta):
+        cancel = current_time + cancel
+    # end if
 
-                else:
-                    exchange.pop(ticker)
-                # end if
-            # end for
-        # end for
-    # end initialize_screeners
+    if isinstance(delay, dt.timedelta):
+        delay = delay.total_seconds()
+    # end if
 
-    def prepare_screeners(self) -> None:
-        """Initializes the screeners."""
+    delay = delay or 0
+    count = 0
 
-        if not (self.market and self.screeners):
-            self.initialize_screeners()
-        # end if
+    saved_screeners = screeners
+    checked_screeners = []
 
-        for screener in self.screeners:
-            path = self.dataset_path(
-                screener=screener, location=self.location
-            )
+    while True:
+        for screener in saved_screeners:
+            if isinstance(screener, BaseScreener):
+                checked_screeners.append(screener)
 
-            threading.Thread(
-                target=self.configure_screener_dataset,
-                kwargs=dict(
-                    screener=screener, path=path,
-                    length=self.length
-                )
-            ).start()
+            elif isinstance(screener, BaseMultiScreener):
+                checked_screeners.extend(screener.screeners)
+            # end if
         # end for
-    # end prepare_screeners
-
-    def start_screeners(
-            self,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
-    ) -> None:
-        """
-        Runs the data collection.
 
-        :param timeout: The valur to add a timeout to the process.
-        :param wait: The value to wait after starting to run the process.
-        """
-
-        self.prepare_screeners()
-
-        for screener in self.screeners:
-            threading.Thread(
-                target=screener.run,
-                kwargs=dict(
-                    timeout=timeout, wait=False, block=False
+        if (
+            (
+                not any(
+                    len(screener.market) == 0
+                    for screener in checked_screeners
                 )
-            ).start()
-        # end for
-
-        if isinstance(wait, dt.datetime):
-            wait = wait - dt.datetime.now()
+            ) or
+            (
+                (cancel is not None) and
+                ((current_time := dt.datetime.now()) > cancel)
+            )
+        ):
+            break
         # end if
 
-        if isinstance(wait, dt.timedelta):
-            wait = wait.total_seconds()
-        # end if
+        count += 1
 
-        if isinstance(wait, bool) and wait:
-            self.wait_for_initialization()
-
-        elif isinstance(wait, (int, float)):
-            time.sleep(wait)
+        if isinstance(delay, (int, float)) and (count > 0):
+            time.sleep(delay)
         # end if
-    # end start_screeners
-
-    def stop(self) -> None:
-        """Stops the screening process."""
-
-        self.saving = False
+    # end while
 
-        terminate_thread(self.saving_process)
-    # end stop
+    if stop and ((stop == count) or once):
+        for screener in checked_screeners:
+            screener.stop()
+        # end for
+    # end if
 
-    def terminate(self) -> None:
-        """Stops the screening process."""
+    return WaitingState(
+        screeners=screeners, delay=delay, count=count,
+        cancel=cancel, canceled=(cancel is None) or (current_time > cancel)
+    )
+# end wait_for_dynamic_initialization
 
-        self.running = False
+def wait_for_initialization(
+        *screeners: Union[BaseScreener, BaseMultiScreener],
+        delay: Optional[Union[Number, dt.timedelta]] = None,
+        once: Optional[bool] = False,
+        stop: Optional[Union[bool, int]] = False,
+        cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
 
-        self.stop()
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param once: The value to get data only once.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
 
-        for screener in self.screeners:
-            screener.terminate()
-        # end for
-    # end terminate
-
-    def blocking(self) -> bool:
-        """
-        returns the value of the process being blocked.
+    :returns: The total delay.
+    """
 
-        :return: The value.
-        """
+    return wait_for_dynamic_initialization(
+        screeners, delay=delay, once=once,
+        stop=stop, cancel=cancel
+    )
+# end wait_for_initialization
 
-        return self.block
-    # end blocking
+def wait_for_dynamic_update(
+        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]],
+        delay: Optional[Union[Number, dt.timedelta]] = None,
+        once: Optional[bool] = False,
+        stop: Optional[Union[bool, int]] = False,
+        cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
 
-    def save_dataset(self, screener: AutoDataCollector) -> None:
-        """
-        Saves the data of the screener.
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param once: The value to get data only once.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
 
-        :param screener: The screener object to save its data.
-        """
+    :returns: The total delay.
+    """
 
-        save_dataset(
-            dataset=screener.market,
-            path=self.dataset_path(
-                screener=screener, location=self.location
-            )
+    if cancel == 0:
+        cancel = None
+    # end if
+
+    if isinstance(cancel, (int, float)):
+        cancel = dt.timedelta(seconds=cancel)
+    # end if
+
+    current_time = dt.datetime.now()
+
+    if isinstance(cancel, dt.timedelta):
+        cancel = current_time + cancel
+    # end if
+
+    if isinstance(delay, dt.timedelta):
+        delay = delay.total_seconds()
+    # end if
+
+    delay = delay or 0
+    count = 0
+
+    if screeners:
+        wait_for_dynamic_initialization(
+            screeners, delay=delay, once=once
         )
-    # end save_dataset
 
-    def handle(self, screener: AutoDataCollector) -> None:
-        """
-        Handles the screener during the screening loop.
+        saved_screeners = screeners
+        checked_screeners = []
 
-        :param screener: The screener object.
-        """
+        for screener in saved_screeners:
+            if isinstance(screener, BaseScreener):
+                checked_screeners.append(screener)
 
-        if len(screener.market) == 0:
-            return
-        # end if
-
-        if (
-            dt.datetime.now() - screener.market.index[-1]
-        ).seconds >= self.cancel + (
-            interval_to_total_time(screener.interval)
-            if isinstance(screener, AutoDataset) else 0
-        ):
-            screener.terminate()
+            elif isinstance(screener, BaseMultiScreener):
+                checked_screeners.extend(screener.screeners)
+            # end if
+        # end for
 
-            self.stopped.append(screener)
-            self.screeners.remove(screener)
+        indexes = [
+            screener.market.index[-1]
+            for screener in checked_screeners
+        ]
 
-        else:
-            self.save_dataset(screener=screener)
-        # end if
-    # end handle
+        new_indexes = indexes
 
-    def run_loop(self) -> None:
-        """Runs the process of the price screening."""
+        length = len(tuple(checked_screeners))
 
-        self.running = True
+        while True:
+            for screener in saved_screeners:
+                if isinstance(screener, BaseScreener):
+                    checked_screeners.append(screener)
 
-        while self.running:
-            for screener in self.screeners.copy():
-                self.handle(screener=screener)
+                elif isinstance(screener, BaseMultiScreener):
+                    checked_screeners.extend(screener.screeners)
+                # end if
             # end for
 
-            delay = self.delay
-
-            if isinstance(self.delay, dt.timedelta):
-                delay = delay.total_seconds()
+            if (
+                all(
+                    indexes[i] != new_indexes[i]
+                    for i in range(length)
+                ) or
+                (
+                    (cancel is not None) and
+                    ((current_time := dt.datetime.now()) > cancel)
+                )
+            ):
+                break
             # end if
 
-            time.sleep(delay or 1)
-        # end while
-    # end run_loop
+            count += 1
 
-    def timeout(
-            self, duration: Union[Number, dt.timedelta, dt.datetime]
-    ) -> threading.Thread:
-        """
-        Runs a timeout for the process.
-
-        :param duration: The duration of the timeout.
+            new_indexes = [
+                screener.market.index[-1]
+                for screener in checked_screeners
+            ]
 
-        :return: The timeout process.
-        """
+            if isinstance(delay, (int, float)) and (count > 0):
+                time.sleep(delay)
+            # end if
+        # end while
 
-        if isinstance(duration, dt.datetime):
-            duration = duration - dt.datetime.now()
+        if stop and ((stop == count) or once):
+            for screener in checked_screeners:
+                screener.stop()
+            # end for
         # end if
+    # end if
 
-        if isinstance(duration, dt.timedelta):
-            duration = duration.total_seconds()
-        # end if
+    return WaitingState(
+        screeners=screeners, delay=delay, count=count, cancel=cancel,
+        canceled=(cancel is None) or (current_time > cancel)
+    )
+# end wait_for_dynamic_update
 
-        self.timeout_process = threading.Thread(
-            target=lambda: (time.sleep(duration), self.stop())
-        )
+def wait_for_update(
+        *screeners: Union[BaseScreener, BaseMultiScreener],
+        delay: Optional[Union[Number, dt.timedelta]] = None,
+        once: Optional[bool] = False,
+        stop: Optional[Union[bool, int]] = False,
+        cancel: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
 
-        self.timeout_process.start()
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param once: The value to get data only once.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
 
-        return self.timeout_process
-    # end timeout
+    :returns: The total delay.
+    """
 
-    def run(
-            self,
-            save: Optional[bool] = True,
-            block: Optional[bool] = False,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
-    ) -> Optional[threading.Thread]:
-        """
-        Runs the process of the price screening.
+    return wait_for_dynamic_update(
+        screeners, delay=delay, once=once,
+        stop=stop, cancel=cancel
+    )
+# end wait_for_update
 
-        :param save: The value to save the data.
-        :param block: The value to block the execution.
-        :param timeout: The valur to add a timeout to the process.
-        :param wait: The value to wait after starting to run the process.
-        """
+def live_screeners(
+        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
+) -> List[Union[BaseScreener, BaseMultiScreener]]:
+    """
+    Returns a list of all the live create_screeners.
 
-        self.start_screeners(timeout=timeout, wait=wait)
+    :param screeners: The create_screeners to search from.
 
-        if save:
-            self.saving = True
+    :return: A list the live create_screeners.
+    """
 
-            self.saving_process = threading.Thread(
-                target=self.run_loop
+    return [
+        screener for screener in screeners
+        if (
+            screener.running and (
+                isinstance(screener, BaseMultiScreener) or
+                len(screener.market) > 0
             )
+        )
+    ]
+# end live_screeners
 
-            self.saving_process.start()
-        # end if
+def structure_screeners(
+        screeners: Iterable[BaseScreener]
+) -> Dict[str, Dict[str, List[BaseScreener]]]:
+    """
+    Structures the screener objects by exchanges and symbols
 
-        if timeout:
-            self.timeout(timeout)
-        # end if
+    :param screeners: The screeners to structure.
 
-        if block:
-            self.block = block
+    :return: The structure of the screeners.
+    """
 
-            while self.blocking() and self.running:
-                pass
-            # end while
-        # end if
+    structure: Dict[str, Dict[str, List[BaseScreener]]] = {}
 
-        if save:
-            return self.saving_process
-        # end if
-    # end run
-# end Screener
+    for screener in screeners:
+        (
+            structure.
+            setdefault(screener.exchange, {}).
+            setdefault(screener.symbol, [])
+        ).append(screener)
+    # end for
+
+    return structure
+# end structure_screeners
```

### Comparing `auto-screener-0.0.9/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.1.0/auto_screener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.9
+Version: 0.1.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.9/auto_screener.egg-info/SOURCES.txt` & `auto-screener-0.1.0/auto_screener.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 MANIFEST.in
 README.md
 build.py
 pyproject.toml
+requirements-dev.txt
 requirements.txt
 setup.py
-test.py
-auto_screener/__init__.py
 auto_screener/base.py
 auto_screener/collect.py
 auto_screener/dataset.py
 auto_screener/document.py
+auto_screener/exchanges.py
+auto_screener/feed.py
 auto_screener/hints.py
 auto_screener/interval.py
-auto_screener/progress.py
+auto_screener/screener.py
 auto_screener/screening.py
-auto_screener/tickers.py
+auto_screener/symbols.py
 auto_screener.egg-info/PKG-INFO
 auto_screener.egg-info/SOURCES.txt
 auto_screener.egg-info/dependency_links.txt
 auto_screener.egg-info/requires.txt
 auto_screener.egg-info/top_level.txt
```

### Comparing `auto-screener-0.0.9/build.py` & `auto-screener-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.9/pyproject.toml` & `auto-screener-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.0.9'
+version = '0.1.0'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.0.9/setup.py` & `auto-screener-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,18 @@
     setup(
         package="auto_screener",
         project="pyproject.toml",
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
-        include=[
-            "test.py",
-            "auto_screener/source"
-        ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.0.9',
+        version='0.1.0',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

