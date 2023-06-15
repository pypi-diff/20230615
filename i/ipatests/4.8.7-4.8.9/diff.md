# Comparing `tmp/ipatests-4.8.7-py2.py3-none-any.whl.zip` & `tmp/ipatests-4.8.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 1693 bytes, number of entries: 5
 -rw-rw-r--  2.0 unx      139 b- defN 19-Apr-08 14:24 ipatests/__init__.py
--rw-rw-r--  2.0 unx     1188 b- defN 20-Jun-10 19:58 ipatests-4.8.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 20-Jun-10 19:58 ipatests-4.8.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 20-Jun-10 19:58 ipatests-4.8.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      378 b- defN 20-Jun-10 19:58 ipatests-4.8.7.dist-info/RECORD
+-rw-rw-r--  2.0 unx     1188 b- defN 20-Aug-20 10:51 ipatests-4.8.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 20-Aug-20 10:51 ipatests-4.8.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 20-Aug-20 10:51 ipatests-4.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      378 b- defN 20-Aug-20 10:51 ipatests-4.8.9.dist-info/RECORD
 5 files, 1824 bytes uncompressed, 987 bytes compressed:  45.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: ipatests/__init__.py
 Comment: 
 
-Filename: ipatests-4.8.7.dist-info/METADATA
+Filename: ipatests-4.8.9.dist-info/METADATA
 Comment: 
 
-Filename: ipatests-4.8.7.dist-info/WHEEL
+Filename: ipatests-4.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: ipatests-4.8.7.dist-info/top_level.txt
+Filename: ipatests-4.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ipatests-4.8.7.dist-info/RECORD
+Filename: ipatests-4.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ipatests-4.8.7.dist-info/METADATA` & `ipatests-4.8.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipatests
-Version: 4.8.7
+Version: 4.8.9
 Summary: Dummy package for FreeIPA
 Home-page: https://www.freeipa.org/
 Author: FreeIPA Developers
 Author-email: freeipa-devel@lists.fedorahosted.org
 Maintainer: FreeIPA Developers
 Maintainer-email: freeipa-devel@redhat.com
 License: GPLv3
@@ -21,12 +21,12 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.6.0
-Requires-Dist: ipaclient (==4.8.7)
+Requires-Dist: ipaclient (==4.8.9)
 
 Dummy package for FreeIPA
```

