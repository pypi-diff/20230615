# Comparing `tmp/ws_cleanup_tool_test-23.6.1.3-py3-none-any.whl.zip` & `tmp/ws_cleanup_tool_test-23.6.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14704 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    21666 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     9175 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       81 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      853 b- defN 23-Jun-15 19:36 ws_cleanup_tool_test-23.6.1.3.dist-info/RECORD
-9 files, 43348 bytes uncompressed, 13194 bytes compressed:  69.6%
+Zip file size: 14731 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    21762 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9175 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jun-15 21:30 ws_cleanup_tool_test-23.6.1.4.dist-info/RECORD
+9 files, 43444 bytes uncompressed, 13221 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/LICENSE
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/METADATA
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/METADATA
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/WHEEL
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/entry_points.txt
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/top_level.txt
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ws_cleanup_tool_test-23.6.1.3.dist-info/RECORD
+Filename: ws_cleanup_tool_test-23.6.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.1.3"
+__version__ = "23.6.1.4"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -136,15 +136,16 @@
         print(f"Filtering projects based on project contain tag value: {CONFIG.analyzed_project_tag_regex_in_value}")
         projects_to_return = filter_projects_by_tag_with_contains_match(projects_to_return)
 
     if CONFIG.operation_mode == FILTER_PROJECTS_BY_LAST_CREATED_COPIES:
         print(f"Filtering projects besides most recent: {CONFIG.days_to_keep}")
         if len(projects_to_return) > CONFIG.days_to_keep:
             index = len(projects_to_return) - CONFIG.days_to_keep
-            print(f"Total: {len(projects_to_return)}. Archiving first {index}")
+            print(f"Total: {len(projects_to_return)}. Removing oldest {index}")
+            projects_to_return = sorted(projects_to_return, key=lambda d: d['lastUpdatedDate'])
             projects_to_return = projects_to_return[:index]
         else:
             print(f"Total: {len(projects_to_return)}. Nothing to filter")
     print(f"{len(projects_to_return)} project(s) to remove after filtering")
     return projects_to_return
 
 def filter_projects_by_tag_with_exact_match(projects):
```

## Comparing `ws_cleanup_tool_test-23.6.1.3.dist-info/LICENSE` & `ws_cleanup_tool_test-23.6.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ws_cleanup_tool_test-23.6.1.3.dist-info/METADATA` & `ws_cleanup_tool_test-23.6.1.4.dist-info/METADATA`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cleanup-tool-test
-Version: 23.6.1.3
+Version: 23.6.1.4
 Summary: Mend SCA Cleanup Tool
 Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
 Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `ws_cleanup_tool_test-23.6.1.3.dist-info/RECORD` & `ws_cleanup_tool_test-23.6.1.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mend_sca_cleanup_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_sca_cleanup_tool/_version.py,sha256=3aTs7mVNzp9xAYZG6VGggngBngkNKFe2sHW64JdIrLU,102
-mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=Tur515deNQPRmpWjQ9nobRVMDCYwpG-oXw1BA5RkBW4,21666
-ws_cleanup_tool_test-23.6.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-ws_cleanup_tool_test-23.6.1.3.dist-info/METADATA,sha256=8nvD0kpREDZu9QPpCiX0hD-i-C4Is_6IApopA2pEegE,9175
-ws_cleanup_tool_test-23.6.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ws_cleanup_tool_test-23.6.1.3.dist-info/entry_points.txt,sha256=3NxakEW57t4XhsFmC3E1HjxztWzvJ627lvMkqKGM6dI,81
-ws_cleanup_tool_test-23.6.1.3.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
-ws_cleanup_tool_test-23.6.1.3.dist-info/RECORD,,
+mend_sca_cleanup_tool/_version.py,sha256=GwZ_CP-ykOCKQiPvHc4-VZlCGpHyUilx2T0UgvX3LZw,102
+mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=cOLCcNt9uSpYNPNjSCIYMUC0ry6pgHCA2i6lI8Cbcwo,21762
+ws_cleanup_tool_test-23.6.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ws_cleanup_tool_test-23.6.1.4.dist-info/METADATA,sha256=sOqhhnzFEXmADLwBSqb9R_Ck2xwFYhJoyXdtHY1zfp0,9175
+ws_cleanup_tool_test-23.6.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ws_cleanup_tool_test-23.6.1.4.dist-info/entry_points.txt,sha256=3NxakEW57t4XhsFmC3E1HjxztWzvJ627lvMkqKGM6dI,81
+ws_cleanup_tool_test-23.6.1.4.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
+ws_cleanup_tool_test-23.6.1.4.dist-info/RECORD,,
```

