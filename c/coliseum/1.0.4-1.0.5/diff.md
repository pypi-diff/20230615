# Comparing `tmp/coliseum-1.0.4.tar.gz` & `tmp/coliseum-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coliseum-1.0.4.tar", last modified: Sun Oct 25 03:39:52 2020, max compression
+gzip compressed data, was "coliseum-1.0.5.tar", last modified: Thu Jun 15 03:51:24 2023, max compression
```

## Comparing `coliseum-1.0.4.tar` & `coliseum-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-10-25 03:39:52.934775 coliseum-1.0.4/
--rw-r--r--   0 sig       (1000) sig       (1000)       24 2020-10-13 16:57:01.000000 coliseum-1.0.4/MANIFEST.in
--rw-r--r--   0 sig       (1000) sig       (1000)     1255 2020-10-25 03:39:52.931382 coliseum-1.0.4/PKG-INFO
--rw-r--r--   0 sig       (1000) sig       (1000)      690 2020-10-13 21:53:49.000000 coliseum-1.0.4/README.md
--rw-r--r--   0 sig       (1000) sig       (1000)      208 2020-10-13 16:57:01.000000 coliseum-1.0.4/requirements.txt
--rw-r--r--   0 sig       (1000) sig       (1000)       38 2020-10-25 03:39:52.934775 coliseum-1.0.4/setup.cfg
--rw-r--r--   0 sig       (1000) sig       (1000)     1934 2020-10-13 21:30:42.000000 coliseum-1.0.4/setup.py
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-10-25 03:39:52.931382 coliseum-1.0.4/src/
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-10-25 03:39:52.931382 coliseum-1.0.4/src/coliseum/
--rw-r--r--   0 sig       (1000) sig       (1000)      430 2020-10-19 21:30:54.000000 coliseum-1.0.4/src/coliseum/__init__.py
--rw-r--r--   0 sig       (1000) sig       (1000)      430 2020-10-19 21:30:58.000000 coliseum-1.0.4/src/coliseum/__main__.py
--rw-r--r--   0 sig       (1000) sig       (1000)      286 2020-10-25 03:39:46.000000 coliseum-1.0.4/src/coliseum/_metadata.py
--rw-r--r--   0 sig       (1000) sig       (1000)       21 2020-10-25 03:39:46.000000 coliseum-1.0.4/src/coliseum/_version.py
--rw-r--r--   0 sig       (1000) sig       (1000)     1695 2020-10-20 16:36:31.000000 coliseum-1.0.4/src/coliseum/debug.py
--rw-r--r--   0 sig       (1000) sig       (1000)      692 2020-10-13 21:01:43.000000 coliseum-1.0.4/src/coliseum/enemies.py
--rw-r--r--   0 sig       (1000) sig       (1000)    15125 2020-10-25 03:39:46.000000 coliseum-1.0.4/src/coliseum/player.py
--rw-r--r--   0 sig       (1000) sig       (1000)     3818 2020-10-20 16:35:14.000000 coliseum-1.0.4/src/coliseum/tournaments.py
-drwxr-xr-x   0 sig       (1000) sig       (1000)        0 2020-10-25 03:39:52.931382 coliseum-1.0.4/src/coliseum.egg-info/
--rw-r--r--   0 sig       (1000) sig       (1000)     1255 2020-10-25 03:39:52.000000 coliseum-1.0.4/src/coliseum.egg-info/PKG-INFO
--rw-r--r--   0 sig       (1000) sig       (1000)      424 2020-10-25 03:39:52.000000 coliseum-1.0.4/src/coliseum.egg-info/SOURCES.txt
--rw-r--r--   0 sig       (1000) sig       (1000)        1 2020-10-25 03:39:52.000000 coliseum-1.0.4/src/coliseum.egg-info/dependency_links.txt
--rw-r--r--   0 sig       (1000) sig       (1000)      208 2020-10-25 03:39:52.000000 coliseum-1.0.4/src/coliseum.egg-info/requires.txt
--rw-r--r--   0 sig       (1000) sig       (1000)        9 2020-10-25 03:39:52.000000 coliseum-1.0.4/src/coliseum.egg-info/top_level.txt
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:51:24.483519 coliseum-1.0.5/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1091 2023-06-15 03:21:42.000000 coliseum-1.0.5/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       24 2021-07-26 03:19:27.000000 coliseum-1.0.5/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1358 2023-06-15 03:51:24.483519 coliseum-1.0.5/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      922 2023-06-15 03:35:30.000000 coliseum-1.0.5/README.md
+-rw-rw-r--   0 sig       (1000) sig       (1000)       40 2023-06-15 03:25:16.000000 coliseum-1.0.5/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-15 03:51:24.483519 coliseum-1.0.5/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1934 2022-10-02 23:44:51.000000 coliseum-1.0.5/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:51:24.479519 coliseum-1.0.5/src/
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:51:24.483519 coliseum-1.0.5/src/coliseum/
+-rw-rw-r--   0 sig       (1000) sig       (1000)      430 2021-07-26 03:19:27.000000 coliseum-1.0.5/src/coliseum/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      430 2021-07-26 03:19:27.000000 coliseum-1.0.5/src/coliseum/__main__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2448 2022-12-15 18:46:29.000000 coliseum-1.0.5/src/coliseum/_map.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      286 2021-07-26 03:19:27.000000 coliseum-1.0.5/src/coliseum/_metadata.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)       21 2023-06-15 03:30:22.000000 coliseum-1.0.5/src/coliseum/_version.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1695 2021-07-26 03:19:27.000000 coliseum-1.0.5/src/coliseum/debug.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      692 2021-07-26 03:19:27.000000 coliseum-1.0.5/src/coliseum/enemies.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)    16315 2023-06-15 03:47:35.000000 coliseum-1.0.5/src/coliseum/player.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4080 2022-10-02 23:13:34.000000 coliseum-1.0.5/src/coliseum/tournaments.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:51:24.483519 coliseum-1.0.5/src/coliseum.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1358 2023-06-15 03:51:24.000000 coliseum-1.0.5/src/coliseum.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      476 2023-06-15 03:51:24.000000 coliseum-1.0.5/src/coliseum.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-15 03:51:24.000000 coliseum-1.0.5/src/coliseum.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       41 2023-06-15 03:51:24.000000 coliseum-1.0.5/src/coliseum.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        9 2023-06-15 03:51:24.000000 coliseum-1.0.5/src/coliseum.egg-info/top_level.txt
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-15 03:51:24.483519 coliseum-1.0.5/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)       40 2021-07-26 03:19:27.000000 coliseum-1.0.5/tests/test_coliseum.py
```

### Comparing `coliseum-1.0.4/PKG-INFO` & `coliseum-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: coliseum
-Version: 1.0.4
+Version: 1.0.5
 Summary: a simple, turn-based command line game in python
 Home-page: https://github.com/signebedi/coliseum
 Author: Sig Janoska-Bedi
 Author-email: signe@siftingwinnowing.com
 License: MIT
