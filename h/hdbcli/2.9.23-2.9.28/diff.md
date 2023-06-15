# Comparing `tmp/hdbcli-2.9.23-cp39-cp39-win_amd64.whl.zip` & `tmp/hdbcli-2.9.28-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3613570 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat  8766600 b- defN 21-Jul-02 17:34 pyhdbcli.pyd
--rw-rw-rw-  2.0 fat      162 b- defN 21-Jul-02 17:34 hdbcli/__init__.py
--rw-rw-rw-  2.0 fat     3174 b- defN 21-Jul-02 17:34 hdbcli/dbapi.py
--rw-rw-rw-  2.0 fat       49 b- defN 21-Jul-02 17:34 hdbcli/resultrow.py
--rw-rw-rw-  2.0 fat    12608 b- defN 21-Jul-02 17:34 hdbcli-2.9.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6132 b- defN 21-Jul-02 17:34 hdbcli-2.9.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat      105 b- defN 21-Jul-02 17:34 hdbcli-2.9.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 21-Jul-02 17:34 hdbcli-2.9.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      680 b- defN 21-Jul-02 17:34 hdbcli-2.9.23.dist-info/RECORD
-9 files, 8789526 bytes uncompressed, 3612418 bytes compressed:  58.9%
+Zip file size: 3614854 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat  8768120 b- defN 21-Aug-04 20:23 pyhdbcli.pyd
+-rw-rw-rw-  2.0 fat      162 b- defN 21-Aug-04 20:22 hdbcli/__init__.py
+-rw-rw-rw-  2.0 fat     3174 b- defN 21-Aug-04 20:22 hdbcli/dbapi.py
+-rw-rw-rw-  2.0 fat       49 b- defN 21-Aug-04 20:22 hdbcli/resultrow.py
+-rw-rw-rw-  2.0 fat    12608 b- defN 21-Aug-04 20:23 hdbcli-2.9.28.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6132 b- defN 21-Aug-04 20:23 hdbcli-2.9.28.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      105 b- defN 21-Aug-04 20:23 hdbcli-2.9.28.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 21-Aug-04 20:23 hdbcli-2.9.28.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      680 b- defN 21-Aug-04 20:23 hdbcli-2.9.28.dist-info/RECORD
+9 files, 8791046 bytes uncompressed, 3613702 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: hdbcli/dbapi.py
 Comment: 
 
 Filename: hdbcli/resultrow.py
 Comment: 
 
-Filename: hdbcli-2.9.23.dist-info/LICENSE
+Filename: hdbcli-2.9.28.dist-info/LICENSE
 Comment: 
 
-Filename: hdbcli-2.9.23.dist-info/METADATA
+Filename: hdbcli-2.9.28.dist-info/METADATA
 Comment: 
 
-Filename: hdbcli-2.9.23.dist-info/WHEEL
+Filename: hdbcli-2.9.28.dist-info/WHEEL
 Comment: 
 
-Filename: hdbcli-2.9.23.dist-info/top_level.txt
+Filename: hdbcli-2.9.28.dist-info/top_level.txt
 Comment: 
 
-Filename: hdbcli-2.9.23.dist-info/RECORD
+Filename: hdbcli-2.9.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hdbcli/__init__.py

```diff
@@ -5,8 +5,8 @@
 # Python DB API v2.0
 # NewDB client library
 
 
 __all__ = [
     'dbapi',
     ]
-__version__ = '2.9.23'
+__version__ = '2.9.28'
```

## Comparing `hdbcli-2.9.23.dist-info/LICENSE` & `hdbcli-2.9.28.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hdbcli-2.9.23.dist-info/METADATA` & `hdbcli-2.9.28.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdbcli
-Version: 2.9.23
+Version: 2.9.28
 Summary: SAP HANA Python Client
 Home-page: https://www.sap.com/
 Author: SAP SE
 License: SAP DEVELOPER LICENSE AGREEMENT
 Project-URL: Documentation, https://help.sap.com/viewer/f1b440ded6144a54ada97ff95dac7adf/latest/en-US/f3b8fabf34324302b123297cdbe710f0.html
 Keywords: SAP HANA client in-memory database SQL business application intelligent enterprise cloud analytics experience
 Platform: UNKNOWN
```

