# Comparing `tmp/pycman_dna-0.4.6.tar.gz` & `tmp/pycman_dna-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycman_dna-0.4.6.tar", last modified: Thu Jun 15 14:59:21 2023, max compression
+gzip compressed data, was "pycman_dna-0.4.7.tar", last modified: Thu Jun 15 16:00:57 2023, max compression
```

## Comparing `pycman_dna-0.4.6.tar` & `pycman_dna-0.4.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:59:21.314055 pycman_dna-0.4.6/
--rw-rw-rw-   0        0        0      564 2023-06-15 14:59:21.312302 pycman_dna-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 14:59:21.108347 pycman_dna-0.4.6/pycman_dna/
--rw-rw-rw-   0        0        0       81 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:59:21.191597 pycman_dna-0.4.6/pycman_dna/images/
--rw-rw-rw-   0        0        0     1017 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/PacmanDEAD.png
--rw-rw-rw-   0        0        0     1113 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/PacmanDOWN.png
--rw-rw-rw-   0        0        0     1075 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/PacmanLEFT.png
--rw-rw-rw-   0        0        0     1046 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/PacmanRIGHT.png
--rw-rw-rw-   0        0        0     1143 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/PacmanUP.png
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/__init__.py
--rw-rw-rw-   0        0        0     5042 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/dot.png
--rw-rw-rw-   0        0        0     6849 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/eatable_ghost.png
--rw-rw-rw-   0        0        0     7058 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/ghost.png
--rw-rw-rw-   0        0        0     9959 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/icon.png
--rw-rw-rw-   0        0        0     5684 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/pill.png
--rw-rw-rw-   0        0        0      650 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/images/wall.png
--rw-rw-rw-   0        0        0     8993 2023-06-15 14:57:10.000000 pycman_dna-0.4.6/pycman_dna/map.py
--rw-rw-rw-   0        0        0      537 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/map_names.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 14:59:21.306909 pycman_dna-0.4.6/pycman_dna/maps/
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/__init__.py
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/all_along_the_watchtowers.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/all_along_the_watchtowers_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/bimble.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/blank.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/broken_line_1.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/broken_line_2.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/broken_line_3.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/central_cavern.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/central_cavern_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/dizzy.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/easy_does_it.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/first_steps.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/follow_the_yellow_brick_road.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/ghost_train.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/i_smell_your_fear.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/killing_time.map
--rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/maze.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/number_one_the_larch.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/on_the_outside.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/on_the_outside_revisited.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/ping_pong.map
--rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/sense_your_way.map
--rw-rw-rw-   0        0        0      454 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/teeth.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/unbroken_line_1.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/unbroken_line_2.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/unbroken_line_3.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/valid_symbols.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/you_make_me_feel_like_dancing.map
--rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.6/pycman_dna/maps/you_will_blink_first.map
--rw-rw-rw-   0        0        0     9889 2023-06-15 14:56:32.000000 pycman_dna-0.4.6/pycman_dna/pacman_game.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:59:21.149382 pycman_dna-0.4.6/pycman_dna.egg-info/
--rw-rw-rw-   0        0        0      564 2023-06-15 14:59:20.000000 pycman_dna-0.4.6/pycman_dna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1778 2023-06-15 14:59:20.000000 pycman_dna-0.4.6/pycman_dna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:59:20.000000 pycman_dna-0.4.6/pycman_dna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-15 14:59:20.000000 pycman_dna-0.4.6/pycman_dna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 14:59:20.000000 pycman_dna-0.4.6/pycman_dna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 14:59:21.314055 pycman_dna-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-15 14:59:05.000000 pycman_dna-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:00:57.836916 pycman_dna-0.4.7/
+-rw-rw-rw-   0        0        0      564 2023-06-15 16:00:57.836916 pycman_dna-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 16:00:57.652256 pycman_dna-0.4.7/pycman_dna/
+-rw-rw-rw-   0        0        0       81 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:00:57.728998 pycman_dna-0.4.7/pycman_dna/images/
+-rw-rw-rw-   0        0        0     1017 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/PacmanDEAD.png
+-rw-rw-rw-   0        0        0     1113 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/PacmanDOWN.png
+-rw-rw-rw-   0        0        0     1075 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/PacmanLEFT.png
+-rw-rw-rw-   0        0        0     1046 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/PacmanRIGHT.png
+-rw-rw-rw-   0        0        0     1143 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/PacmanUP.png
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/__init__.py
+-rw-rw-rw-   0        0        0     5042 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/dot.png
+-rw-rw-rw-   0        0        0     6849 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/eatable_ghost.png
+-rw-rw-rw-   0        0        0     7058 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/ghost.png
+-rw-rw-rw-   0        0        0     9959 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/icon.png
+-rw-rw-rw-   0        0        0     5684 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/pill.png
+-rw-rw-rw-   0        0        0      650 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/images/wall.png
+-rw-rw-rw-   0        0        0     8993 2023-06-15 14:57:10.000000 pycman_dna-0.4.7/pycman_dna/map.py
+-rw-rw-rw-   0        0        0      537 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/map_names.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 16:00:57.836916 pycman_dna-0.4.7/pycman_dna/maps/
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/__init__.py
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/all_along_the_watchtowers.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/all_along_the_watchtowers_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/bimble.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/blank.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/broken_line_1.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/broken_line_2.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/broken_line_3.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/central_cavern.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/central_cavern_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/dizzy.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/easy_does_it.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/first_steps.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/follow_the_yellow_brick_road.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/ghost_train.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/i_smell_your_fear.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/impossible_to_solve_do_not_even_try.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/killing_time.map
+-rw-rw-rw-   0        0        0      451 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/maze.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/number_one_the_larch.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/on_the_outside.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/on_the_outside_revisited.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/ping_pong.map
+-rw-rw-rw-   0        0        0      452 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/sense_your_way.map
+-rw-rw-rw-   0        0        0      454 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/teeth.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/unbroken_line_1.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/unbroken_line_2.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/unbroken_line_3.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/valid_symbols.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/you_make_me_feel_like_dancing.map
+-rw-rw-rw-   0        0        0      453 2023-06-15 14:37:57.000000 pycman_dna-0.4.7/pycman_dna/maps/you_will_blink_first.map
+-rw-rw-rw-   0        0        0    10226 2023-06-15 16:00:08.000000 pycman_dna-0.4.7/pycman_dna/pacman_game.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:00:57.677923 pycman_dna-0.4.7/pycman_dna.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-06-15 16:00:57.000000 pycman_dna-0.4.7/pycman_dna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2023-06-15 16:00:57.000000 pycman_dna-0.4.7/pycman_dna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:00:57.000000 pycman_dna-0.4.7/pycman_dna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 16:00:57.000000 pycman_dna-0.4.7/pycman_dna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 16:00:57.000000 pycman_dna-0.4.7/pycman_dna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:00:57.836916 pycman_dna-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-15 16:00:45.000000 pycman_dna-0.4.7/setup.py
```

### Comparing `pycman_dna-0.4.6/PKG-INFO` & `pycman_dna-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman_dna
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.4.6/pycman_dna/images/PacmanDEAD.png` & `pycman_dna-0.4.7/pycman_dna/images/PacmanDEAD.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/PacmanDOWN.png` & `pycman_dna-0.4.7/pycman_dna/images/PacmanDOWN.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/PacmanLEFT.png` & `pycman_dna-0.4.7/pycman_dna/images/PacmanLEFT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/PacmanRIGHT.png` & `pycman_dna-0.4.7/pycman_dna/images/PacmanRIGHT.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/PacmanUP.png` & `pycman_dna-0.4.7/pycman_dna/images/PacmanUP.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/dot.png` & `pycman_dna-0.4.7/pycman_dna/images/dot.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/eatable_ghost.png` & `pycman_dna-0.4.7/pycman_dna/images/eatable_ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/ghost.png` & `pycman_dna-0.4.7/pycman_dna/images/ghost.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/icon.png` & `pycman_dna-0.4.7/pycman_dna/images/icon.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/pill.png` & `pycman_dna-0.4.7/pycman_dna/images/pill.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/images/wall.png` & `pycman_dna-0.4.7/pycman_dna/images/wall.png`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/map.py` & `pycman_dna-0.4.7/pycman_dna/map.py`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/map_names.txt` & `pycman_dna-0.4.7/pycman_dna/map_names.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/pycman_dna/pacman_game.py` & `pycman_dna-0.4.7/pycman_dna/pacman_game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 from tkinter import simpledialog;
 import importlib.resources as pkg_resources;
 import time;
 import threading, sys, os;
 import platform;
