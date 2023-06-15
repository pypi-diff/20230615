# Comparing `tmp/nonebot_plugin_game_collection-2.1.9.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.9.tar", last modified: Tue Jun  6 13:30:49 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.0.tar", last modified: Thu Jun 15 17:17:30 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.9.tar` & `nonebot_plugin_game_collection-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.837005 nonebot_plugin_game_collection-2.1.9/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.9/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-06 13:30:49.836505 nonebot_plugin_game_collection-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.770448 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    50156 2023-06-06 13:16:15.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.788963 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16157 2023-06-06 13:24:53.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    30876 2023-06-06 12:22:52.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.795970 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.801474 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.824995 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5357 2023-06-06 13:25:50.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.826996 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.834503 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:30:49.780456 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-06 13:30:49.000000 nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 13:30:49.837505 nonebot_plugin_game_collection-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-06 13:27:00.000000 nonebot_plugin_game_collection-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.515615 nonebot_plugin_game_collection-2.2.0/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-15 17:17:30.515114 nonebot_plugin_game_collection-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.468074 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21085 2023-06-15 17:07:52.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    55947 2023-06-13 16:02:57.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.481586 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13548 2023-06-15 16:58:29.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20126 2023-06-15 15:00:24.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16157 2023-06-06 15:49:58.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    33097 2023-06-15 17:08:45.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.485589 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.491094 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.507108 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5278 2023-06-12 13:50:26.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.510111 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.514114 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7825 2023-06-15 17:13:10.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:17:30.474580 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-15 17:17:30.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-15 17:17:30.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:17:30.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-15 17:17:30.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-15 17:17:30.000000 nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 17:17:30.516116 nonebot_plugin_game_collection-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-15 17:17:25.000000 nonebot_plugin_game_collection-2.2.0/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.9/LICENSE` & `nonebot_plugin_game_collection-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/README.md` & `nonebot_plugin_game_collection-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Account.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     )
 
 import random
 import time
 import datetime
 
 from .utils.utils import line_wrap
-from .utils.chart import bbcode_to_png, bbcode_to_PIL, my_info_head, my_info_statistics, info_Splicing
+from .utils.chart import bbcode_to_png, bbcode_to_PIL, bar_chart,my_info_head, my_info_statistics, info_Splicing
 from .data.data import UserDict, GroupAccount
 from .data.data import props_library, props_index
-from .config import sign_gold, revolt_gold, revolt_cd, revolt_gini, max_bet_gold
-from .Manager import BG_path
-from .Manager import data, company_index
+from .config import bot_name,sign_gold, revolt_gold, revolt_cd, revolt_gini, max_bet_gold
+from .Manager import BG_path, bot_list
+from .Manager import data, company_index, update_company_index
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
 def gold_create(event:MessageEvent,gold:int) -> str:
     """
@@ -100,17 +100,14 @@
         return None
 
     group = group_data[group_id]
 
     if time.time() - group.revolution_time < revolt_cd:
         return f"重置正在冷却中，结束时间：{datetime.datetime.fromtimestamp(group.revolution_time + revolt_cd).strftime('%H:%M:%S')}"
 
-    if time.time() - group.revolution_time < revolt_cd:
-        return f"重置正在冷却中，结束时间：{datetime.datetime.fromtimestamp(group.revolution_time + revolt_cd).strftime('%d日 %H:%M:%S')}"
-
     if (gold := (Manager.group_wealths(group_id) or 0)) < (limit := 15 * max_bet_gold):
         return f"本群金币（{round(gold,2)}）小于{limit}，未满足重置条件。"
 
     if (gini := Manager.Gini(group_id)) < revolt_gini:
         return f"当前基尼系数为{round(gini,3)}，未满足重置条件。"
 
     rank = Manager.group_ranklist(group_id,"资产")
@@ -129,15 +126,16 @@
     j = i**2
     for x in rank[:10]:
         user = user_data[x[0]]
         group_account = user.group_accounts[group_id]
         gold = int(group_account.value*j - group_account.gold*(1-j))
         user.gold += gold
         group_account.gold += gold
-        for company_id in group_account.stocks:
+        company_ids = [company_id for company_id in group_account.stocks]
+        for company_id in company_ids:
             company = group_data[company_id].company
             if user_id in company.exchange:
                 del company.exchange[user_id]
             company.stock += group_account.stocks[company_id]
             del group_account.stocks[company_id]
         i += 0.1
         j = i**2
@@ -308,15 +306,15 @@
         company_name = group_data[stock].company.company_name
         if i := group_account.stocks[stock]:
             msg += f"[size=40][align=left]{company_name}[/align][align=right][color=green]{i}[/color][/align][/size]"
     if msg:
         msg = msg + linestr + "[align=right][size=30][color=gray]股票信息[/color][/size][/align]\n"
         info.append(bbcode_to_PIL(msg))
 
-    return MessageSegment.image(info_Splicing(info,BG_path(event)))
+    return MessageSegment.image(info_Splicing(info,BG_path(event.user_id)))
 
 def my_props(event:MessageEvent) -> Message:
     """
     我的道具
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
@@ -344,14 +342,114 @@
             linestr
             )
     if msg:
         return MessageSegment.image(bbcode_to_png(msg,60))
     else:
         return "您的仓库空空如也。"
 
