# Comparing `tmp/ipaserver-4.8.7-py2.py3-none-any.whl.zip` & `tmp/ipaserver-4.8.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1706 bytes, number of entries: 5
+Zip file size: 1704 bytes, number of entries: 5
 -rw-rw-r--  2.0 unx      140 b- defN 19-Apr-08 14:24 ipaserver/__init__.py
--rw-rw-r--  2.0 unx     1189 b- defN 20-Jun-10 19:58 ipaserver-4.8.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 20-Jun-10 19:58 ipaserver-4.8.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 20-Jun-10 19:58 ipaserver-4.8.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      384 b- defN 20-Jun-10 19:58 ipaserver-4.8.7.dist-info/RECORD
-5 files, 1833 bytes uncompressed, 990 bytes compressed:  46.0%
+-rw-rw-r--  2.0 unx     1189 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      384 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/RECORD
+5 files, 1833 bytes uncompressed, 988 bytes compressed:  46.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: ipaserver/__init__.py
 Comment: 
 
-Filename: ipaserver-4.8.7.dist-info/METADATA
+Filename: ipaserver-4.8.9.dist-info/METADATA
 Comment: 
 
-Filename: ipaserver-4.8.7.dist-info/WHEEL
+Filename: ipaserver-4.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: ipaserver-4.8.7.dist-info/top_level.txt
+Filename: ipaserver-4.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ipaserver-4.8.7.dist-info/RECORD
+Filename: ipaserver-4.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ipaserver-4.8.7.dist-info/METADATA` & `ipaserver-4.8.9.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipaserver
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

