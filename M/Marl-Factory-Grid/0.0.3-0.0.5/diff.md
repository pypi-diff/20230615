# Comparing `tmp/Marl_Factory_Grid-0.0.3-py3-none-any.whl.zip` & `tmp/Marl_Factory_Grid-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 97653 bytes, number of entries: 114
+Zip file size: 209118 bytes, number of entries: 135
 -rw-rw-rw-  2.0 fat       78 b- defN 21-Sep-14 08:50 algorithms/__init__.py
 -rw-rw-rw-  2.0 fat     2763 b- defN 23-May-11 14:32 algorithms/utils.py
 -rw-rw-rw-  2.0 fat      294 b- defN 22-Apr-11 14:15 algorithms/marl/__init__.py
 -rw-rw-rw-  2.0 fat     8879 b- defN 23-May-30 10:30 algorithms/marl/base_ac.py
 -rw-rw-rw-  2.0 fat     2127 b- defN 23-May-16 14:53 algorithms/marl/iac.py
 -rw-rw-rw-  2.0 fat     3212 b- defN 23-May-16 14:53 algorithms/marl/mappo.py
 -rw-rw-rw-  2.0 fat     7984 b- defN 23-May-16 14:53 algorithms/marl/memory.py
@@ -14,18 +14,27 @@
 -rw-rw-rw-  2.0 fat     2410 b- defN 23-Jun-06 07:24 algorithms/static/TSP_item_agent.py
 -rw-rw-rw-  2.0 fat     1093 b- defN 23-Jun-06 07:24 algorithms/static/TSP_target_agent.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 09:50 algorithms/static/__init__.py
 -rw-rw-rw-  2.0 fat      388 b- defN 23-May-26 10:16 algorithms/static/random_agent.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 11:49 environment/__init__.py
 -rw-rw-rw-  2.0 fat     2727 b- defN 23-May-19 13:29 environment/actions.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 23-Jun-05 14:26 environment/constants.py
--rw-rw-rw-  2.0 fat     7086 b- defN 23-Jun-06 14:03 environment/factory.py
+-rw-rw-rw-  2.0 fat     7082 b- defN 23-Jun-15 13:56 environment/factory.py
 -rw-rw-rw-  2.0 fat      128 b- defN 23-May-11 15:13 environment/rewards.py
 -rw-rw-rw-  2.0 fat     2648 b- defN 23-Jun-06 06:18 environment/rules.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-14 08:51 environment/assets/__init__.py
+-rw-rw-rw-  2.0 fat     1415 b- defN 21-May-18 10:41 environment/assets/wall.png
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 14:31 environment/assets/agent/__init__.py
+-rw-rw-rw-  2.0 fat     8521 b- defN 21-May-19 14:52 environment/assets/agent/adversary.png
+-rw-rw-rw-  2.0 fat     3402 b- defN 21-May-18 12:44 environment/assets/agent/agent.png
+-rw-rw-rw-  2.0 fat    18857 b- defN 21-May-18 15:32 environment/assets/agent/agent_collision.png
+-rw-rw-rw-  2.0 fat     1631 b- defN 21-Jun-09 11:54 environment/assets/agent/idle.png
+-rw-rw-rw-  2.0 fat     1599 b- defN 21-Jun-09 11:54 environment/assets/agent/invalid.png
+-rw-rw-rw-  2.0 fat     5933 b- defN 21-Aug-31 13:57 environment/assets/agent/move.png
+-rw-rw-rw-  2.0 fat     5717 b- defN 21-Aug-31 13:57 environment/assets/agent/valid.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 13:43 environment/entity/__init__.py
 -rw-rw-rw-  2.0 fat     2378 b- defN 23-Jun-06 14:03 environment/entity/agent.py
 -rw-rw-rw-  2.0 fat     2204 b- defN 23-Jun-09 08:25 environment/entity/entity.py
 -rw-rw-rw-  2.0 fat      418 b- defN 23-Jun-02 10:48 environment/entity/mixin.py
 -rw-rw-rw-  2.0 fat     3457 b- defN 23-Jun-09 10:23 environment/entity/object.py
 -rw-rw-rw-  2.0 fat     1249 b- defN 23-Jun-02 13:55 environment/entity/util.py
 -rw-rw-rw-  2.0 fat     3206 b- defN 23-Jun-09 08:02 environment/entity/wall_floor.py
@@ -38,17 +47,17 @@
 -rw-rw-rw-  2.0 fat     2415 b- defN 23-Jun-05 14:46 environment/groups/utils.py
 -rw-rw-rw-  2.0 fat     1590 b- defN 23-Jun-05 14:34 environment/groups/wall_n_floors.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-May-19 12:48 environment/logging/__init__.py
 -rw-rw-rw-  2.0 fat     2266 b- defN 23-Jun-06 06:44 environment/logging/envmonitor.py
 -rw-rw-rw-  2.0 fat     5627 b- defN 23-Jun-05 15:20 environment/logging/recorder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-14 08:51 environment/utils/__init__.py
 -rw-rw-rw-  2.0 fat     5281 b- defN 23-Jun-13 12:16 environment/utils/config_parser.py
