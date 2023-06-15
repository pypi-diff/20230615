# Comparing `tmp/xmlrecords-0.2.5.tar.gz` & `tmp/xmlrecords-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlrecords-0.2.5.tar", last modified: Mon Jul 19 10:00:26 2021, max compression
+gzip compressed data, was "xmlrecords-0.3.0.tar", last modified: Thu Jun 15 11:50:12 2023, max compression
```

## Comparing `xmlrecords-0.2.5.tar` & `xmlrecords-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1043 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/xmlrecords/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/xmlrecords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/xmlrecords/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/xmlrecords/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9095 2021-07-19 10:00:17.000000 xmlrecords-0.2.5/xmlrecords/src/xmlrecords.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 10:00:26.076964 xmlrecords-0.2.5/xmlrecords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2021-07-19 10:00:25.000000 xmlrecords-0.2.5/xmlrecords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-07-19 10:00:25.000000 xmlrecords-0.2.5/xmlrecords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-19 10:00:25.000000 xmlrecords-0.2.5/xmlrecords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-07-19 10:00:25.000000 xmlrecords-0.2.5/xmlrecords.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1049 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.341069 xmlrecords-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.341069 xmlrecords-0.3.0/xmlrecords/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/xmlrecords/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/src/xmlrecords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/xmlrecords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/top_level.txt
```

### Comparing `xmlrecords-0.2.5/LICENSE` & `xmlrecords-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.2.5/PKG-INFO` & `xmlrecords-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: xmlrecords
-Version: 0.2.5
+Version: 0.3.0
 Summary: This package can convert an XML files to a list of records
 Home-page: UNKNOWN
 Author: Yaroslav Kopotilov
 Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
 Description: # XML Records
         
-        `xmlrecords` is a user-friendly wrapper of `xml` package for extraction of tabular data from XML files.
+        `xmlrecords` is a user-friendly wrapper of `lxml` package for extraction of tabular data from XML files.
         
         >>> This data provider sends all his data in... XML. You know nothing about XML, except that it looks kind of weird and you would *definitely* never use it for tabular data. How could you just transform all this XML nightmare into a sensible tabular format, like a DataFrame? Don't worry: you are in the right place!
         
         
         # Installation
         
         ```shell script
         pip install xmlrecords
         ```
         
-        - The package requires `python 3.7+` and no external dependencies.
-        - The package uses `xml.etree.ElementTree` so it's vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/Billion_laughs_attack).
-        
+        The package requires `python 3.7+` and one external dependency `lxml`.
         
         # Usage
         
         ## Basic example
         
         Usually, you only need to specify path to table rows; optionally, you can specify paths to any extra data you'd like to add to your table:
         
@@ -116,15 +114,15 @@
         ```
         
         
         # FAQ
         
         1. **Why not `xmltodict`?** `xmltodict` can convert arbitrary XML to a python dict. However, it is 2-3 times slower than `xmlrecords` and does not support some features specific for tablular data.
         
-        2. **Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
+        2. **Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
         
 Keywords: xml parsing
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: xmlrecords Version: 0.2.5 Summary: This package can
+Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.0 Summary: This package can
 convert an XML files to a list of records Home-page: UNKNOWN Author: Yaroslav
 Kopotilov Author-email: datascience@tuta.io License: Apache License, Version
-2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of `xml`
-package for extraction of tabular data from XML files. >>> This data provider
-sends all his data in... XML. You know nothing about XML, except that it looks
-kind of weird and you would *definitely* never use it for tabular data. How
-could you just transform all this XML nightmare into a sensible tabular format,
-like a DataFrame? Don't worry: you are in the right place! # Installation
-```shell script pip install xmlrecords ``` - The package requires `python 3.7+`
-and no external dependencies. - The package uses `xml.etree.ElementTree` so
-it's vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/
-Billion_laughs_attack). # Usage ## Basic example Usually, you only need to
-specify path to table rows; optionally, you can specify paths to any extra data
-you'd like to add to your table: ```python # XML object xml_bytes = b"""\ <?xml
-version="1.0" encoding="utf-8"?>   Virtual Shore   2020-02-02T05:12:22
+2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of
+`lxml` package for extraction of tabular data from XML files. >>> This data
+provider sends all his data in... XML. You know nothing about XML, except that
+it looks kind of weird and you would *definitely* never use it for tabular
+data. How could you just transform all this XML nightmare into a sensible
+tabular format, like a DataFrame? Don't worry: you are in the right place! #
+Installation ```shell script pip install xmlrecords ``` The package requires
+`python 3.7+` and one external dependency `lxml`. # Usage ## Basic example
+Usually, you only need to specify path to table rows; optionally, you can
+specify paths to any extra data you'd like to add to your table: ```python #
+XML object xml_bytes = b"""\ <?xml version="1.0" encoding="utf-8"?>   Virtual
+Shore   2020-02-02T05:12:22
  2017 112.34
  1963 10    """ # Transform XML to records (= a list of key-value pairs) import
 xmlrecords records = xmlrecords.parse( xml=xml_bytes, records_path=['Shelf',
 'Book'], # The rows are XML nodes with the repeating tag  meta_paths=[
 ['Library', 'Name'], ['Shelf', 'Timestamp']], # Add additional "meta" nodes )
 for r in records: print(r) # Output: # {'Name': 'Virtual Shore', 'Timestamp':
 '2020-02-02T05:12:22', 'Title': 'Sunny Night', 'alive': 'no', 'name':
