# Comparing `tmp/neon_phal_plugin_core_updater-1.1.2a2-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6763 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8789 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2411 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD
-7 files, 13781 bytes uncompressed, 5435 bytes compressed:  60.6%
+Zip file size: 6736 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8789 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2403 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      714 b- defN 23-Jun-15 18:57 neon_phal_plugin_core_updater-1.2.0.dist-info/RECORD
+7 files, 13760 bytes uncompressed, 5432 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.2.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.1.2a2
+Version: 1.2.0
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: neon-utils (~=1.1)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
 
 # Core Updater Plugin
@@ -68,7 +68,8 @@
 msg_type: neon.core_updater.start_update
 data:
   version: <new_version>
 ```
 will start the configured update command in a shell with `version` passed as the
 first and only argument. If `version` is omitted, the configured update command
 will be called with no commands.
+
```

