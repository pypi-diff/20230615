# Comparing `tmp/breeze_strategies-1.0.tar.gz` & `tmp/breeze_strategies-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.tar", last modified: Thu Jun 15 05:48:51 2023, max compression
+gzip compressed data, was "breeze_strategies-2.0.tar", last modified: Thu Jun 15 08:13:26 2023, max compression
```

## Comparing `breeze_strategies-1.0.tar` & `breeze_strategies-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 05:48:51.663624 breeze_strategies-1.0/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-1.0/LICENSE
--rw-rw-rw-   0        0        0     1103 2023-06-15 05:48:51.662623 breeze_strategies-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 05:44:05.000000 breeze_strategies-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 05:48:51.591861 breeze_strategies-1.0/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:35:19.000000 breeze_strategies-1.0/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    18708 2023-06-15 05:44:49.000000 breeze_strategies-1.0/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:48:51.659559 breeze_strategies-1.0/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1103 2023-06-15 05:48:51.000000 breeze_strategies-1.0/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-15 05:48:51.000000 breeze_strategies-1.0/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 05:48:51.000000 breeze_strategies-1.0/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-15 05:48:51.000000 breeze_strategies-1.0/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 05:48:51.000000 breeze_strategies-1.0/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 05:48:51.663624 breeze_strategies-1.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-06-15 05:42:49.000000 breeze_strategies-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:26.006896 breeze_strategies-2.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-2.0/LICENSE
+-rw-rw-rw-   0        0        0     1103 2023-06-15 08:13:26.005554 breeze_strategies-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-15 08:11:56.000000 breeze_strategies-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:25.943369 breeze_strategies-2.0/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-2.0/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18726 2023-06-15 08:12:02.000000 breeze_strategies-2.0/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:13:25.998040 breeze_strategies-2.0/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1103 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:13:26.007906 breeze_strategies-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-06-15 08:11:49.000000 breeze_strategies-2.0/setup.py
```

### Comparing `breeze_strategies-1.0/LICENSE` & `breeze_strategies-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0/PKG-INFO` & `breeze_strategies-2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 1.0
+Version: 2.0
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0
+pip install breeze_strategies==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-1.0/README.md` & `breeze_strategies-2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0
+pip install breeze_strategies==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-1.0/breeze_strategies/breeze_strategies.py` & `breeze_strategies-2.0/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,47 +96,47 @@
             self.flag = True
             
     async def calculate_current_call(self,product_type,rightval,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag):
         print(f"inside current call() method:{rightval}")
         resultcall = []
         formatted_date = self.get_date_format(expiry_date)
         
-        def ticks2(data):
+        def on_ticks2(data):
             resultcall.append(data)
             with self.calllock:
                 #while(result!=[]):
                 value = resultcall.pop(0)
                 print(f"Call : current market value of call order is {value['last']} Rs and executed price : {value['last']}")
                 self.currentcall = float(value['last']) - float(executed_price)
                 #print(f"current market value of call order is {value} Rs, The difference between current put price and executed price is {self.currentcall}")
                 if(self.flag == False):
                     self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
                 #time.sleep(2)
                 
-        self.client.ticks2 = ticks2
+        self.client.on_ticks2 = on_ticks2
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
          
     async def calculate_current_put(self,product_type,rightval,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag):
         print(f"inside current put method():{rightval}")
         result = []
         formatted_date = self.get_date_format(expiry_date)
         
-        def ticks(data):
+        def on_ticks(data):
             result.append(data)
             with self.putlock:
                 
                 value = result.pop(0)
                 print(f"Put : current market value of call order is {value['last']} Rs and executed price : {value['last']}")
                 self.currentput = float(value['last']) - float(executed_price)
                 #print(f"current market value of put order is {value} Rs , The difference between current put price and executed price is {self.currentput}")
                 if(self.flag == False):
                     self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
                 #time.sleep(2)
         
-        self.client.ticks = ticks
+        self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
         
     def profit_and_loss2(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
         #self.calculate_current_call(product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,flag = False)
         #self.calculate_current_put(product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,put_execution,flag = False)
         p1  =  mp.Process(target = self.calculate_current_call, args = (product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, False))
         p2  =  mp.Process(target = self.calculate_current_put, args = (product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, put_execution, False))
```

### Comparing `breeze_strategies-1.0/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-2.0/breeze_strategies.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 1.0
+Version: 2.0
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0
+pip install breeze_strategies==2.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-1.0/setup.py` & `breeze_strategies-2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0",
+    version="2.0",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

