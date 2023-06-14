# Comparing `tmp/cns-1.0.15-py3-none-any.whl.zip` & `tmp/cns-1.0.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 841246 bytes, number of entries: 26
+Zip file size: 778670 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-14 14:45 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   162304 b- defN 23-Jun-14 14:47 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    91648 b- defN 23-Jun-14 23:19 cns/ScrapyX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    80896 b- defN 23-Jun-14 23:20 cns/ScrapyX.cp39-win_amd64.pyd
@@ -15,14 +15,13 @@
 -rw-rw-rw-  2.0 fat    68096 b- defN 20-Aug-06 08:59 cns/auto_dump.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82432 b- defN 20-Mar-13 09:16 cns/lbsql.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    52736 b- defN 20-Aug-27 02:31 cns/mailyanzheng.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Apr-17 01:55 cns/sql_str.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    77312 b- defN 21-Nov-08 02:21 cns/str2sql.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    81920 b- defN 20-Aug-27 07:07 cns/tpass.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    62976 b- defN 20-Sep-15 11:09 cns/wxlogin.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat   148480 b- defN 22-Dec-28 07:55 cns/xdata.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-14 23:24 cns-1.0.15.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-14 23:24 cns-1.0.15.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 23:24 cns-1.0.15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 23:24 cns-1.0.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2200 b- defN 23-Jun-14 23:24 cns-1.0.15.dist-info/RECORD
-26 files, 1932564 bytes uncompressed, 837742 bytes compressed:  56.7%
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2113 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/RECORD
+25 files, 1783997 bytes uncompressed, 775298 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -54,26 +54,23 @@
 
 Filename: cns/tpass.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/wxlogin.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns/xdata.cp36-win_amd64.pyd
+Filename: cns-1.0.16.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.15.dist-info/LICENSE
+Filename: cns-1.0.16.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.15.dist-info/METADATA
+Filename: cns-1.0.16.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.15.dist-info/WHEEL
+Filename: cns-1.0.16.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.15.dist-info/top_level.txt
-Comment: 
-
-Filename: cns-1.0.15.dist-info/RECORD
+Filename: cns-1.0.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cns-1.0.15.dist-info/METADATA` & `cns-1.0.16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.15
+Version: 1.0.16
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.15.dist-info/RECORD` & `cns-1.0.16.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,12 @@
 cns/auto_dump.cp36-win_amd64.pyd,sha256=GD6r61Kv1liA5jjwRqThGpV5y-tuZIsCVy7GcVErY4A,68096
 cns/lbsql.cp36-win_amd64.pyd,sha256=a4BJsW6afDKZpon8EtAyMfSqXZXKpD-lJ6p31tRQ17A,82432
 cns/mailyanzheng.cp36-win_amd64.pyd,sha256=xN0mbUUgqjQTpZbSzxtMoEb86DbvBzWLxCGszZL1PjI,52736
 cns/sql_str.cp36-win_amd64.pyd,sha256=icFmVu1qbAu18pQp5tsh3UnPNZZbGrNyr745WraWUOY,88576
 cns/str2sql.cp36-win_amd64.pyd,sha256=76YB5PQgAMzhg-r_658einLms215CuIlp3NBs4Gi6cA,77312
 cns/tpass.cp36-win_amd64.pyd,sha256=ZxUB2uszEbd6l-Dc6cfVEqgO2FrIyy9ab7hsET89nKE,81920
 cns/wxlogin.cp36-win_amd64.pyd,sha256=PTfms5LF-AmF_ofWLr_pLZg-yybVJnMzblZ-0kqNb6I,62976
-cns/xdata.cp36-win_amd64.pyd,sha256=2GZLU9ShrOZIcTBQnscVzNNsrIvpXnseGFRFL1iNZK8,148480
-cns-1.0.15.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.15.dist-info/METADATA,sha256=7FmwDoZLEl1fN47pgaBIjL1JQ0r25UcXB2njMGlu7T0,1905
-cns-1.0.15.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.15.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.15.dist-info/RECORD,,
+cns-1.0.16.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.16.dist-info/METADATA,sha256=KLPh3YIQE2DvWi82Tf_uEjkjTetZxLP7A9EjkP3AoSg,1905
+cns-1.0.16.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.16.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.16.dist-info/RECORD,,
```

