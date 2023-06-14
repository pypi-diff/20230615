# Comparing `tmp/cns-1.0.11-py3-none-any.whl.zip` & `tmp/cns-1.0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 710129 bytes, number of entries: 23
+Zip file size: 750762 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-14 14:45 cns/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   162304 b- defN 23-Jun-14 14:47 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    92672 b- defN 23-Jun-14 21:55 cns/ScrapyX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   138752 b- defN 21-May-25 06:18 cns/SqlAdm.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    53248 b- defN 20-Nov-17 06:13 cns/Xtoken.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   162304 b- defN 21-May-14 09:02 cns/ZdyLogic.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1125 b- defN 23-Jun-14 16:08 cns/__init__.py
+-rw-rw-rw-  2.0 fat     1174 b- defN 23-Jun-14 21:57 cns/__init__.py
 -rw-rw-rw-  2.0 fat    68096 b- defN 20-Aug-06 08:59 cns/auto_dump.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82432 b- defN 20-Mar-13 09:16 cns/lbsql.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    52736 b- defN 20-Aug-27 02:31 cns/mailyanzheng.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Apr-17 01:55 cns/sql_str.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    77312 b- defN 21-Nov-08 02:21 cns/str2sql.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     2787 b- defN 23-Jun-14 15:47 cns/test_DataX.py
 -rw-rw-rw-  2.0 fat    81920 b- defN 20-Aug-27 07:07 cns/tpass.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    62976 b- defN 20-Sep-15 11:09 cns/wxlogin.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   148480 b- defN 22-Dec-28 07:55 cns/xdata.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-14 21:33 cns-1.0.11.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2013 b- defN 23-Jun-14 21:33 cns-1.0.11.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 21:33 cns-1.0.11.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 21:33 cns-1.0.11.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1926 b- defN 23-Jun-14 21:33 cns-1.0.11.dist-info/RECORD
-23 files, 1637097 bytes uncompressed, 707051 bytes compressed:  56.8%
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-14 22:13 cns-1.0.12.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1905 b- defN 23-Jun-14 22:13 cns-1.0.12.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 22:13 cns-1.0.12.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-14 22:12 cns-1.0.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2014 b- defN 23-Jun-14 22:13 cns-1.0.12.dist-info/RECORD
+24 files, 1729798 bytes uncompressed, 747548 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: cns/DateTimeX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/DateTimeX.cp39-win_amd64.pyd
 Comment: 
 
+Filename: cns/ScrapyX.cp36-win_amd64.pyd
+Comment: 
+
 Filename: cns/SqlAdm.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/Xtoken.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/ZdyLogic.cp36-win_amd64.pyd
@@ -48,23 +51,23 @@
 
 Filename: cns/wxlogin.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/xdata.cp36-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.0.11.dist-info/LICENSE
+Filename: cns-1.0.12.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.11.dist-info/METADATA
+Filename: cns-1.0.12.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.11.dist-info/WHEEL
+Filename: cns-1.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.11.dist-info/top_level.txt
+Filename: cns-1.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.11.dist-info/RECORD
+Filename: cns-1.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -9,14 +9,16 @@
 from .mailyanzheng import MailYanZheng #邮箱验证码
 from .tpass import Tpass             # 手机动态密码
 from .SqlAdm import SqlAdm           # 数据库增删改查
 from .Xtoken import Xtoken           # URL动态令牌
 from .sql_str import SQLstr          # RPA机器人 SQL转换
 from .DateTimeX import DateTimeX     # 超级日期获取
 from .DataX import DataX             # 数据处理
+from .ScrapyX import ScrapyX         # Scrapy
+
 
 #from .dbcfg import DATABASES, CACHES  # 数据库配置
 #from .login import login              # 登录
 #from .hy_tl_task import hy_tl_task    # 塔罗
 #from .hy_bk_task import hy_bk_task    # 必看
 #from .hy_download import hy_download  # 下载
 #from .zg_download import ZhuGe        # 下载
```

## Comparing `cns-1.0.11.dist-info/METADATA` & `cns-1.0.12.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.11
+Version: 1.0.12
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,27 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: python-dateutil
 
 # cns
-cns 常用的工具包，目前支持日期快速,后续将不断增多
+cns常用的工具包, 更多功能探索中
 
 ## 安装方法
-
-要安装，只需要运行
-
 pip install cns
 
 
 ## 使用方法
