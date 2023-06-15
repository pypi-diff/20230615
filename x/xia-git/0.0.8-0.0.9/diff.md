# Comparing `tmp/xia_git-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 118962 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-08 17:35 xia_git/__init__.py
--rw-r--r--  2.0 unx   285696 b- defN 23-Jun-08 17:37 xia_git/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-08 17:37 xia_git-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      625 b- defN 23-Jun-08 17:37 xia_git-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-08 17:37 xia_git-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-08 17:37 xia_git-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      550 b- defN 23-Jun-08 17:37 xia_git-0.0.8.dist-info/RECORD
-7 files, 287205 bytes uncompressed, 117984 bytes compressed:  58.9%
+Zip file size: 118955 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-10 15:33 xia_git/__init__.py
+-rw-r--r--  2.0 unx   285696 b- defN 23-Jun-10 15:36 xia_git/git.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-10 15:36 xia_git-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      625 b- defN 23-Jun-10 15:36 xia_git-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 15:36 xia_git-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-10 15:36 xia_git-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      550 b- defN 23-Jun-10 15:36 xia_git-0.0.9.dist-info/RECORD
+7 files, 287205 bytes uncompressed, 117977 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
 Filename: xia_git/git.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_git-0.0.8.dist-info/LICENSE.txt
+Filename: xia_git-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.0.8.dist-info/METADATA
+Filename: xia_git-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.0.8.dist-info/WHEEL
+Filename: xia_git-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.0.8.dist-info/top_level.txt
+Filename: xia_git-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.0.8.dist-info/RECORD
+Filename: xia_git-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## Comparing `xia_git-0.0.8.dist-info/METADATA` & `xia_git-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git
-Version: 0.0.8
+Version: 0.0.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

