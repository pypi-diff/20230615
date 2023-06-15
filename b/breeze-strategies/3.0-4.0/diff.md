# Comparing `tmp/breeze_strategies-3.0.tar.gz` & `tmp/breeze_strategies-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-3.0.tar", last modified: Thu Jun 15 09:16:12 2023, max compression
+gzip compressed data, was "breeze_strategies-4.0.tar", last modified: Thu Jun 15 09:19:01 2023, max compression
```

## Comparing `breeze_strategies-3.0.tar` & `breeze_strategies-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.468001 breeze_strategies-3.0/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-3.0/LICENSE
--rw-rw-rw-   0        0        0     1544 2023-06-15 09:16:12.466817 breeze_strategies-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-06-15 09:11:25.000000 breeze_strategies-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.392958 breeze_strategies-3.0/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-3.0/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    19226 2023-06-15 09:05:32.000000 breeze_strategies-3.0/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:16:12.462669 breeze_strategies-3.0/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1544 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 09:16:12.000000 breeze_strategies-3.0/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:16:12.468001 breeze_strategies-3.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-06-15 09:15:36.000000 breeze_strategies-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.261194 breeze_strategies-4.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-4.0/LICENSE
+-rw-rw-rw-   0        0        0     1544 2023-06-15 09:19:01.258161 breeze_strategies-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-06-15 09:18:49.000000 breeze_strategies-4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.221019 breeze_strategies-4.0/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-4.0/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    19225 2023-06-15 09:18:21.000000 breeze_strategies-4.0/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.254194 breeze_strategies-4.0/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1544 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:19:01.261194 breeze_strategies-4.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-06-15 09:18:57.000000 breeze_strategies-4.0/setup.py
```

### Comparing `breeze_strategies-3.0/LICENSE` & `breeze_strategies-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-3.0/PKG-INFO` & `breeze_strategies-4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 3.0
+Version: 4.0
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
 
-pip install breeze_strategies==3.0
+pip install breeze_strategies==4.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-3.0/README.md` & `breeze_strategies-4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==3.0
+pip install breeze_strategies==4.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-3.0/breeze_strategies/breeze_strategies.py` & `breeze_strategies-4.0/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
         self.client.ws_connect()
         self.quantity = 0
     
-    def squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right = None, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity):
+    def squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right = None):
         data = self.client.square_off(exchange_code=exchange_code,
                             product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
                             right=rightval,
                             strike_price=strike_price,
                             action=action,
```

### Comparing `breeze_strategies-3.0/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-4.0/breeze_strategies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 3.0
+Version: 4.0
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
 
-pip install breeze_strategies==3.0
+pip install breeze_strategies==4.0
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-3.0/setup.py` & `breeze_strategies-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="3.0",
+    version="4.0",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

