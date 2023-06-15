# Comparing `tmp/ipa-4.8.9-py2.py3-none-any.whl.zip` & `tmp/ipa-4.9.12-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1353 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     1183 b- defN 20-Aug-20 10:51 ipa-4.8.9.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 20-Aug-20 10:51 ipa-4.8.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 20-Aug-20 10:51 ipa-4.8.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      282 b- defN 20-Aug-20 10:51 ipa-4.8.9.dist-info/RECORD
-4 files, 1576 bytes uncompressed, 803 bytes compressed:  49.0%
+Zip file size: 1361 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1183 b- defN 23-Jun-15 05:41 ipa-4.9.12.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 05:41 ipa-4.9.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-15 05:41 ipa-4.9.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      286 b- defN 23-Jun-15 05:41 ipa-4.9.12.dist-info/RECORD
+4 files, 1580 bytes uncompressed, 803 bytes compressed:  49.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: ipa-4.8.9.dist-info/METADATA
+Filename: ipa-4.9.12.dist-info/METADATA
 Comment: 
 
-Filename: ipa-4.8.9.dist-info/WHEEL
+Filename: ipa-4.9.12.dist-info/WHEEL
 Comment: 
 
-Filename: ipa-4.8.9.dist-info/top_level.txt
+Filename: ipa-4.9.12.dist-info/top_level.txt
 Comment: 
 
-Filename: ipa-4.8.9.dist-info/RECORD
+Filename: ipa-4.9.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ipa-4.8.9.dist-info/METADATA` & `ipa-4.9.12.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ipa
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