-
-安装后，只需导入和使用:
-
 ```python代码
 from cns import DateTimeX
 
 if __name__ == "__main__":
 
     dfx  = DateTimeX()  # 可初始化 "2023-05-28 23:23:51"
 
@@ -49,19 +43,18 @@
     print("前35天的日期:", dfx.get("{[年-月-日||复位-35日]}"))
 
     print("昨天的月1号:", dfx.get("{[年-月-初||复位-1日]}"))
 
     print("昨天的本月:", dfx.get("{[年-月||复位-1日]}"))
 
 
-
 '''
 # 说明：
 1、分隔符“||” 左侧是获取的时间格式，右侧是时间计算的指令；
 2、左左侧的字符串中通包含年、月、日、时、分、秒、初、末，用来获取时间和格式，其中“初”是获数字1，“末”最后一天的日期；
 3、右侧是时间计算的指令支持年、月、日、时、分、秒、复位，用来对当前的时间进行加和减的计算，其中“复位”代表恢复到初始时间；
 
-注意：目前仅支持Python 3.6  3.9  
-请联系作者  6566666@qq.com
+目前支持Python 3.6、3.9  
+联系作者：6566666@qq.com
 '''
```

## Comparing `cns-1.0.11.dist-info/RECORD` & `cns-1.0.12.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 cns/DataX.cp36-win_amd64.pyd,sha256=DfOcY3McK3IopN5AF4knaWYzsyb-YTt-6fWVbLc6kv0,178176
 cns/DataX.cp39-win_amd64.pyd,sha256=RRrJWWU0eJJv-stRpdnAR1OfbT3MjSVEfBVGLGIrY_8,162304
 cns/DateTimeX.cp36-win32.pyd,sha256=X6jjFZbOMmTTqnw0r3SfmiTRG9RFEpRdfVyU6AiFvCk,82944
 cns/DateTimeX.cp36-win_amd64.pyd,sha256=w-g6QPTK_U3il2bFu7PcucBGixhSX2Gm4M54ItAYMTk,99840
 cns/DateTimeX.cp39-win_amd64.pyd,sha256=bp9N6_ettlJ1odtrHJ3qU_yTBAsvULggzIyfz-eJuEk,88576
+cns/ScrapyX.cp36-win_amd64.pyd,sha256=wOqEBUULwmklSAOaINa7rSvpkURD3gA5y-e7hmyRqo0,92672
 cns/SqlAdm.cp36-win_amd64.pyd,sha256=K3sJ3Xj1Klfhv5dCfC3h3KOvrjf2HDnPerymWvqVMFU,138752
 cns/Xtoken.cp36-win_amd64.pyd,sha256=C8PfvwOnWljeFCvXlYWr9Iuehhrdo5i5GH3oEWYsldA,53248
 cns/ZdyLogic.cp36-win_amd64.pyd,sha256=FINLf_x1rGQNbEyVtuf9DVDfCeelcqMqFfja53wTHww,162304
-cns/__init__.py,sha256=Mmn-ye9dejieZfAZag1NYhAiHGOoTrFPliPj7cAozr8,1125
+cns/__init__.py,sha256=lmzDj5HawoOUqsWXD8tluM61wrqoIpMqcioWErUNfpQ,1174
 cns/auto_dump.cp36-win_amd64.pyd,sha256=GD6r61Kv1liA5jjwRqThGpV5y-tuZIsCVy7GcVErY4A,68096
 cns/lbsql.cp36-win_amd64.pyd,sha256=a4BJsW6afDKZpon8EtAyMfSqXZXKpD-lJ6p31tRQ17A,82432
 cns/mailyanzheng.cp36-win_amd64.pyd,sha256=xN0mbUUgqjQTpZbSzxtMoEb86DbvBzWLxCGszZL1PjI,52736
 cns/sql_str.cp36-win_amd64.pyd,sha256=icFmVu1qbAu18pQp5tsh3UnPNZZbGrNyr745WraWUOY,88576
 cns/str2sql.cp36-win_amd64.pyd,sha256=76YB5PQgAMzhg-r_658einLms215CuIlp3NBs4Gi6cA,77312
 cns/test_DataX.py,sha256=98if38kvAdIm314Od1WRdO2VqaXwE5yQEvRRGJdWcVY,2787
 cns/tpass.cp36-win_amd64.pyd,sha256=ZxUB2uszEbd6l-Dc6cfVEqgO2FrIyy9ab7hsET89nKE,81920
 cns/wxlogin.cp36-win_amd64.pyd,sha256=PTfms5LF-AmF_ofWLr_pLZg-yybVJnMzblZ-0kqNb6I,62976
 cns/xdata.cp36-win_amd64.pyd,sha256=2GZLU9ShrOZIcTBQnscVzNNsrIvpXnseGFRFL1iNZK8,148480
-cns-1.0.11.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.11.dist-info/METADATA,sha256=jjPNozul6sFGlBoP80bpM3hjetK7mAeUNsZ7CHi2XEg,2013
-cns-1.0.11.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.11.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.11.dist-info/RECORD,,
+cns-1.0.12.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.12.dist-info/METADATA,sha256=YAYfyI4My53R5MMNinnUisCxpRWzmNv01imMyY0uyEw,1905
+cns-1.0.12.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.12.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.12.dist-info/RECORD,,
```

