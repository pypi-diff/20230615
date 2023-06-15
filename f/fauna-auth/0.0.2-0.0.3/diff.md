# Comparing `tmp/fauna_auth-0.0.2-py3-none-any.whl.zip` & `tmp/fauna_auth-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5308 bytes, number of entries: 7
+Zip file size: 5310 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 fauna_auth/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 fauna_auth/accounts.py
 -rw-r--r--  2.0 unx     2372 b- defN 80-Jan-01 00:00 fauna_auth/oauth.py
 -rw-r--r--  2.0 unx     3813 b- defN 80-Jan-01 00:00 fauna_auth/public_key.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx      525 b- defN 16-Jan-01 00:00 fauna_auth-0.0.2.dist-info/RECORD
-7 files, 7465 bytes uncompressed, 4380 bytes compressed:  41.3%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fauna_auth-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 fauna_auth-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx      525 b- defN 16-Jan-01 00:00 fauna_auth-0.0.3.dist-info/RECORD
+7 files, 7465 bytes uncompressed, 4382 bytes compressed:  41.3%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: fauna_auth/oauth.py
 Comment: 
 
 Filename: fauna_auth/public_key.py
 Comment: 
 
-Filename: fauna_auth-0.0.2.dist-info/WHEEL
+Filename: fauna_auth-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: fauna_auth-0.0.2.dist-info/METADATA
+Filename: fauna_auth-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: fauna_auth-0.0.2.dist-info/RECORD
+Filename: fauna_auth-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fauna_auth-0.0.2.dist-info/METADATA` & `fauna_auth-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fauna-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: Helper library
 Author: Edward FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.86.0,<0.87.0)
+Requires-Dist: fastapi (>=0.97.0,<0.98.0)
 Requires-Dist: jwcrypto (>=1.5.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # fauna-auth
 
 A helper library for working with authentication
```