--rw-rw-rw-  2.0 fat    10791 b- defN 23-Jun-12 21:04 environment/utils/helpers.py
+-rw-rw-rw-  2.0 fat    10978 b- defN 23-Jun-13 13:31 environment/utils/helpers.py
 -rw-rw-rw-  2.0 fat     2255 b- defN 23-Jun-05 13:58 environment/utils/level_parser.py
--rw-rw-rw-  2.0 fat    12714 b- defN 23-Jun-09 11:27 environment/utils/observation_builder.py
+-rw-rw-rw-  2.0 fat    12774 b- defN 23-Jun-15 15:38 environment/utils/observation_builder.py
 -rw-rw-rw-  2.0 fat      299 b- defN 23-Jun-06 14:03 environment/utils/render.py
 -rw-rw-rw-  2.0 fat     5903 b- defN 23-Jun-12 21:40 environment/utils/renderer.py
 -rw-rw-rw-  2.0 fat     1152 b- defN 23-Jun-06 09:33 environment/utils/results.py
 -rw-rw-rw-  2.0 fat     3677 b- defN 23-Jun-06 06:18 environment/utils/states.py
 -rw-rw-rw-  2.0 fat      838 b- defN 23-Jun-05 15:11 environment/utils/utility_classes.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 11:00 modules/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 07:08 modules/_template/__init__.py
@@ -60,42 +69,54 @@
 -rw-rw-rw-  2.0 fat     2405 b- defN 23-Jun-06 14:03 modules/batteries/entitites.py
 -rw-rw-rw-  2.0 fat     1055 b- defN 23-Jun-06 07:24 modules/batteries/groups.py
 -rw-rw-rw-  2.0 fat       86 b- defN 23-May-11 15:27 modules/batteries/rewards.py
 -rw-rw-rw-  2.0 fat     2136 b- defN 23-Jun-06 07:24 modules/batteries/rules.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 07:06 modules/clean_up/__init__.py
 -rw-rw-rw-  2.0 fat     1295 b- defN 23-Jun-06 07:24 modules/clean_up/actions.py
 -rw-rw-rw-  2.0 fat      157 b- defN 23-May-19 12:27 modules/clean_up/constants.py
+-rw-rw-rw-  2.0 fat    39296 b- defN 21-May-18 14:50 modules/clean_up/dirtpiles.png
 -rw-rw-rw-  2.0 fat     1173 b- defN 23-Jun-06 14:03 modules/clean_up/entitites.py
 -rw-rw-rw-  2.0 fat     2585 b- defN 23-Jun-06 13:08 modules/clean_up/groups.py
 -rw-rw-rw-  2.0 fat       85 b- defN 23-May-11 15:13 modules/clean_up/rewards.py
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 07:24 modules/clean_up/rule_done_on_all_clean.py
 -rw-rw-rw-  2.0 fat      953 b- defN 23-Jun-06 07:24 modules/clean_up/rule_respawn.py
 -rw-rw-rw-  2.0 fat     1030 b- defN 23-Jun-06 07:24 modules/clean_up/rule_smear_on_move.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 07:05 modules/destinations/__init__.py
 -rw-rw-rw-  2.0 fat      911 b- defN 23-Jun-06 07:24 modules/destinations/actions.py
 -rw-rw-rw-  2.0 fat      328 b- defN 23-May-25 14:42 modules/destinations/constants.py
+-rw-rw-rw-  2.0 fat     7037 b- defN 22-Jan-11 12:50 modules/destinations/destinations.png
 -rw-rw-rw-  2.0 fat     1786 b- defN 23-Jun-06 14:03 modules/destinations/entitites.py
 -rw-rw-rw-  2.0 fat      808 b- defN 23-Jun-06 07:24 modules/destinations/groups.py
 -rw-rw-rw-  2.0 fat       75 b- defN 23-May-11 15:31 modules/destinations/rewards.py
 -rw-rw-rw-  2.0 fat     3739 b- defN 23-Jun-06 09:38 modules/destinations/rules.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 07:07 modules/doors/__init__.py
 -rw-rw-rw-  2.0 fat     1132 b- defN 23-Jun-06 07:24 modules/doors/actions.py
 -rw-rw-rw-  2.0 fat      811 b- defN 23-Jun-05 13:03 modules/doors/constants.py
+-rw-rw-rw-  2.0 fat      699 b- defN 21-Jul-27 15:28 modules/doors/door_closed.png
+-rw-rw-rw-  2.0 fat     4224 b- defN 21-Jul-27 15:33 modules/doors/door_open.png
 -rw-rw-rw-  2.0 fat     2777 b- defN 23-Jun-06 14:03 modules/doors/entitites.py
 -rw-rw-rw-  2.0 fat      880 b- defN 23-Jun-06 07:24 modules/doors/groups.py
 -rw-rw-rw-  2.0 fat       59 b- defN 23-May-11 15:15 modules/doors/rewards.py
 -rw-rw-rw-  2.0 fat      861 b- defN 23-Jun-06 09:41 modules/doors/rule_door_auto_close.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 06:45 modules/items/__init__.py
 -rw-rw-rw-  2.0 fat     1658 b- defN 23-Jun-06 07:24 modules/items/actions.py
 -rw-rw-rw-  2.0 fat      245 b- defN 23-May-26 06:51 modules/items/constants.py
 -rw-rw-rw-  2.0 fat     2078 b- defN 23-Jun-06 14:03 modules/items/entitites.py
 -rw-rw-rw-  2.0 fat     3166 b- defN 23-Jun-06 08:28 modules/items/groups.py
 -rw-rw-rw-  2.0 fat      112 b- defN 23-May-11 16:28 modules/items/rewards.py
 -rw-rw-rw-  2.0 fat     3154 b- defN 23-Jun-06 09:29 modules/items/rules.py