+async def info_profile(user_id:int) -> list:
+    """
+    总览资料卡
+    """
+    user = user_data[user_id]
+    info = []
+    # 加载全局信息
+    nickname = user.nickname
+    info.append(await my_info_head(user,nickname))
+    # 加载资产分析
+    dist = []
+    for x in user.group_accounts:
+        account = user.group_accounts[x]
+        if not (group_name := group_data[x].company.company_name):
+            group_name = f"（{str(x)[-4:]}）"
+        dist.append([account.gold + account.value, group_name])
+    dist = [x for x in dist if x[0] > 0]
+    if dist:
+        info.append(my_info_statistics(dist))
+    return info
+
+def format_ranktitle(title:str = "金币"):
+    """
+    根据排行榜将数据格式化
+    """
+    if title == "金币":
+        func = lambda x:'{:,}'.format(x)
+    elif title == "资产" or title == "财富":
+        func = lambda x:'{:,}'.format(round(x,2))
+    elif title == "胜率":
+        func = lambda x:f"{round(x*100,2)}%"
+    else:
+        func = lambda x:x
+    return func
+
+async def info_group_rank(group_id:int, title:str = "金币", top:int = 20) -> list:
+    """
+    群内排名信息
+    """
+    if not (ranklist := Manager.group_ranklist(group_id, title)):
+        return None
+    info = []
+    i = 1
+    first = ranklist[0][1]
+    for x in ranklist[:top]:
+        user = user_data[x[0]]
+        user_id = user.user_id
+        group_account = user.group_accounts[group_id]
+        nicname = group_account.nickname
+        info.append(await bar_chart(user_id,f"{i}.{nicname}：{format_ranktitle(title)(x[1])}\n", x[1]/first))
+        i += 1
+    return info
+
+async def group_rank(event:MessageEvent, title:str = "金币") -> str:
+    """
+    生成群内排行榜
+    """
+    user,group_account = Manager.locate_user(event)
+    if not group_account:
+        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+    user_id = user.user_id
+    group_id = group_account.group_id
+    if not (ranklist := Manager.group_ranklist(group_id, title)):
+        return "无数据。"
+    info = await info_group_rank(group_id, title, 20)
+    if info:
+        return MessageSegment.image(info_Splicing(info,BG_path(user_id)))
+    else:
+        return "无数据。"
+
+async def All_rank(event:MessageEvent, title:str = "金币", top:int = 10) -> list:
+    """
+    生成总排行榜
+    """
+    if not (ranklist := Manager.All_ranklist(title)):
+        return None
+    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
+    msg = []
+    i = 1
+    l = len(user_data)
+    for x in ranklist[:top]:
+        user_id = x[0]
+        info = await info_profile(user_id)
+        tmp = (
+            "[align=center]"
+            f"{title}：{format_ranktitle(title)(x[1])}\n"
+            f'[size=300]{i}[/size]\n'
+            "[/align]"
+            + linestr +
+            f"[align=right][size=30][color=gray]{title}总排行 {i}/{l}[/color][/size][/align]\n"
+            )
+        info.append(bbcode_to_PIL(tmp,60))
+        msg.append({"type":"node",
+                    "data":{
+                        "name":f"{bot_name}",
+                        "uin":str(event.self_id),
+                        "content":MessageSegment.image(info_Splicing(info,BG_path(user_id)))}})
+        i += 1
+    return msg
+
 def transfer_fee(amount:int,limit:int) -> int:
     limit = limit if limit > 0 else 0
     if amount <= limit:
         fee = amount * 0.02
     else:
         fee = limit * 0.02 + (amount - limit) * 0.2
     return int(fee)
@@ -419,23 +517,28 @@
     target.props.setdefault("03101",0)
     target.props["03101"] += count
 
     data.save()
 
     return f"【冻结】清算完成，总价值为 {round(x,2)}（金币 {gold} 股票 {round(value,2)}）"
 
-async def delist(bot:Bot):
+async def delist():
         """
         清理无效账户
         """
-        groups = await bot.get_group_list(no_cache = True)
+        mapping = {}
+        for bot in bot_list:
+            group_list = await bot.get_group_list(no_cache = True)
+            for group in group_list:
+                mapping[group["group_id"]] = bot
         if not groups:
             return "群组获取失败"
+
         # 存在的群
-        groups = set(x["group_id"] for x in groups)
+        groups = set(mapping.keys())
         # 注册过的群
         login_groups= set(group_data.keys())
         # 已注册但不存在的群
         delist_group = login_groups - groups
 
         log = ""
         # 处理与不存在的群相关的群账户
@@ -455,24 +558,24 @@
                     group_account.stocks = {stock:count for stock, count in group_account.stocks.items() if stock not in delist_group_accounts}
         # 删除不存在的群
         for group_id in delist_group:
             log += f'删除群：{group_id}\n'
             del group_data[group_id]
 
         # 已注册且存在的群
-        for group_id in list(group_data.keys()):
-            users = await bot.get_group_member_list(group_id = group_id, no_cache = True)
+        for group_id in login_groups:
+            users = await mapping[group_id].get_group_member_list(group_id = group_id, no_cache = True)
             if users:
                 users = set(x["user_id"] for x in users)
             else:
                 continue
             # 删除已注册但不存在的用户
             namelist = group_data[group_id].namelist
             delist_users = namelist - users
             for user_id in delist_users:
                 log += f'删除群账户：{user_id} - {group_id}\n'
                 del user_data[user_id].group_accounts[group_id]
                 namelist.discard(user_id)
-
+        update_company_index()
         # 保存数据
         data.save()
         return log[:-1] if log else "没有要清理的数据！"
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Game.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .utils.chart import text_to_png
 from .data.data import props_library
 from .config import bot_name, security_gold, max_bet_gold, max_player, min_player
 
 from .HorseRace.start import load_dlcs
 from .HorseRace.race_group import race_group
 
-from .Manager import data
+from .Manager import data, try_send_private_msg
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
 
 
@@ -209,15 +209,14 @@
             user = user_data[uid]
             user.gold += session.gold
             user.group_accounts[group_id].gold += session.gold
 
     del current_games[group_id]
     return "赛马场已重置。"
 
-
 """+++++++++++++++++
 ——————————
      其他小游戏
 ——————————
 +++++++++++++++++"""
 
 def slot(event:MessageEvent, gold:int):
@@ -381,25 +380,27 @@
     global current_games
     session = current_games[group_id]
     if msg := session.try_join_game(event):
         return None if msg == " " else msg
     group_account = Manager.locate_user(event)[1]
     if session.info["game"] == "random":
         session.gold = random.randint(0, 0 if(mingold := min(group_account.gold,session.info["gold"])) < 0 else mingold) if session.gold == -1 else session.gold
-        game = random.choice(["russian","dice","poker","lucky_number","cantrell"])
+        game = random.choice(["russian","dice","lucky_number","cantrell", "Blackjack"])
         if game == "russian":
             session.info = russian_info(random.randint(1,6))
         elif game == "dice":
             session.info = dice_info(session.gold)
         elif game == "poker":
             session.info = poker_info()
         elif game == "lucky_number":
             session.info = lucky_number_info(session.gold)
         elif game == "cantrell":
             session.info = cantrell_info(session.gold)
+        elif game == "Blackjack":
+            session.info = Blackjack_info()
     elif group_account.gold <  session.gold:
         del current_games[group_id]
         return Message(MessageSegment.at(event.user_id) + f"你的金币不足以接受这场对决！\n——你还有{group_account.gold}枚金币。")
 
     bet_limit = min(
         user_data[session.player1_id].group_accounts[group_id].gold,
         user_data[session.player2_id].group_accounts[group_id].gold)
@@ -409,57 +410,61 @@
     return acceptmessage(session)
 
 def acceptmessage(session:Session):
     """
     生成接受挑战的提示信息
     """
     game = session.info.get("game")
+    gold = session.gold
     if game == "russian":
-        gold = session.gold
         tip1 = "本场对决为【俄罗斯轮盘】\n"
         tip2 = "开枪！"
     elif game == "dice":
         gold = session.info["max_gold"]
         tip1 = "本场对决为【掷色子】\n"
         tip2 = "开数！"
     elif game == "poker":
