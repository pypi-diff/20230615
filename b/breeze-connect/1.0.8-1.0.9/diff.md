# Comparing `tmp/breeze_connect-1.0.8.tar.gz` & `tmp/breeze_connect-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_connect-1.0.8.tar", last modified: Mon Jan 31 04:45:32 2022, max compression
+gzip compressed data, was "breeze_connect-1.0.9.tar", last modified: Mon Jan 31 05:23:18 2022, max compression
```

## Comparing `breeze_connect-1.0.8.tar` & `breeze_connect-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 04:45:32.087992 breeze_connect-1.0.8/
--rw-rw-r--   0 oneture   (1000) oneture   (1000)      695 2022-01-31 04:45:32.087992 breeze_connect-1.0.8/PKG-INFO
--rw-rw-r--   0 oneture   (1000) oneture   (1000)      228 2021-12-20 10:37:29.000000 breeze_connect-1.0.8/README.md
-drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 04:45:32.087992 breeze_connect-1.0.8/breeze_connect/
--rw-rw-r--   0 oneture   (1000) oneture   (1000)       56 2022-01-31 04:24:00.000000 breeze_connect-1.0.8/breeze_connect/__init__.py
--rw-rw-r--   0 oneture   (1000) oneture   (1000)    42108 2022-01-31 04:38:49.000000 breeze_connect-1.0.8/breeze_connect/breeze_connect.py
-drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 04:45:32.087992 breeze_connect-1.0.8/breeze_connect.egg-info/
--rw-rw-r--   0 oneture   (1000) oneture   (1000)      695 2022-01-31 04:45:31.000000 breeze_connect-1.0.8/breeze_connect.egg-info/PKG-INFO
--rw-rw-r--   0 oneture   (1000) oneture   (1000)      267 2022-01-31 04:45:32.000000 breeze_connect-1.0.8/breeze_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 oneture   (1000) oneture   (1000)        1 2022-01-31 04:45:31.000000 breeze_connect-1.0.8/breeze_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 oneture   (1000) oneture   (1000)       33 2022-01-31 04:45:31.000000 breeze_connect-1.0.8/breeze_connect.egg-info/requires.txt
--rw-rw-r--   0 oneture   (1000) oneture   (1000)       15 2022-01-31 04:45:31.000000 breeze_connect-1.0.8/breeze_connect.egg-info/top_level.txt
--rw-rw-r--   0 oneture   (1000) oneture   (1000)       38 2022-01-31 04:45:32.087992 breeze_connect-1.0.8/setup.cfg
--rw-rw-r--   0 oneture   (1000) oneture   (1000)      720 2022-01-31 04:44:28.000000 breeze_connect-1.0.8/setup.py
+drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 05:23:18.877447 breeze_connect-1.0.9/
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)      695 2022-01-31 05:23:18.877447 breeze_connect-1.0.9/PKG-INFO
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)      228 2021-12-20 10:37:29.000000 breeze_connect-1.0.9/README.md
+drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 05:23:18.877447 breeze_connect-1.0.9/breeze_connect/
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)       55 2022-01-31 05:21:42.000000 breeze_connect-1.0.9/breeze_connect/__init__.py
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)    45889 2022-01-31 05:22:24.000000 breeze_connect-1.0.9/breeze_connect/breeze_connect.py
+drwxrwxr-x   0 oneture   (1000) oneture   (1000)        0 2022-01-31 05:23:18.877447 breeze_connect-1.0.9/breeze_connect.egg-info/
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)      695 2022-01-31 05:23:18.000000 breeze_connect-1.0.9/breeze_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)      267 2022-01-31 05:23:18.000000 breeze_connect-1.0.9/breeze_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)        1 2022-01-31 05:23:18.000000 breeze_connect-1.0.9/breeze_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)       33 2022-01-31 05:23:18.000000 breeze_connect-1.0.9/breeze_connect.egg-info/requires.txt
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)       15 2022-01-31 05:23:18.000000 breeze_connect-1.0.9/breeze_connect.egg-info/top_level.txt
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)       38 2022-01-31 05:23:18.877447 breeze_connect-1.0.9/setup.cfg
+-rw-rw-r--   0 oneture   (1000) oneture   (1000)      720 2022-01-31 05:23:09.000000 breeze_connect-1.0.9/setup.py
```

### Comparing `breeze_connect-1.0.8/PKG-INFO` & `breeze_connect-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_connect
-Version: 1.0.8
+Version: 1.0.9
 Summary: Testing Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: Sarang Surve
 Author-email: author@example.com
 License: UNKNOWN
 Description: ## Breeze Connect SDK
         This is a package to integrate streaming stocks for subscribed users & call APIs through which you can fetch live/historical data, automate your trading strategies, and monitor your portfolio in real time.