@@ -35,15 +34,15 @@
 conn.cursor() c.execute("""\ CREATE TABLE BOOKS ( LIBRARY_NAME TEXT,
 SHELF_TIMESTAMP TEXT, TITLE TEXT, AUTHOR_ALIVE TEXT, AUTHOR_NAME TEXT, YEAR
 INT, PRICE FLOAT, PRIMARY KEY (TITLE, AUTHOR_NAME) ) """ ) c.executemany
 ( """INSERT INTO BOOKS VALUES (?,?,?,?,?,?,?)""", [list(x.values()) for x in
 records], ) conn.commit() ``` # FAQ 1. **Why not `xmltodict`?** `xmltodict` can
 convert arbitrary XML to a python dict. However, it is 2-3 times slower than
 `xmlrecords` and does not support some features specific for tablular data. 2.
-**Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using
+**Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using
 `xml` or `lxml` directly is a viable option too - in case this package doesn't
 cover your particular use case. Keywords: xml parsing Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
```

### Comparing `xmlrecords-0.2.5/README.md` & `xmlrecords-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # XML Records
 
-`xmlrecords` is a user-friendly wrapper of `xml` package for extraction of tabular data from XML files.
+`xmlrecords` is a user-friendly wrapper of `lxml` package for extraction of tabular data from XML files.
 
 >>> This data provider sends all his data in... XML. You know nothing about XML, except that it looks kind of weird and you would *definitely* never use it for tabular data. How could you just transform all this XML nightmare into a sensible tabular format, like a DataFrame? Don't worry: you are in the right place!
 
 
 # Installation
 
 ```shell script
 pip install xmlrecords
 ```
 
-- The package requires `python 3.7+` and no external dependencies.
-- The package uses `xml.etree.ElementTree` so it's vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/Billion_laughs_attack).
-
+The package requires `python 3.7+` and one external dependency `lxml`.
 
 # Usage
 
 ## Basic example
 
 Usually, you only need to specify path to table rows; optionally, you can specify paths to any extra data you'd like to add to your table:
 
@@ -108,8 +106,8 @@
 ```
 
 
 # FAQ
 
 1. **Why not `xmltodict`?** `xmltodict` can convert arbitrary XML to a python dict. However, it is 2-3 times slower than `xmlrecords` and does not support some features specific for tablular data.
 
-2. **Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
+2. **Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-# XML Records `xmlrecords` is a user-friendly wrapper of `xml` package for
+# XML Records `xmlrecords` is a user-friendly wrapper of `lxml` package for
 extraction of tabular data from XML files. >>> This data provider sends all his
 data in... XML. You know nothing about XML, except that it looks kind of weird
 and you would *definitely* never use it for tabular data. How could you just
 transform all this XML nightmare into a sensible tabular format, like a
 DataFrame? Don't worry: you are in the right place! # Installation ```shell