-        gold = session.gold
         tip1 = "本场对决为【扑克对战】\n"
         tip2 = "加注！\n"
         tip2 += MessageSegment.image(text_to_png(
             "P1初始状态\n"
             f'HP {session.info["P1"]["HP"]} SP {session.info["P1"]["SP"]} DEF {session.info["P1"]["DEF"]}\n'
             "——————————————\n"
             "P2初始状态\n"
             f'HP {session.info["P2"]["HP"]} SP {session.info["P2"]["SP"]} DEF {session.info["P2"]["DEF"]}\n'
             "——————————————\n"
             "P1初始手牌\n" + 
             "".join([f'【{pokerACT.suit[suit]}{pokerACT.point[point]}】' for suit, point in session.info["P1"]["hand"]])
             ),30)
     elif game == "lucky_number":
-        gold = session.gold
         tip1 = "本场对决为【猜数字】\n"
         tip2 = "发送数字"
     elif game == "cantrell":
-        gold = session.gold
         tip1 = "本场对决为【港式五张】\n"
         tip2 = "开牌！\n"
         tip2 += MessageSegment.image(text_to_png(
                 "P1初始手牌：\n"
                 "|"
                 + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:3]]) +
                 "   |   |"
                 "\n——————————————\n"
                 'P2初始手牌\n'
                 "|"
                 + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"][0:3]]) +
                 "   |   |"
                 ),30)
+    elif game == "Blackjack":
+        hand1 = session.info["hand1"][0]
+        hand2 = session.info["hand2"][0]
+        tip1 = "本场对决为【21点】\n"
+        tip2 = "\n抽牌|停牌|双倍下注\n"
+        tip2 += (
+            f"P1：{Blackjack_suit[hand1[0]]}{Blackjack_point[hand1[1]]}\n"
+            f"P2：{Blackjack_suit[hand2[0]]}{Blackjack_point[hand2[1]]}")
     else:
-        gold = session.gold
         tip1 = ""
         tip2 = ""
     return Message(
         f"{MessageSegment.at(session.player2_id)}接受了对决！\n" +
         tip1 +
         f"赌注为 {gold} 金币\n" +
         f"请{MessageSegment.at(session.player1_id)}{tip2}"
@@ -1129,102 +1134,98 @@
         "round_gold":gold,
         "hand1":deck[0:5],
         "pt1":cantrell_pt(deck[0:5]),
         "hand2":deck[5:10],
         "pt2":cantrell_pt(deck[5:10])
         }
 
-def happy_cantrell_info(gold, times = 2):
+def happy_cantrell_info(gold, level = 2):
     """
     生成快乐港式五张游戏内容
-        times:抽牌次数，1次到5次。
+        level:抽牌次数，1次到5次。
     """
-    times = 1 if times < 1 else times
-    times = 5 if times > 5 else times
-
     deck = random_poker()
     deck = [deck[i:i+5] for i in range(0, 50, 5)]
 
-    hand1,pt1 = max_hand(deck[0:times])
-    hand2,pt2 = max_hand(deck[times:2*times])
+    hand1,pt1 = max_hand(deck[0:level])
+    hand2,pt2 = max_hand(deck[level:2*level])
 
     return {
         "game":"cantrell",
         "round_gold":gold,
         "hand1":hand1,
         "pt1":pt1,
         "hand2":hand2,
         "pt2":pt2
         }
 
-def cantrell(event:GroupMessageEvent, gold:int ,times:int = 1):
+def cantrell(event:GroupMessageEvent, gold:int ,level:int = 1):
     """
     发起游戏：港式五张
     """
     flag, msg = start(event, gold, max_bet_gold * 10)
     if flag == False:
         return msg
     group_id = event.group_id
     session = current_games[group_id]
     session.gold = gold
-    if times == 1:
+    if level == 1:
         session.info = cantrell_info(gold)
     else:
-        session.info = happy_cantrell_info(gold,times)
+        level = 1 if level < 1 else level
+        level = 5 if level > 5 else level
+        session.info = happy_cantrell_info(gold,level)
     return (f"随机牌堆已生成\n"
             f"开局金额：{gold}\n"
-            + (f"等级：Lv.{times}\n" if times > 1 else "") +
+            + (f"等级：Lv.{level}\n" if level > 1 else "") +
             f"{msg}")
 
 async def cantrell_check(bot:Bot, event:GroupMessageEvent):
     """
     看牌
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
         return None if msg == " " else msg
     session.time = time.time() + 120
     expose = int(round((session.round  + 0.5)/ 2)) + 3
-    expose = expose if expose < 5 else 5
+    expose = min(expose,5)
     if event.user_id == session.player1_id:
         hand = "hand1"
     else:
         hand = "hand2"
     msg = (
         "你的手牌：\n"
         + ("|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info[hand][0:expose]]) + (5 - expose)*"   |")
         )
-    await bot.send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30)))
-    return
+    if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
+        await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
 
 async def cantrell_play(bot:Bot, event:GroupMessageEvent, gold:int, max_bet_gold:int = max_bet_gold * 10):
     """
     加注
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
         return None if msg == " " else msg
     if gold > max_bet_gold:
         return MessageSegment.at(event.user_id) + f"加注金额不能超过{max_bet_gold}"
-    if gold > session.info["bet_limit"]:
-        gold = session.info["bet_limit"]
+    if session.gold + gold > session.info["bet_limit"]:
+        gold = session.info["bet_limit"] - session.gold
     expose = session.round / 2
     if expose == int(expose):
         session.nextround()
         session.time += 120
         expose = int(expose) + 3
-        if gold > session.info["round_gold"]:
-            session.gold += gold
-        else:
-            session.gold += session.info["round_gold"]
-        session.info["bet_limit"] -= gold
+        gold = max(gold,session.info["round_gold"])
+        session.gold += gold
         msg = (
             f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
             "手牌：\n"
             "|"
             + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:expose]]) + (5 - expose)*"   |"
             "\n——————————————\n"
             f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
@@ -1237,22 +1238,172 @@
                 session.win = session.player1_id
             else:
                 session.win = session.player2_id
             await end(bot, event)
         else:
             return MessageSegment.image(text_to_png(f"您已跟注{gold}金币\n" + msg,30))
     else:
