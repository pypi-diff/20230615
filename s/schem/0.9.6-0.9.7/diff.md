# Comparing `tmp/schem-0.9.6.tar.gz` & `tmp/schem-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schem-0.9.6.tar", last modified: Sun Apr 25 21:30:17 2021, max compression
+gzip compressed data, was "schem-0.9.7.tar", last modified: Mon Jul 19 02:54:24 2021, max compression
```

## Comparing `schem-0.9.6.tar` & `schem-0.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-04-25 21:30:17.223325 schem-0.9.6/
--rw-rw-rw-   0        0        0     1319 2021-02-13 19:18:31.000000 schem-0.9.6/LICENSE
--rw-rw-rw-   0        0        0     1130 2021-04-25 21:30:17.223325 schem-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0      418 2021-03-22 04:50:02.000000 schem-0.9.6/README.md
--rw-rw-rw-   0        0        0      110 2021-02-15 03:12:01.000000 schem-0.9.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2021-04-25 21:30:17.215002 schem-0.9.6/schem/
--rw-rw-rw-   0        0        0      476 2021-03-22 04:50:02.000000 schem-0.9.6/schem/__init__.py
--rw-rw-rw-   0        0        0     4317 2021-04-19 00:52:01.000000 schem-0.9.6/schem/__main__.py
--rw-rw-rw-   0        0        0    86332 2021-04-25 21:28:22.000000 schem-0.9.6/schem/components.py
--rw-rw-rw-   0        0        0     5111 2021-03-22 04:50:02.000000 schem-0.9.6/schem/elements.py
--rw-rw-rw-   0        0        0      395 2021-03-22 04:50:02.000000 schem-0.9.6/schem/exceptions.py
--rw-rw-rw-   0        0        0     4841 2021-04-19 00:52:23.000000 schem-0.9.6/schem/game.py
--rw-rw-rw-   0        0        0     2903 2021-02-14 01:54:46.000000 schem-0.9.6/schem/grid.py
--rw-rw-rw-   0        0        0     5317 2021-03-22 04:50:02.000000 schem-0.9.6/schem/level.py
--rw-rw-rw-   0        0        0   145348 2021-03-22 04:50:02.000000 schem-0.9.6/schem/levels.py
--rw-rw-rw-   0        0        0    23810 2021-03-22 04:50:02.000000 schem-0.9.6/schem/molecule.py
--rw-rw-rw-   0        0        0     3563 2021-02-14 21:36:45.000000 schem-0.9.6/schem/schem_random.py
--rw-rw-rw-   0        0        0    42576 2021-04-25 21:26:46.000000 schem-0.9.6/schem/solution.py
--rw-rw-rw-   0        0        0    17253 2021-04-17 01:09:24.000000 schem-0.9.6/schem/terrains.py
--rw-rw-rw-   0        0        0    11034 2021-03-22 04:50:02.000000 schem-0.9.6/schem/waldo.py
-drwxrwxrwx   0        0        0        0 2021-04-25 21:30:17.222981 schem-0.9.6/schem.egg-info/
--rw-rw-rw-   0        0        0     1130 2021-04-25 21:30:17.000000 schem-0.9.6/schem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2021-04-25 21:30:17.000000 schem-0.9.6/schem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-25 21:30:17.000000 schem-0.9.6/schem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2021-04-25 21:30:17.000000 schem-0.9.6/schem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-04-25 21:30:17.000000 schem-0.9.6/schem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      670 2021-04-25 21:30:17.223325 schem-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2021-07-19 02:54:24.046886 schem-0.9.7/
+-rw-rw-rw-   0        0        0     1319 2021-02-13 19:18:31.000000 schem-0.9.7/LICENSE
+-rw-rw-rw-   0        0        0      992 2021-07-19 02:54:24.046886 schem-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2021-03-22 04:50:02.000000 schem-0.9.7/README.md
+-rw-rw-rw-   0        0        0      110 2021-02-15 03:12:01.000000 schem-0.9.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2021-07-19 02:54:24.033969 schem-0.9.7/schem/
+-rw-rw-rw-   0        0        0      476 2021-03-22 04:50:02.000000 schem-0.9.7/schem/__init__.py
+-rw-rw-rw-   0        0        0     4317 2021-04-19 00:52:01.000000 schem-0.9.7/schem/__main__.py
+-rw-rw-rw-   0        0        0    86343 2021-07-19 02:35:06.000000 schem-0.9.7/schem/components.py
+-rw-rw-rw-   0        0        0     5111 2021-03-22 04:50:02.000000 schem-0.9.7/schem/elements.py
+-rw-rw-rw-   0        0        0      395 2021-03-22 04:50:02.000000 schem-0.9.7/schem/exceptions.py
+-rw-rw-rw-   0        0        0     4841 2021-04-19 00:52:23.000000 schem-0.9.7/schem/game.py
+-rw-rw-rw-   0        0        0     2903 2021-02-14 01:54:46.000000 schem-0.9.7/schem/grid.py
+-rw-rw-rw-   0        0        0     5317 2021-03-22 04:50:02.000000 schem-0.9.7/schem/level.py
+-rw-rw-rw-   0        0        0   145348 2021-03-22 04:50:02.000000 schem-0.9.7/schem/levels.py
+-rw-rw-rw-   0        0        0    24495 2021-07-19 02:15:17.000000 schem-0.9.7/schem/molecule.py
+-rw-rw-rw-   0        0        0     3563 2021-02-14 21:36:45.000000 schem-0.9.7/schem/schem_random.py
+-rw-rw-rw-   0        0        0    42576 2021-04-25 21:26:46.000000 schem-0.9.7/schem/solution.py
+-rw-rw-rw-   0        0        0    17253 2021-04-17 01:09:24.000000 schem-0.9.7/schem/terrains.py
+-rw-rw-rw-   0        0        0    11034 2021-03-22 04:50:02.000000 schem-0.9.7/schem/waldo.py
+drwxrwxrwx   0        0        0        0 2021-07-19 02:54:24.045888 schem-0.9.7/schem.egg-info/
+-rw-rw-rw-   0        0        0      992 2021-07-19 02:54:23.000000 schem-0.9.7/schem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2021-07-19 02:54:23.000000 schem-0.9.7/schem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-19 02:54:23.000000 schem-0.9.7/schem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2021-07-19 02:54:23.000000 schem-0.9.7/schem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-07-19 02:54:23.000000 schem-0.9.7/schem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      670 2021-07-19 02:54:24.048880 schem-0.9.7/setup.cfg
```

### Comparing `schem-0.9.6/LICENSE` & `schem-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/__main__.py` & `schem-0.9.7/schem/__main__.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/components.py` & `schem-0.9.7/schem/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1488,18 +1488,18 @@
 
             # If the bond being increased is already at the max bond size of 3, don't do
             # anything. However, due to weirdness of Spacechem's bonding algorithm, we still
             # mark the molecule as modified below
             if direction not in atom_A.bonds or atom_A.bonds[direction] != 3:
                 atom_B = molecule_B[neighbor_posn]
 
