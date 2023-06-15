# Comparing `tmp/card_data_parsers-0.8.0.tar.gz` & `tmp/card_data_parsers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "card_data_parsers-0.8.0.tar", last modified: Mon Feb  7 12:13:30 2022, max compression
+gzip compressed data, was "card_data_parsers-0.9.0.tar", last modified: Mon Apr 18 17:02:30 2022, max compression
```

## Comparing `card_data_parsers-0.8.0.tar` & `card_data_parsers-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:13:30.705512 card_data_parsers-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-02-07 12:13:30.705512 card_data_parsers-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:13:30.697512 card_data_parsers-0.8.0/card_data_parsers/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:13:30.701512 card_data_parsers-0.8.0/card_data_parsers/models/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/amex_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/cdf_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/happay_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/s3df_transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/models/vcf_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:13:30.705512 card_data_parsers-0.8.0/card_data_parsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8929 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/amex_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    13301 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/cdf_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/happay_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11051 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/s3df_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    13264 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/parsers/vcf_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/card_data_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 12:13:30.701512 card_data_parsers-0.8.0/card_data_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-02-07 12:13:30.000000 card_data_parsers-0.8.0/card_data_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-02-07 12:13:30.000000 card_data_parsers-0.8.0/card_data_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 12:13:30.000000 card_data_parsers-0.8.0/card_data_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-02-07 12:13:30.000000 card_data_parsers-0.8.0/card_data_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-07 12:13:30.000000 card_data_parsers-0.8.0/card_data_parsers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 12:13:30.705512 card_data_parsers-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-02-07 12:13:19.000000 card_data_parsers-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/card_data_parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/card_data_parsers/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/amex_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/cdf_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/happay_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/s3df_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/models/vcf_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/card_data_parsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8956 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/amex_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13328 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/cdf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4313 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/happay_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11115 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/s3df_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13230 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/parsers/vcf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/card_data_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/card_data_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-04-18 17:02:30.000000 card_data_parsers-0.9.0/card_data_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-04-18 17:02:30.000000 card_data_parsers-0.9.0/card_data_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-18 17:02:30.000000 card_data_parsers-0.9.0/card_data_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-18 17:02:30.000000 card_data_parsers-0.9.0/card_data_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-18 17:02:30.000000 card_data_parsers-0.9.0/card_data_parsers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-18 17:02:30.296759 card_data_parsers-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-04-18 17:02:20.000000 card_data_parsers-0.9.0/setup.py
```

### Comparing `card_data_parsers-0.8.0/LICENSE` & `card_data_parsers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/PKG-INFO` & `card_data_parsers-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: card_data_parsers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Parsing bank feed data files
 Home-page: https://www.fylehq.com
 Author: Siva Narayanan
 Author-email: siva@fyle.in
 License: MIT
 Keywords: fyle,api,python,sdk,cards,parsers,amex,visa,cdf,vcf,s3df,happay,mastercard,diners club
 Platform: UNKNOWN