-        session.info["bet_limit"] -= gold
         session.nextround()
         session.time += 120
         session.info["round_gold"] = gold
         return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
 
 """+++++++++++++++++
 ——————————
+        21点
+——————————
++++++++++++++++++"""
+
+Blackjack_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
+Blackjack_point = {1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"J",12:"Q",13:"K"}
+
+def Blackjack_info():
+    """
+    生成21点游戏内容
+    """
+    deck = random_poker()
+    return {
+        "game":"Blackjack",
+        "deck":deck[2:],
+        "hand1":[deck[0],],
+        "hand2":[deck[1],],
+        }
+
+def Blackjack(event:GroupMessageEvent, gold:int):
+    """
+    发起游戏：21点
+    """
+    flag, msg = start(event, gold, max_bet_gold * 10)
+    if flag == False:
+        return msg
+    group_id = event.group_id
+    session = current_games[group_id]
+    session.gold = gold
+    session.info = Blackjack_info()
+    return ("唰唰~，随机牌库已生成\n"
+            f"挑战金额：{gold}\n"
+            f"{msg}")
+
+def Blackjack_pt(hand:list) -> int:
+    """
+    返回21点牌组点数。
+    """
+    pts = [x[1] if x[1] < 10 else 10 for x in hand]
+    pt = sum(pts)
+    if 1 in pts and pt <= 11:
+        pt += 10
+    return pt
+
+async def Blackjack_Hit(bot:Bot, event:GroupMessageEvent):
+    """
+    抽牌
+    """
+    group_id = event.group_id
+    global current_games
+    session = current_games[group_id]
+    if msg := session.shot_check(event):
+        return None if msg == " " else msg
+    session.time = time.time()
+
+    if event.user_id == session.player1_id:
+        hand = "hand1"
+        session.win = session.player2_id
+    else:
+        hand = "hand2"
+        session.win = session.player1_id
+    deck = session.info["deck"]
+    card = deck[0]
+    del deck[0]
+    hand = session.info[hand]
+    hand.append(card)
+    pt = Blackjack_pt(hand)
+    if pt > 21:
+        await end(bot, event)
+    else:
+        msg = (
+            "你的手牌：\n"
+            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand]))
+            + f'\n合计:{pt}点'
+            )
+        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
+            await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
+
+async def Blackjack_stand(bot:Bot, event:GroupMessageEvent):
+    """
+    停牌
+    """
+    group_id = event.group_id
+    global current_games
+    session = current_games[group_id]
+    if msg := session.shot_check(event):
+        return None if msg == " " else msg
+    session.time = time.time()
+    session.nextround()
+    if session.round == 2:
+        return Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注")
+    else:
+        hand1 = session.info["hand1"]
+        hand2 = session.info["hand2"]
+        if Blackjack_pt(hand1) > Blackjack_pt(hand2):
+            session.win = session.player1_id
+        else:
+            session.win = session.player2_id
+        await end(bot, event)
+
+async def Blackjack_DoubleDown(bot:Bot, event:GroupMessageEvent):
+    """
+    双倍下注
+    """
+    group_id = event.group_id
+    global current_games
+    session = current_games[group_id]
+    if msg := session.shot_check(event):
+        return None if msg == " " else msg
+    session.time = time.time()
+    gold = session.gold
+    bet_limit = session.info["bet_limit"]
+    gold = gold*2
+    gold = min(bet_limit, gold)
+    session.gold = gold
+    if event.user_id == session.player1_id:
+        hand = "hand1"
+        session.win = session.player2_id
+    else:
+        hand = "hand2"
+        session.win = session.player1_id
+    deck = session.info["deck"]
+    card = deck[0]
+    del deck[0]
+    hand = session.info[hand]
+    hand.append(card)
+    pt = Blackjack_pt(hand)
+    if pt > 21:
+        await end(bot, event)
+    else:
+        msg = (
+            "你的手牌：\n"
+            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand]))
+            + f'\n合计:{pt}点'
+            )
+        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
+            await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
+        session.nextround()
+        if session.round == 2:
+            return Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注")
+        else:
+            hand1 = session.info["hand1"]
+            hand2 = session.info["hand2"]
+            if Blackjack_pt(hand1) > Blackjack_pt(hand2):
+                session.win = session.player1_id
+            else:
+                session.win = session.player2_id
+            await end(bot, event)
+
+"""+++++++++++++++++
+——————————
       随机对战
 ——————————
 +++++++++++++++++"""
 
 def random_game(event:GroupMessageEvent, gold:int):
     """
     发起游戏：随机对战
@@ -1378,28 +1529,39 @@
     """
     结束附件
     """
     game = session.info["game"]
     if game == "russian":
         return " ".join(("—" if x == 0 else "|") for x in session.info["bullet"])
     if game == "dice":
-        return (f'玩家 1\n'
-                f'组合：{" ".join(str(x) for x in session.info["dice_array1"])}\n'
-                f'玩家 2\n'
-                f'组合：{" ".join(str(x) for x in session.info["dice_array2"])}')
+        return (
+            f'玩家 1\n'
+            f'组合：{" ".join(str(x) for x in session.info["dice_array1"])}\n'
+            f'玩家 2\n'
+            f'组合：{" ".join(str(x) for x in session.info["dice_array2"])}')
     if game == "cantrell":
-        return MessageSegment.image(text_to_png(("P1手牌：\n"
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"]]) +
-                f"\n牌型：\n{session.info['pt1'][1]}"
-                "\n——————————————\n"
-                "P2手牌：\n"
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"]]) +
-                f"\n牌型：\n{session.info['pt2'][1]}"),30))
+        return MessageSegment.image(text_to_png((
+            "P1手牌：\n"
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"]]) +
+            f"\n牌型：\n{session.info['pt1'][1]}"
+            "\n——————————————\n"
+            "P2手牌：\n"
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"]]) +
+            f"\n牌型：\n{session.info['pt2'][1]}"),30))
+    if game == "Blackjack":
+        hand1 = session.info["hand1"]
+        hand2 = session.info["hand2"]
+        return MessageSegment.image(text_to_png((
+            "P1手牌：\n"
+            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand1]))
+            + f'\n合计:{Blackjack_pt(hand1)}点'
+            "\n——————————————\n"
+            "P2手牌：\n"
+            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand2]))
+            + f'\n合计:{Blackjack_pt(hand2)}点'),30))
     else:
         return ""
 
 async def end(bot:Bot, event:GroupMessageEvent):
     """
     输出结算界面
     """
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Tuple,Dict
 from pathlib import Path
 from nonebot.adapters.onebot.v11 import (
     Bot,
+    Message,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment,
     )
+from collections import Counter
 
 from .utils.utils import image_url
 from .utils.chart import text_to_png, gini_coef, default_BG
 from .utils.avatar import download_url
 from .data.data import DataBase, UserDict, GroupAccount, GroupDict
 from .data.data import props_library
 from .config import revolt_gold, max_bet_gold, lucky_clover, path, BG_image
@@ -83,30 +85,29 @@
         user.group_accounts[group_id] = GroupAccount(group_id = group_id, nickname = user.nickname)
         data.save()
 
     group_account = user.group_accounts[group_id]
 
     return user,group_account
 
+company_index:Dict[str,int] = {}
+
 def update_company_index():
     """
     从群数据生成公司名查找群号的字典
     """
-    company_index = {}
     for group_id in group_data:
         if company_name := group_data[group_id].company.company_name:
             company_index[company_name] = group_id
             company_index[str(group_id)] = group_id
-    return company_index
 
-company_index:Dict[str,int] = {}
-company_index = update_company_index()
+update_company_index()
 
-def BG_path(event:MessageEvent):
-    my_BG = BG_image / f"{str(event.user_id)}.png"
+def BG_path(user_id:int) -> Path:
+    my_BG = BG_image / f"{str(user_id)}.png"
     if my_BG.exists():
         return my_BG
     else:
         return default_BG
 
 async def add_BG_image(event:MessageEvent):
     user = locate_user(event)[0]
@@ -220,34 +221,80 @@
         for user_id in namelist:
             user = user_data[user_id]
             rank.append([user_id, user.win])
     elif title == "败场":
         for user_id in namelist:
             user = user_data[user_id]
             rank.append([user_id, user.lose])
-    elif title == "路灯":
+    elif title == "路灯挂件":
         rank = group_data[group_id].Achieve_revolution.items()
     else:
         return None
     rank = [x for x in rank if x[1]]
     rank.sort(key=lambda x:x[1],reverse=True)
     return rank
 
-def group_rank(group_id:int, title:str = "金币", top:int = 20) -> str:
-    if not (ranklist := group_ranklist(group_id, title)):
-        return "无数据。"
-    rank = ""
-    i = 1
-    for x in ranklist[:top]:
-        user = user_data[x[0]]
-        group_account = user.group_accounts[group_id]
-        nicname = group_account.nickname
-        rank += f"{i}.{nicname}：{x[1]}\n"
-        i += 1
-    return MessageSegment.image(text_to_png(rank[:-1]))
+#def group_rank(group_id:int, title:str = "金币", top:int = 20) -> str:
+#    if not (ranklist := group_ranklist(group_id, title)):
+#        return "无数据。"
+#    rank = ""
+#    i = 1
+#    for x in ranklist[:top]:
+#        user = user_data[x[0]]
+#        group_account = user.group_accounts[group_id]
+#        nicname = group_account.nickname
+#        rank += f"{i}.{nicname}：{x[1]}\n"
+#        i += 1
+#    return MessageSegment.image(text_to_png(rank[:-1]))
+
+def All_ranklist(title:str) -> list:
+    """
+    总排行榜
+        param:
+        title:排名内容
+        return:List[data]
+        data[0]:QQ号
+        data[1]:title
+    """
+    namelist = user_data.keys()
+    rank = []
+    if title == "金币":
+        for user_id in namelist:
+            gold = user_data[user_id].gold
+            rank.append([user_id,gold])
+    elif title == "资产" or title == "财富":
+        for user_id in namelist:
+            user = user_data[user_id]
+            gold = user.gold
+            value = sum([group.value for group in user.group_accounts.values()])
+            rank.append([user_id, gold + value])
+    elif title == "胜率":
+        for user_id in namelist:
+            user = user_data[user_id]
+            if (count := user.win + user.lose) > 2:
+                rank.append([user_id, user.win / count])
+    elif title == "胜场":
+        for user_id in namelist:
+            user = user_data[user_id]
+            rank.append([user_id, user.win])
+    elif title == "败场":
+        for user_id in namelist:
+            user = user_data[user_id]
+            rank.append([user_id, user.lose])
+    elif title == "路灯挂件":
+        result = Counter()
+        for group in group_data.values():
+            result += Counter(group.Achieve_revolution)
+        rank = result.items()
+    else:
+        return None
+
+    rank = [x for x in rank if x[1]]
+    rank.sort(key=lambda x:x[1],reverse=True)
+    return rank
 
 def Gini(group_id:int, limit:int = revolt_gold[0]) -> float:
     """
     本群基尼系数
     """
     if group_id in group_data:
         namelist = group_data[group_id].namelist
@@ -264,16 +311,15 @@
 
 def Newday():
     """
     刷新每日
     """
     log = ""
     group_check = {k:set() for k in group_data}
-    global company_index
-    company_index = update_company_index()
+    update_company_index()
     company_ids = company_index.values()
     stock_check = {k:0 for k in company_ids}
     # 检查user_data
     for user_id in user_data:
         user = user_data[user_id]
         user.transfer_limit = 0
         props = user.props
@@ -285,14 +331,15 @@
             if group_id not in group_check:
                 log += f"{user.nickname} 群账户{group_id}无效，已删除。\n"
                 del group_accounts[group_id]
             else:
                 group_check[group_id].add(user_id)
                 group_account = group_accounts[group_id]
                 group_account.is_sign = False
+                group_account.security = 0
                 gold += group_account.gold
                 props = group_account.props
                 props = {k:v-1 if k[2] == '0' else v for k, v in props.items()}
                 group_account.props = {k:v for k, v in props.items() if v > 0}
                 stocks = group_account.stocks
                 for company_id in list(stocks.keys()):
                     if company_id in stock_check:
@@ -323,8 +370,27 @@
                     f"{company.company_name} 股票数量异常。\n"
                     f"记录值：{company.stock}\n"
                     f"实测值：{company.issuance - stock_check[group_id]}\n"
                     "数据已修正。\n"
                     )
                 company.stock = company.issuance - stock_check[group_id]
     data.save()
-    return log[:-1] if log else "数据一切正常！"
+    return log[:-1] if log else "数据一切正常！"
+
+from nonebot import get_driver
+driver = get_driver()
+bot_list = set()
+driver.on_bot_connect(lambda bot:bot_list.add(bot))
+driver.on_bot_disconnect(lambda bot:bot_list.discard(bot))
+
+async def try_send_private_msg(user_id:int, message: Message) -> bool:
+    """
+    发送私聊消息
+    """
+    global bot_list
+    for bot in bot_list:
+        friend_list = await bot.get_friend_list()
+        friend_list = [friend["user_id"] for friend in friend_list]
+        if user_id in friend_list:
+            await bot.send_private_msg(user_id = user_id, message = message)
+            return True
+    return False
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Market.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
 def check_company_name(company_name:str):
     """
     检查公司名是否合法
     """
     if not company_name:
         return f"公司名称不能为空"
-    global company_index
-    company_index = update_company_index()
+    update_company_index()
     if company_name in company_index:
         return f"{company_name} 已被注册"
     if " " in company_name or "\n" in company_name:
         return "公司名称不能含有空格或回车"
     count = 0
     for x in company_name:
         if ord(x) < 0x200:
@@ -79,16 +78,15 @@
     company.time = time.time()
     company.stock = 20000
     company.issuance = 20000
     company.gold = gold * 0.8
     company.float_gold = company.gold
     company.group_gold = gold
     company.intro = f"发行初始信息\n金币 {round(gold,2)}\n基尼系数{round(gini,3)}\n{company_name} 名称检查通过\n发行成功！"
-    company_index[company_name] = group_id
-    company_index[str(group_id)] = group_id
+    update_company_index()
     data.save()
     return f'{company_name}发行成功，发行价格为每股{round((gold/ 20000),2)}金币'
 
 def rename(event:GroupMessageEvent,company_name:str):
     """
     公司重命名
         company_name:公司名
