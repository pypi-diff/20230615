# Comparing `tmp/enderchest-0.1.1rc1.tar.gz` & `tmp/enderchest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.1rc1.tar", last modified: Fri Jun  9 22:57:09 2023, max compression
+gzip compressed data, was "enderchest-0.1.2.tar", last modified: Thu Jun 15 01:56:31 2023, max compression
```

## Comparing `enderchest-0.1.1rc1.tar` & `enderchest-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.836967 enderchest-0.1.1rc1/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.955998 enderchest-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 01:56:23.000000 enderchest-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-15 01:56:31.955998 enderchest-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-15 01:56:23.000000 enderchest-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.955998 enderchest-0.1.2/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 01:56:31.955998 enderchest-0.1.2/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29632 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.951998 enderchest-0.1.2/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/sync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.951998 enderchest-0.1.2/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.955998 enderchest-0.1.2/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-15 01:56:23.000000 enderchest-0.1.2/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:56:31.951998 enderchest-0.1.2/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 01:56:31.000000 enderchest-0.1.2/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 01:56:31.955998 enderchest-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-15 01:56:23.000000 enderchest-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-06-15 01:56:23.000000 enderchest-0.1.2/versioneer.py
```

### Comparing `enderchest-0.1.1rc1/LICENSE` & `enderchest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/PKG-INFO` & `enderchest-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.1rc1/README.md` & `enderchest-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/cli.py` & `enderchest-0.1.2/enderchest/cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/config.py` & `enderchest-0.1.2/enderchest/config.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/craft.py` & `enderchest-0.1.2/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/enderchest.py` & `enderchest-0.1.2/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/filesystem.py` & `enderchest-0.1.2/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/gather.py` & `enderchest-0.1.2/enderchest/gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
     )
 
     matches = [
         instance for instance in chest.instances if shulker_box.matches(instance)
     ]
 
     if len(matches) == 0:
-        report = "is not link to by any registered instances"
+        report = "is not linked to by any registered instances"
     else:
         report = "is linked to by the following instances:\n" + "\n".join(
             f"  - {_render_instance(instance)}" for instance in matches
         )
 
     GATHER_LOGGER.info(f"The shulker box {_render_shulker_box(shulker_box)} {report}")
