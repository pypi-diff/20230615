# Comparing `tmp/byquant-1.5.30.tar.gz` & `tmp/byquant-1.6.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.5.30.tar", last modified: Tue May 30 01:03:20 2023, max compression
+gzip compressed data, was "byquant-1.6.15.tar", last modified: Thu Jun 15 06:01:34 2023, max compression
```

## Comparing `byquant-1.5.30.tar` & `byquant-1.6.15.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 01:03:20.596186 byquant-1.5.30/
--rw-rw-rw-   0        0        0     1266 2023-05-30 01:03:20.594190 byquant-1.5.30/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.5.30/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 01:03:20.176876 byquant-1.5.30/byquant/
--rw-rw-rw-   0        0        0    21857 2023-05-17 05:50:41.000000 byquant-1.5.30/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:03:20.590247 byquant-1.5.30/byquant/exchange/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.5.30/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.5.30/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264349 2023-05-17 05:18:59.000000 byquant-1.5.30/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.5.30/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:03:20.194753 byquant-1.5.30/byquant.egg-info/
--rw-rw-rw-   0        0        0     1266 2023-05-30 01:03:20.000000 byquant-1.5.30/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3413 2023-05-30 01:03:20.000000 byquant-1.5.30/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 01:03:20.000000 byquant-1.5.30/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 01:03:20.000000 byquant-1.5.30/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 01:03:20.000000 byquant-1.5.30/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.5.30/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0       97 2023-05-30 01:02:36.000000 byquant-1.5.30/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 01:03:20.596312 byquant-1.5.30/setup.cfg
--rw-rw-rw-   0        0        0     2682 2023-05-30 01:01:20.000000 byquant-1.5.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.588982 byquant-1.6.15/
+-rw-rw-rw-   0        0        0     1266 2023-06-15 06:01:34.588982 byquant-1.6.15/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.15/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.141578 byquant-1.6.15/byquant/
+-rw-rw-rw-   0        0        0    21857 2023-05-17 05:50:41.000000 byquant-1.6.15/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.588982 byquant-1.6.15/byquant/exchange/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.15/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.15/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.15/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.162793 byquant-1.6.15/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1266 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3413 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.15/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       97 2023-06-15 05:53:38.000000 byquant-1.6.15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:01:34.588982 byquant-1.6.15/setup.cfg
+-rw-rw-rw-   0        0        0     2682 2023-06-15 05:51:16.000000 byquant-1.6.15/setup.py
```

### Comparing `byquant-1.5.30/PKG-INFO` & `byquant-1.6.15/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.5.30
+Version: 1.6.15
 Summary: A Python trading library with support for 130+ exchanges
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: algorithmic,algotrading
```

### Comparing `byquant-1.5.30/byquant/__init__.py` & `byquant-1.6.15/byquant/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/ace.py` & `byquant-1.6.15/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/alpaca.py` & `byquant-1.6.15/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/ascendex.py` & `byquant-1.6.15/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bequant.py` & `byquant-1.6.15/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bigone.py` & `byquant-1.6.15/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/binance.py` & `byquant-1.6.15/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/binancecoinm.py` & `byquant-1.6.15/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/binanceus.py` & `byquant-1.6.15/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/binanceusdm.py` & `byquant-1.6.15/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bit2c.py` & `byquant-1.6.15/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitbank.py` & `byquant-1.6.15/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitbns.py` & `byquant-1.6.15/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitfinex.py` & `byquant-1.6.15/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitfinex2.py` & `byquant-1.6.15/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitflyer.py` & `byquant-1.6.15/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitforex.py` & `byquant-1.6.15/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitget.py` & `byquant-1.6.15/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bithumb.py` & `byquant-1.6.15/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitmart.py` & `byquant-1.6.15/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitmex.py` & `byquant-1.6.15/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitopro.py` & `byquant-1.6.15/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitpanda.py` & `byquant-1.6.15/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitrue.py` & `byquant-1.6.15/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitso.py` & `byquant-1.6.15/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitstamp.py` & `byquant-1.6.15/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitstamp1.py` & `byquant-1.6.15/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bittrex.py` & `byquant-1.6.15/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bitvavo.py` & `byquant-1.6.15/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bkex.py` & `byquant-1.6.15/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bl3p.py` & `byquant-1.6.15/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/blockchaincom.py` & `byquant-1.6.15/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btcalpha.py` & `byquant-1.6.15/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btcbox.py` & `byquant-1.6.15/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btcex.py` & `byquant-1.6.15/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btcmarkets.py` & `byquant-1.6.15/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btctradeua.py` & `byquant-1.6.15/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/btcturk.py` & `byquant-1.6.15/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/buda.py` & `byquant-1.6.15/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/bybit.py` & `byquant-1.6.15/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/cex.py` & `byquant-1.6.15/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinbase.py` & `byquant-1.6.15/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinbaseprime.py` & `byquant-1.6.15/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinbasepro.py` & `byquant-1.6.15/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coincheck.py` & `byquant-1.6.15/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinex.py` & `byquant-1.6.15/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinfalcon.py` & `byquant-1.6.15/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinmate.py` & `byquant-1.6.15/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinone.py` & `byquant-1.6.15/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinsph.py` & `byquant-1.6.15/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/coinspot.py` & `byquant-1.6.15/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/cryptocom.py` & `byquant-1.6.15/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/currencycom.py` & `byquant-1.6.15/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/delta.py` & `byquant-1.6.15/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/deribit.py` & `byquant-1.6.15/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/digifinex.py` & `byquant-1.6.15/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/exmo.py` & `byquant-1.6.15/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/flowbtc.py` & `byquant-1.6.15/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/fmfwio.py` & `byquant-1.6.15/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/gate.py` & `byquant-1.6.15/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/gemini.py` & `byquant-1.6.15/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/hitbtc.py` & `byquant-1.6.15/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/hitbtc3.py` & `byquant-1.6.15/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/hollaex.py` & `byquant-1.6.15/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/huobi.py` & `byquant-1.6.15/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/huobijp.py` & `byquant-1.6.15/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/huobipro.py` & `byquant-1.6.15/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/idex.py` & `byquant-1.6.15/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/independentreserve.py` & `byquant-1.6.15/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/indodax.py` & `byquant-1.6.15/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/itbit.py` & `byquant-1.6.15/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/kraken.py` & `byquant-1.6.15/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/krakenfutures.py` & `byquant-1.6.15/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/kucoin.py` & `byquant-1.6.15/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/kucoinfutures.py` & `byquant-1.6.15/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/kuna.py` & `byquant-1.6.15/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/latoken.py` & `byquant-1.6.15/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/lbank.py` & `byquant-1.6.15/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/lbank2.py` & `byquant-1.6.15/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/luno.py` & `byquant-1.6.15/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/lykke.py` & `byquant-1.6.15/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/mercado.py` & `byquant-1.6.15/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/mexc.py` & `byquant-1.6.15/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/ndax.py` & `byquant-1.6.15/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/novadax.py` & `byquant-1.6.15/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/oceanex.py` & `byquant-1.6.15/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/okcoin.py` & `byquant-1.6.15/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/okx.py` & `byquant-1.6.15/byquant/exchange/okx.py`

 * *Files 0% similar despite different names*

```diff
@@ -837,15 +837,16 @@
                     'option': 'OPTION',
                     'SPOT': 'SPOT',
                     'MARGIN': 'MARGIN',
                     'SWAP': 'SWAP',
                     'FUTURES': 'FUTURES',
                     'OPTION': 'OPTION',
                 },