@@ -100,16 +98,16 @@
     user = Manager.locate_user(event)[0]
     if user.props.get("33001",0) < 1:
         return f"你的【{props_library['33001']['name']}】已失效"
     if check := check_company_name(company_name):
         return check
     old_company_name = company.company_name
     company.company_name = company_name
-    global company_index
-    company_index = update_company_index()
+    del company_index[old_company_name]
+    update_company_index()
     return f'【{old_company_name}】已重命名为【{company_name}】'
 
 def value_update(group_account:GroupAccount):
     """
     刷新持股价值
     group_account:用户群账户
     """
@@ -147,15 +145,15 @@
         return "已售空，请等待结算或在交易市场购买。"
 
     group_gold = Manager.group_wealths(company_id) or 0
     company.group_gold = group_gold
     if group_gold < 10 * max_bet_gold:
         return f"【{company_name}】金币过少({group_gold})，无法交易。"
 
-    gold = group_gold if group_gold > company.float_gold else company.float_gold
+    gold = max(group_gold, company.float_gold)
     SI = company.issuance
     gini = Manager.Gini(company_id)
     value = 0.0
     for _ in range(buy):
         unit = gold/SI
         gold += unit * gini
         value += unit
@@ -412,15 +410,19 @@
         return f"没有 {group_id} 的注册信息"
 
     info = []
     # 加载群信息
     company_name = company.company_name
     group_info = await bot.get_group_info(group_id = group_id)
     group_name = group_info["group_name"]