+-rw-rw-rw-  2.0 fat     6610 b- defN 22-Jan-11 12:50 modules/items/assets/charge_pod.png
+-rw-rw-rw-  2.0 fat     2318 b- defN 21-Aug-16 12:39 modules/items/assets/dropofflocations.png
+-rw-rw-rw-  2.0 fat     3102 b- defN 21-Aug-16 12:40 modules/items/assets/items.png
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-14 08:51 modules/levels/__init__.py
+-rw-rw-rw-  2.0 fat     1534 b- defN 23-Jun-06 09:00 modules/levels/large.txt
+-rw-rw-rw-  2.0 fat     5873 b- defN 23-Jun-06 09:04 modules/levels/large_qquad.txt
+-rw-rw-rw-  2.0 fat      219 b- defN 21-Jun-17 12:48 modules/levels/rooms.txt
+-rw-rw-rw-  2.0 fat      180 b- defN 21-Nov-11 17:42 modules/levels/shelves.txt
+-rw-rw-rw-  2.0 fat      166 b- defN 21-May-18 10:41 modules/levels/simple.txt
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 07:06 modules/machines/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-Jun-02 13:55 modules/machines/constants.py
 -rw-rw-rw-  2.0 fat     1885 b- defN 23-Jun-06 14:03 modules/machines/entitites.py
 -rw-rw-rw-  2.0 fat      398 b- defN 23-Jun-06 07:24 modules/machines/groups.py
 -rw-rw-rw-  2.0 fat      117 b- defN 23-Jun-02 14:02 modules/machines/rewards.py
 -rw-rw-rw-  2.0 fat      883 b- defN 23-Jun-06 07:24 modules/machines/rules.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-14 08:51 plotting/__init__.py
@@ -105,12 +126,12 @@
 -rw-rw-rw-  2.0 fat    24447 b- defN 23-May-16 14:53 studies/e_1.py
 -rw-rw-rw-  2.0 fat    10359 b- defN 23-May-16 14:53 studies/e_1_mix.py
 -rw-rw-rw-  2.0 fat      809 b- defN 22-Apr-11 14:15 studies/normalization_study.py
 -rw-rw-rw-  2.0 fat      729 b- defN 22-Apr-11 14:15 studies/playground_file.py
 -rw-rw-rw-  2.0 fat    12666 b- defN 23-May-16 14:53 studies/single_run_with_export.py
 -rw-rw-rw-  2.0 fat     7604 b- defN 23-May-16 14:53 studies/test.py
 -rw-rw-rw-  2.0 fat     1330 b- defN 22-Apr-11 14:15 studies/viz_policy.py
--rw-rw-rw-  2.0 fat     3126 b- defN 23-Jun-13 12:18 Marl_Factory_Grid-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 12:18 Marl_Factory_Grid-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-13 12:18 Marl_Factory_Grid-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     9561 b- defN 23-Jun-13 12:18 Marl_Factory_Grid-0.0.3.dist-info/RECORD
-114 files, 265152 bytes uncompressed, 82551 bytes compressed:  68.9%
+-rw-rw-rw-  2.0 fat     3147 b- defN 23-Jun-15 16:18 Marl_Factory_Grid-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 16:18 Marl_Factory_Grid-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-15 16:18 Marl_Factory_Grid-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    11426 b- defN 23-Jun-15 16:18 Marl_Factory_Grid-0.0.5.dist-info/RECORD
+135 files, 385614 bytes uncompressed, 191074 bytes compressed:  50.4%
```

## zipnote {}

```diff
@@ -63,14 +63,41 @@
 
 Filename: environment/rules.py
 Comment: 
 
 Filename: environment/assets/__init__.py
 Comment: 
 
+Filename: environment/assets/wall.png
+Comment: 
+
+Filename: environment/assets/agent/__init__.py
+Comment: 
+
+Filename: environment/assets/agent/adversary.png
+Comment: 
+
+Filename: environment/assets/agent/agent.png
+Comment: 
+
+Filename: environment/assets/agent/agent_collision.png
+Comment: 
+
+Filename: environment/assets/agent/idle.png
+Comment: 
+
+Filename: environment/assets/agent/invalid.png
+Comment: 
+
+Filename: environment/assets/agent/move.png
+Comment: 
+
+Filename: environment/assets/agent/valid.png
+Comment: 
+
 Filename: environment/entity/__init__.py
 Comment: 
 
 Filename: environment/entity/agent.py
 Comment: 
 
 Filename: environment/entity/entity.py
@@ -189,14 +216,17 @@
 
 Filename: modules/clean_up/actions.py
 Comment: 
 
 Filename: modules/clean_up/constants.py
 Comment: 
 
+Filename: modules/clean_up/dirtpiles.png
+Comment: 
+
 Filename: modules/clean_up/entitites.py
 Comment: 
 
 Filename: modules/clean_up/groups.py
 Comment: 
 
 Filename: modules/clean_up/rewards.py