```

### Comparing `enderchest-0.1.1rc1/enderchest/instance.py` & `enderchest-0.1.2/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/loggers.py` & `enderchest-0.1.2/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/place.py` & `enderchest-0.1.2/enderchest/place.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,29 @@
             instance altogether but to otherwise continue on with other instances
           - pass in `error_handling="skip-shulker-box"` to abort linking to the current
             shulker box altogether but to otherwise continue on with other boxes
           - pass in `error_handling="prompt"` to ask what to do on each failure
     relative : bool, optional
         By default, links will use relative paths when possible. To use absolute
         paths instead (see: https://bugs.mojang.com/projects/MC/issues/MC-263046),
-        pass in `relative=False`.
+        pass in `relative=False`. See note below.
     rollback: bool, optional
         In the future in the event of linking errors passing in `rollback=True`
         can be used to roll back any changes that have already been applied
         based on the error-handling method specified.
+
+    Notes
+    -----
+    - If one of the files or folders being placed is itself a symlink, relative
+      links will be created as *nested* links (a link pointing to the link),
+      whereas in "absolute" mode (`relative=False`), the link that will be
+      placed will point **directly** to the final target.
+    - This can lead to the stale-link cleanup behavior not correctly removing
+      an outdated symlink if the fully resolved target of a link falls outside
+      the EnderChest folder.
     """
     if rollback is not False:
         raise NotImplementedError("Rollbacks are not currently supported")
 
     try:
         host = load_ender_chest(minecraft_root).name
     except (FileNotFoundError, ValueError) as bad_chest:
@@ -193,15 +203,15 @@
 
             match_exit = "pass"
             for link_folder in shulker_box.link_folders:
                 resources -= {box_root / link_folder}
                 resources -= set((box_root / link_folder).rglob("*"))
                 try:
                     link_resource(link_folder, box_root, instance_root, relative)
-                except (OSError, NotADirectoryError) as oh_no:
+                except OSError:
                     PLACE_LOGGER.error(
                         f"Error linking shulker box {shulker_box.name}"
                         f" to instance {instance.name}:"
                         f"\n  {(instance.root / link_folder)} is a"
                         " non-empty directory"
                     )
                     match handle_error(shulker_box):
@@ -235,15 +245,15 @@
                         try:
                             link_resource(
                                 resource_path,
                                 box_root,
                                 instance_root,
                                 relative,
                             )
-                        except (OSError, NotADirectoryError) as oh_no:
+                        except OSError:
                             PLACE_LOGGER.error(
                                 f"Error linking shulker box {shulker_box.name}"
                                 f" to instance {instance.name}:"
                                 f"\n  {(instance.root / resource_path)}"
                                 " already exists"
                             )
                             match handle_error(shulker_box):
@@ -290,32 +300,32 @@
     relative : bool
         If True, the link will be use a relative path if possible. Otherwise,
         an absolute path will be used, regardless of whether a a relative or
         absolute path was provided.
 
     Raises
     ------
-    NotADirectoryError
-        If a file already exists where you're attempting to place the symlink
     OSError
-        If a non-empty directory already exists where you're attempting to
-        place the symlink
+        If a file or non-empty directory already exists where you're attempting
+        to place the symlink
 
     Notes
     -----
     - This method will create any folders that do not exist within an instance
     - This method will overwrite existing symlinks and empty folders
       but will not overwrite or delete any actual files.
     """
     instance_path = (instance_root / resource_path).expanduser().absolute()
     instance_path.parent.mkdir(parents=True, exist_ok=True)
 
     target: str | Path = (shulker_root / resource_path).expanduser().absolute()
     if relative:
         target = os.path.relpath(target, instance_path.parent)
+    else:
+        target = target.resolve()  # type: ignore
 
     if instance_path.is_symlink():
         # remove previous symlink in this spot
         instance_path.unlink()
         PLACE_LOGGER.debug(f"Removed previous link at {instance_path}")
     else:
         try:
```

### Comparing `enderchest-0.1.1rc1/enderchest/prompt.py` & `enderchest-0.1.2/enderchest/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utilities for helping build interactive prompts"""
 
-CURSOR = "==>"
+CURSOR = "\x1b[35;1m==>\x1b[0m"
 
 # https://stackoverflow.com/a/18472142
 YES = ("y", "yes", "t", "true", "on", "1")
 
 NO = ("n", "no", "f", "false", "off", "0")
 
 
@@ -28,17 +28,17 @@
     - The output will be stripped of trailing and leading whitespace, but no
       other validation or processing will be used.
     - Regardless of whether a suggestion is provided, if the user provides an
       empty input, this method will return an empty string. To reiterate: the
       suggestion *does not serve* as a default / fallback value.
     """
     lines = message.splitlines() + [""]
-    message = "\n".join(f"{CURSOR} {line}" for line in lines)
+    message = "\n".join(f"{CURSOR}\x1b[1m {line}\x1b[0m" for line in lines)
     if suggestion is not None:
-        message += f"[{suggestion}] "
+        message += f"\x1b[35;1m[{suggestion}]\x1b[0m "
     return input(message)
 
 
 def confirm(default: bool) -> bool:
     """Confirm that the user wishes to continue
 
     Parameters
```

### Comparing `enderchest-0.1.1rc1/enderchest/remote.py` & `enderchest-0.1.2/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/shulker_box.py` & `enderchest-0.1.2/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/__init__.py` & `enderchest-0.1.2/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/file.py` & `enderchest-0.1.2/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/rsync.py` & `enderchest-0.1.2/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/utils.py` & `enderchest-0.1.2/enderchest/sync/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/conftest.py` & `enderchest-0.1.2/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_cli.py` & `enderchest-0.1.2/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_config.py` & `enderchest-0.1.2/enderchest/test/test_config.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_craft.py` & `enderchest-0.1.2/enderchest/test/test_craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_gather.py` & `enderchest-0.1.2/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_instance.py` & `enderchest-0.1.2/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_place.py` & `enderchest-0.1.2/enderchest/test/test_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,36 +175,52 @@
 
         assert (instance_folder / "crash-reports").is_symlink()
 
         assert (instance_folder / "crash-reports" / "20230524.log").resolve() == (
             minecraft_root / "crash-reports" / "20230524.log"
         )
 
+    @pytest.mark.parametrize("link_type", ("absolute", "relative"))
     @utils.parametrize_over_instances("official", "axolotl")
-    def test_place_places_symlinks(self, minecraft_root, instance):
-        place.place_ender_chest(minecraft_root)
+    def test_place_places_symlinks(self, minecraft_root, instance, link_type):
+        place.place_ender_chest(minecraft_root, relative=link_type == "relative")
 
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         # the counterpoint to the whole "one assertion per test" rule--this
         # is a cascading case of figuring way of figuring out just how badly
         # the impl is borked
 
         assert (instance_folder / "saves" / "test").exists()
         assert (instance_folder / "saves" / "test" / "level.dat").exists()
         assert (
             instance_folder / "saves" / "test" / "level.dat"
         ).read_text() == "hello world\n"
 
+        assert (instance_folder / "saves" / "test").is_symlink()
         assert not (instance_folder / "saves" / "test" / "level.dat").is_symlink()
 
         assert (instance_folder / "saves" / "test" / "level.dat").resolve() == (
             minecraft_root / "worlds" / "testbench" / "level.dat"
         )
 
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_absolute_symlinks_fully_resolve_target(self, minecraft_root, instance):
+        place.place_ender_chest(minecraft_root, relative=False)
+
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        link_target = os.path.abspath(os.readlink(instance_folder / "saves" / "test"))
+
+        # Windows shenanigans: https://bugs.python.org/issue42957
+        if link_target.startswith(("\\\\?\\", "\\??\\")):  # pragma: no cover
+            link_target = link_target[4:]
+
+        assert link_target == str(minecraft_root / "worlds" / "testbench")
+
     @utils.parametrize_over_instances("axolotl", "bee")
     def test_place_cleans_up_broken_symlinks_by_default(self, minecraft_root, instance):
         instance_folder = utils.resolve(instance.root, minecraft_root)
         broken_link = instance_folder / "shaderpacks" / "Seuss CitH.zip.txt"
         broken_link.symlink_to(minecraft_root / "i-do-not-exist.txt")
         assert broken_link in broken_link.parent.iterdir()
 
@@ -269,14 +285,44 @@
 
         place.place_ender_chest(minecraft_root)
 
         assert stale_link in stale_link.parent.iterdir()
 
     @pytest.mark.parametrize("link_type", ("absolute", "relative"))
     @utils.parametrize_over_instances("official", "axolotl")
+    def test_stale_link_cleaning_is_based_on_direct_target(
+        self,
+        minecraft_root,
+        instance,
+        link_type,
+    ):
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+        working_file = minecraft_root / "workspace" / "i-do-exist.txt"
+        working_file.write_text("Hello there\n")
+
+        box_link = fs.shulker_box_root(minecraft_root, "some_box") / "valid.txt"
+        box_link.parent.mkdir()
+        box_link.symlink_to(working_file)
+
+        link_link = instance_folder / "valid.txt"
+        if link_type == "absolute":
+            link_link.symlink_to(box_link)
+        else:
+            link_link.symlink_to(os.path.relpath(box_link, link_link.parent))
+
+        place.place_ender_chest(minecraft_root)
+
+        assert link_link not in link_link.parent.iterdir()
+
+        # and then just make sure that the originals are okay
+        assert working_file.read_text() == "Hello there\n"
+        assert box_link.resolve() == working_file
+
+    @pytest.mark.parametrize("link_type", ("absolute", "relative"))
+    @utils.parametrize_over_instances("official", "axolotl")
     def test_place_can_be_told_to_leave_stale_links_alone(
         self,
         minecraft_root,
         instance,
         link_type,
     ):
         instance_folder = utils.resolve(instance.root, minecraft_root)
```

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_sync.py` & `enderchest-0.1.2/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.2/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.2/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/utils.py` & `enderchest-0.1.2/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.2/enderchest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.2/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/setup.py` & `enderchest-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/versioneer.py` & `enderchest-0.1.2/versioneer.py`

 * *Files identical despite different names*

