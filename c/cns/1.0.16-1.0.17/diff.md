# Comparing `tmp/cns-1.0.16-py3-none-any.whl.zip` & `tmp/cns-1.0.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,17 @@
-Zip file size: 778670 bytes, number of entries: 25
+Zip file size: 393194 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-14 14:45 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   162304 b- defN 23-Jun-14 14:47 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    91648 b- defN 23-Jun-14 23:19 cns/ScrapyX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    80896 b- defN 23-Jun-14 23:20 cns/ScrapyX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   138752 b- defN 21-May-25 06:18 cns/SqlAdm.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    81408 b- defN 23-Jun-15 01:46 cns/SQLstrX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    70144 b- defN 23-Jun-15 01:46 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    69120 b- defN 23-Jun-14 22:59 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    56320 b- defN 23-Jun-14 23:01 cns/TextX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    53248 b- defN 20-Nov-17 06:13 cns/Xtoken.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat   162304 b- defN 21-May-14 09:02 cns/ZdyLogic.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1229 b- defN 23-Jun-14 23:02 cns/__init__.py
--rw-rw-rw-  2.0 fat    68096 b- defN 20-Aug-06 08:59 cns/auto_dump.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    82432 b- defN 20-Mar-13 09:16 cns/lbsql.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    52736 b- defN 20-Aug-27 02:31 cns/mailyanzheng.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    88576 b- defN 23-Apr-17 01:55 cns/sql_str.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    77312 b- defN 21-Nov-08 02:21 cns/str2sql.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    81920 b- defN 20-Aug-27 07:07 cns/tpass.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    62976 b- defN 20-Sep-15 11:09 cns/wxlogin.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2113 b- defN 23-Jun-14 23:37 cns-1.0.16.dist-info/RECORD
-25 files, 1783997 bytes uncompressed, 775298 bytes compressed:  56.5%
+-rw-rw-rw-  2.0 fat      342 b- defN 23-Jun-15 01:47 cns/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-15 01:49 cns-1.0.17.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-15 01:49 cns-1.0.17.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-15 01:49 cns-1.0.17.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-15 01:49 cns-1.0.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1228 b- defN 23-Jun-15 01:49 cns-1.0.17.dist-info/RECORD
+15 files, 892881 bytes uncompressed, 391186 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -9,68 +9,38 @@
 
 Filename: cns/DateTimeX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/DateTimeX.cp39-win_amd64.pyd
 Comment: 
 
-Filename: cns/ScrapyX.cp36-win_amd64.pyd
+Filename: cns/SQLstrX.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns/ScrapyX.cp39-win_amd64.pyd
-Comment: 
-
-Filename: cns/SqlAdm.cp36-win_amd64.pyd
+Filename: cns/SQLstrX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/TextX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/TextX.cp39-win_amd64.pyd
 Comment: 
 
-Filename: cns/Xtoken.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/ZdyLogic.cp36-win_amd64.pyd
-Comment: 
-
 Filename: cns/__init__.py
 Comment: 
 
-Filename: cns/auto_dump.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/lbsql.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/mailyanzheng.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/sql_str.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/str2sql.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/tpass.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns/wxlogin.cp36-win_amd64.pyd
-Comment: 
-
-Filename: cns-1.0.16.dist-info/LICENSE
+Filename: cns-1.0.17.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.16.dist-info/METADATA
+Filename: cns-1.0.17.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.16.dist-info/WHEEL
+Filename: cns-1.0.17.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.16.dist-info/top_level.txt
+Filename: cns-1.0.17.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.16.dist-info/RECORD
+Filename: cns-1.0.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -1,28 +1,7 @@
 # 定义当使用“from my_package import *”时导入的内容
 #__all__ = ["DateTimeX"]  # *导入类时限制在此范围
 
-from .ZdyLogic import ZdyLogic       # 自定义逻辑
-from .lbsql import LbSQL             # 数据库查
-from .auto_dump import AutoDump      # 自动镜像
-from .str2sql import Str2SQL         # WEB表单TO SQL
-from .wxlogin import WxLogin         # 微信服务接口
-from .mailyanzheng import MailYanZheng #邮箱验证码
-from .tpass import Tpass             # 手机动态密码
-from .SqlAdm import SqlAdm           # 数据库增删改查
-from .Xtoken import Xtoken           # URL动态令牌
-from .sql_str import SQLstr          # RPA机器人 SQL转换
-from .DateTimeX import DateTimeX     # 超级日期获取
+from .DateTimeX import DateTimeX     # 日期获取
 from .DataX import DataX             # 数据处理
-from .ScrapyX import ScrapyX         # Scrapy
 from .TextX import TextX             # 文本处理
