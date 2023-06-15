# Comparing `tmp/mend_sca_cleanup_tool-23.6.1.3-py3-none-any.whl.zip` & `tmp/mend_sca_cleanup_tool-23.6.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14710 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    21666 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     9176 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD
-9 files, 43361 bytes uncompressed, 13188 bytes compressed:  69.6%
+Zip file size: 14733 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    21762 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9176 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-15 21:30 mend_sca_cleanup_tool-23.6.1.4.dist-info/RECORD
+9 files, 43457 bytes uncompressed, 13211 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/METADATA
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/WHEEL
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/entry_points.txt
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/top_level.txt
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD
+Filename: mend_sca_cleanup_tool-23.6.1.4.dist-info/RECORD
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

## Comparing `mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE` & `mend_sca_cleanup_tool-23.6.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA` & `mend_sca_cleanup_tool-23.6.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-sca-cleanup-tool
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

