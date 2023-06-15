# Comparing `tmp/coindicator-2.0.4.linux-x86_64.tar.gz` & `tmp/coindicator-2.0.5.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.0.4.linux-x86_64.tar", last modified: Thu Jun 15 14:47:48 2023, max compression
+gzip compressed data, was "coindicator-2.0.5.linux-x86_64.tar", last modified: Thu Jun 15 14:52:47 2023, max compression
```

## Comparing `coindicator-2.0.4.linux-x86_64.tar` & `coindicator-2.0.5.linux-x86_64.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./home/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./home/sander/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./home/sander/code/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./home/sander/code/coinprice-indicator/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.333449 ./home/sander/code/coinprice-indicator/venv/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.333449 ./home/sander/code/coinprice-indicator/venv/bin/
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1016 2023-06-15 14:47:48.333449 ./home/sander/code/coinprice-indicator/venv/bin/coindicator
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.197448 ./home/sander/code/coinprice-indicator/venv/lib/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.201448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.269448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.217448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.651798 ./
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.651798 ./home/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.651798 ./home/sander/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.651798 ./home/sander/code/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.655798 ./home/sander/code/coinprice-indicator/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.803799 ./home/sander/code/coinprice-indicator/venv/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.803799 ./home/sander/code/coinprice-indicator/venv/bin/
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1016 2023-06-15 14:52:47.803799 ./home/sander/code/coinprice-indicator/venv/bin/coindicator
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.655798 ./home/sander/code/coinprice-indicator/venv/lib/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.655798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.735798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.671798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/
 -rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__init__.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.265448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/
--rw-rw-r--   0 sander    (1000) sander    (1000)      197 2023-06-15 14:47:48.261448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     3826 2023-06-15 14:47:48.261448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/about.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)    11508 2023-06-15 14:47:48.253448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/alarm.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)    11146 2023-06-15 14:47:48.217448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/asset_selection.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)    20848 2023-06-15 14:47:48.261448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/coin.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     3406 2023-06-15 14:47:48.265448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/coingecko_client.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     1917 2023-06-15 14:47:48.249448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/config.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     3235 2023-06-15 14:47:48.241448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/downloader.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2580 2023-06-15 14:47:48.221448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/error.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)    15966 2023-06-15 14:47:48.241448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/exchange.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)    16848 2023-06-15 14:47:48.245448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/indicator.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     5810 2023-06-15 14:47:48.249448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/plugin_selection.cpython-311.pyc
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.723798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/
+-rw-rw-r--   0 sander    (1000) sander    (1000)      197 2023-06-15 14:52:47.723798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3826 2023-06-15 14:52:47.723798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/about.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)    11508 2023-06-15 14:52:47.711798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/alarm.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)    11146 2023-06-15 14:52:47.671798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/asset_selection.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)    20848 2023-06-15 14:52:47.719798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/coin.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3406 2023-06-15 14:52:47.723798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/coingecko_client.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1917 2023-06-15 14:52:47.707798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/config.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3235 2023-06-15 14:52:47.695798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/downloader.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2580 2023-06-15 14:52:47.671798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/error.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)    15966 2023-06-15 14:52:47.695798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/exchange.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)    16848 2023-06-15 14:52:47.703798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/indicator.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5810 2023-06-15 14:52:47.707798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/__pycache__/plugin_selection.cpython-311.pyc
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2022-11-16 17:06:14.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/about.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/alarm.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/asset_selection.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)    12669 2023-06-15 14:37:39.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/coin.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1679 2023-06-15 14:42:47.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/coingecko_client.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/config.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)      977 2022-11-16 17:07:14.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/config.yaml
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/downloader.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/error.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)    10512 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.221448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.237448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/
--rw-rw-r--   0 sander    (1000) sander    (1000)     2778 2023-06-15 14:47:48.229448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/binance.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2479 2023-06-15 14:47:48.237448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitfinex.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2969 2023-06-15 14:47:48.233448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitkub.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2577 2023-06-15 14:47:48.225448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitstamp.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2474 2023-06-15 14:47:48.225448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bittrex.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2550 2023-06-15 14:47:48.221448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/cexio.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2790 2023-06-15 14:47:48.229448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/gemini.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2725 2023-06-15 14:47:48.221448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/hitbtc.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     3093 2023-06-15 14:47:48.225448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/kraken.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2237 2023-06-15 14:47:48.229448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/okcoin.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2460 2023-06-15 14:47:48.233448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/poloniex.cpython-311.pyc
--rw-rw-r--   0 sander    (1000) sander    (1000)     2270 2023-06-15 14:47:48.233448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/unocoin.cpython-311.pyc
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.675798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.687798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2778 2023-06-15 14:52:47.683798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/binance.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2479 2023-06-15 14:52:47.687798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitfinex.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2969 2023-06-15 14:52:47.683798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitkub.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2577 2023-06-15 14:52:47.679798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bitstamp.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2474 2023-06-15 14:52:47.675798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/bittrex.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2550 2023-06-15 14:52:47.675798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/cexio.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2790 2023-06-15 14:52:47.683798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/gemini.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2725 2023-06-15 14:52:47.675798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/hitbtc.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3093 2023-06-15 14:52:47.679798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/kraken.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2237 2023-06-15 14:52:47.679798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/okcoin.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2460 2023-06-15 14:52:47.687798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/poloniex.cpython-311.pyc
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2270 2023-06-15 14:52:47.687798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/__pycache__/unocoin.cpython-311.pyc
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/binance.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/bitfinex.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/bitkub.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/bitstamp.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2022-11-16 17:02:06.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/bittrex.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/cexio.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/gemini.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/hitbtc.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/kraken.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/okcoin.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/poloniex.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/exchanges/unocoin.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/indicator.py
 -rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.209448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.663798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/
 -rwxrwxr-x   0 sander    (1000) sander    (1000)   294232 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/ca-ching.wav
 -rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/icon.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/icon_32px.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/icon_48px.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/icon_64px.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/loading.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/logo_124px.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/logo_124pxs.png
 -rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:47:48.273448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4489 2023-06-15 14:47:48.125447 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1373 2023-06-15 14:47:48.169448 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-15 14:47:48.125447 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-15 14:47:48.125447 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2022-10-30 18:46:33.906658 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      212 2023-06-15 14:47:48.125447 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-15 14:47:48.125447 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-15 14:52:47.739798 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4584 2023-06-15 14:52:47.443796 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1373 2023-06-15 14:52:47.491797 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-15 14:52:47.443796 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-15 14:52:47.443796 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2022-10-30 18:46:33.906658 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-15 14:52:47.443796 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-15 14:52:47.443796 ./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/top_level.txt