@@ -216,14 +246,17 @@
 
 Filename: modules/destinations/actions.py
 Comment: 
 
 Filename: modules/destinations/constants.py
 Comment: 
 
+Filename: modules/destinations/destinations.png
+Comment: 
+
 Filename: modules/destinations/entitites.py
 Comment: 
 
 Filename: modules/destinations/groups.py
 Comment: 
 
 Filename: modules/destinations/rewards.py
@@ -237,14 +270,20 @@
 
 Filename: modules/doors/actions.py
 Comment: 
 
 Filename: modules/doors/constants.py
 Comment: 
 
+Filename: modules/doors/door_closed.png
+Comment: 
+
+Filename: modules/doors/door_open.png
+Comment: 
+
 Filename: modules/doors/entitites.py
 Comment: 
 
 Filename: modules/doors/groups.py
 Comment: 
 
 Filename: modules/doors/rewards.py
@@ -270,17 +309,41 @@
 
 Filename: modules/items/rewards.py
 Comment: 
 
 Filename: modules/items/rules.py
 Comment: 
 
+Filename: modules/items/assets/charge_pod.png
+Comment: 
+
+Filename: modules/items/assets/dropofflocations.png
+Comment: 
+
+Filename: modules/items/assets/items.png
+Comment: 
+
 Filename: modules/levels/__init__.py
 Comment: 
 
+Filename: modules/levels/large.txt
+Comment: 
+
+Filename: modules/levels/large_qquad.txt
+Comment: 
+
+Filename: modules/levels/rooms.txt
+Comment: 
+
+Filename: modules/levels/shelves.txt
+Comment: 
+
+Filename: modules/levels/simple.txt
+Comment: 
+
 Filename: modules/machines/__init__.py
 Comment: 
 
 Filename: modules/machines/constants.py
 Comment: 
 
 Filename: modules/machines/entitites.py
@@ -324,20 +387,20 @@
 
 Filename: studies/test.py
 Comment: 
 
 Filename: studies/viz_policy.py
 Comment: 
 
-Filename: Marl_Factory_Grid-0.0.3.dist-info/METADATA
+Filename: Marl_Factory_Grid-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: Marl_Factory_Grid-0.0.3.dist-info/WHEEL
+Filename: Marl_Factory_Grid-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: Marl_Factory_Grid-0.0.3.dist-info/top_level.txt
+Filename: Marl_Factory_Grid-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: Marl_Factory_Grid-0.0.3.dist-info/RECORD
+Filename: Marl_Factory_Grid-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## environment/factory.py

```diff
@@ -53,15 +53,15 @@
         self.close()
 
     def __init__(self, config_file: Union[str, PathLike]):
         self._config_file = config_file
         self.conf = FactoryConfigParser(self._config_file)
         # Attribute Assignment
         self.level_filepath = Path(__file__).parent.parent / h.LEVELS_DIR / f'{self.conf.level_name}.txt'
-        self._renderer = None  # expensive - don't use it when not required !
+        self._renderer = None  # expensive - don't use; unless required !
 
         parsed_entities = self.conf.load_entities()
         self.map = LevelParser(self.level_filepath, parsed_entities, self.conf.pomdp_r)
 
         # Init for later usage:
         self.state: Gamestate
         self.map: LevelParser
@@ -169,15 +169,15 @@
         return not self.conf.do_record
 
     # noinspection PyGlobalUndefined
     def render(self, mode='human'):
         if not self._renderer:  # lazy init
             from environment.utils.renderer import Renderer
             global Renderer
-            self._renderer = Renderer(self.map.level_shape,  view_radius=self.conf.pomdp_r, fps=20)
+            self._renderer = Renderer(self.map.level_shape,  view_radius=self.conf.pomdp_r, fps=10)
 
         render_entities = self.state.entities.render()
         if self.conf.pomdp_r:
             for render_entity in render_entities:
                 if render_entity.name == c.AGENT:
                     render_entity.aux = self.obs_builder.curr_lightmaps[render_entity.real_name]
         return self._renderer.render(render_entities)
```

## environment/utils/helpers.py

