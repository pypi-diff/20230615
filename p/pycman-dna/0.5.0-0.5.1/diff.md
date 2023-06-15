# Comparing `tmp/pycman_dna-0.5.0.tar.gz` & `tmp/pycman_dna-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycman_dna-0.5.0.tar", last modified: Thu Jun 15 16:48:00 2023, max compression
+gzip compressed data, was "pycman_dna-0.5.1.tar", last modified: Thu Jun 15 16:57:30 2023, max compression
```

## Comparing `pycman_dna-0.5.0.tar` & `pycman_dna-0.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:48:00.741536 pycman_dna-0.5.0/
--rw-rw-rw-   0        0        0      564 2023-06-15 16:48:00.741536 pycman_dna-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 16:48:00.556157 pycman_dna-0.5.0/pycman_dna/
--rw-rw-rw-   0        0        0       81 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:48:00.636286 pycman_dna-0.5.0/pycman_dna/images/
--rw-rw-rw-   0        0        0     1017 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/PacmanDEAD.png
--rw-rw-rw-   0        0        0     1113 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/PacmanDOWN.png
--rw-rw-rw-   0        0        0     1075 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/PacmanLEFT.png
--rw-rw-rw-   0        0        0     1046 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/PacmanRIGHT.png
--rw-rw-rw-   0        0        0     1143 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/PacmanUP.png
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/__init__.py
--rw-rw-rw-   0        0        0     5042 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/dot.png
--rw-rw-rw-   0        0        0     6849 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/eatable_ghost.png
--rw-rw-rw-   0        0        0     7058 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/ghost.png
--rw-rw-rw-   0        0        0     9959 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/icon.png
--rw-rw-rw-   0        0        0     5684 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/pill.png
--rw-rw-rw-   0        0        0      650 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/images/wall.png
--rw-rw-rw-   0        0        0     9125 2023-06-15 16:46:59.000000 pycman_dna-0.5.0/pycman_dna/map.py
--rw-rw-rw-   0        0        0      537 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/map_names.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 16:48:00.738152 pycman_dna-0.5.0/pycman_dna/maps/
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/__init__.py
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/all_along_the_watchtowers.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/all_along_the_watchtowers_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/bimble.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/blank.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/broken_line_1.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/broken_line_2.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/broken_line_3.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/central_cavern.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/central_cavern_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/dizzy.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/easy_does_it.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/first_steps.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/follow_the_yellow_brick_road.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/ghost_train.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/i_smell_your_fear.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/killing_time.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/maze.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/number_one_the_larch.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/on_the_outside.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/on_the_outside_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/ping_pong.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/sense_your_way.map
--rw-rw-rw-   0        0        0      454 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/teeth.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/unbroken_line_1.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/unbroken_line_2.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/unbroken_line_3.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/valid_symbols.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/you_make_me_feel_like_dancing.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.0/pycman_dna/maps/you_will_blink_first.map
--rw-rw-rw-   0        0        0    11048 2023-06-15 16:25:27.000000 pycman_dna-0.5.0/pycman_dna/pacman_game.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:48:00.592384 pycman_dna-0.5.0/pycman_dna.egg-info/
--rw-rw-rw-   0        0        0      564 2023-06-15 16:48:00.000000 pycman_dna-0.5.0/pycman_dna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1778 2023-06-15 16:48:00.000000 pycman_dna-0.5.0/pycman_dna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:48:00.000000 pycman_dna-0.5.0/pycman_dna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 16:48:00.000000 pycman_dna-0.5.0/pycman_dna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 16:48:00.000000 pycman_dna-0.5.0/pycman_dna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:48:00.741536 pycman_dna-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-15 16:47:41.000000 pycman_dna-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:30.548383 pycman_dna-0.5.1/
+-rw-rw-rw-   0        0        0      564 2023-06-15 16:57:30.548383 pycman_dna-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:30.348210 pycman_dna-0.5.1/pycman_dna/
+-rw-rw-rw-   0        0        0       81 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:30.416803 pycman_dna-0.5.1/pycman_dna/images/
+-rw-rw-rw-   0        0        0     1017 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/PacmanDEAD.png
+-rw-rw-rw-   0        0        0     1113 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/PacmanDOWN.png
+-rw-rw-rw-   0        0        0     1075 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/PacmanLEFT.png
+-rw-rw-rw-   0        0        0     1046 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/PacmanRIGHT.png
+-rw-rw-rw-   0        0        0     1143 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/PacmanUP.png
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/__init__.py
+-rw-rw-rw-   0        0        0     5042 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/dot.png
+-rw-rw-rw-   0        0        0     6849 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/eatable_ghost.png
+-rw-rw-rw-   0        0        0     7058 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/ghost.png
+-rw-rw-rw-   0        0        0     9959 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/icon.png
+-rw-rw-rw-   0        0        0     5684 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/pill.png
+-rw-rw-rw-   0        0        0      650 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/images/wall.png
+-rw-rw-rw-   0        0        0     9122 2023-06-15 16:57:04.000000 pycman_dna-0.5.1/pycman_dna/map.py
+-rw-rw-rw-   0        0        0      537 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/map_names.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:30.543099 pycman_dna-0.5.1/pycman_dna/maps/
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/__init__.py
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/all_along_the_watchtowers.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/all_along_the_watchtowers_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/bimble.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/blank.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/broken_line_1.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/broken_line_2.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/broken_line_3.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/central_cavern.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/central_cavern_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/dizzy.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/easy_does_it.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/first_steps.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/follow_the_yellow_brick_road.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/ghost_train.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/i_smell_your_fear.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/killing_time.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/maze.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/number_one_the_larch.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/on_the_outside.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/on_the_outside_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/ping_pong.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/sense_your_way.map
+-rw-rw-rw-   0        0        0      454 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/teeth.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/unbroken_line_1.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/unbroken_line_2.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/unbroken_line_3.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/valid_symbols.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/you_make_me_feel_like_dancing.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.5.1/pycman_dna/maps/you_will_blink_first.map
+-rw-rw-rw-   0        0        0    11048 2023-06-15 16:25:27.000000 pycman_dna-0.5.1/pycman_dna/pacman_game.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:57:30.385094 pycman_dna-0.5.1/pycman_dna.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-06-15 16:57:30.000000 pycman_dna-0.5.1/pycman_dna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2023-06-15 16:57:30.000000 pycman_dna-0.5.1/pycman_dna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:57:30.000000 pycman_dna-0.5.1/pycman_dna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 16:57:30.000000 pycman_dna-0.5.1/pycman_dna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 16:57:30.000000 pycman_dna-0.5.1/pycman_dna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:57:30.548383 pycman_dna-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-15 16:57:23.000000 pycman_dna-0.5.1/setup.py
```

### Comparing `pycman_dna-0.5.0/PKG-INFO` & `pycman_dna-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman_dna
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.5.0/pycman_dna/images/PacmanDEAD.png` & `pycman_dna-0.5.1/pycman_dna/images/PacmanDEAD.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/PacmanDOWN.png` & `pycman_dna-0.5.1/pycman_dna/images/PacmanDOWN.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/PacmanLEFT.png` & `pycman_dna-0.5.1/pycman_dna/images/PacmanLEFT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/PacmanRIGHT.png` & `pycman_dna-0.5.1/pycman_dna/images/PacmanRIGHT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/PacmanUP.png` & `pycman_dna-0.5.1/pycman_dna/images/PacmanUP.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/dot.png` & `pycman_dna-0.5.1/pycman_dna/images/dot.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/eatable_ghost.png` & `pycman_dna-0.5.1/pycman_dna/images/eatable_ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/ghost.png` & `pycman_dna-0.5.1/pycman_dna/images/ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/icon.png` & `pycman_dna-0.5.1/pycman_dna/images/icon.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/pill.png` & `pycman_dna-0.5.1/pycman_dna/images/pill.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/images/wall.png` & `pycman_dna-0.5.1/pycman_dna/images/wall.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/map.py` & `pycman_dna-0.5.1/pycman_dna/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
     def __build_map_model(self, map_name : str) -> None:
         map_data = self.__read_map(map_name)
         if(platform.system() == "Windows"):
             self.__difficulty = map_data[0][3:];
         else:
-            self.__difficulty = map_data[0][0];
+            self.__difficulty = map_data[0];
         self.__total_moves = int(map_data[1]);
         for i in range(0, len(map_data) - 2):
             chars = list(map_data[i + 2])
             for j in range(0, len(chars)):
                 match chars[j]:
                     case '-':
                         self.__board_model[j][i] = Obstacle.EMPTY
```

### Comparing `pycman_dna-0.5.0/pycman_dna/map_names.txt` & `pycman_dna-0.5.1/pycman_dna/map_names.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna/pacman_game.py` & `pycman_dna-0.5.1/pycman_dna/pacman_game.py`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/pycman_dna.egg-info/PKG-INFO` & `pycman_dna-0.5.1/pycman_dna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman-dna
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.5.0/pycman_dna.egg-info/SOURCES.txt` & `pycman_dna-0.5.1/pycman_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.5.0/setup.py` & `pycman_dna-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.0' 
+VERSION = '0.5.1' 
 DESCRIPTION = 'Python Pacman Tool'
 LONG_DESCRIPTION = 'A teaching tool based on arcade icon Pacman, written in Python. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="pycman_dna",
```