-                'brokerId': 'badf77d98a0bBCDE',  #Uakee
+                #'brokerId': 'badf77d98a0bBCDE',
+                'brokerId': 'f09cb09d13b0BCDE',  # Uakee
             },
             'commonCurrencies': {
                 # the exchange refers to ERC20 version of Aeternity(AEToken)
                 'AE': 'AET',  # https://github.com/ccxt/ccxt/issues/4981
                 'BOX': 'DefiBox',
                 'HOT': 'Hydro Protocol',
                 'HSR': 'HC',
```

### Comparing `byquant-1.5.30/byquant/exchange/paymium.py` & `byquant-1.6.15/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/phemex.py` & `byquant-1.6.15/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/poloniex.py` & `byquant-1.6.15/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/poloniexfutures.py` & `byquant-1.6.15/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/probit.py` & `byquant-1.6.15/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/ripio.py` & `byquant-1.6.15/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/stex.py` & `byquant-1.6.15/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/tidex.py` & `byquant-1.6.15/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/timex.py` & `byquant-1.6.15/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/tokocrypto.py` & `byquant-1.6.15/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/upbit.py` & `byquant-1.6.15/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/wavesexchange.py` & `byquant-1.6.15/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/wazirx.py` & `byquant-1.6.15/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/whitebit.py` & `byquant-1.6.15/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/woo.py` & `byquant-1.6.15/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/xt.py` & `byquant-1.6.15/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/yobit.py` & `byquant-1.6.15/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/zaif.py` & `byquant-1.6.15/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/zb.py` & `byquant-1.6.15/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant/exchange/zonda.py` & `byquant-1.6.15/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/byquant.egg-info/PKG-INFO` & `byquant-1.6.15/byquant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.5.30
+Version: 1.6.15
 Summary: A Python trading library with support for 130+ exchanges
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
 Keywords: algorithmic,algotrading
```

### Comparing `byquant-1.5.30/byquant.egg-info/SOURCES.txt` & `byquant-1.6.15/byquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byquant-1.5.30/setup.py` & `byquant-1.6.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.5.30",
+  "version": "1.6.15",
   "description": "A Python trading library with support for 130+ exchanges",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
```