```diff
@@ -1,9 +1,9 @@
 import importlib
-import itertools
+
 from collections import defaultdict
 from pathlib import PurePath, Path
 from typing import Union, Dict, List
 
 import numpy as np
 from numpy.typing import ArrayLike
 
@@ -209,28 +209,30 @@
         return c.AGENT, 'idle'
 
 
 def locate_and_import_class(class_name, folder_path: Union[str, PurePath] = ''):
     """Locate an object by name or dotted path, importing as necessary."""
     import sys
     sys.path.append("..")
-    folder_path = Path(folder_path)
-    module_paths = [x for x in folder_path.rglob('*.py') if x.is_file() and '__init__' not in x.name]
+    folder_path = Path(folder_path).resolve()
+    module_paths = [x.resolve() for x in folder_path.rglob('*.py') if x.is_file() and '__init__' not in x.name]
     # possible_package_path = folder_path / '__init__.py'
     # package = str(possible_package_path) if possible_package_path.exists() else None
     all_found_modules = list()
+    package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'environment')
     for module_path in module_paths:
-        mod = importlib.import_module('.'.join([x.replace('.py', '') for x in module_path.parts]))
+        module_parts = [x.replace('.py', '') for idx, x in enumerate(module_path.parts) if idx >= package_pos]
+        mod = importlib.import_module('.'.join(module_parts))
         all_found_modules.extend([x for x in dir(mod) if not(x.startswith('__') or len(x) < 2 or x.isupper())
                                   and x not in ['Entity',  'NamedTuple', 'List', 'Rule', 'Union', 'random', 'Floor'
                                                 'TickResult', 'ActionResult', 'Action', 'Agent', 'deque',
                                                 'BoundEntityMixin', 'RenderEntity', 'TemplateRule', 'defaultdict',
                                                 'is_move', 'Objects', 'PositionMixin', 'IsBoundMixin', 'EnvObject',
-                                                'EnvObjects',]])
+                                                'EnvObjects']])
         try:
             model_class = mod.__getattribute__(class_name)
             return model_class
         except AttributeError:
             continue
     raise AttributeError(f'Class "{class_name}" was not found!!!"\n'
                          f'Check the {folder_path.name} name.\n'
-                         f'Possible Options are:\n{set(all_found_modules)}')
+                         f'Possible Options are:\n{set(all_found_modules)}')
```

## environment/utils/observation_builder.py

```diff
@@ -187,68 +187,70 @@
         self.agent = agent
         self.pomdp_r = pomdp_r
         self.n_rays = 100  # (self.pomdp_r + 1) * 8
         self.degs = degs
         self.ray_targets = self.build_ray_targets()
         self.obs_shape_cube = np.array([self.pomdp_r, self.pomdp_r])
 
+    def __repr__(self):
+        return f'{self.__class__.__name__}({self.agent.name})'
+
     def build_ray_targets(self):
         north = np.array([0, -1])*self.pomdp_r
         thetas = [np.deg2rad(deg) for deg in np.linspace(-self.degs // 2, self.degs // 2, self.n_rays)[::-1]]
         rot_M = [
             [[math.cos(theta), -math.sin(theta)],
              [math.sin(theta), math.cos(theta)]] for theta in thetas
         ]
         rot_M = np.stack(rot_M, 0)
         rot_M = np.unique(np.round(rot_M @ north), axis=0)
         return rot_M.astype(int)
 
-    @staticmethod
-    def ray_block_cache(cache_dict, key, callback, ents):
+    def ray_block_cache(self, cache_dict, key, callback, ents):
         if key not in cache_dict:
             cache_dict[key] = callback()
-        if any(True for e in ents.pos_dict[key] if e.is_blocking_light) and not cache_dict[key]:
-            print()
         return cache_dict[key]
 
     def visible_entities(self, entities):
         visible = list()
         cache_blocking = {}
 
         for ray in self.get_rays():
             rx, ry = ray[0]
             for x, y in ray:
                 cx, cy = x - rx, y - ry
 
                 entities_hit = entities.pos_dict[(x, y)]
                 hits = self.ray_block_cache(cache_blocking,
                                             (x, y),
-                                            lambda: any(True for e in entities_hit if e.is_blocking_light),
+                                            lambda: any(e.is_blocking_light for e in entities_hit),
                                             entities)
 
-                diag_hits = all([
+                try:
+                    d = next(x for x in entities_hit if 'Door' in x.name)
+                    if d.pos in entities.pos_dict.keys():
+                        if d.is_closed and not entities.pos_dict[d.pos]:
+                            print()
+                except StopIteration:
+                    pass
+
+                diag_hits = any([
                     self.ray_block_cache(
                         cache_blocking,
                         key,
-                        lambda: all(False for e in entities.pos_dict[key] if not e.is_blocking_light),
+                        # lambda: all(False for e in entities.pos_dict[key] if not e.is_blocking_light),
+                        lambda: any(e.is_blocking_light for e in entities.pos_dict[key]),
                                             entities)
                     for key in ((x, y-cy), (x-cx, y))
                 ]) if (cx != 0 and cy != 0) else False
 
                 visible += entities_hit if not diag_hits else []
                 if hits or diag_hits:
                     break
                 rx, ry = x, y
-        try:
-            d = next(x for x in visible if 'Door' in x.name)
-            v = [x for x in visible if tuple(np.subtract(x.pos, d.pos)) in [(1, 0), (0, 1), (-1, 0), (0, -1)] and x.name.startswith('Floor')]
-            if len(v) > 2:
-                pass
-        except StopIteration:
-            pass
         return visible
 
     def get_rays(self):
         a_pos = self.agent.pos
         outline = self.ray_targets + a_pos
         return self.bresenham_loop(a_pos, outline)
```

## Comparing `Marl_Factory_Grid-0.0.3.dist-info/METADATA` & `Marl_Factory_Grid-0.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.3
+Version: 0.0.5
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Requires-Dist: numba (>=0.56)
 Requires-Dist: gymnasium (>=0.26)
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: networkx
 Requires-Dist: torch
+Requires-Dist: tqdm
 
 # EDYS
 
 Tackling emergent dysfunctions (EDYs) in cooperation with Fraunhofer-IKS
 
 ## Setup
 Just install this environment by `pip install marl-factory-grid`.
