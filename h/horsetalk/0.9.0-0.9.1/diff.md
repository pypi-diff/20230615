# Comparing `tmp/horsetalk-0.9.0.tar.gz` & `tmp/horsetalk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.9.0.tar", max compression
+gzip compressed data, was "horsetalk-0.9.1.tar", max compression
```

## Comparing `horsetalk-0.9.0.tar` & `horsetalk-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1591 2023-05-24 23:29:51.698275 horsetalk-0.9.0/horsetalk/__init__.py
--rw-r--r--   0        0        0      244 2023-04-13 18:30:57.122742 horsetalk-0.9.0/horsetalk/age_category.py
--rw-r--r--   0        0        0      443 2023-05-08 22:18:34.194898 horsetalk-0.9.0/horsetalk/aw_going_description.py
--rw-r--r--   0        0        0      289 2023-04-13 18:30:57.122742 horsetalk-0.9.0/horsetalk/breed.py
--rw-r--r--   0        0        0      514 2023-04-13 16:41:40.705711 horsetalk-0.9.0/horsetalk/coat_colour.py
--rw-r--r--   0        0        0      302 2023-05-08 22:18:34.194898 horsetalk-0.9.0/horsetalk/dirt_going_description.py
--rw-r--r--   0        0        0     1187 2023-04-13 18:30:57.123742 horsetalk-0.9.0/horsetalk/disaster.py
--rw-r--r--   0        0        0      378 2023-04-13 18:30:57.123742 horsetalk-0.9.0/horsetalk/finishing_position.py
--rw-r--r--   0        0        0      223 2023-04-13 18:30:57.124742 horsetalk-0.9.0/horsetalk/form_break.py
--rw-r--r--   0        0        0     1426 2023-04-13 18:30:57.124742 horsetalk-0.9.0/horsetalk/form_figures.py
--rw-r--r--   0        0        0     2566 2023-04-13 18:30:57.124742 horsetalk-0.9.0/horsetalk/gender.py
--rw-r--r--   0        0        0      219 2023-05-08 22:18:34.195971 horsetalk-0.9.0/horsetalk/going_description.py
--rw-r--r--   0        0        0      544 2023-04-13 18:30:57.125741 horsetalk-0.9.0/horsetalk/headgear.py
--rw-r--r--   0        0        0     4549 2023-04-13 18:30:57.125741 horsetalk-0.9.0/horsetalk/horse_age.py
--rw-r--r--   0        0        0      291 2023-04-13 18:30:57.125741 horsetalk-0.9.0/horsetalk/horse_experience_level.py
--rw-r--r--   0        0        0     1148 2023-04-13 18:30:57.125741 horsetalk-0.9.0/horsetalk/horse_height.py
--rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.9.0/horsetalk/horselength.py
--rw-r--r--   0        0        0      390 2023-04-13 18:30:57.127246 horsetalk-0.9.0/horsetalk/jockey_experience_level.py
--rw-r--r--   0        0        0      490 2023-05-08 20:55:40.939618 horsetalk-0.9.0/horsetalk/jump_category.py
--rw-r--r--   0        0        0      362 2023-05-08 20:55:40.940617 horsetalk-0.9.0/horsetalk/obstacle_style.py
--rw-r--r--   0        0        0      529 2023-04-13 16:39:41.041691 horsetalk-0.9.0/horsetalk/parsing_enum.py
--rw-r--r--   0        0        0      420 2023-04-13 18:30:57.128251 horsetalk-0.9.0/horsetalk/race_designation.py
--rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.9.0/horsetalk/race_distance.py
--rw-r--r--   0        0        0     2735 2023-05-08 20:55:40.941616 horsetalk-0.9.0/horsetalk/race_title.py
--rw-r--r--   0        0        0      372 2023-04-13 18:30:57.128251 horsetalk-0.9.0/horsetalk/racing_code.py
--rw-r--r--   0        0        0      258 2023-04-13 18:30:57.129251 horsetalk-0.9.0/horsetalk/sex.py
--rw-r--r--   0        0        0    10594 2023-05-24 23:29:53.681869 horsetalk-0.9.0/horsetalk/silks.py
--rw-r--r--   0        0        0      342 2023-05-21 17:59:50.962571 horsetalk-0.9.0/horsetalk/surface.py
--rw-r--r--   0        0        0      845 2023-05-08 22:18:34.196964 horsetalk-0.9.0/horsetalk/turf_going_description.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.9.0/LICENSE
--rw-r--r--   0        0        0      741 2023-05-25 21:18:18.182983 horsetalk-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.9.0/README.md
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1591 2023-06-14 22:41:03.667137 horsetalk-0.9.1/horsetalk/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-13 18:30:57.122742 horsetalk-0.9.1/horsetalk/age_category.py
+-rw-r--r--   0        0        0      443 2023-05-08 22:18:34.194898 horsetalk-0.9.1/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      289 2023-04-13 18:30:57.122742 horsetalk-0.9.1/horsetalk/breed.py
+-rw-r--r--   0        0        0      514 2023-04-13 16:41:40.705711 horsetalk-0.9.1/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      302 2023-05-08 22:18:34.194898 horsetalk-0.9.1/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0     1187 2023-04-13 18:30:57.123742 horsetalk-0.9.1/horsetalk/disaster.py
+-rw-r--r--   0        0        0      378 2023-04-13 18:30:57.123742 horsetalk-0.9.1/horsetalk/finishing_position.py
+-rw-r--r--   0        0        0      223 2023-04-13 18:30:57.124742 horsetalk-0.9.1/horsetalk/form_break.py
+-rw-r--r--   0        0        0     1426 2023-04-13 18:30:57.124742 horsetalk-0.9.1/horsetalk/form_figures.py
+-rw-r--r--   0        0        0     2566 2023-04-13 18:30:57.124742 horsetalk-0.9.1/horsetalk/gender.py
+-rw-r--r--   0        0        0      219 2023-05-08 22:18:34.195971 horsetalk-0.9.1/horsetalk/going_description.py
+-rw-r--r--   0        0        0      544 2023-04-13 18:30:57.125741 horsetalk-0.9.1/horsetalk/headgear.py
+-rw-r--r--   0        0        0     4549 2023-04-13 18:30:57.125741 horsetalk-0.9.1/horsetalk/horse_age.py
+-rw-r--r--   0        0        0      291 2023-04-13 18:30:57.125741 horsetalk-0.9.1/horsetalk/horse_experience_level.py
+-rw-r--r--   0        0        0     1148 2023-04-13 18:30:57.125741 horsetalk-0.9.1/horsetalk/horse_height.py
+-rw-r--r--   0        0        0     3780 2023-04-08 20:26:53.419404 horsetalk-0.9.1/horsetalk/horselength.py
+-rw-r--r--   0        0        0      390 2023-04-13 18:30:57.127246 horsetalk-0.9.1/horsetalk/jockey_experience_level.py
+-rw-r--r--   0        0        0      490 2023-05-08 20:55:40.939618 horsetalk-0.9.1/horsetalk/jump_category.py
+-rw-r--r--   0        0        0      362 2023-05-08 20:55:40.940617 horsetalk-0.9.1/horsetalk/obstacle_style.py
+-rw-r--r--   0        0        0      529 2023-04-13 16:39:41.041691 horsetalk-0.9.1/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      420 2023-04-13 18:30:57.128251 horsetalk-0.9.1/horsetalk/race_designation.py
+-rw-r--r--   0        0        0     1345 2023-04-08 20:26:53.420403 horsetalk-0.9.1/horsetalk/race_distance.py
+-rw-r--r--   0        0        0     2735 2023-05-08 20:55:40.941616 horsetalk-0.9.1/horsetalk/race_title.py
+-rw-r--r--   0        0        0      372 2023-04-13 18:30:57.128251 horsetalk-0.9.1/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      258 2023-04-13 18:30:57.129251 horsetalk-0.9.1/horsetalk/sex.py
+-rw-r--r--   0        0        0    10721 2023-06-14 23:03:02.339555 horsetalk-0.9.1/horsetalk/silks.py
+-rw-r--r--   0        0        0      342 2023-05-21 17:59:50.962571 horsetalk-0.9.1/horsetalk/surface.py
+-rw-r--r--   0        0        0      845 2023-05-08 22:18:34.196964 horsetalk-0.9.1/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.9.1/LICENSE
+-rw-r--r--   0        0        0      741 2023-06-14 22:41:16.147175 horsetalk-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.9.1/README.md
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 horsetalk-0.9.1/PKG-INFO
```

### Comparing `horsetalk-0.9.0/horsetalk/__init__.py` & `horsetalk-0.9.1/horsetalk/__init__.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/coat_colour.py` & `horsetalk-0.9.1/horsetalk/coat_colour.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/disaster.py` & `horsetalk-0.9.1/horsetalk/disaster.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/form_figures.py` & `horsetalk-0.9.1/horsetalk/form_figures.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/gender.py` & `horsetalk-0.9.1/horsetalk/gender.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/headgear.py` & `horsetalk-0.9.1/horsetalk/headgear.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/horse_age.py` & `horsetalk-0.9.1/horsetalk/horse_age.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/horse_height.py` & `horsetalk-0.9.1/horsetalk/horse_height.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/horselength.py` & `horsetalk-0.9.1/horsetalk/horselength.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/parsing_enum.py` & `horsetalk-0.9.1/horsetalk/parsing_enum.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/race_distance.py` & `horsetalk-0.9.1/horsetalk/race_distance.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/race_title.py` & `horsetalk-0.9.1/horsetalk/race_title.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/horsetalk/silks.py` & `horsetalk-0.9.1/horsetalk/silks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Callable
+from typing import Callable, Optional
 from horsetalk.parsing_enum import ParsingEnum
 
 
 class Silks:
+    description: str
+
     class Colour(ParsingEnum):
         """An enumeration of colours that can appear on jockey silks."""
 
         BEIGE = 1
         BLACK = 2
         BROWN = 3
         DARK_BLUE = 4
@@ -101,16 +103,16 @@
                 cls.TRIPLE_DIAMOND,
             ]
 
     class Element:
         def __init__(
             self,
             primary: "Silks.Colour",
-            secondary: "Silks.Colour" = None,
-            pattern: "Silks.Shape" = None,
+            secondary: Optional["Silks.Colour"] = None,
+            pattern: Optional["Silks.Pattern"] = None,
         ):
             self.primary = primary
             self.secondary = secondary
             self.pattern = pattern
 
         def __repr__(self):
             return f"Element(primary={self.primary}, secondary={self.secondary}, pattern={self.pattern})"
@@ -184,15 +186,15 @@
             or "armlets" in self.description
             or "armlet" in self.description
             else []
         )
         return self._apply_defaults(element)
 
     @property
-    def _clauses(self) -> list[str]:
+    def _clauses(self) -> list[list[str]]:
         clauses = [
             Silks._conjoin_words(clause.split(" "))
             for clause in self.description.lower()
             .replace("(", "")
             .replace(")", "")
             .replace(" on ", " ")
             .split(", ")
@@ -229,15 +231,15 @@
                 to_add[i + 1] = new_clause
 
         for key in to_add:
             clauses.insert(key, to_add[key])
 
         return clauses
 
-    def _parts_for_element(self, element_selector: Callable) -> str:
+    def _parts_for_element(self, element_selector: Callable) -> list[str]:
         main_clause = element_selector(self._clauses)
         index = self._clauses.index(main_clause)
         next_clause = (
             self._clauses[index + 1]
             if index + 1 != len(self._clauses)
             and not (
                 "cap" in self._clauses[index + 1]
@@ -267,15 +269,15 @@
             if element.primary
             or self.body.pattern in Silks.Pattern.body_only()
             or ", sleeves and cap" in self.description
             else self.body.pattern
         )
         default_primary = (
             self.body.secondary
-            if ", sleeves and cap" in self.description
+            if ", sleeves and cap" in self.description and self.body.secondary
             else self.body.primary
         )
 
         element.secondary = element.secondary or element.primary or default_secondary
         element.pattern = element.pattern or default_pattern
 
         uses_solid_pattern = element.pattern not in [
@@ -315,16 +317,17 @@
             key=lambda x: (
                 isinstance(x, Silks.Pattern),
                 x is None,
                 isinstance(x, Silks.Colour),
             )
         )
 
-        return Silks.Element(*details)
+        return Silks.Element(*details)  # type: ignore
 
+    @staticmethod
     def _conjoin_words(words: list[str]) -> list[str]:
         FIRST_WORDS = [
             "dark",
             "light",
             "royal",
             "emerald",
             "cross",
```

### Comparing `horsetalk-0.9.0/horsetalk/turf_going_description.py` & `horsetalk-0.9.1/horsetalk/turf_going_description.py`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/LICENSE` & `horsetalk-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.9.0/pyproject.toml` & `horsetalk-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.9.0"
+version = "0.9.1"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -18,15 +18,15 @@
 coverage = "^7.2.2"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
-ruff = ">=0.0.261,<0.0.270"
+ruff = ">=0.0.261,<0.0.273"
 
 [tool.ruff]
 ignore = ["E501", "E741", "F821"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `horsetalk-0.9.0/PKG-INFO` & `horsetalk-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