-script pip install xmlrecords ``` - The package requires `python 3.7+` and no
-external dependencies. - The package uses `xml.etree.ElementTree` so it's
-vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/
-Billion_laughs_attack). # Usage ## Basic example Usually, you only need to
+script pip install xmlrecords ``` The package requires `python 3.7+` and one
+external dependency `lxml`. # Usage ## Basic example Usually, you only need to
 specify path to table rows; optionally, you can specify paths to any extra data
 you'd like to add to your table: ```python # XML object xml_bytes = b"""\ <?xml
 version="1.0" encoding="utf-8"?>   Virtual Shore   2020-02-02T05:12:22
  2017 112.34
  1963 10    """ # Transform XML to records (= a list of key-value pairs) import
 xmlrecords records = xmlrecords.parse( xml=xml_bytes, records_path=['Shelf',
 'Book'], # The rows are XML nodes with the repeating tag  meta_paths=[
@@ -32,10 +30,10 @@
 conn.cursor() c.execute("""\ CREATE TABLE BOOKS ( LIBRARY_NAME TEXT,
 SHELF_TIMESTAMP TEXT, TITLE TEXT, AUTHOR_ALIVE TEXT, AUTHOR_NAME TEXT, YEAR
 INT, PRICE FLOAT, PRIMARY KEY (TITLE, AUTHOR_NAME) ) """ ) c.executemany
 ( """INSERT INTO BOOKS VALUES (?,?,?,?,?,?,?)""", [list(x.values()) for x in
 records], ) conn.commit() ``` # FAQ 1. **Why not `xmltodict`?** `xmltodict` can
 convert arbitrary XML to a python dict. However, it is 2-3 times slower than
 `xmlrecords` and does not support some features specific for tablular data. 2.
-**Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using
+**Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using
 `xml` or `lxml` directly is a viable option too - in case this package doesn't
 cover your particular use case.
```

### Comparing `xmlrecords-0.2.5/pyproject.toml` & `xmlrecords-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.2.5/setup.cfg` & `xmlrecords-0.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 include_package_data = true
 python_requires = >= 3.7
 packages = find:
 test_suite = tests
 setup_requires = 
 	setuptools
 install_requires = 
+	lxml
 tests_require = 
 	pytest
 
 [flake8]
 max-line-length = 119
 exclude = .git, .eggs, __pycache__, build/, dist/, notebooks/, data/, logs/, artifacts/
```

### Comparing `xmlrecords-0.2.5/tests/test_core.py` & `xmlrecords-0.3.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,8 +615,46 @@
 00002660: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
 00002670: 7328 786d 6c72 6563 6f72 6473 2e58 4d4c  s(xmlrecords.XML
 00002680: 5661 6c69 6461 7469 6f6e 4572 726f 7229  ValidationError)
 00002690: 3a0a 2020 2020 2020 2020 786d 6c72 6563  :.        xmlrec
 000026a0: 6f72 6473 2e76 616c 6964 6174 6528 7265  ords.validate(re
 000026b0: 636f 7264 732c 206c 6973 7428 6578 7065  cords, list(expe
 000026c0: 6374 6564 5f6f 7574 7075 745b 305d 2e6b  cted_output[0].k
-000026d0: 6579 7328 2929 5b3a 2d31 5d29 0a         eys())[:-1]).
+000026d0: 6579 7328 2929 5b3a 2d31 5d29 0a0a 0a78  eys())[:-1])...x
+000026e0: 6d6c 5f62 6164 5f74 6f6b 656e 7320 3d20  ml_bad_tokens = 
+000026f0: 6222 2222 5c0a 3c43 6174 616c 6f67 3e0a  b"""\.<Catalog>.
+00002700: 2020 2020 3c42 6f6f 6b20 7469 746c 653d      <Book title=
+00002710: 2253 756e 6e79 2026 2043 6f6c 6422 2061  "Sunny & Cold" a
+00002720: 7574 686f 723d 224d 7973 7465 7269 6f75  uthor="Mysteriou
+00002730: 7320 416c 6578 2220 7965 6172 3d22 3230  s Alex" year="20
+00002740: 3233 2220 2f3e 0a20 2020 203c 426f 6f6b  23" />.    <Book
+00002750: 2074 6974 6c65 3d22 4261 6265 6c2d 3137   title="Babel-17
+00002760: 2220 6175 7468 6f72 3d22 5361 6d75 656c  " author="Samuel
+00002770: 2052 2e10 4465 6c61 6e79 2220 7965 6172   R..Delany" year
+00002780: 3d22 3139 3636 2220 2f3e 0a3c 2f43 6174  ="1966" />.</Cat
+00002790: 616c 6f67 3e0a 2222 220a 0a0a 7265 636f  alog>."""...reco
+000027a0: 7264 735f 6261 645f 746f 6b65 6e73 203d  rds_bad_tokens =
+000027b0: 205b 0a20 2020 207b 2274 6974 6c65 223a   [.    {"title":
+000027c0: 2022 5375 6e6e 7920 436f 6c64 222c 2022   "Sunny Cold", "
+000027d0: 6175 7468 6f72 223a 2022 4d79 7374 6572  author": "Myster
+000027e0: 696f 7573 2041 6c65 7822 2c20 2279 6561  ious Alex", "yea
+000027f0: 7222 3a20 2232 3032 3322 7d2c 0a20 2020  r": "2023"},.   
+00002800: 207b 2274 6974 6c65 223a 2022 4261 6265   {"title": "Babe
+00002810: 6c2d 3137 222c 2022 6175 7468 6f72 223a  l-17", "author":
+00002820: 2022 5361 6d75 656c 2052 2e44 656c 616e   "Samuel R.Delan
+00002830: 7922 2c20 2279 6561 7222 3a20 2231 3936  y", "year": "196
+00002840: 3622 7d2c 0a5d 0a0a 0a64 6566 2074 6573  6"},.]...def tes
+00002850: 745f 7061 7273 655f 786d 6c5f 7769 7468  t_parse_xml_with
+00002860: 5f62 6164 5f63 6861 7261 6374 6572 7328  _bad_characters(
+00002870: 293a 0a20 2020 2077 6974 6820 7079 7465  ):.    with pyte
+00002880: 7374 2e72 6169 7365 7328 786d 6c72 6563  st.raises(xmlrec
+00002890: 6f72 6473 2e58 4d4c 5061 7273 696e 6745  ords.XMLParsingE
+000028a0: 7272 6f72 293a 0a20 2020 2020 2020 2078  rror):.        x
+000028b0: 6d6c 7265 636f 7264 732e 7061 7273 6528  mlrecords.parse(
+000028c0: 786d 6c5f 6261 645f 746f 6b65 6e73 2c20  xml_bad_tokens, 
+000028d0: 726f 7773 5f70 6174 683d 5b22 426f 6f6b  rows_path=["Book
+000028e0: 225d 2c20 7265 636f 7665 723d 4661 6c73  "], recover=Fals
+000028f0: 6529 0a20 2020 2078 6d6c 7265 636f 7264  e).    xmlrecord
+00002900: 732e 7061 7273 6528 786d 6c5f 6261 645f  s.parse(xml_bad_
+00002910: 746f 6b65 6e73 2c20 726f 7773 5f70 6174  tokens, rows_pat
+00002920: 683d 5b22 426f 6f6b 225d 2c20 7265 636f  h=["Book"], reco
+00002930: 7665 723d 5472 7565 290a                 ver=True).
```

### Comparing `xmlrecords-0.2.5/xmlrecords/src/xmlrecords.py` & `xmlrecords-0.3.0/xmlrecords/src/xmlrecords.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# from dataclasses import dataclass
-from typing import Dict, List, Optional
-from xml.etree import ElementTree
+from typing import Any, Dict, List, Optional
 
+from lxml import etree
 
-class XMLParsingError(ValueError):
-    pass
+XMLParsingError = etree.XMLSyntaxError
 
 
 def _update_dict_nocollision(d1: dict, d2: dict) -> None:
     """Update the first dict with key-value pairs of the second dict
 
     :raises: XMLParsingError
         If the dicts have common keys
