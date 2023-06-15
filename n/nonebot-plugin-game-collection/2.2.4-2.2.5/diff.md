# Comparing `tmp/nonebot_plugin_game_collection-2.2.4.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.4.tar", last modified: Thu Jun 15 18:53:54 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.5.tar", last modified: Thu Jun 15 19:17:22 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.4.tar` & `nonebot_plugin_game_collection-2.2.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.319353 nonebot_plugin_game_collection-2.2.4/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.4/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-15 18:53:54.317852 nonebot_plugin_game_collection-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.268602 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21158 2023-06-15 18:18:05.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    55947 2023-06-13 16:02:57.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.283115 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13585 2023-06-15 18:51:34.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20126 2023-06-15 15:00:24.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16157 2023-06-06 15:49:58.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    33104 2023-06-15 18:17:34.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.288120 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.292453 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.310846 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5278 2023-06-12 13:50:26.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.312348 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.316351 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7825 2023-06-15 17:13:10.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:53:54.277111 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-15 18:53:54.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-15 18:53:54.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 18:53:54.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-15 18:53:54.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-15 18:53:54.000000 nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 18:53:54.319854 nonebot_plugin_game_collection-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-15 18:53:39.000000 nonebot_plugin_game_collection-2.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.763799 nonebot_plugin_game_collection-2.2.5/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.5/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-15 19:17:22.762797 nonebot_plugin_game_collection-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.713992 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21158 2023-06-15 18:18:05.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    55947 2023-06-13 16:02:57.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.727504 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13575 2023-06-15 19:12:41.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20085 2023-06-15 19:15:09.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16157 2023-06-06 15:49:58.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    33104 2023-06-15 18:17:34.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.734160 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.738163 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.756290 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5278 2023-06-12 13:50:26.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.757293 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.761297 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7825 2023-06-15 17:13:10.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.720497 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:17:22.763799 nonebot_plugin_game_collection-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-15 19:17:18.000000 nonebot_plugin_game_collection-2.2.5/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.4/LICENSE` & `nonebot_plugin_game_collection-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/README.md` & `nonebot_plugin_game_collection-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 company_index:Dict[str,int] = {}
 
 def update_company_index():
     """
     从群数据生成公司名查找群号的字典
     """
-    globals()['company_index'] = {}
+    company_index.clear()
     for group_id in group_data:
         if company_name := group_data[group_id].company.company_name:
             company_index[company_name] = group_id
             company_index[str(group_id)] = group_id
 
 update_company_index()
```

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Market.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     user = Manager.locate_user(event)[0]
     if user.props.get("33001",0) < 1:
         return f"你的【{props_library['33001']['name']}】已失效"
     if check := check_company_name(company_name):
         return check
     old_company_name = company.company_name
     company.company_name = company_name
-    del company_index[old_company_name]
     update_company_index()
     return f'【{old_company_name}】已重命名为【{company_name}】'
 
 def value_update(group_account:GroupAccount):
     """
     刷新持股价值
     group_account:用户群账户
```

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.4/setup.py` & `nonebot_plugin_game_collection-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.4',
+version='2.2.5',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