```

### Comparing `breeze_connect-1.0.8/breeze_connect/breeze_connect.py` & `breeze_connect-1.0.9/breeze_connect/breeze_connect.py`

 * *Files 15% similar despite different names*

```diff
@@ -160,72 +160,138 @@
                 dict["BestSellQty-"+str(counter)] = lis[5]
                 dict["SellNoOfOrders-"+str(counter)] = lis[6]
                 dict["SellFlag-"+str(counter)] = lis[7]
                 depth.append(dict)
         return depth
 
     def parse_data(self, data):
-        if len(data) == 45:
+        if data and len(data) == 46:
             order_dict = {}
-            order_dict["sourcenumber"] = msgArray[0]                                                            #Source Number
-            order_dict["group"] = msgArray[1]                                                                   #Group
-            order_dict["user_id"] = msgArray[2].slice(1) if (msgArray[2] != None) else None                     #User_id 
-            order_dict["key"] = msgArray[3]                                                                     #Key
-            order_dict["messageLength"] = msgArray[4]                                                           #Message Length
-            order_dict["requestType"] = msgArray[5]                                                             #Request Type
-            order_dict["messageSequence"] = None
-            order_dict["messageDate"] = None
-            order_dict["messagePriority"] = None
-            order_dict["messageType"] = None
-            if msgArray[6] != None:
-                order_dict["messageSequence"] = msgArray[6].split(" ")[0]                                       #Message Sequence
-                order_dict["messageDate"] = msgArray[6].split(" ")[1]                                           #Date
-            order_dict["messageTime"] = msgArray[7]                                                             #Time
-            order_dict["messageCategory"] = msgArray[8]                                                         #Message Category
-            if msgArray[9] != None:
-                order_dict["messagePriority"] = msgArray[9].split("-")[0]                                       #Priority
-                order_dict["messageType"] = msgArray[9].split("-")[1]                                           #Message Type
-            order_dict["orderMatchAccount"] = msgArray[10]                                                      #Order Match Account
-            order_dict["exchangeCode"] = msgArray[11]                                                           #Exchange Code
-            order_dict["stockCode"] = msgArray[12]                                                              #Stock Code
-            order_dict["orderFlow"] = msgArray[13]                                                              #Order Flow
-            order_dict["limitMarketFlag"] = msgArray[14]                                                        #Limit Market Flag
-            order_dict["orderType"] = msgArray[15]                                                              #OrderType
-            order_dict["limitRate"] = parseFloat(msgArray[16])                                                  #Limit Rate
-            order_dict["productCode"] = msgArray[17]                                                            #Product Code
-            order_dict["orderStatus"] = msgArray[18]                                                            #Order Status
-            order_dict["orderPlacementTime"] = msgArray[19]                                                     #Order Placement Time
-            order_dict["tradeDate"] = msgArray[20]                                                              #Trade Date
-            order_dict["orderReference"] = msgArray[21]                                                         #Order Reference
-            order_dict["orderQuantity"] = parseFloat(msgArray[22]) if (msgArray[22] != undefined) else 0        #Order Quantity
-            order_dict["openQuantity"] = parseFloat(msgArray[23]) if (msgArray[24] != undefined) else 0         #Open Quantity
-            order_dict["executedQuantity"] = parseFloat(msgArray[24]) if (msgArray[25] != undefined) else 0     #Executed Quantity
-            order_dict["cancelledQuantity"] = parseFloat(msgArray[25]) if (msgArray[26] != undefined) else 0    #Cancelled Quantity
-            order_dict["expiredQuantity"] = parseFloat(msgArray[26]) if (msgArray[27] != undefined) else 0      #Expired Quantity
-            order_dict["disclosedQuantity"] = parseFloat(msgArray[27]) if (msgArray[28] != undefined) else 0    #Disclosed Quantity
-            order_dict["stopLossTriger"] = parseFloat(msgArray[28]) if (msgArray[29] != undefined) else 0       #Stop Loss Triger
-            order_dict["squareFlag"] = msgArray[29]                                                             #Square Flag
-            order_dict["amountBlocked"] = parseFloat(msgArray[30]) if (msgArray[31] != undefined) else 0        #Amount Blocked
-            order_dict["pipeId"] = msgArray[31]                                                                 #PipeId
-            order_dict["channel"] = msgArray[32]                                                                #Channel
-            order_dict["segementCode"] = msgArray[33]                                                           #Segement Code
-            order_dict["settlementNo"] = parseFloat(msgArray[34]) if (msgArray[35] != undefined) else 0         #Settlement Number
-            order_dict["segmentDescription"] = msgArray[35]                                                     #Segment Description
-            order_dict["marginSquareOffMode"] = msgArray[36]                                                    #Margin Square Off Mode
-            order_dict["orderValidDate"] = msgArray[38]                                                         #Order Valid Date
-            order_dict["order_msc_char"] = msgArray[39]
-            order_dict["avg_exctd_rt"] = msgArray[40]                                                           #Average Exited Rate
-            order_dict["ord_prc_imp_flg"] = msgArray[41]                                                        #Order Price Flag
-            order_dict["ord_mbc_flg"] = msgArray[42]
-            order_dict["orderLimitOffset"] = msgArray[43]                                                       #Order Limit Offset
-            order_dict["systemPartnerCode"] = msgArray[44]                                                      #System Partner Code
+            order_dict["sourceNumber"] = data[0]                            #Source Number
+            order_dict["group"] = data[1]                                   #Group
+            order_dict["userId"] = data[2]                                  #User_id
+            order_dict["key"] = data[3]                                     #Key
+            order_dict["messageLength"] = data[4]                           #Message Length
+            order_dict["requestType"] = data[5]                             #Request Type
+            order_dict["messageSequence"] = data[6]                         #Message Sequence
+            order_dict["messageDate"] = data[7]                             #Date
+            order_dict["messageTime"] = data[8]                             #Time
+            order_dict["messageCategory"] = data[9]                         #Message Category
+            order_dict["messagePriority"] = data[10]                        #Priority
+            order_dict["messageType"] = data[11]                            #Message Type
+            order_dict["orderMatchAccount"] = data[12]                      #Order Match Account
+            order_dict["orderExchangeCode"] = data[13]                      #Exchange Code
+            if data[11] == '4' or data[11] == '5':
+                order_dict["stockCode"] = data[14]                     #Stock Code
+                order_dict["orderFlow"] = data[15]                          # Order Flow
+                order_dict["limitMarketFlag"] = data[16]                    #Limit Market Flag
+                order_dict["orderType"] = data[17]                          #OrderType
+                order_dict["orderLimitRate"] = data[18]                     #Limit Rate
+                order_dict["productType"] = data[19]                        #Product Type
+                order_dict["orderStatus"] = data[20]                        # Order Status
+                order_dict["orderDate"] = data[21]                          #Order  Date
+                order_dict["orderTradeDate"] = data[22]                     #Trade Date
+                order_dict["orderReference"] = data[23]                     #Order Reference
+                order_dict["orderQuantity"] = data[24]                      #Order Quantity
+                order_dict["openQuantity"] = data[25]                       #Open Quantity
+                order_dict["orderExecutedQuantity"] = data[26]              #Order Executed Quantity
+                order_dict["cancelledQuantity"] = data[27]                  #Cancelled Quantity
+                order_dict["expiredQuantity"] = data[28]                    #Expired Quantity
+                order_dict["orderDisclosedQuantity"] = data[29]             # Order Disclosed Quantity
+                order_dict["orderStopLossTrigger"] = data[30]               #Order Stop Loss Triger
+                order_dict["orderSquareFlag"] = data[31]                    #Order Square Flag
+                order_dict["orderAmountBlocked"] = data[32]                 # Order Amount Blocked
+                order_dict["orderPipeId"] = data[33]                        #Order PipeId
+                order_dict["channel"] = data[34]                            #Channel
+                order_dict["exchangeSegmentCode"] = data[35]                #Exchange Segment Code
+                order_dict["exchangeSegmentSettlement"] = data[36]          #Exchange Segment Settlement 
+                order_dict["segmentDescription"] = data[37]                 #Segment Description
+                order_dict["marginSquareOffMode"] = data[38]                #Margin Square Off Mode
+                order_dict["orderValidDate"] = data[40]                     #Order Valid Date
+                order_dict["orderMessageCharacter"] = data[41]              #Order Message Character
+                order_dict["averageExecutedRate"] = data[42]                #Average Exited Rate
+                order_dict["orderPriceImprovementFlag"] = data[43]          #Order Price Flag
+                order_dict["orderMBCFlag"] = data[44]                       #Order MBC Flag
+                order_dict["orderLimitOffset"] = data[45]                   #Order Limit Offset
+                order_dict["systemPartnerCode"] = data[46]                  #System Partner Code
+            elif data[11] == '6' or data[11] == '7':
+                order_dict["underlying"] = data[14]                         #Underlying
+                order_dict["productType"] = data[15]                        #Product Type
+                order_dict["optionType"] = data[16]                         #Option Type
+                order_dict["exerciseType"] = data[17]                       #Exercise Type
+                order_dict["strikePrice"] = data[18]                        #Strike Price
+                order_dict["expiryDate"] = data[19]                         #Expiry Date
+                order_dict["orderValidDate"] = data[20]                     #Order Valid Date
+                order_dict["orderFlow"] = data[21]                          #Order  Flow
+                order_dict["limitMarketFlag"] = data[22]                    #Limit Market Flag
+                order_dict["orderType"] = data[23]                          #Order Type
+                order_dict["limitRate"] = data[24]                          #Limit Rate
+                order_dict["orderStatus"] = data[25]                        #Order Status
+                order_dict["orderReference"] = data[26]                     #Order Reference
+                order_dict["orderTotalQuantity"] = data[27]                 #Order Total Quantity
+                order_dict["executedQuantity"] = data[28]                   #Executed Quantity
+                order_dict["cancelledQuantity"] = data[29]                  #Cancelled Quantity
+                order_dict["expiredQuantity"] = data[30]                    #Expired Quantity
+                order_dict["stopLossTrigger"] = data[31]                    #Stop Loss Trigger
+                order_dict["specialFlag"] = data[32]                        #Special Flag
+                order_dict["pipeId"] = data[33]                             #PipeId
+                order_dict["channel"] = data[34]                            #Channel
+                order_dict["modificationOrCancelFlag"] = data[35]           #Modification or Cancel Flag
+                order_dict["tradeDate"] = data[36]                          #Trade Date
+                order_dict["acknowledgeNumber"] = data[37]                  #Acknowledgement Number
+                order_dict["stopLossOrderReference"] = data[37]             #Stop Loss Order Reference
+                order_dict["totalAmountBlocked"] = data[38]                 # Total Amount Blocked
+                order_dict["averageExecutedRate"] = data[39]                #Average Executed Rate
+                order_dict["cancelFlag"] = data[40]                         #Cancel Flag
+                order_dict["squareOffMarket"] = data[41]                    #SquareOff Market
+                order_dict["quickExitFlag"] = data[42]                      #Quick Exit Flag
+                order_dict["stopValidTillDateFlag"] = data[43]              #Stop Valid till Date Flag
+                order_dict["priceImprovementFlag"] = data[44]               #Price Improvement Flag
+                order_dict["conversionImprovementFlag"] = data[45]          #Conversion Improvement Flag
+                order_dict["trailUpdateCondition"] = data[45]               #Trail Update Condition
+                order_dict["systemPartnerCode"] = data[46]                  #System Partner Code
             return order_dict
         exchange = str.split(data[0], '!')[0].split('.')[0]
         data_type = str.split(data[0], '!')[0].split('.')[1]
