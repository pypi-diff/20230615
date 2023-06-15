# Comparing `tmp/breeze_strategies-2.0.tar.gz` & `tmp/breeze_strategies-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-2.0.tar", last modified: Thu Jun 15 08:13:26 2023, max compression
+gzip compressed data, was "breeze_strategies-3.0.tar", last modified: Thu Jun 15 09:16:12 2023, max compression
```

## Comparing `breeze_strategies-2.0.tar` & `breeze_strategies-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:13:26.006896 breeze_strategies-2.0/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-2.0/LICENSE
--rw-rw-rw-   0        0        0     1103 2023-06-15 08:13:26.005554 breeze_strategies-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 08:11:56.000000 breeze_strategies-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 08:13:25.943369 breeze_strategies-2.0/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-2.0/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    18726 2023-06-15 08:12:02.000000 breeze_strategies-2.0/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:13:25.998040 breeze_strategies-2.0/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1103 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 08:13:25.000000 breeze_strategies-2.0/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 08:13:26.007906 breeze_strategies-2.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-06-15 08:11:49.000000 breeze_strategies-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.468001 breeze_strategies-3.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-3.0/LICENSE
+-rw-rw-rw-   0        0        0     1544 2023-06-15 09:16:12.466817 breeze_strategies-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-06-15 09:11:25.000000 breeze_strategies-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.392958 breeze_strategies-3.0/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-3.0/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    19226 2023-06-15 09:05:32.000000 breeze_strategies-3.0/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.462669 breeze_strategies-3.0/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1544 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:16:12.468001 breeze_strategies-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-06-15 09:15:36.000000 breeze_strategies-3.0/setup.py
```

### Comparing `breeze_strategies-2.0/LICENSE` & `breeze_strategies-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-2.0/breeze_strategies/breeze_strategies.py` & `breeze_strategies-3.0/breeze_strategies/breeze_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,19 @@
         self.putlock = threading.Lock()
         self.currentcall = 0
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
         self.client.ws_connect()
+        self.quantity = 0
     
-    def squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity):
+    def squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right = None, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity):
         data = self.client.square_off(exchange_code=exchange_code,
-                            product_type="options",
+                            product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
                             right=rightval,
                             strike_price=strike_price,
                             action=action,
                             order_type=order_type,
                             validity=validity,
@@ -66,15 +67,15 @@
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
     def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, executed_price,flag):
         #print(f"current call is {self.currentcall} Rs and current put is {self.currentput} Rs")
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
-        print(f"net gain/loss received : {net_gain_loss} Rs with call gain per quantity :{self.currentcall} Rs and with put gain per quantity: {self.currentput} Rs")
+        print(f"net gain/loss received : {net_gain_loss} Rs \n call gain per quantity :{self.currentcall} Rs \n put gain per quantity: {self.currentput} Rs")
         
         formatted_date = self.get_date_format(expiry_date)
         
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
@@ -101,40 +102,40 @@
         formatted_date = self.get_date_format(expiry_date)
         
         def on_ticks2(data):
             resultcall.append(data)
             with self.calllock:
                 #while(result!=[]):
                 value = resultcall.pop(0)
-                print(f"Call : current market value of call order is {value['last']} Rs and executed price : {value['last']}")
-                self.currentcall = float(value['last']) - float(executed_price)
+                print(f"{rightval} : current market value of call order is {value['last']}/- Rs and executed price : {executed_price}/- Rs")
+                self.currentcall = round(float(value['last']) - float(executed_price),2)
                 #print(f"current market value of call order is {value} Rs, The difference between current put price and executed price is {self.currentcall}")
                 if(self.flag == False):
                     self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
-                #time.sleep(2)
+                time.sleep(2)
                 
         self.client.on_ticks2 = on_ticks2
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
          
     async def calculate_current_put(self,product_type,rightval,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag):
         print(f"inside current put method():{rightval}")
         result = []
         formatted_date = self.get_date_format(expiry_date)
         
         def on_ticks(data):
             result.append(data)
             with self.putlock:
                 
                 value = result.pop(0)
-                print(f"Put : current market value of call order is {value['last']} Rs and executed price : {value['last']}")
-                self.currentput = float(value['last']) - float(executed_price)
+                print(f"Put : current market value of put order is {value['last']} Rs and executed price : {executed_price}")
+                self.currentput = round(float(value['last']) - float(executed_price),2)
                 #print(f"current market value of put order is {value} Rs , The difference between current put price and executed price is {self.currentput}")
                 if(self.flag == False):
                     self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
-                #time.sleep(2)
+                time.sleep(2)
         
         self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
         
     def profit_and_loss2(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
         #self.calculate_current_call(product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,flag = False)
         #self.calculate_current_put(product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,put_execution,flag = False)
@@ -157,14 +158,15 @@
         #task2 = asyncio.create_task(perform_operation2())
 
         # Wait for all tasks to complete
         await asyncio.gather(p1, p2)
         
         
     async def long_straddle(self, stock_code, strike_price, qty, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+        self.quantity = qty
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
                     action = "buy",
                     order_type=order_type,
@@ -300,8 +302,17 @@
                     print("put order could not execute due to some reason so cancelling order")
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 await self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
-            
+            
+    def stop(self):
+        self.client.ws_disconnect()
+
+    def get_pnl(self):
+        print("- Negative indicates loss")
+        print(f"current call gain/loss per qty {self.currentcall} Rs")
+        print(f"current put gain/loss per qty {self.currentput} Rs")
+        outcome = (self.currentcall + self.currentput)*int(self.quantity)
+        print(f"Total Profit/Loss for {self.quantity} is {outcome} Rs")
```

### Comparing `breeze_strategies-2.0/setup.py` & `breeze_strategies-3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="2.0",
+    version="3.0",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