-                # Do nothing if either atom is at its bond limit (spacechem does not mark
-                # any molecules as modified in this case unless the bond was size 3)
-                if (sum(atom_A.bonds.values()) == atom_A.element.max_bonds
-                        or sum(atom_B.bonds.values()) == atom_B.element.max_bonds):
+                # Do nothing if either atom is at (or above) its bond limit (spacechem does not mark any molecules as
+                # modified in this case unless the bond was size 3)
+                if (sum(atom_A.bonds.values()) >= atom_A.element.max_bonds
+                        or sum(atom_B.bonds.values()) >= atom_B.element.max_bonds):
                     continue
 
                 direction_B = direction.opposite()
 
                 if direction not in atom_A.bonds:
                     atom_A.bonds[direction] = 0
                 atom_A.bonds[direction] += 1
```

### Comparing `schem-0.9.6/schem/elements.py` & `schem-0.9.7/schem/elements.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/game.py` & `schem-0.9.7/schem/game.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/grid.py` & `schem-0.9.7/schem/grid.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/level.py` & `schem-0.9.7/schem/level.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/levels.py` & `schem-0.9.7/schem/levels.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/molecule.py` & `schem-0.9.7/schem/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -441,16 +441,26 @@
                                       their_visited_posns: dict, their_posn: Position):
             '''Attempt to recursively map any unvisited atoms of the molecules onto each other
             starting from the given position in each.
 
             If unsuccessful, revert any changes made to the given visit dicts, and return 0.
             If successful, return the number of items added to each dict.
             '''
+            # Make sure the two atoms have the same element / bond counts
             if this_posn_to_atom_struct[our_posn] != other_posn_to_atom_struct[their_posn]:
-                return False
+                return 0
+
+            # Make sure the two atoms have the same number of unvisited neighbors. This avoids issues if all of A's
+            # neighbors get matched but unmatched neighbors of B remain, which shouldn't count as a successful match
+            # even if they have the same atom structures
+            if (sum(1 for _, our_neighbor in self.neighbor_bonds(our_posn)
+                    if our_neighbor not in our_visited_posns)
+                    != sum(1 for _, their_neighbor in other.neighbor_bonds(their_posn)
+                           if their_neighbor not in their_visited_posns)):
+                return 0
 
             # Mark the current nodes as visited (storing a dummy None; we'd use set() but we need ordering and popitem())
             total_visits = 1
             our_visited_posns[our_posn] = None
             their_visited_posns[their_posn] = None
 
             # Attempt to recursively match each of our bonded neighbors in turn (comparing against all possible
```

### Comparing `schem-0.9.6/schem/schem_random.py` & `schem-0.9.7/schem/schem_random.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/solution.py` & `schem-0.9.7/schem/solution.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/terrains.py` & `schem-0.9.7/schem/terrains.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/schem/waldo.py` & `schem-0.9.7/schem/waldo.py`

 * *Files identical despite different names*

### Comparing `schem-0.9.6/setup.cfg` & `schem-0.9.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6368 656d 0d0a 7665 7273 696f   = schem..versio
-00000020: 6e20 3d20 302e 392e 360d 0a61 7574 686f  n = 0.9.6..autho
+00000020: 6e20 3d20 302e 392e 370d 0a61 7574 686f  n = 0.9.7..autho
 00000030: 7220 3d20 5a69 670d 0a61 7574 686f 725f  r = Zig..author_
 00000040: 656d 6169 6c20 3d20 6a75 6e6b 6e65 6e6f  email = junkneno
 00000050: 706f 6b40 676d 6169 6c2e 636f 6d0d 0a64  pok@gmail.com..d
 00000060: 6573 6372 6970 7469 6f6e 203d 2043 6c65  escription = Cle
 00000070: 616e 2052 6f6f 6d20 696d 706c 656d 656e  an Room implemen
 00000080: 7461 7469 6f6e 206f 6620 7468 6520 6261  tation of the ba
 00000090: 636b 656e 6420 6f66 2053 7061 6365 4368  ckend of SpaceCh
```