-        if data_type == '1':
+        if data_type == '6':
+            data_dict = {}
+            data_dict["Symbol"] = data[0]
+            data_dict["AndiOPVolume"] = data[1]
+            data_dict["Reserved"] = data[2]
+            data_dict["IndexFlag"] = data[3]
+            data_dict["TotalQNTTraded"] = data[4]
+            data_dict["LastTradedPrice"] = data[5]
+            data_dict["LastTradedQuantity"] = data[6]
+            data_dict["LastTradeTime"] = data[7]
+            data_dict["AvgTradedPrice"] = data[8]
+            data_dict["TotalBuyQnt"] = data[9]
+            data_dict["TotalSellQnt"] = data[10]
+            data_dict["ReservedStr"] = data[11]
+            data_dict["ClosePrice"] = data[12]
+            data_dict["OpenPrice"] = data[13]
+            data_dict["HighPrice"] = data[14]
+            data_dict["LowPrice"] = data[15]
+            data_dict["ReservedShort"] = data[16]
+            data_dict["CurrOpenInterest"] = data[17]
+            data_dict["TotalTrades"] = data[18]
+            data_dict["HightestPriceEver"] = data[19]
+            data_dict["LowestPriceEver"] = data[20]
+            data_dict["TotalTradedValue"] = data[21]
+            marketDepthIndex = 0
+            for i in range(22,len(data)):
+                data_dict["Quantity-"+marketDepthIndex] = data[i][0]
+                data_dict["OrderPrice-"+marketDepthIndex] = data[i][1]
+                data_dict["TotalOrders-"+marketDepthIndex] = data[i][2]
+                data_dict["Reserved-"+marketDepthIndex] = data[i][3]
+                data_dict["SellQuantity-"+marketDepthIndex] = data[i][4]
+                data_dict["SellOrderPrice-"+marketDepthIndex] = data[i][5]
+                data_dict["SellTotalOrders-"+marketDepthIndex] = data[i][6]
+                data_dict["SellReserved-"+marketDepthIndex] = data[i][7]
+                marketDepthIndex += 1
+        elif data_type == '1':
             data_dict = {
                 "symbol": data[0],
                 "open": data[1],
                 "last": data[2],
                 "high": data[3],
                 "low": data[4],
                 "change": data[5],
@@ -266,20 +332,24 @@
         else:
             data_dict = {
                 "symbol": data[0],
                 "time": datetime.fromtimestamp(data[1]).strftime('%c'),
                 "depth": self.parse_market_depth(data[2], exchange),
                 "quotes": "Market Depth"
             }
-        if exchange == '4':
+        if exchange == '4' and len(data) == 21:
             data_dict['exchange'] = 'NSE Equity'
         elif exchange == '1':
             data_dict['exchange'] = 'BSE'
         elif exchange == '13':
             data_dict['exchange'] = 'NSE Currency'
+        elif exchange == '4' and len(data) == 23:
+            data_dict['exchange'] = 'NSE Futures & Options'
+        elif exchange == '6':
+            data_dict['exchange'] = 'Commodity'
         return data_dict
 
     def api_util(self):
         try:
             headers = {
                 "Content-Type": "application/json"
             }
@@ -289,16 +359,16 @@
             }
             body = json.dumps(body, separators=(',', ':'))
             url = "https://api.icicidirect.com/breezeapi/api/v1/customerdetails"
             response = requests.get(url=url, data=body, headers=headers)
             if response.json()['Success']!=None:
                 base64_session_token = response.json()['Success']['session_token']
                 result = base64.b64decode(base64_session_token.encode('ascii')).decode('ascii')
-                self.session_key = result.split(":")[0]
-                self.user_id = result.split(":")[1]
+                self.user_id = result.split(":")[0]
+                self.session_key = result.split(":")[1]
             else:
                 raise Exception("Could not authenticate credentials. Please check token and keys")
         except Exception as e:
             print("Could not authenticate credentials. Please check token and keys")
 
     def get_stock_script_list(self):
         try:
```

### Comparing `breeze_connect-1.0.8/breeze_connect.egg-info/PKG-INFO` & `breeze_connect-1.0.9/breeze_connect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-connect
-Version: 1.0.8
+Version: 1.0.9
 Summary: Testing Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: Sarang Surve
 Author-email: author@example.com
 License: UNKNOWN
 Description: ## Breeze Connect SDK
         This is a package to integrate streaming stocks for subscribed users & call APIs through which you can fetch live/historical data, automate your trading strategies, and monitor your portfolio in real time.
```

### Comparing `breeze_connect-1.0.8/setup.py` & `breeze_connect-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_connect",
-    version="1.0.8",
+    version="1.0.9",
     author="Sarang Surve",
     author_email="author@example.com",
     description="Testing Breeze Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['python-socketio[client]','requests'],
     url="https://github.com/pypa/sampleproject",
```