```

## Comparing `Marl_Factory_Grid-0.0.3.dist-info/RECORD` & `Marl_Factory_Grid-0.0.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,27 @@
 algorithms/static/TSP_item_agent.py,sha256=eLJjcerXZHrxv5vI2AGtmXw3_hSYRyM0npvwuYJ0wK8,2410
 algorithms/static/TSP_target_agent.py,sha256=cJ2lAd_s667JxgDC8T7Vk7eDJeXi8kHUgPE1G6Yc-n4,1093
 algorithms/static/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algorithms/static/random_agent.py,sha256=bO5rsNvN6WkYF3tP6xA7eVs14RVxmcWREsF_XYMQDX8,388
 environment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 environment/actions.py,sha256=fnRVblaYyIpkNy6vxL2Yyjvq8w3xUILBentuzG1RfuA,2727
 environment/constants.py,sha256=d4__uWqLuqCBkRk9mlRVL2RifK-vVZif9jzYVlTip_k,2826
-environment/factory.py,sha256=oMQ2KRYtQeyw6YrKjHm4GIkTfKgdJsLWctoAIuShbho,7086
+environment/factory.py,sha256=ZU01hbBB46DZtbPTWgfWP3ZzuZTFrE4q7A8CvUROsww,7082
 environment/rewards.py,sha256=lqKaFyeNED1BpoDzxyqPTKA7OyXxxNgNlwnqIsN9QcM,128
 environment/rules.py,sha256=0uA7nn2af-eukEd-HIaLRMZsSzotZVGAd4b50StWEdk,2648
 environment/assets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+environment/assets/wall.png,sha256=Bnj5KYj1Aj0KPSrKkeutWzr2mEEbt6H8evrQ5uWrg6o,1415
+environment/assets/agent/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+environment/assets/agent/adversary.png,sha256=_YJn-sjqCOB6j1BhA0qi-edl9kF-c44fEM1_byHTJjo,8521
+environment/assets/agent/agent.png,sha256=xhRk5IpQErNgQVsRD6ysTsDrMbYU35stuOLSojTX7e4,3402
+environment/assets/agent/agent_collision.png,sha256=f5T3pTe02kerALWdgb4VJRZLprJSqgvj3lW-4UROwTg,18857
+environment/assets/agent/idle.png,sha256=AkshaZqY6Qt9xOfJqHLskBn3wyZ5PcNK9xXc0JJNLIc,1631
+environment/assets/agent/invalid.png,sha256=Io5zHC5jter6ir88vKvjeo3sd7no4vmWagxKOQw3iyg,1599
+environment/assets/agent/move.png,sha256=VRdZ41uRRuvR9nCW1vTJb1axzrV4FAtRIKEn873PSxQ,5933
+environment/assets/agent/valid.png,sha256=8a0ms6gedMs56ltKKmbA9WRe76GvX6_s0cyTJ-WVYMw,5717
 environment/entity/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 environment/entity/agent.py,sha256=AD6DQbVeEqA2mNpE8xizALYTDqogYyfrCSGezSfZpIA,2378
 environment/entity/entity.py,sha256=RVAz14jcxrG03pFvPb-PyLSqXZTN2jm_G1gMHpaCRxA,2204
 environment/entity/mixin.py,sha256=MleXX9np7yXGq5xwww__UNIY9utgs7x1zg-jwByKcWU,418
 environment/entity/object.py,sha256=I9JTsuxO7mZx5FLlYEtfa_8l6u3WBzSIvSBg-LMRfvQ,3457
 environment/entity/util.py,sha256=anbYYeapR_U2Agi0gjBnskXQscKbxFA6y088YAh5B3A,1249
 environment/entity/wall_floor.py,sha256=o_8AS9tTgrhkybDbjoB8xivYaGIsjE_93zFfDwnrl5Y,3206
@@ -37,17 +46,17 @@
 environment/groups/utils.py,sha256=e-vAs-VZIxRDyi4Jp6C-FNRCufXaa2Ffp3VvDmJAww4,2415
 environment/groups/wall_n_floors.py,sha256=EtsL9U1D1-junrI26T-d_E5nrcQTThZpxvTLI3vPaZU,1590
 environment/logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 environment/logging/envmonitor.py,sha256=f5nbwdOBrYRxG4CbJc2nwU7q9Zsw3YHR-iTIjNIDkzQ,2266
 environment/logging/recorder.py,sha256=4ZXsh47NwXch4XjWg4xg_nohXRVPFp3L7gNcergDYN4,5627
 environment/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 environment/utils/config_parser.py,sha256=lecTZ7zz0yXNrI0KZ0VtvHpLV0BoxbWuDNyWAMIuiLw,5281
-environment/utils/helpers.py,sha256=YLubLEB3LifpjXHov-WmRHOK2bfhwGvbRvkIiOUywBI,10791
+environment/utils/helpers.py,sha256=95vMJFVwzGoaEgQXuCkxRgNO2vwaOfy-bqpBKmOW-V8,10978
 environment/utils/level_parser.py,sha256=fWPhRdTZuLGkyfd9sVRDBEJ57cjWEqZqO9wEQQ034AI,2255
