# Comparing `tmp/statsbombpy-1.8.1.tar.gz` & `tmp/statsbombpy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsbombpy-1.8.1.tar", last modified: Mon Mar 27 23:37:21 2023, max compression
+gzip compressed data, was "statsbombpy-1.9.0.tar", last modified: Tue Mar 28 13:07:49 2023, max compression
```

## Comparing `statsbombpy-1.8.1.tar` & `statsbombpy-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-27 23:37:21.547706 statsbombpy-1.8.1/
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)    63014 2023-03-27 23:37:21.547706 statsbombpy-1.8.1/PKG-INFO
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)    62734 2023-03-24 17:00:22.000000 statsbombpy-1.8.1/README.md
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       38 2023-03-27 23:37:21.547706 statsbombpy-1.8.1/setup.cfg
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)      708 2023-03-27 23:36:43.000000 statsbombpy-1.8.1/setup.py
-drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-27 23:37:21.547706 statsbombpy-1.8.1/statsbombpy/
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2021-10-16 21:20:31.000000 statsbombpy-1.8.1/statsbombpy/__init__.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     2673 2022-11-17 12:15:47.000000 statsbombpy-1.8.1/statsbombpy/api_client.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     1242 2023-03-24 17:00:22.000000 statsbombpy-1.8.1/statsbombpy/config.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)      896 2022-11-17 12:15:47.000000 statsbombpy-1.8.1/statsbombpy/entities.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     2772 2023-03-24 17:00:22.000000 statsbombpy-1.8.1/statsbombpy/helpers.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     1064 2023-03-27 14:20:13.000000 statsbombpy-1.8.1/statsbombpy/public.py
--rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     9298 2023-03-24 17:00:22.000000 statsbombpy-1.8.1/statsbombpy/sb.py
-drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-27 23:37:21.547706 statsbombpy-1.8.1/statsbombpy.egg-info/
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)    63014 2023-03-27 23:37:21.000000 statsbombpy-1.8.1/statsbombpy.egg-info/PKG-INFO
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)      351 2023-03-27 23:37:21.000000 statsbombpy-1.8.1/statsbombpy.egg-info/SOURCES.txt
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)        1 2023-03-27 23:37:21.000000 statsbombpy-1.8.1/statsbombpy.egg-info/dependency_links.txt
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       59 2023-03-27 23:37:21.000000 statsbombpy-1.8.1/statsbombpy.egg-info/requires.txt
--rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       12 2023-03-27 23:37:21.000000 statsbombpy-1.8.1/statsbombpy.egg-info/top_level.txt
+drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-28 13:07:49.602735 statsbombpy-1.9.0/
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)    63014 2023-03-28 13:07:49.602735 statsbombpy-1.9.0/PKG-INFO
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)    62734 2023-03-28 13:06:34.000000 statsbombpy-1.9.0/README.md
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       38 2023-03-28 13:07:49.602735 statsbombpy-1.9.0/setup.cfg
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)      708 2023-03-28 13:06:43.000000 statsbombpy-1.9.0/setup.py
+drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-28 13:07:49.602735 statsbombpy-1.9.0/statsbombpy/
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2021-10-16 21:20:31.000000 statsbombpy-1.9.0/statsbombpy/__init__.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     2673 2022-11-17 12:15:47.000000 statsbombpy-1.9.0/statsbombpy/api_client.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     1242 2023-03-28 13:06:34.000000 statsbombpy-1.9.0/statsbombpy/config.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)      896 2022-11-17 12:15:47.000000 statsbombpy-1.9.0/statsbombpy/entities.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     3586 2023-03-28 13:06:43.000000 statsbombpy-1.9.0/statsbombpy/helpers.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     1064 2023-03-27 14:20:13.000000 statsbombpy-1.9.0/statsbombpy/public.py
+-rwxrwxr-x   0 scotty779  (1000) scotty779  (1000)     9298 2023-03-28 13:06:34.000000 statsbombpy-1.9.0/statsbombpy/sb.py
+drwxrwxr-x   0 scotty779  (1000) scotty779  (1000)        0 2023-03-28 13:07:49.602735 statsbombpy-1.9.0/statsbombpy.egg-info/
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)    63014 2023-03-28 13:07:49.000000 statsbombpy-1.9.0/statsbombpy.egg-info/PKG-INFO
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)      351 2023-03-28 13:07:49.000000 statsbombpy-1.9.0/statsbombpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)        1 2023-03-28 13:07:49.000000 statsbombpy-1.9.0/statsbombpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       59 2023-03-28 13:07:49.000000 statsbombpy-1.9.0/statsbombpy.egg-info/requires.txt
+-rw-rw-r--   0 scotty779  (1000) scotty779  (1000)       12 2023-03-28 13:07:49.000000 statsbombpy-1.9.0/statsbombpy.egg-info/top_level.txt
```

### Comparing `statsbombpy-1.8.1/PKG-INFO` & `statsbombpy-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: statsbombpy
-Version: 1.8.1
-Summary: Easily stream StatsBomb data into Python
+Version: 1.9.0
+Summary: easily stream StatsBomb data into Python
 Home-page: https://github.com/statsbomb/statsbombpy
 Author: StatsBomb
 Author-email: support@statsbombservices.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # statsbombpy