-
-
-
-#from .dbcfg import DATABASES, CACHES  # 数据库配置
-#from .login import login              # 登录
-#from .hy_tl_task import hy_tl_task    # 塔罗
-#from .hy_bk_task import hy_bk_task    # 必看
-#from .hy_download import hy_download  # 下载
-#from .zg_download import ZhuGe        # 下载
-
-
+from .SQLstrX import SQLstrX         # RPASQL处理
```

## Comparing `cns-1.0.16.dist-info/METADATA` & `cns-1.0.17.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.16
+Version: 1.0.17
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.16.dist-info/RECORD` & `cns-1.0.17.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 cns/DataX.cp36-win_amd64.pyd,sha256=DfOcY3McK3IopN5AF4knaWYzsyb-YTt-6fWVbLc6kv0,178176
 cns/DataX.cp39-win_amd64.pyd,sha256=RRrJWWU0eJJv-stRpdnAR1OfbT3MjSVEfBVGLGIrY_8,162304
 cns/DateTimeX.cp36-win32.pyd,sha256=X6jjFZbOMmTTqnw0r3SfmiTRG9RFEpRdfVyU6AiFvCk,82944
 cns/DateTimeX.cp36-win_amd64.pyd,sha256=w-g6QPTK_U3il2bFu7PcucBGixhSX2Gm4M54ItAYMTk,99840
 cns/DateTimeX.cp39-win_amd64.pyd,sha256=bp9N6_ettlJ1odtrHJ3qU_yTBAsvULggzIyfz-eJuEk,88576
-cns/ScrapyX.cp36-win_amd64.pyd,sha256=4ILgkKmpcl-JN-c78Z7HpesHz0m3kun3OqHaCSADgEo,91648
-cns/ScrapyX.cp39-win_amd64.pyd,sha256=RD7BzkICoauBh8m9-DikOQts0hiTzaLmDGds_zaPOXM,80896
-cns/SqlAdm.cp36-win_amd64.pyd,sha256=K3sJ3Xj1Klfhv5dCfC3h3KOvrjf2HDnPerymWvqVMFU,138752
+cns/SQLstrX.cp36-win_amd64.pyd,sha256=bequp2YIkC8eDH-HhI3bt7nVK1Fe30LCVjg5iCNU6Vo,81408
+cns/SQLstrX.cp39-win_amd64.pyd,sha256=LgXb-6X5DLVXXozjWVxP95cFSIidIOuor1vL_1d7XqI,70144
 cns/TextX.cp36-win_amd64.pyd,sha256=NunYn84nTxrd0_PfZng43gek6VXrD8OBRSEnEQaCVZM,69120
 cns/TextX.cp39-win_amd64.pyd,sha256=3ltkD0qvLBqDjYHqp14FR_Df6NAGM19T74HN2Q9ROsQ,56320
-cns/Xtoken.cp36-win_amd64.pyd,sha256=C8PfvwOnWljeFCvXlYWr9Iuehhrdo5i5GH3oEWYsldA,53248
-cns/ZdyLogic.cp36-win_amd64.pyd,sha256=FINLf_x1rGQNbEyVtuf9DVDfCeelcqMqFfja53wTHww,162304
-cns/__init__.py,sha256=e7weXnKPex-nbYNC3AvfT2IouDAVLy4WYtz9KlVubJc,1229
-cns/auto_dump.cp36-win_amd64.pyd,sha256=GD6r61Kv1liA5jjwRqThGpV5y-tuZIsCVy7GcVErY4A,68096
-cns/lbsql.cp36-win_amd64.pyd,sha256=a4BJsW6afDKZpon8EtAyMfSqXZXKpD-lJ6p31tRQ17A,82432
-cns/mailyanzheng.cp36-win_amd64.pyd,sha256=xN0mbUUgqjQTpZbSzxtMoEb86DbvBzWLxCGszZL1PjI,52736
-cns/sql_str.cp36-win_amd64.pyd,sha256=icFmVu1qbAu18pQp5tsh3UnPNZZbGrNyr745WraWUOY,88576
-cns/str2sql.cp36-win_amd64.pyd,sha256=76YB5PQgAMzhg-r_658einLms215CuIlp3NBs4Gi6cA,77312
-cns/tpass.cp36-win_amd64.pyd,sha256=ZxUB2uszEbd6l-Dc6cfVEqgO2FrIyy9ab7hsET89nKE,81920
-cns/wxlogin.cp36-win_amd64.pyd,sha256=PTfms5LF-AmF_ofWLr_pLZg-yybVJnMzblZ-0kqNb6I,62976
-cns-1.0.16.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.16.dist-info/METADATA,sha256=KLPh3YIQE2DvWi82Tf_uEjkjTetZxLP7A9EjkP3AoSg,1905
-cns-1.0.16.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.16.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.16.dist-info/RECORD,,
+cns/__init__.py,sha256=E3XCxd-Z01Q13FBOOMwYpfPHdhGSSaB12uEwy33EqBg,342
+cns-1.0.17.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.17.dist-info/METADATA,sha256=Y0yYpcT7XvbvBbrtVBHTgir_lwZ77aGPKHZIitbylUs,1905
+cns-1.0.17.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.17.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.17.dist-info/RECORD,,
```