@@ -27,25 +25,18 @@
     if remove_namespace:
         _, _, tag = tag.rpartition("}")
         if ("{" in tag) or ("}" in tag):
             raise AssertionError(f"Unexpected tag format after namespace removal: {tag}")
     return tag
 
 
-# TODO: add option to specify text, attributes and child nodes to parse
-# @dataclass
-# class Fields:
-#     text: bool = True
-#     attributes: Optional[List[str]] = None
-#     nodes: Optional[List[str]] = None
-
-
 def _update_dict_from_node(
     d: dict,
-    node: ElementTree.Element,
+    # node: ElementTree.Element,
+    node: etree.Element,
     prefix: Optional[str],
     sep: str,
     max_depth: Optional[int],
     strip: bool,
     rm_namespace: bool,
     skip_child_tag: Optional[str],
 ) -> None:
@@ -88,14 +79,15 @@
     meta_prefix: bool = False,
     sep: str = "_",
     rows_max_depth: Optional[int] = None,
     meta_max_depth: Optional[int] = None,
     strip_text: bool = True,
     namespace: str = "*",
     remove_namespace: bool = True,
+    recover: bool = False,
 ) -> List[Dict]:
     """Convert XML data to a list of records
 
     :param xml: XML bytes object
     :param rows_path: bits to construct XPath to a "row" node
         Rows are XML nodes with the same tag and (usually) the same structure
     :param subrow_tag: tag of a "subrow" node
@@ -121,19 +113,20 @@
         0 = no nested nodes
     :param meta_max_depth: maximum depth of nested nodes for metadata
     :param strip_text: if true, apply str.strip function to XML values
         Set to True if XML has redundant space or new line characters
     :param namespace: XML namespace to search
         * = all namespaces
     :param remove_namespace: if true, do not include namespace in the record key
+    :param recover: if true, try to recover from XML parsing errors
     :return: list of records
     :raises: XMLParsingError (subclass of ValueError)
     """