```

### Comparing `card_data_parsers-0.8.0/README.md` & `card_data_parsers-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/models/amex_transaction.py` & `card_data_parsers-0.9.0/card_data_parsers/models/amex_transaction.py`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/models/cdf_transaction.py` & `card_data_parsers-0.9.0/card_data_parsers/models/cdf_transaction.py`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/models/s3df_transaction.py` & `card_data_parsers-0.9.0/card_data_parsers/models/s3df_transaction.py`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/models/transaction.py` & `card_data_parsers-0.9.0/card_data_parsers/models/transaction.py`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/models/vcf_transaction.py` & `card_data_parsers-0.9.0/card_data_parsers/models/vcf_transaction.py`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/card_data_parsers/parsers/amex_parser.py` & `card_data_parsers-0.9.0/card_data_parsers/parsers/amex_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     txn, txn_line)
 
             txn.transaction_type = AmexParser.__extract_transaction_type(
                         txn.transaction_type)
             if txn.transaction_type is None:
                 raise ParserError(f'Transaction type is missing')
 
-            if txn.foreign_currency == txn.currency and txn.foreign_amount == txn.amount:
+            if txn.foreign_currency is None or txn.foreign_amount is None or (txn.foreign_currency == txn.currency):
                 txn.foreign_amount = None
                 txn.foreign_currency = None
             else:
                 txn.foreign_currency = AmexParser.__extract_currency(
                     txn.foreign_currency)
                 if txn.foreign_currency is None:
                     raise ParserError(f'foreign_currency is missing')
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers/parsers/cdf_parser.py` & `card_data_parsers-0.9.0/card_data_parsers/parsers/cdf_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         txn.foreign_currency = CDFParser.__get_element_by_tag(
             ftrxn, 'OriginalCurrencyCode').text
         if txn.foreign_currency is None:
             return None
         txn.foreign_currency = get_currency_from_country_code(
             txn.foreign_currency)
 
-        if txn.foreign_currency is not None and txn.foreign_currency == txn.currency:
+        if txn.foreign_currency is None or txn.foreign_amount is None or (txn.foreign_currency == txn.currency):
             txn.foreign_currency = None
             txn.foreign_amount = None
 
         # Vendor
         txn.vendor = CDFParser.__get_element_by_tag(
             card_acceptor, 'CardAcceptorName').text
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers/parsers/happay_parser.py` & `card_data_parsers-0.9.0/card_data_parsers/parsers/happay_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,18 @@
         # orig amount and orig currency
         if txn.foreign_amount and txn.foreign_currency:
             txn.foreign_amount = abs(float(txn.foreign_amount))
         else:
             txn.foreign_amount = None
             txn.foreign_currency = None
 
+        if txn.foreign_currency is None or txn.foreign_amount is None or (txn.foreign_currency == txn.currency):
+            txn.foreign_amount = None
+            txn.foreign_currency = None
+
         # external id
         unique_for_transaction = str(txn.account_number) + str(txn.transaction_dt) + str(
             txn.amount) + str(txn.external_id) + str(txn.vendor) + txn.bank_name
         txn.external_id = generate_external_id(unique_for_transaction)
 
         return txn
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers/parsers/s3df_parser.py` & `card_data_parsers-0.9.0/card_data_parsers/parsers/s3df_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             ftrxn, 'OriginalCurrencyCode').text
         if txn.foreign_currency is not None:
             txn.foreign_currency = get_currency_from_country_code(
                 txn.foreign_currency)
         else:
             return None
 
-        if txn.foreign_currency == txn.currency:
+        if txn.foreign_currency is None or txn.foreign_amount is None or (txn.foreign_currency == txn.currency):
             txn.foreign_currency = None
             txn.foreign_amount = None
 
         # Vendor
         txn.vendor = S3DFParser.__get_element_by_tag(
             card_acceptor, 'CardAcceptorName').text
         txn.vendor = str(txn.vendor) + ', ' + S3DFParser.__get_element_by_tag(
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers/parsers/vcf_parser.py` & `card_data_parsers-0.9.0/card_data_parsers/parsers/vcf_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     @staticmethod
     def __process_transaction(txn, account_number_mask_begin, account_number_mask_end):
         txn.transaction_type = VCFParser.__extract_transaction_type(
             txn.transaction_type)
         if txn.transaction_type == None:
             raise ParserError('Transaction type missing.')
 
-        if txn.foreign_currency is None or txn.foreign_amount is None or txn.foreign_currency == txn.currency or txn.foreign_amount == txn.amount:
+        if txn.foreign_currency is None or txn.foreign_amount is None or (txn.foreign_currency == txn.currency):
             txn.foreign_currency = None
             txn.foreign_amount = None
         else:
             txn.foreign_currency = remove_leading_zeros(
                 txn.foreign_currency, 3)
             txn.foreign_currency = get_currency_from_country_code(
                 txn.foreign_currency)
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers/utils.py` & `card_data_parsers-0.9.0/card_data_parsers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
 from datetime import datetime
 import hashlib
 import pycountry
+import numbers
 
 
 country_code_to_currency_dict = {
     "040": "EUR",  # Austria
     "076": "BRL",  # Brazil
     "276": "EUR",  # Germany
     "380": "EUR",  # Italy
@@ -72,15 +73,15 @@
     value = value.lstrip('0')
     if min_len:
         value = value.zfill(min_len)
     return value
 
 
 def get_iso_date_string(date_string, date_format):
-    if date_string is not '':
+    if date_string != '':
         iso_date_string = datetime.strptime(date_string.strip(), date_format)
         # hack for timezones: set time to 10 o clock
         iso_date_string = iso_date_string.replace(hour=10)
         iso_date_string = iso_date_string.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
     else:
         iso_date_string = None
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers.egg-info/PKG-INFO` & `card_data_parsers-0.9.0/card_data_parsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: card-data-parsers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Parsing bank feed data files
 Home-page: https://www.fylehq.com
 Author: Siva Narayanan
 Author-email: siva@fyle.in
 License: MIT
 Keywords: fyle,api,python,sdk,cards,parsers,amex,visa,cdf,vcf,s3df,happay,mastercard,diners club
 Platform: UNKNOWN
```

### Comparing `card_data_parsers-0.8.0/card_data_parsers.egg-info/SOURCES.txt` & `card_data_parsers-0.9.0/card_data_parsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `card_data_parsers-0.8.0/setup.py` & `card_data_parsers-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='card_data_parsers',
-    version='0.8.0',
+    version='0.9.0',
     author='Siva Narayanan',
     author_email='siva@fyle.in',
     url='https://www.fylehq.com',
     license='MIT',
     description='Parsing bank feed data files',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