-environment/utils/observation_builder.py,sha256=_X-2sY5E1KQUHTdxTDwsOrjvirtkkj7uefg982rwTTU,12714
+environment/utils/observation_builder.py,sha256=OOBa9mUz7uOnc8T44Ydrc3U9Jt3CSXmM85rRI9vUPto,12774
 environment/utils/render.py,sha256=0P_dmYIYT_gW_yjrPwBZPwgSfY84OfaapA9_GlrYm24,299
 environment/utils/renderer.py,sha256=XbqFSa2NIOTYFoS53yMiHtKJQlo4Gldf_EiiIb82mCQ,5903
 environment/utils/results.py,sha256=-AA38VdMyeNB7ID7tu_5lkuFPSL9WgJt5aD3LCAp0D0,1152
 environment/utils/states.py,sha256=4c7MdGSMRfWmn5t5KkWOQdu9YRJeKGN2ln0c_6ERayQ,3677
 environment/utils/utility_classes.py,sha256=w6XqcchU_EVdG_fmYBL1mqB3Oeo6jkloQHyy_fkrG7c,838
 modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/_template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -59,42 +68,54 @@
 modules/batteries/entitites.py,sha256=4x4aeKNHqefvmSKvsbKmCS0CqJJD1LH3wkzh7wf3lPM,2405
 modules/batteries/groups.py,sha256=Ylx1a1tq8NPef9kYD8vnpYVB5F3cUKPUpJhVssNH0L0,1055
 modules/batteries/rewards.py,sha256=8iX_Rty7k5dt2KSifHRLBKqipElLHQARR-ILMLc6BnQ,86
 modules/batteries/rules.py,sha256=a2XW0Ma7_z9_5UbQZ7AmV3SJj4Kc_mG6pkv5I5ecDow,2136
 modules/clean_up/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/clean_up/actions.py,sha256=yj-qL55l-IXwIB_jiVAyrCkZM5AZbeolyjJv0pkw4L0,1295
 modules/clean_up/constants.py,sha256=N-PxyDWs-f18i9xo5XMqd-zgI_hlwoTiyF1jiMubSo8,157
+modules/clean_up/dirtpiles.png,sha256=UsVE6k92qOPTj-NuWNHkPDGyIvd7xrb0FPSr0W6gbgc,39296
 modules/clean_up/entitites.py,sha256=vhRl20NDl3l0s4t7gXfZm5KHKA92ntdHxMAtUzzrXvM,1173
 modules/clean_up/groups.py,sha256=f4HyR3_blLmpWHTlzSOXKJSw5ZRrbjlRx4q0RJ1RCtQ,2585
 modules/clean_up/rewards.py,sha256=PnT29DkDM0Usw5FIF83wmMzxq0xvYOPYnajr0tya-uE,85
 modules/clean_up/rule_done_on_all_clean.py,sha256=ISwF1D8RatWWPAyYmiPW_VuNWVE4GP4V3PrYYGG7qg0,566
 modules/clean_up/rule_respawn.py,sha256=bv-x1nCY6Tq1_gpkTmf94ynh0wEyRVcV0-cqHcr_UD0,953
 modules/clean_up/rule_smear_on_move.py,sha256=vDT-mHGNA0xmg5xrHqYxGSVuEc8IooQXWPbxpIyCBPw,1030
 modules/destinations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/destinations/actions.py,sha256=PZGiQ2gAStwmzh6hbnvmruPeT2C0hJEDHwIVs0vUCE0,911
 modules/destinations/constants.py,sha256=_dmIdrrQX5pxvPMIN1UPOg2q65yRimKGdws3Nytoo4c,328
+modules/destinations/destinations.png,sha256=J6LhYFEWxKatiNZX3-A1NoEMsrIwmrfhBjl1agUe9yo,7037
 modules/destinations/entitites.py,sha256=aaMFsOo4txZFQ3yoTLeBt15gNSSTODH6apRrjsmOj9Q,1786
 modules/destinations/groups.py,sha256=aETalA7Yx5M1QYvEzsNs36wQ8iyR-nZusz041WWmKB0,808
 modules/destinations/rewards.py,sha256=QP4AJGPMv9DQDMp761mrsM4kmC0t3sdW6tNAKUsabn4,75
 modules/destinations/rules.py,sha256=a0poQY_93Pqa0fTvzLbM-gtgPea5NwtROINMqWIreN4,3739
 modules/doors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/doors/actions.py,sha256=vqwwFv7r8v-FzZ9zH-PfsVOei0RA5iYLGIXGXATJ0jI,1132
 modules/doors/constants.py,sha256=tGl_uIuBxPS-oRss9vveri3_9d1HhnJkeoknRZYMcd0,811