-    member_count = group_info["member_count"] - 1
+    member_count = group_info["member_count"]
+    if member_count == 0:
+        member_count = 3000
+    else:
+        member_count = member_count - 1
 
     info.append(await group_info_head(group_name, company_name, group_id, (len(group.namelist),member_count)))
 
     linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
 
     msg = ""
     ranklist = list(group.Achieve_revolution.items())
@@ -461,37 +463,38 @@
         if msg:
             info.append(bbcode_to_PIL(msg + linestr + "[align=right][size=30][color=gray]市场详情[/color][/size][/align]", 40))
 
         msg = company.intro
         if msg:
             info.append(bbcode_to_PIL(msg + "\n" +linestr + "[align=right][size=30][color=gray]公司介绍[/color][/size][/align]", 40))
 
-    return MessageSegment.image(info_Splicing(info, BG_path(event)))
+    return MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))
 
 def stock_profile(company:Company) -> str:
     """
     产业信息
     """
     group_gold = company.group_gold
     float_gold = company.float_gold
     issuance = company.issuance
     msg = (
         f"固定资产 {'{:,}'.format(round(company.gold,2))}\n"
         f"市场流动 {'{:,}'.format(round(company.group_gold))}\n"
-        f"发行价格 {'{:,}'.format(round((group_gold if group_gold > float_gold else float_gold)/issuance,2))}\n"
-        f"结算价格 {'{:,}'.format(round((group_gold if group_gold < float_gold else float_gold)/issuance,2))}\n"
+        f"发行价格 {'{:,}'.format(round(max(group_gold,float_gold)/issuance,2))}\n"
+        f"结算价格 {'{:,}'.format(round(float_gold/issuance,2))}\n"
         f"剩余数量 {company.stock}\n"
         )
     return msg
 
 def Market_info_All(event:MessageEvent, ohlc:bool = False):
     """
     市场信息总览
     """
-    company_ids = list(set([company_index[x] for x in company_index]))
+    global company_index
+    company_ids = set([company_index[company_id] for company_id in company_index])
     companys = []
     for company_id in company_ids:
         company = group_data[company_id].company
         companys.append(company)
     companys.sort(key = lambda x:x.group_gold, reverse = True)
 
     lst = [companys[i:i+5] for i in range(0, len(companys), 5)]
@@ -501,15 +504,15 @@
         info = []
         for company in seg:
             info.append(bbcode_to_PIL(company.company_name +"\n" + linestr + stock_profile(company), 60))
         msg.append({"type":"node",
                     "data":{
                         "name":f"{bot_name}",
                         "uin":str(event.self_id),
-                        "content":MessageSegment.image(info_Splicing(info, BG_path(event)))}})
+                        "content":MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))}})
     return msg
 
 def update_intro(company_name:str, intro:str):
     if company_name in company_index:
         company_id = company_index[company_name]
     else:
         return f"没有 {company_name} 的注册信息"
@@ -546,24 +549,22 @@
     deviation = gold - float_gold
     float_gold += deviation * 0.1 * abs(deviation)/gold
     # 更新浮动价格
     company.float_gold = float_gold
     # 记录价格历史
     global market_history
     market_history.setdefault(company_id,[]).append((time.time(), group_gold / company.issuance, float_gold / company.issuance))
-    while len(market_history[company_id]) > 720:
-        del market_history[company_id][0]
+    market_history[company_id] = market_history[company_id][-720:]
 
 def update():
     """
     刷新市场
     """
     log = ""
-
-    company_ids = set(company_index.values())
+    company_ids = set([company_index[company_id] for company_id in company_index])
     for company_id in company_ids:
         company = group_data[company_id].company
         company_update(company)
         log += f"{company.company_name} 更新成功！\n"
 
     for user_id in user_data:
         group_accounts = user_data[user_id].group_accounts
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/Prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
         props["63101"] -= 1
         if props["63101"] < 1:
             del props["63101"]
 
         gold = group_account.gold
 
-        if random.randint(0,2) == 0:
+        if random.randint(0,1) == 0:
             user.gold += gold
             group_account.gold += gold
             return f"你获得了{gold}金币"
         else:
             user.gold -= gold
             group_account.gold -= gold
             user.props.setdefault("53101",0)
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
     GROUP_OWNER,
     Bot,
     MessageEvent,
     GroupMessageEvent,
     Message,
 )
 from nonebot.permission import SUPERUSER
-from nonebot import on_command, on_regex, on_fullmatch
+from nonebot import on_message, on_command, on_regex, on_fullmatch
 from nonebot.params import CommandArg, Arg
+from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me
 from nonebot import require
 from nonebot.log import logger
 
 try:
     import ujson as json
@@ -244,35 +245,36 @@
 russian = on_command("俄罗斯轮盘", aliases={"装弹", "俄罗斯转盘"}, permission = GROUP, priority = 20, block = True)
 
 @russian.handle()
 async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
     if not (msg := arg.extract_plain_text().strip().split()):
         bullet_num = 1
         gold = bet_gold
-    if len(msg) == 1:
-        msg = msg[0]
-        if not msg.isdigit():
-            return
-        if 0 < (msg := int(msg)) < 7:
-            bullet_num = msg
-            gold = bet_gold
-        else:
-            bullet_num = 1
-            gold = int(msg)
     else:
-        if not (msg[0].isdigit() and msg[1].isdigit()):
-            return
-        bullet_num = int(msg[0])
-        gold = int(msg[1])
-        if 0 < bullet_num < 7:
-            pass
-        elif 0 < gold < 7:
-            bullet_num ,gold = gold, bullet_num
+        if len(msg) == 1:
+            msg = msg[0]
+            if not msg.isdigit():
+                return
+            if 0 < (msg := int(msg)) < 7:
+                bullet_num = msg
+                gold = bet_gold
+            else:
+                bullet_num = 1
+                gold = int(msg)
         else:
-            return
+            if not (msg[0].isdigit() and msg[1].isdigit()):
+                return
+            bullet_num = int(msg[0])
+            gold = int(msg[1])
+            if 0 < bullet_num < 7:
+                pass
+            elif 0 < gold < 7:
+                bullet_num ,gold = gold, bullet_num
+            else:
+                return
     msg = Game.russian(event,bullet_num,gold)
     await russian.finish(msg)
 
 # 开枪
 russian_shot = on_command(
     "开枪",
     aliases = {"咔", "嘭", "嘣"},
@@ -377,37 +379,37 @@
 cantrell = on_command("同花顺", aliases = {"五张牌","港式五张","梭哈"}, permission = GROUP, priority = 20, block = True)
 
 @cantrell.handle()
 async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
     arg = arg.extract_plain_text().strip().split()
     if not arg:
         gold = bet_gold
-        times = 1
+        level = 1
     else:
         test = len(arg)
         if test == 1:
             gold = arg[0]
             if gold.isdigit():
                 gold = int(gold)
             else:
                 gold = bet_gold
-            times = 1
+            level = 1
         else:
             gold = arg[0]
             if gold.isdigit():
                 gold = int(gold)
             else:
                 gold = bet_gold
-            times = arg[1]
-            if times.isdigit():
-                times = int(times)
+            level = arg[1]
+            if level.isdigit():
+                level = int(level)
             else:
-                times = 1
+                level = 1
 
-    msg = Game.cantrell(event, gold, times)
+    msg = Game.cantrell(event, gold, level)
     await cantrell.finish(msg)
 
 # 看牌
 cantrell_check = on_command(
     "看牌",
     rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "cantrell",
     permission = GROUP,
@@ -436,14 +438,57 @@
     if gold.isdigit():
         gold = int(gold)
     else:
         gold =  current_games[event.group_id].info["round_gold"]
     msg = await Game.cantrell_play(bot, event, gold)
     await cantrell_play.finish(msg)
 
+# 21点
+Blackjack = on_command("21点", permission = GROUP, priority = 20, block = True)
+
+@Blackjack.handle()
+async def _(event:MessageEvent, arg:Message = CommandArg()):
+    gold = arg.extract_plain_text().strip()
+    if gold.isdigit():
+        gold = int(gold)
+    else:
+        gold = bet_gold
+    msg = Game.Blackjack(event, gold)
+    await Blackjack.finish(msg)
+
+# 抽牌
+
+def is_Blackjack(event:GroupMessageEvent,state:T_State) -> bool:
+    if event.group_id in current_games and current_games[event.group_id].info.get("game") == "Blackjack":
+        command = str(event.message)
+        if command == "抽牌":
+            state["Blackjack_play"] = Game.Blackjack_Hit
+        elif command == "停牌":
+            state["Blackjack_play"] = Game.Blackjack_stand
+        elif command == "双倍下注":
+            state["Blackjack_play"] = Game.Blackjack_DoubleDown
+        else:
+            return False
+        return True
+    else:
+        return False
+
+Blackjack_play = on_message(
+    rule = is_Blackjack,
+    permission = GROUP,
+    priority = 20,
+    block = True
+    )
+
+@Blackjack_play.handle()
+async def _(bot:Bot, event:GroupMessageEvent,state:T_State):
+    Blackjack_play = state["Blackjack_play"]
+    msg = await Blackjack_play(bot, event)
+    await cantrell_play.finish(msg)
+
 # 随机对战
 random_game = on_command("随机对战", permission = GROUP, priority = 5, block = True)
 
 @random_game.handle()
 async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
     if gold.isdigit():
@@ -476,15 +521,15 @@
     await refuse.finish(msg)
 
 # 超时结算
 overtime = on_command("超时结算", rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @overtime.handle()
 async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.overtime(event)
+    msg = await Game.overtime(bot, event)
     await overtime.finish(msg)
 
 # 认输结算
 fold = on_fullmatch(("认输", "投降", "结束"), rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @fold.handle()
 async def _(bot:Bot, event:GroupMessageEvent):
@@ -596,27 +641,46 @@
 @del_BG_image.handle()
 async def _(event:MessageEvent):
     msg = await Manager.del_BG_image(event)
     await del_BG_image.finish(msg, at_sender = True)
 
 # 查看排行榜
 russian_rank = on_regex(
-    r"^(总金币|总资产|金币|资产|财富|胜率|胜场|败场|路灯)(排行|榜)",
-    permission = GROUP,
+    r"^(总金币|总资产|金币|资产|财富|胜率|胜场|败场|路灯挂件)(排行|榜)",
     priority = 20,
     block = True
     )
 
 @russian_rank.handle()
-async def _(event:GroupMessageEvent):
+async def _(event:MessageEvent):
     cmd = event.get_plaintext().strip().split()
-    title = re.search(r"^(总金币|总资产|金币|资产|财富|胜率|胜场|败场|路灯)(排行|榜)",cmd[0]).group(1)
-    msg = Manager.group_rank(event.group_id, title)
+    title = re.search(r"^(总金币|总资产|金币|资产|财富|胜率|胜场|败场|路灯挂件)(排行|榜)",cmd[0]).group(1)
+    msg = await Account.group_rank(event, title)
     await russian_rank.finish(msg)
 
+# 查看总排行
+russian_All_rank = on_regex(
+    r"^(金币|资产|财富|胜率|胜场|败场|路灯挂件)(总排行|总榜)",
+    priority = 20,
+    block = True
+    )
+
+@russian_All_rank.handle()
+async def _(bot:Bot, event:MessageEvent):
+    cmd = event.get_plaintext().strip().split()
+    title = re.search(r"^(金币|资产|财富|胜率|胜场|败场|路灯挂件)(总排行|总榜)",cmd[0]).group(1)
+    msg = await Account.All_rank(event, title)
+    if msg:
+        if isinstance(event, GroupMessageEvent):
+            await bot.send_group_forward_msg(group_id = event.group_id, messages = msg)
+        else:
+            await bot.send_private_forward_msg(user_id = event.user_id, messages = msg)
+    else:
+        await russian_All_rank.finish("无数据。")
+
 # 公司上市
 Market_public = on_command(
     "市场注册",
     aliases = {"公司注册","注册公司"},
     rule = to_me(),
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
@@ -865,17 +929,17 @@
     else:
         await freeze.finish("【冻结】已取消。")
 
 # 清理无效账户
 delist = on_command("清理无效账户", rule = to_me(), permission = SUPERUSER, priority = 20, block = True)
 
 @delist.handle()
-async def _(bot:Bot):
+async def _():
     await delist.send("正在启动清理程序。")
-    log = await Account.delist(bot)
+    log = await Account.delist()
     logger.info("\n" + log)
     with open(path / "delist.log","a",encoding = "utf8") as f:
         f.write(
             f"\n{datetime.datetime.fromtimestamp(time.time()).strftime('%Y 年 %m 月 %d 日 %H:%M:%S')}\n"
             "——————————————\n"
             + log + "\n"
             "——————————————\n"
@@ -885,15 +949,15 @@
 # 股市更新
 @scheduler.scheduled_job("cron", minute = "0,*/5")
 async def _():
     log = Market.update()
     if log:
         logger.info("\n" + log)
 
-# 市场指数更新和数据备份
+# 数据备份
 Backup = on_command("Backup", aliases = {"数据备份", "游戏备份"}, permission = SUPERUSER, priority = 20, block = True)
 
 @Backup.handle()
 @scheduler.scheduled_job("cron", hour = "0,*/4")
 async def _():
     now = time.strftime('%Y-%m-%d %H-%M-%S', time.localtime(time.time()))
     now = now.split()
@@ -919,15 +983,15 @@
             + log + "\n"
             "——————————————\n"
             )
 
     folders = [f for f in backup.iterdir() if f.is_dir()]
     for folder in folders:
         if time.time() - folder.stat().st_ctime > 604800:
-            folder.unlink(True)
+            folder.rmdir()
             logger.info(f'备份 {folder} 已删除！')
 
 # 保存数据
 DataSave = on_command("DataSave", aliases = {"保存数据", "保存游戏"},permission = SUPERUSER, priority = 20, block = True)
 
 @DataSave.handle()
 @scheduler.scheduled_job("cron", minute = "0,*/10")
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937499999999999%*

 * *Differences: {"'02101'": "{'intro': '每个人随时都可以发起重置来打破现状。'}",*

 * * "'63101'": "{'intro': '有50%的概率金币翻倍，50%的概率金币清零。没有上限', 'des': '你可以一直相信自己的运气。'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "02101": {
         "color": "#696969",
         "des": "\u6bcf\u6b21\u91cd\u7f6e\u90fd\u4f1a\u7559\u4e0b\u8fd9\u6837\u4e00\u4e2a\u6807\u8bb0\u3002",
-        "intro": "\u5f53\u4e00\u4e2a\u4eba\u7684\u91d1\u5e01\u6570\u91cf\u8d85\u8fc7\u5176\u4ed6\u4eba\u7684\u603b\u548c\uff0c\u90a3\u4e48\u8fd9\u91cc\u5c31\u4e0d\u7a33\u5b9a\u4e86\u3002\u6bcf\u4e2a\u4eba\u968f\u65f6\u90fd\u53ef\u4ee5\u53d1\u8d77\u91cd\u7f6e\u6765\u6253\u7834\u73b0\u72b6\u3002",
+        "intro": "\u6bcf\u4e2a\u4eba\u968f\u65f6\u90fd\u53ef\u4ee5\u53d1\u8d77\u91cd\u7f6e\u6765\u6253\u7834\u73b0\u72b6\u3002",
         "name": "\u8def\u706f\u6302\u4ef6\u6807\u8bb0",
         "rare": 0
     },
     "03100": {
         "color": "#CC0000",
         "des": "\u68a6\u91cc\u4ec0\u4e48\u90fd\u6709\u3002",
         "intro": "\u5185\u542b10\u4ebf\u91d1\u5e01\uff0c100\u4e07\u94bb\u77f3",
@@ -151,16 +151,16 @@
         "des": "\u201c\u94bb\u77f3\u6709\u4ec0\u4e48\u7528\uff1f\u201d\n\u201c\u6ca1\u7528\u3002\u201d",
         "intro": "\u65e0\u6bd4\u73cd\u8d35\u7684\u94bb\u77f3\uff0c\u53ea\u6709\u5343\u5206\u4e4b\u4e94\u7684\u6982\u7387\u83b7\u5f97\uff0c\u4ee5\u540e\u53ef\u80fd\u6709\u7528\u3002",
         "name": "\u94bb\u77f3",
         "rare": 6
     },
     "63101": {
         "color": "#FF3300",
-        "des": "\u5956\u52b1\u7ffb\u500d\uff0c\u60e9\u7f5a\u7ffb\u500d\u3002",
-        "intro": "\u670933.3%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c66.6%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\u6ca1\u6709\u4e0a\u9650",
+        "des": "\u4f60\u53ef\u4ee5\u4e00\u76f4\u76f8\u4fe1\u81ea\u5df1\u7684\u8fd0\u6c14\u3002",
+        "intro": "\u670950%\u7684\u6982\u7387\u91d1\u5e01\u7ffb\u500d\uff0c50%\u7684\u6982\u7387\u91d1\u5e01\u6e05\u96f6\u3002\u6ca1\u6709\u4e0a\u9650",
         "name": "\u8d85\u7ea7\u5e78\u8fd0\u786c\u5e01",
         "rare": 6
     },
     "63102": {
         "color": "#006633",
         "des": "\u4e8b\u4e86\u62c2\u8863\u53bb\uff0c\u6df1\u85cf\u8eab\u4e0e\u540d\u3002",
         "intro": "\u6e05\u7a7a\u81ea\u5df1\u7684\u91d1\u5e01\uff0c\u80a1\u7968",
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,30 @@
     '''
     bbcode文字转png
     '''
     output = BytesIO()
     bbcode_to_PIL(msg = msg ,fontsize = fontsize, spacing = spacing, bg_colour = "white").save(output, format="png")
     return output
 
+async def bar_chart(user_id:int, info:str, lenth:float):
+    """
+    带头像的条形图
+    """
+    canvas = Image.new("RGBA", (880, 60))
+    avatar = Image.open(await download_avatar(user_id))
+    avatar = avatar.resize((60,60))
+    circle_mask = Image.new("RGBA", avatar.size, (255, 255, 255, 0))
+    ImageDraw.Draw(circle_mask).ellipse(((0,0),avatar.size), fill="black")
+    canvas.paste(avatar, (5, 0), circle_mask)
+    draw = ImageDraw.Draw(canvas)
+    draw.rectangle(((70,10), (860, 50)), fill = "#00000033")
+    draw.rectangle(((70,10), (80 + int(lenth*780), 50)), fill = "#99CCFF")
+    draw.text((80,10), info, fill = (0,0,0), font = font_small)
+    return canvas
+
 async def my_info_head(user:UserDict, nickname:str):
     """
     我的资料卡第一个信息
     """
     gold = user.gold
     win = user.win
     lose = user.lose
```

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.0/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.9/setup.py` & `nonebot_plugin_game_collection-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.9',
+version='2.2.0',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