```

### Comparing `statsbombpy-1.8.1/README.md` & `statsbombpy-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/setup.py` & `statsbombpy-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")) as f:
     README = f.read()
 
 setup(
     name="statsbombpy",
-    version="1.8.1",
-    description="Easily stream StatsBomb data into Python",
+    version="1.9.0",
+    description="easily stream StatsBomb data into Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/statsbomb/statsbombpy",
     author="StatsBomb",
     author_email="support@statsbombservices.com",
     packages=["statsbombpy"],
     install_requires=[
```

### Comparing `statsbombpy-1.8.1/statsbombpy/api_client.py` & `statsbombpy-1.9.0/statsbombpy/api_client.py`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/statsbombpy/config.py` & `statsbombpy-1.9.0/statsbombpy/config.py`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/statsbombpy/entities.py` & `statsbombpy-1.9.0/statsbombpy/entities.py`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/statsbombpy/helpers.py` & `statsbombpy-1.9.0/statsbombpy/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,48 @@
 from collections import defaultdict
 
-import inflect
 import pandas as pd
-from joblib import Memory
+
+PLURALS = {
+    'Starting XI': 'starting_xis',
+    'Half Start': 'half_starts',
+    'Camera On': 'camera ons',
+    'Camera off': 'camera offs',
+    'Pass': 'passes',
+    'Ball Receipt*': 'ball_receipts',
+    'Carry': 'carrys',
+    'Pressure': 'pressures',
+    'Foul Committed': 'foul_committeds',
+    'Foul Won': 'foul_wons',
+    'Duel': 'duels',
+    'Interception': 'interceptions',
+    'Block': 'blocks',
+    'Referee Ball-Drop': 'referee_ball_drops',
+    'Ball Recovery': 'ball_recoverys',
+    'Dispossessed': 'dispossesseds',
+    'Clearance': 'clearances',
+    'Dribble': 'dribbles',
+    'Miscontrol': 'miscontrols',
+    'Shot': 'shots',
+    'Goal Keeper': 'goal_keepers',
+    'Dribbled Past': 'dribbled_pasts',
+    'Injury Stoppage': 'injury_stoppages',
+    'Half End': 'half_ends',
+    'Substitution': 'substitutions',
+    'Shield': 'shields',
+    'Tactical Shift': 'tactical_shifts',
+    'Own Goal Against': 'own_goal_againsts',
+    'Own Goal For': 'own_goal_fors',
+    'Bad Behaviour': 'bad_behaviours',
+    'Player Off': 'player_offs',
+    'Player On': 'player_ons',
+    '50/50': '50/50s',
+    'Error': 'errors',
+    'Offside': 'offsides'
+}
 
 
 def flatten_event(event, flatten_attrs):
     if flatten_attrs:
         ev_type = event["type"]["name"].lower().replace(" ", "_").replace("*", "")
         ev_type = ev_type if event["type"]["name"] != "Goal Keeper" else "goalkeeper"
         if ev_type in event:
@@ -21,15 +57,15 @@
                 event[f"{k}_id"] = v["id"]
     return event
 
 
 def filter_and_group_events(events, filters, fmt, flatten_attrs):
     events_ = defaultdict(list)
     for ev in events.values():
-        ev_type = pluralize(ev["type"]["name"])
+        ev_type = PLURALS[ev["type"]["name"]]
         if not is_relevant(ev, filters):
             continue
         if fmt == "dataframe":
             ev = flatten_event(ev, flatten_attrs)
         events_[ev_type].append(ev)
     return events_
 
@@ -71,21 +107,7 @@
                     else:
                         event["visible_opponents"] = team["count"]
             if key in drop_keys:
                 del event[key]
     return events
 
 
-engine = inflect.engine()
-
-cachedir = ".cache/"
-memory = Memory(cachedir, verbose=0)
-
-
-@memory.cache
-def pluralize(word):
-    word = engine.plural(word)
-    word = word.replace("*", "")
-    word = word.replace("-", "_")
-    word = word.replace(" ", "_")
-    word = word.lower()
-    return word
```

### Comparing `statsbombpy-1.8.1/statsbombpy/public.py` & `statsbombpy-1.9.0/statsbombpy/public.py`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/statsbombpy/sb.py` & `statsbombpy-1.9.0/statsbombpy/sb.py`

 * *Files identical despite different names*

### Comparing `statsbombpy-1.8.1/statsbombpy.egg-info/PKG-INFO` & `statsbombpy-1.9.0/statsbombpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: statsbombpy
-Version: 1.8.1
-Summary: Easily stream StatsBomb data into Python
+Version: 1.9.0
+Summary: easily stream StatsBomb data into Python
 Home-page: https://github.com/statsbomb/statsbombpy
 Author: StatsBomb
 Author-email: support@statsbombservices.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # statsbombpy
```

