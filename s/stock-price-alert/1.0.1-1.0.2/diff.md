# Comparing `tmp/stock_price_alert-1.0.1-py3-none-any.whl.zip` & `tmp/stock_price_alert-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,8 @@
-Zip file size: 2152 bytes, number of entries: 4
--rw-rw-rw-  2.0 fat     3128 b- defN 23-Jun-15 20:10 stock_price_alert-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 20:10 stock_price_alert-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-15 20:10 stock_price_alert-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      337 b- defN 23-Jun-15 20:10 stock_price_alert-1.0.1.dist-info/RECORD
-4 files, 3558 bytes uncompressed, 1490 bytes compressed:  58.1%
+Zip file size: 3426 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-15 19:23 stockpricealert/__init.__.py
+-rw-rw-rw-  2.0 fat     2486 b- defN 23-Jun-15 19:21 stockpricealert/bot.py
+-rw-rw-rw-  2.0 fat     3128 b- defN 23-Jun-15 20:28 stock_price_alert-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 20:28 stock_price_alert-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-15 20:28 stock_price_alert-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      501 b- defN 23-Jun-15 20:28 stock_price_alert-1.0.2.dist-info/RECORD
+6 files, 6490 bytes uncompressed, 2512 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
-Filename: stock_price_alert-1.0.1.dist-info/METADATA
+Filename: stockpricealert/__init.__.py
 Comment: 
 
-Filename: stock_price_alert-1.0.1.dist-info/WHEEL
+Filename: stockpricealert/bot.py
 Comment: 
 
-Filename: stock_price_alert-1.0.1.dist-info/top_level.txt
+Filename: stock_price_alert-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: stock_price_alert-1.0.1.dist-info/RECORD
+Filename: stock_price_alert-1.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: stock_price_alert-1.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: stock_price_alert-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stock_price_alert-1.0.1.dist-info/METADATA` & `stock_price_alert-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-price-alert
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for retrieving stock prices and setting price alerts
 Home-page: https://github.com/piritheeviraman/stock-price-alert-lib
 Author: piritheevi
 Author-email: gkappdeveloper@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