-
-    tree = ElementTree.fromstring(xml)
+    parser = etree.XMLParser(recover=recover)
+    tree = etree.fromstring(xml, parser=parser)
 
     if meta_paths is None:
         meta_paths = []
 
     meta_d: dict = {}
     for m_path in meta_paths:
         m_path_ = _list_to_path(m_path, namespace)
@@ -173,15 +166,15 @@
         if subrow_tag is None:
             records.append(row_d)
         else:
             subrow_nodes = r_node.findall(subrows_path_)
             if subrow_explode is None:
                 subrow_list = []
                 for sr_count, sr_node in enumerate(subrow_nodes):
-                    subrow_d = {}
+                    subrow_d: Dict[str, Any] = {}
                     _update_dict_from_node(
                         d=subrow_d,
                         node=sr_node,
                         prefix=prefix,
                         sep=sep,
                         max_depth=rows_max_depth,
                         strip=strip_text,
```

### Comparing `xmlrecords-0.2.5/xmlrecords.egg-info/PKG-INFO` & `xmlrecords-0.3.0/xmlrecords.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: xmlrecords
-Version: 0.2.5
+Version: 0.3.0
 Summary: This package can convert an XML files to a list of records
 Home-page: UNKNOWN
 Author: Yaroslav Kopotilov
 Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
 Description: # XML Records
         
-        `xmlrecords` is a user-friendly wrapper of `xml` package for extraction of tabular data from XML files.
+        `xmlrecords` is a user-friendly wrapper of `lxml` package for extraction of tabular data from XML files.
         
         >>> This data provider sends all his data in... XML. You know nothing about XML, except that it looks kind of weird and you would *definitely* never use it for tabular data. How could you just transform all this XML nightmare into a sensible tabular format, like a DataFrame? Don't worry: you are in the right place!
         
         
         # Installation
         
         ```shell script
         pip install xmlrecords
         ```
         
-        - The package requires `python 3.7+` and no external dependencies.
-        - The package uses `xml.etree.ElementTree` so it's vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/Billion_laughs_attack).
-        
+        The package requires `python 3.7+` and one external dependency `lxml`.
         
         # Usage
         
         ## Basic example
         
         Usually, you only need to specify path to table rows; optionally, you can specify paths to any extra data you'd like to add to your table:
         
@@ -116,15 +114,15 @@
         ```
         
         
         # FAQ
         
         1. **Why not `xmltodict`?** `xmltodict` can convert arbitrary XML to a python dict. However, it is 2-3 times slower than `xmlrecords` and does not support some features specific for tablular data.
         
-        2. **Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
+        2. **Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using `xml` or `lxml` directly is a viable option too - in case this package doesn't cover your particular use case.
         
 Keywords: xml parsing
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: xmlrecords Version: 0.2.5 Summary: This package can
+Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.0 Summary: This package can
 convert an XML files to a list of records Home-page: UNKNOWN Author: Yaroslav
 Kopotilov Author-email: datascience@tuta.io License: Apache License, Version
-2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of `xml`
-package for extraction of tabular data from XML files. >>> This data provider
-sends all his data in... XML. You know nothing about XML, except that it looks
-kind of weird and you would *definitely* never use it for tabular data. How
-could you just transform all this XML nightmare into a sensible tabular format,
-like a DataFrame? Don't worry: you are in the right place! # Installation
-```shell script pip install xmlrecords ``` - The package requires `python 3.7+`
-and no external dependencies. - The package uses `xml.etree.ElementTree` so
-it's vulnerable to [billion laughs attack](https://en.wikipedia.org/wiki/
-Billion_laughs_attack). # Usage ## Basic example Usually, you only need to
-specify path to table rows; optionally, you can specify paths to any extra data
-you'd like to add to your table: ```python # XML object xml_bytes = b"""\ <?xml
-version="1.0" encoding="utf-8"?>   Virtual Shore   2020-02-02T05:12:22
+2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of
+`lxml` package for extraction of tabular data from XML files. >>> This data
+provider sends all his data in... XML. You know nothing about XML, except that
+it looks kind of weird and you would *definitely* never use it for tabular
+data. How could you just transform all this XML nightmare into a sensible
+tabular format, like a DataFrame? Don't worry: you are in the right place! #
+Installation ```shell script pip install xmlrecords ``` The package requires
+`python 3.7+` and one external dependency `lxml`. # Usage ## Basic example
+Usually, you only need to specify path to table rows; optionally, you can
+specify paths to any extra data you'd like to add to your table: ```python #
+XML object xml_bytes = b"""\ <?xml version="1.0" encoding="utf-8"?>   Virtual
+Shore   2020-02-02T05:12:22
  2017 112.34
  1963 10    """ # Transform XML to records (= a list of key-value pairs) import
 xmlrecords records = xmlrecords.parse( xml=xml_bytes, records_path=['Shelf',
 'Book'], # The rows are XML nodes with the repeating tag  meta_paths=[
 ['Library', 'Name'], ['Shelf', 'Timestamp']], # Add additional "meta" nodes )
 for r in records: print(r) # Output: # {'Name': 'Virtual Shore', 'Timestamp':
 '2020-02-02T05:12:22', 'Title': 'Sunny Night', 'alive': 'no', 'name':
@@ -35,15 +34,15 @@
 conn.cursor() c.execute("""\ CREATE TABLE BOOKS ( LIBRARY_NAME TEXT,
 SHELF_TIMESTAMP TEXT, TITLE TEXT, AUTHOR_ALIVE TEXT, AUTHOR_NAME TEXT, YEAR
 INT, PRICE FLOAT, PRIMARY KEY (TITLE, AUTHOR_NAME) ) """ ) c.executemany
 ( """INSERT INTO BOOKS VALUES (?,?,?,?,?,?,?)""", [list(x.values()) for x in
 records], ) conn.commit() ``` # FAQ 1. **Why not `xmltodict`?** `xmltodict` can
 convert arbitrary XML to a python dict. However, it is 2-3 times slower than
 `xmlrecords` and does not support some features specific for tablular data. 2.
-**Why not `xml` or `lxml`**? `xmlrecords` uses `xml` under the hood. Using
+**Why not `xml` or `lxml`**? `xmlrecords` uses `lxml` under the hood. Using
 `xml` or `lxml` directly is a viable option too - in case this package doesn't
 cover your particular use case. Keywords: xml parsing Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
```

