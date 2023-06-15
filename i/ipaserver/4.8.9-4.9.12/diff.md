# Comparing `tmp/ipaserver-4.8.9-py2.py3-none-any.whl.zip` & `tmp/ipaserver-4.9.12-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1704 bytes, number of entries: 5
--rw-rw-r--  2.0 unx      140 b- defN 19-Apr-08 14:24 ipaserver/__init__.py
--rw-rw-r--  2.0 unx     1189 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      384 b- defN 20-Aug-20 10:51 ipaserver-4.8.9.dist-info/RECORD
-5 files, 1833 bytes uncompressed, 988 bytes compressed:  46.1%
+Zip file size: 1711 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      140 b- defN 20-Sep-30 13:07 ipaserver/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 23-Jun-15 05:41 ipaserver-4.9.12.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 05:41 ipaserver-4.9.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-15 05:41 ipaserver-4.9.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      388 b- defN 23-Jun-15 05:41 ipaserver-4.9.12.dist-info/RECORD
+5 files, 1837 bytes uncompressed, 987 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: ipaserver/__init__.py
 Comment: 
 
-Filename: ipaserver-4.8.9.dist-info/METADATA
+Filename: ipaserver-4.9.12.dist-info/METADATA
 Comment: 
 
-Filename: ipaserver-4.8.9.dist-info/WHEEL
+Filename: ipaserver-4.9.12.dist-info/WHEEL
 Comment: 
 
-Filename: ipaserver-4.8.9.dist-info/top_level.txt
+Filename: ipaserver-4.9.12.dist-info/top_level.txt
 Comment: 
 
-Filename: ipaserver-4.8.9.dist-info/RECORD
+Filename: ipaserver-4.9.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ipaserver-4.8.9.dist-info/METADATA` & `ipaserver-4.9.12.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ipaserver
-Version: 4.8.9
+Version: 4.9.12
 Summary: Dummy package for FreeIPA
 Home-page: https://www.freeipa.org/
+Download-URL: https://www.freeipa.org/page/Downloads
 Author: FreeIPA Developers
 Author-email: freeipa-devel@lists.fedorahosted.org
 Maintainer: FreeIPA Developers
 Maintainer-email: freeipa-devel@redhat.com
 License: GPLv3
-Download-URL: https://www.freeipa.org/page/Downloads
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -21,12 +21,10 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Requires-Python: >=3.6.0
-Requires-Dist: ipaclient (==4.8.9)
+Requires-Dist: ipaclient (==4.9.12)
 
 Dummy package for FreeIPA
-
-
```