-
-if(platform.system() == "Windows"):
-    import ctypes;
+import ctypes;
 
 from pycman_dna.map import Map
 from pycman_dna.map  import Direction;
 
 class PacmanGame:
     """
     PacmanGame's base constructor method. Performs initial setup.
     """
     __update_rate = 0.25;
     __moves_taken = 0;
     def __init__(self):
         self.__screen = None
+        self.__render_surface = None
         self.__game_running = True;
         self.__message = "No message"
         self.__map = None;
         self.__map_name = ""
         self.set_update_rate(250)
         if(platform.system() == "Windows"):
             ctypes.windll.shcore.SetProcessDpiAwareness(2)
+        if(platform.system() == "Linux"):
+            ctypes
 
 
     def __run_game(self) -> None:
         """
         
         """
         import pygame;
         pygame.init();
         
-        self.__screen = pygame.display.set_mode([784, 784], pygame.SCALED)
-        #self.__screen = pygame.display.set_mode([600, 600], pygame.SCALED)
+        self.__render_surface = pygame.Surface((784, 784))
+        if platform.system() == "Windows":
+            self.__screen = pygame.display.set_mode([784, 784], pygame.SCALED)
+        else:
+            self.__screen = pygame.display.set_mode([600, 600], pygame.SCALED)
         pygame.display.set_icon(pygame.image.load(os.path.dirname(__file__) + "/images/icon.png"))
         pygame.display.set_caption("Pycman - " + "\"" +self.__map_name + "\"")
 
         while True:
             for event in pygame.event.get():
                 if event.type == pygame.QUIT or (event.type == pygame.KEYDOWN and event.key == pygame.K_ESCAPE):
                     self.__game_running = False
                     os._exit(1)
             # Fill the background with black
             self.__screen.fill((0, 0, 0))
+            self.__render_surface.fill((0, 0, 0))
             
-            self.__map.draw_map(self.__screen);
+            self.__map.draw_map(self.__render_surface);
+            self.__screen.blit(pygame.transform.smoothscale(self.__render_surface, self.__screen.get_size()), (0,0))
             
             # Flip the display
             pygame.display.flip()
-        pygame.quit() 
         
 
     def __check_end_conditions(self):
         if self.__map._Map__dot_count <= 0:
             self.__game_running = False
             self.send_message("All dots collected - well done!")
         elif self.__moves_taken >= self.__map._Map__total_moves:
```

### Comparing `pycman_dna-0.4.6/pycman_dna.egg-info/PKG-INFO` & `pycman_dna-0.4.7/pycman_dna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycman-dna
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Pacman Tool
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pacman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pycman_dna-0.4.6/pycman_dna.egg-info/SOURCES.txt` & `pycman_dna-0.4.7/pycman_dna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycman_dna-0.4.6/setup.py` & `pycman_dna-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.6' 
+VERSION = '0.4.7' 
 DESCRIPTION = 'Python Pacman Tool'
 LONG_DESCRIPTION = 'A teaching tool based on arcade icon Pacman, written in Python. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="pycman_dna",
```