+modules/doors/door_closed.png,sha256=uSBXHmS5JvdvMfBjY6jYxFe4ABVTUfnanJtzAyJaN4o,699
+modules/doors/door_open.png,sha256=IuOrcr3809ULOMt_ABINH_-3W6Yr80rcB3DYWwmjwcM,4224
 modules/doors/entitites.py,sha256=gowvFLeSW95tuHuSQWzF_L-RzZWaqED3ef8jmbVmxN0,2777
 modules/doors/groups.py,sha256=NaEqqd-NZdy9EorDaPPHLpNiVtbDjUhL-UyaZjg3vWc,880
 modules/doors/rewards.py,sha256=a5tq-lY1R84lS9q2BHrTzjeSboCu5tp2nrG2gGxU4RY,59
 modules/doors/rule_door_auto_close.py,sha256=NkZ4q7zOLmLgmW_FMeq1f3wfNntsj1cJOuPQ6kKVNfM,861
 modules/items/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/items/actions.py,sha256=3d0TGQrLaxHlME_fKF21FFMs9yOaoA3_U1JqdLxVvGM,1658
 modules/items/constants.py,sha256=qNcpzx3OIFMKxCorrk1SvzDXCiCxXVdxb8vHw8ZOus0,245
 modules/items/entitites.py,sha256=MBIUI3lqNgPxYjYGO0lBzt33ZinBE3Xd0L0JmUtX180,2078
 modules/items/groups.py,sha256=e0CKr4wsBtAMNwQnuS9zy6uvixZBOM1PS6LRIBRnK6A,3166
 modules/items/rewards.py,sha256=4GmQ0Ii7U--h2DTRSUJOHu5i0Ox_IAf1UnJBB1HoWww,112
 modules/items/rules.py,sha256=p9xxCYM4U7FBqC7dgOvAPPvGShdQ4JgKXJohSa_SlS4,3154
+modules/items/assets/charge_pod.png,sha256=aSQcmULQFYwS5IITPh2qRK-sG-HCIyf0FT7-pohrvjw,6610
+modules/items/assets/dropofflocations.png,sha256=RgzYGa62W2cZ2v0q-hFeUZEun3dVSQj0OFiO3RG-auU,2318
+modules/items/assets/items.png,sha256=LKWWKqFFbTcyqd0E-0lPHiUqtddfePr5eIjg69r2p1g,3102
 modules/levels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+modules/levels/large.txt,sha256=-InV4RyKzElR_cxcU2onkY_pLc3dvKVY7m1tBjeDP3s,1534
+modules/levels/large_qquad.txt,sha256=ogRYGPcjmXjOj-7GgienIC67AwytE0iOeJmLxkwnXCs,5873
+modules/levels/rooms.txt,sha256=KjKA_F2FL3yapx1w17jb_ea7fErTBgnreCjwgpsv-l0,219
+modules/levels/shelves.txt,sha256=sMYVdMO-SsetMONnM-r9JbloqPV4WwXjA4sjzQlChSc,180
+modules/levels/simple.txt,sha256=YOzuDIA97bMYuCggSBIE06JhZq68Y8zp99euuKRAlag,166
 modules/machines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 modules/machines/constants.py,sha256=tYRm89C-8RcY2Yz6EjSO66RPFGqT8QMOpIg1rMAdHog,189
 modules/machines/entitites.py,sha256=nhIPYKv689VbVhcQkP1BMMzbYBN6qYbTFjOmhkB8ogo,1885
 modules/machines/groups.py,sha256=Y12hJ_bTKMvvUuhbJo3PMO3ycqEFppDvq9rmKUDHExc,398
 modules/machines/rewards.py,sha256=PCqawqAlHydPLxcp69RWdUAVG9_WZ-bVaRbFyAoH6dw,117
 modules/machines/rules.py,sha256=Dio_oge94BGd2-VbAYs_K5slrpVOElZEwtZTAujrvTg,883
 plotting/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -104,11 +125,11 @@
 studies/e_1.py,sha256=GboE8f8lqK_lpkpp2jNpqmvr1RoC8zv0G0HGpI-FAcs,24447
 studies/e_1_mix.py,sha256=-LzmgSsHNMU_1ovFc3k6vbsOvLw6mN3HcOFIf5E_t4o,10359
 studies/normalization_study.py,sha256=dtsq-qkTV_PFfoQGh8jujIa1_Wgjp4JD_YGZaNAsYSs,809
 studies/playground_file.py,sha256=KC6XV2__npofGJ_O9dcdW2caAL8rQac1wqhv4xQxvdA,729
 studies/single_run_with_export.py,sha256=nBtLqQJzh5LTd82i-pIbO6kQRuC1uIPlN1V47lIkZCw,12666
 studies/test.py,sha256=62RQo3idkFb-xSDM9eO1TiUuy3EeTq3Jf-U577pZauM,7604
 studies/viz_policy.py,sha256=rcC37stj4eK9RSZdbznFwUz0Fia7RC6c9akJS--vhQM,1330
-Marl_Factory_Grid-0.0.3.dist-info/METADATA,sha256=D0RVMRFD8PkaXzXCMjnMVIfhkJsiglLUstPs4-nXLvo,3126
-Marl_Factory_Grid-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Marl_Factory_Grid-0.0.3.dist-info/top_level.txt,sha256=NSyFZwMZq6F_GTv3l0iQXv07doEggO3d-7H-mmi2eqs,48
-Marl_Factory_Grid-0.0.3.dist-info/RECORD,,
+Marl_Factory_Grid-0.0.5.dist-info/METADATA,sha256=yukMUkHa8-j7LaokA-pg5Di-Op1Y1lUwAsbcA3bJZs0,3147
+Marl_Factory_Grid-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Marl_Factory_Grid-0.0.5.dist-info/top_level.txt,sha256=NSyFZwMZq6F_GTv3l0iQXv07doEggO3d-7H-mmi2eqs,48
+Marl_Factory_Grid-0.0.5.dist-info/RECORD,,
```