```

### ./home/sander/code/coinprice-indicator/venv/bin/coindicator

```diff
@@ -1,14 +1,14 @@
 #!/home/sander/code/coinprice-indicator/venv/bin/python3
-# EASY-INSTALL-ENTRY-SCRIPT: 'coindicator==2.0.4','console_scripts','coindicator'
+# EASY-INSTALL-ENTRY-SCRIPT: 'coindicator==2.0.5','console_scripts','coindicator'
 import re
 import sys
 
 # for compatibility with easy_install; see #2198
-__requires__ = 'coindicator==2.0.4'
+__requires__ = 'coindicator==2.0.5'
 
 try:
     from importlib.metadata import distribution
 except ImportError:
     try:
         from importlib_metadata import distribution
     except ImportError:
@@ -26,8 +26,8 @@
 
 
 globals().setdefault('load_entry_point', importlib_load_entry_point)
 
 
 if __name__ == '__main__':
     sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
-    sys.exit(load_entry_point('coindicator==2.0.4', 'console_scripts', 'coindicator')())
+    sys.exit(load_entry_point('coindicator==2.0.5', 'console_scripts', 'coindicator')())
```

### Comparing `./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/PKG-INFO` & `./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.0.4
+Version: 2.0.5
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
@@ -78,14 +78,19 @@
 
 ## Extending (Plug-ins)
 
 Adding your own exchange plug-in is easy. Just create class file with methods for returning a ticker URL, a discovery URL, and parsing the responses from the ticker and discovery APIs. Then add the file to the `exchanges` folder.
 
 Have a peek at the existing plug-ins (e.g. **kraken.py**) for an example and don't forget to contribute your plug-ins here on GitHub!
 
+## Building
+
+- Activate environment
+- run pip install -e .[develop] to install required tools
+
 ## Troubleshooting
 
 This software was tested and found working on the following configurations:
 * Ubuntu Linux 16.04 (Xenial Xurus) with Unity 7
 * Ubuntu Linux 17.10 (Artful Aardvark) with GNOME 3 and Unity 7
 * Ubuntu Linux 18.04 (Bionic Beaver) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.04 (Disco Dingo) with GNOME 3 and Unity 7
```

### Comparing `./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.4.egg-info/SOURCES.txt` & `./home/sander/code/coinprice-indicator/venv/lib/python3.11/site-packages/coindicator-2.0.5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