-Description: 
-        
-        # coliseum
-        
-        [![Build Status](https://travis-ci.org/signebedi/coliseum.svg?branch=master)](https://travis-ci.org/signebedi/coliseum)
-        [![Documentation Status](https://readthedocs.org/projects/coliseum/badge/?version=stable)](https://coliseum.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/coliseum)](https://pypi.org/project/coliseum/)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
-        
-        a simple, turn-based command line game in python
-        
-        Read the docs at [coliseum.readthedocs.io/en/latest/](https://coliseum.readthedocs.io/en/latest/).
-        
-        ---
-        Copyright (c) 2020 Signe Janoska-Bedi and Jamey Kane
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# coliseum
+
+[![Documentation Status](https://readthedocs.org/projects/coliseum/badge/?version=stable)](https://coliseum.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/coliseum?color=brightgreen)](https://pypi.org/project/coliseum/)
+[![Downloads](https://static.pepy.tech/personalized-badge/coliseum?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/coliseum)
+[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
+[![Flask-Signing tests](https://github.com/signebedi/coliseum/workflows/tests/badge.svg)](https://github.com/signebedi/coliseum/actions)
+
+simple, turn-based, in your TTY 
+
+Read the docs at [coliseum.readthedocs.io/en/latest/](https://coliseum.readthedocs.io/en/latest/).
+
+---
+Copyright (c) 2020-23 Signe Janoska-Bedi and Jamey Kane
```

### Comparing `coliseum-1.0.4/README.md` & `coliseum-1.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ![gladiator gif](docs/cropped.gif)
 
 # coliseum
 
-[![Build Status](https://travis-ci.org/signebedi/coliseum.svg?branch=master)](https://travis-ci.org/signebedi/coliseum)
 [![Documentation Status](https://readthedocs.org/projects/coliseum/badge/?version=stable)](https://coliseum.readthedocs.io/en/latest/?badge=latest)
-[![PyPI](https://img.shields.io/pypi/v/coliseum)](https://pypi.org/project/coliseum/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/coliseum?color=brightgreen)](https://pypi.org/project/coliseum/)
+[![Downloads](https://static.pepy.tech/personalized-badge/coliseum?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/coliseum)
+[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
+[![Flask-Signing tests](https://github.com/signebedi/coliseum/workflows/tests/badge.svg)](https://github.com/signebedi/coliseum/actions)
 
-a simple, turn-based command line game in python
+simple, turn-based, in your TTY 
 
 Read the docs at [coliseum.readthedocs.io/en/latest/](https://coliseum.readthedocs.io/en/latest/).
 
 ---
-Copyright (c) 2020 Signe Janoska-Bedi and Jamey Kane
+Copyright (c) 2020-23 Signe Janoska-Bedi and Jamey Kane
```

### Comparing `coliseum-1.0.4/setup.py` & `coliseum-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,9 +47,9 @@
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=REQUIRED,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

### Comparing `coliseum-1.0.4/src/coliseum/debug.py` & `coliseum-1.0.5/src/coliseum/debug.py`

 * *Files identical despite different names*

### Comparing `coliseum-1.0.4/src/coliseum/enemies.py` & `coliseum-1.0.5/src/coliseum/enemies.py`

 * *Files identical despite different names*

### Comparing `coliseum-1.0.4/src/coliseum/player.py` & `coliseum-1.0.5/src/coliseum/player.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """player.py: primary source file for coliseum, a simple, turn-based command line game in python"""
 
 import time, colorama, os, random, pickle, sys
 from colorama import Fore, Back, Style 
 
 class Player:
-    def __init__(self):
+    def __init__(self, headless=False, ask_load_game=True, player_name=None):
         
         colorama.init(autoreset=True)
         
         header = [  '   _____ ____  _      _____  _____ ______ _    _ __  __ ',
                     '  / ____/ __ \| |    |_   _|/ ____|  ____| |  | |  \/  |',
                     ' | |   | |  | | |      | | | (___ | |__  | |  | | \  / |',
                     ' | |   | |  | | |      | |  \___ \|  __| | |  | | |\/| |',
                     ' | |___| |__| | |____ _| |_ ____) | |____| |__| | |  | |',
                     '  \_____\____/|______|_____|_____/|______|\____/|_|  |_|',
                 ]
+
+        if not headless:
+
+            for item in header: print(item)
         
-        for item in header: print(item)
-    
-        print('\nWelcome to the Coliseum. Earn ducats in the Work Room, buy equipment in the Shop, and battle for glory in the Arena!')
+            print('\nThe great Greek hero, Hercules, is inviting you to fight in his new golden coliseum! He is growing old, and wishes to see one last fight before he is laid to rest. He hashundreds of fighters from both Greece and Rome, that have all trained heavily their entire life - just like you! You will have to battle gladiators and knights alike, and it won\'t be easy! Armed with a bronze dagger, you will take on all the foes before you! Good luck, young fighter. You will need it!')
 
         self.lvl = 1
         self.xp = 0
         self.str = 1
         self.spd = 1
         self.con = 1
         self.weapon = 1
@@ -31,19 +33,30 @@
         self.potions = 0
         self.is_alive = True
         self.hp = 10*(self.lvl+self.con)
         self.gold = 5
         self.kills = 0
         self.victories = []
         
-        if os.path.exists("save.pickle"):
+        if ask_load_game and os.path.exists("save.pickle"):
             load_game = input('\nDo you want to load a save file? (yes, no; defaults to no)\n')
-            if load_game == 'yes': self.load()
-            else: self.name = input('\nWhat is your character\'s name?\n> ')
-        else: self.name = input('\nWhat is your character\'s name?\n> ')
+            if load_game == 'yes': 
+                self.load()
+            else: 
+                if not player_name:
+                    self.name = input('\nWhat is your character\'s name?\n> ')
+                else:
+                    self.name = player_name
+
+
+        else: 
+            if not player_name:
+                self.name = input('\nWhat is your character\'s name?\n> ')
+            else:
+                self.name = player_name
         
     def input(self):
         i = input('\nWhat would you like to do next? (type "help" for options)\n> ')
 
         if i == 'help': print('\nOPTIONS:\nwork\nstats\nstore\nbattle\ntournament\nsave\nload\n')
         elif i == 'work': self.work()
         elif i == 'stats': self.stats()
@@ -79,31 +92,37 @@
                 else: print('\nInsufficient gold -- you need 10 gold to purchase a potion\n')
             elif i == "stats": self.stats()
             elif i == "leave": print('\nyou left the armory\n'); break
             else: print('\nUnknown command! Please try again\n')
 
 
     def tournament(self, tournaments=None):
-        if not tournaments:
-            from coliseum.tournaments import tournaments
-        cmd = input(f'\nWhich tournament do you want to fight in? (options: {", ".join([t["name"] for t in tournaments])}) \n> ')
+        # if not tournaments:
+        from coliseum.tournaments import tournaments 
         
+        OPTS = [f'{t["name"]} ({t["short_name"]})' for t in tournaments]
+        cmd = input(f'\nWhich tournament do you want to fight in? (options: {", ".join(OPTS)}) \n> ')
+        # cmd = input(f'\nWhich tournament do you want to fight in? (options: {", ".join([f"{t['name']} ({t['short_name']})"] for t in tournaments])}) \n> ')
+
         for t in tournaments:
-            if cmd in t["name"]:
-                print(f'\nYou have opted to fight in the {cmd} and your enemies are {", ".join([e["name"] for e in t["enemies"]])}\n')
+            # if cmd == t["short_name"]:
+            if cmd == t["short_name"] or cmd == t['name']:
+            # if cmd in t['name'].lower():
+                print(f'\nYou have opted to fight in the {t["name"]} and your enemies are {", ".join([e["name"] for e in t["enemies"]])}\n')
 
                 player_lost_tournament = False
                 
                 for enemy in t["enemies"]:
-                    if self.battle(enemy, battle_type='tournament'): # assess the truth value of each battle and...
+                    temp_enemy = enemy.copy() # we create a mirror of the enemy object to keep the source unchanged (eg. for repeat battles)
+                    if self.battle(temp_enemy, battle_type='tournament'): # assess the truth value of each battle and...
                         player_lost_tournament = True # if returns true, break this loop and set player_lost_tournament to True
                         break
 
                 if player_lost_tournament: # only give the reward if the player actually wins the tournament
-                    print(f'\nYou lost the {cmd}\n')
+                    print(f'\nYou lost the {t["name"]}\n')
                 else:    
                     self.gold += t["gold"]
                     t["won"] = True
                     self.victories.append(t['name'])
                     print(f'\nYou won the {t["name"]} and earned {t["gold"]} ducats!\n')
             # else: print('\nInvalid tournament\n')
 
@@ -197,15 +216,15 @@
                         break
                     else:
                         self.dead()
                         break
     
             elif cmd == 'stats': self.stats()
             
-            elif cmd == 'help': print('\nOPTIONS:\natk\nstats\nrun\n')
+            elif cmd == 'help': print('\nOPTIONS:\na(tk)\nstats\npotion\nrun\n')
             
             elif cmd == 'potion': 
                 if self.potions > 0:
                     self.potions -= 1
                     self.hp = 10*(self.lvl+self.con)
                     print('\nYou used a potion and regained full health\n')
                 else: print ('\nInsufficient potions\n')
@@ -331,8 +350,8 @@
                     assert isinstance(enemy['def'], int)
                     assert isinstance(enemy['spd'], int)
                     assert isinstance(enemy['gold'], int)
 
             self.tournament(tournaments)
 
         except Exception as e:
-            print(f'\nsorry, could not find a file named tournament.py in the current working directory. See our docs for instructions on adding your own tournaments. {e}\n')
+            print(f'\nsorry, could not find a file named tournament.py in the current working directory. See our docs for instructions on adding your own tournaments. {e}\n')
```

### Comparing `coliseum-1.0.4/src/coliseum/tournaments.py` & `coliseum-1.0.5/src/coliseum/tournaments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,95 @@
 """tournaments.py: a set of tournaments the player can fight in coliseum, a simple, turn-based command line game in python"""
 
 tournaments = [
     {
         'name': 'Tutorial Cup',
+        'short_name': 'tutorial',
         'type': 'beginner',
         'enemies': [
             {'name':'Glardon the Greek', 'hp': 1, 'atk': 1, 'def': 1, 'spd': 1, 'gold': 0},
             {'name':'Filibert the Frank', 'hp': 17, 'atk': 3, 'def': 3, 'spd': 5, 'gold': 0},
             {'name':'Estek the Mamluk', 'hp': 28, 'atk': 5, 'def': 5, 'spd': 2, 'gold': 0},
         ],
         'gold': 10,
         'won': False,
     },
     {
         'name': 'Historical Cup',
+        'short_name': 'historical',
         'type': 'beginner',
         'enemies': [
             {'name':'Titus Livius', 'hp': 25, 'atk': 3, 'def': 3, 'spd': 3, 'gold': 0},
             {'name':'Thucydides', 'hp': 35, 'atk': 4, 'def': 4, 'spd': 5, 'gold': 0},
             {'name':'Plutarch', 'hp': 40, 'atk': 5, 'def': 5, 'spd': 4, 'gold': 0},
             {'name':'Aulus Hirtius', 'hp': 55, 'atk': 7, 'def': 6, 'spd': 6, 'gold': 0},
         ],
         'gold': 50,
         'won': False,
      },
     
     {
         'name': 'Mathematical Cup',
+        'short_name': 'mathematical',
         'type': 'beginner',
         'enemies': [
             {'name':'Thales', 'hp': 28, 'atk': 3, 'def': 4, 'spd': 4, 'gold': 0},
             {'name':'Pythagoras', 'hp': 36, 'atk': 3, 'def': 5, 'spd': 5, 'gold': 0},
             {'name':'Euclid', 'hp': 42, 'atk': 4, 'def': 6, 'spd': 5, 'gold': 0},
             {'name':'Archimedes of Syracuse', 'hp': 58, 'atk': 7, 'def': 7, 'spd': 7, 'gold': 0},
         ],
         'gold': 50,
         'won': False,
      },
     
     {
          'name': 'Dramatist Cup',
+         'short_name': 'dramatist',
          'type': 'beginner',
          'enemies': [
              {'name':'Aeschylus', 'hp': 23, 'atk': 4, 'def': 3, 'spd': 4, 'gold': 0},
              {'name':'Euripides', 'hp': 33, 'atk': 5, 'def': 4, 'spd': 5, 'gold': 0},
              {'name':'Aristophanes', 'hp': 38, 'atk': 5, 'def': 5, 'spd': 4, 'gold': 0},
              {'name':'Sophocles', 'hp': 55, 'atk': 8, 'def': 5, 'spd': 7, 'gold': 0},
          ],
          'gold': 50,
          'won': False,
      },
     
     {
          'name': 'Hellenic Cup',
+         'short_name': 'hellenic',
          'type': 'intermediate',
          'enemies': [
              {'name':'Pyrrhus of Epirus', 'hp': 65, 'atk': 7, 'def': 8, 'spd': 8, 'gold': 0},
              {'name':'Cleopatra', 'hp': 80, 'atk': 8, 'def': 8, 'spd': 8, 'gold': 0},
              {'name':'Hannibal Barca', 'hp': 100, 'atk': 12, 'def': 12, 'spd': 14, 'gold': 0},
              {'name':'Mithridates VI of Pontus', 'hp': 150, 'atk': 15, 'def': 15, 'spd': 15, 'gold': 0},        
          ],
          'gold': 75,
          'won': False,
      }, 
 
-    {'name': 'Barbarian Cup',
+    {
+        'name': 'Barbarian Cup',
+        'short_name': 'barbarian',
          'type': 'intermediate',
          'enemies': [
              {'name':'Jugurtha', 'hp': 85, 'atk': 8, 'def': 6, 'spd': 8, 'gold': 0},
              {'name':'Cassivellaunus', 'hp': 100, 'atk': 9, 'def': 7, 'spd': 8, 'gold': 0},
              {'name':'Vercingetorix', 'hp': 140, 'atk': 11, 'def': 8, 'spd': 12, 'gold': 0},
              {'name':'Arminius', 'hp': 175, 'atk': 17, 'def': 14, 'spd': 16, 'gold': 0},        
          ],
          'gold': 75,
          'won': False,
     },
 
-    {'name': 'Hero Cup',
+    {
+        'name': 'Hero Cup',
+        'short_name': 'hero',
          'type': 'advanced',
          'enemies': [
              {'name':'Publius Decius Mus', 'hp': 200, 'atk': 20, 'def': 14, 'spd': 17, 'gold': 0},
              {'name':'Quintus Fabius Maximus', 'hp': 300, 'atk': 18, 'def': 25, 'spd': 20, 'gold': 0},
              {'name':'Publius Cornelius Scipio', 'hp': 250, 'atk': 25, 'def': 20, 'spd': 20, 'gold': 0},
              {'name':'Gnaeus Pompey Magnus', 'hp': 500, 'atk': 30, 'def': 30, 'spd': 30, 'gold': 0},        
              {'name':'Gaius Julius Caesar', 'hp': 1000, 'atk': 35, 'def': 25, 'spd': 100, 'gold': 0},
```

### Comparing `coliseum-1.0.4/src/coliseum.egg-info/PKG-INFO` & `coliseum-1.0.5/src/coliseum.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: coliseum
-Version: 1.0.4
+Version: 1.0.5
 Summary: a simple, turn-based command line game in python
 Home-page: https://github.com/signebedi/coliseum
 Author: Sig Janoska-Bedi
 Author-email: signe@siftingwinnowing.com
 License: MIT
-Description: 
-        
-        # coliseum
-        
-        [![Build Status](https://travis-ci.org/signebedi/coliseum.svg?branch=master)](https://travis-ci.org/signebedi/coliseum)
-        [![Documentation Status](https://readthedocs.org/projects/coliseum/badge/?version=stable)](https://coliseum.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/coliseum)](https://pypi.org/project/coliseum/)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
-        
-        a simple, turn-based command line game in python
-        
-        Read the docs at [coliseum.readthedocs.io/en/latest/](https://coliseum.readthedocs.io/en/latest/).
-        
-        ---
-        Copyright (c) 2020 Signe Janoska-Bedi and Jamey Kane
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# coliseum
+
+[![Documentation Status](https://readthedocs.org/projects/coliseum/badge/?version=stable)](https://coliseum.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/coliseum?color=brightgreen)](https://pypi.org/project/coliseum/)
+[![Downloads](https://static.pepy.tech/personalized-badge/coliseum?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/coliseum)
+[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
+[![Flask-Signing tests](https://github.com/signebedi/coliseum/workflows/tests/badge.svg)](https://github.com/signebedi/coliseum/actions)
+
+simple, turn-based, in your TTY 
+
+Read the docs at [coliseum.readthedocs.io/en/latest/](https://coliseum.readthedocs.io/en/latest/).
+
+---
+Copyright (c) 2020-23 Signe Janoska-Bedi and Jamey Kane
```

