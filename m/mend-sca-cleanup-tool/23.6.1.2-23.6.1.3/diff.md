# Comparing `tmp/mend_sca_cleanup_tool-23.6.1.2-py3-none-any.whl.zip` & `tmp/mend_sca_cleanup_tool-23.6.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14524 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    20930 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     9107 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-14 19:56 mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD
-9 files, 42556 bytes uncompressed, 13002 bytes compressed:  69.4%
+Zip file size: 14710 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    21666 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9176 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-15 19:36 mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD
+9 files, 43361 bytes uncompressed, 13188 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD
+Filename: mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.1.2"
+__version__ = "23.6.1.3"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -74,15 +74,15 @@
                 else:
                     print("skipReportGeneration flag found, skipping report generation")
                 if not CONFIG.skip_project_deletion:
                     delete_scan(product_token, project)
                 else:
                     print("skipProjectDeletion flag found, skipping project deletion")
     else:
-        print(f"Dry Run found {total_projects_to_delete} project(s) to delete")
+        print(f"Dry Run found {total_projects_to_delete} project(s) to delete: {[project['name'] for projects in product_project_dict.values() for project in projects]}")
 
 def check_response_error(obj_response):
     if isinstance(obj_response, dict):
         if "errorMessage" in obj_response:
             print(f"There was an issue with the request: {obj_response['errorMessage']}")
             return True
         else:
@@ -118,42 +118,57 @@
     if len(projects_to_return) == 0:
         return []
 
     if CONFIG.excluded_project_name_patterns:
         print(f"Filtering projects with name containing values {CONFIG.project_name_exclude_list}")
         for patt in CONFIG.project_name_exclude_list:
             projects_to_return = [project for project in projects_to_return for k, v in project.items() if k == "name" and patt not in v]
-        print(f"Found {len(projects_to_return)} project(s)")
 
     if CONFIG.operation_mode == FILTER_PROJECTS_BY_UPDATE_TIME:
         archive_date = (datetime.utcnow() - timedelta(days=CONFIG.days_to_keep))
         print(f"Filtering projects older than: {archive_date}")
         projects_to_return = [project for project in projects_to_return if archive_date.timestamp() > datetime.strptime(project['lastUpdatedDate'],'%Y-%m-%d %H:%M:%S %z').timestamp()]
-        print(f"Found {len(projects_to_return)} project(s)")
 
     if CONFIG.analyzed_project_tag:
         print(f"Filtering projects based on project tag: {CONFIG.analyzed_project_tag}")
-        projects_to_return = [project for project in [get_project_tag(project) for project in projects_to_return] if CONFIG.tag_pair[1] in project['tags'][0].get(CONFIG.tag_pair[0], '')]
-        print(f"Found {len(projects_to_return)} project(s)")
+        projects_to_return = filter_projects_by_tag_with_exact_match(projects_to_return) 
 
     if CONFIG.analyzed_project_tag_regex_in_value:
-        print(f"Filtering projects based on project tag value with regex: {CONFIG.analyzed_project_tag_regex_in_value}")
-        projects_to_return = [project for project in [get_project_tag(project) for project in projects_to_return] for k, v in project['tags'][0].items() if CONFIG.tag_pair[0] in k and any(CONFIG.tag_pair[1] in item for item in v) ]
-        print(f"Found {len(projects_to_return)} project(s)")
+        print(f"Filtering projects based on project contain tag value: {CONFIG.analyzed_project_tag_regex_in_value}")
+        projects_to_return = filter_projects_by_tag_with_contains_match(projects_to_return)
 
     if CONFIG.operation_mode == FILTER_PROJECTS_BY_LAST_CREATED_COPIES:
         print(f"Filtering projects besides most recent: {CONFIG.days_to_keep}")
         if len(projects_to_return) > CONFIG.days_to_keep:
             index = len(projects_to_return) - CONFIG.days_to_keep
             print(f"Total: {len(projects_to_return)}. Archiving first {index}")
             projects_to_return = projects_to_return[:index]
         else:
             print(f"Total: {len(projects_to_return)}. Nothing to filter")
+    print(f"{len(projects_to_return)} project(s) to remove after filtering")
     return projects_to_return
 
+def filter_projects_by_tag_with_exact_match(projects):
+    projects_to_return = []
+    for project in projects:
+        project_tags = get_project_tags(project)
+        if CONFIG.tag_pair[1] in project_tags.get(CONFIG.tag_pair[0], ''):
+            print(f"{project['name']} has matching tag")
+            projects_to_return.append(project)
+    return projects_to_return
+
+def filter_projects_by_tag_with_contains_match(projects):
+    projects_to_return = []
+    for project in projects:
+        project_tags = get_project_tags(project)
+        for k, v in project_tags.items():
+            if CONFIG.tag_pair[0] in k and any(CONFIG.tag_pair[1] in item for item in v):
+                print(f"{project['name']} contains tag value")
+                projects_to_return.append(project)
+    return projects_to_return
 
 def generate_reports(project):
     print(f"Generating reports for project: {project['name']}")
     project_token = project['token']
     reports_to_generate = get_reports_to_generate()
     if len(reports_to_generate) > 0:
         output_dir = create_output_directory(project['productName'], project['name'])
@@ -259,58 +274,61 @@
     })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         exit()
     else:
         return [vital_Response for vital_Response in response_obj['projectVitals']]
 
-def get_project_tag(project):
+def get_project_tags(project):
+    print(f"Getting tags for project {project['name']}")
     request = json.dumps({
             "requestType": "getProjectTags",
             "userKey": CONFIG.mend_user_key,
             "projectToken": project['token'],
         })
     response_obj = json.loads(post_api_request(request).decode("utf-8"))
     if check_response_error(response_obj):
         exit()
-    project['tags'] = [project_tags['tags'] for project_tags in response_obj['projectTags']]
-    return project
+    return [project_tags['tags'] for project_tags in response_obj['projectTags']][0]
 
 def get_projects_to_remove():
     projects_to_remove = {}
     products = get_products()
     for product in products:
         print(f"Getting projects to remove for product: {product['productName']}")
         projects = get_projects(product['productToken'])
-        if len(projects) > 0:
+        projects_length = len(projects)
+        if projects_length:
+            print(f"Product has {projects_length} project(s)")
             filtered_projects = filter_projects_by_config(projects)
-            if len(filtered_projects) > 0:
+            filted_projects_total = len(filtered_projects)
+            if filted_projects_total > 0:
                 projects_to_remove[product['productToken']] = filtered_projects
         else:
             print(f"No projects found for product: {product['productName']}")
     return projects_to_remove
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Mend SCA Clean up tool")
     parser.add_argument('-a', '--mendURL', '--wsURL', help="Mend URL", dest='mend_url', default="saas.whitesourcesoftware.com")
     parser.add_argument('-e', '--excludedProductTokens', help="Excluded Product Tokens (comma seperated list)", dest='excluded_product_tokens')
-    parser.add_argument('-g', '--analyzedProjectTag', help="Analyze only the projects whose contain the specific Mend tag (key:value)", dest='analyzed_project_tag')
+    parser.add_argument('-g', '--analyzedProjectTag', help="Analyze only the projects whose contain the specific Mend tag (key:value). Case sensitive.", dest='analyzed_project_tag')
     parser.add_argument('-i', '--includedProductTokens', help="Included Product Tokens (comma seperated list)", dest='included_product_tokens')
     parser.add_argument('-j', '--skipProjectDeletion', help="Skip Project Deletion", dest='skip_project_deletion', type=strtobool, default=False)
     parser.add_argument('-k', '--apiToken', '--orgToken', help="Mend API token", dest='mend_api_token', required=True)
     parser.add_argument('-m', '--operationMode', help="Clean up operation method", dest='operation_mode', default=FILTER_PROJECTS_BY_UPDATE_TIME,
                                 choices=[s for s in [FILTER_PROJECTS_BY_UPDATE_TIME, FILTER_PROJECTS_BY_LAST_CREATED_COPIES]])
-    parser.add_argument('-n', '--excludedProjectNamePatterns', help="List of excluded project name patterns (comma seperated list)", dest='excluded_project_name_patterns')
+    parser.add_argument('-n', '--excludedProjectNamePatterns', help="List of excluded project name patterns (comma seperated list). Case sensitive.", dest='excluded_project_name_patterns')
     parser.add_argument('-o', '--outputDir', help="Output directory", dest='output_dir', default=os.getcwd() + "\\Mend\\Reports\\")
     parser.add_argument('-p', '--projectParallelismLevel', help="Project parallelism level directory Note: This is currently not used in this version of the mend-sca-cleanup-tool", dest='project_parallelism_level')
     parser.add_argument('-r', '--daysToKeep', help="Number of days to keep (overridden by --dateToKeep)", dest='days_to_keep', type=int, default=50000)
     parser.add_argument('-s', '--skipReportGeneration', help="Skip Report Generation", dest='skip_report_generation', type=strtobool, default=False)
     parser.add_argument('-t', '--reportTypes', help="Report Types to generate (comma seperated list)", dest='report_types')
     parser.add_argument('-u', '--userKey', help="Mend UserKey", dest='mend_user_key', required=True)
-    parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:value) Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.", dest='analyzed_project_tag_regex_in_value')
+    parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:value). Case sensitive. Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.", dest='analyzed_project_tag_regex_in_value')
     parser.add_argument('-x', '--excludedProjectTokens', help="Excluded Project Tokens (comma seperated list)", dest='excluded_project_tokens')
     parser.add_argument('-y', '--dryRun', help="Whether to run the tool without performing anything", dest='dry_run', type=strtobool, default=False)
     return parser.parse_args()
 
 def parse_config_file(filepath):
     if os.path.exists(filepath):
         config = ConfigParser()
```

## Comparing `mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE` & `mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA` & `mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-sca-cleanup-tool
-Version: 23.6.1.2
+Version: 23.6.1.3
 Summary: Mend SCA Cleanup Tool
 Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
 Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -119,17 +119,17 @@
   -o OUTPUT_DIR, --outputDir
                     Output directory
   -e EXCLUDED_PRODUCT_TOKENS, --excludedProductTokens
                     List of excluded products
   -i INCLUDED_PRODUCT_TOKENS, --includedProductTokens
                     List of included products
   -g ANALYZED_PROJECT_TAG, --AnalyzedProjectTag
-                    Analyze only the projects whose contain the specific Mend tag (key:value)
+                    Analyze only the projects whose contain the specific Mend tag (key:value). Case sensitive.
   -v ANALYZED_PROJECT_TAG_REGEX_IN_VALUE, --AnalyzedProjectTagRegexInValue
-                    Analyze only the projects whose match their tag key and the tag value contains the specified value (key:value)
+                    Analyze only the projects whose match their tag key and the tag value contains the specified value (key:value). Case sensitive.
                     Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.
   -r DAYS_TO_KEEP, --DaysToKeep
                     Number of days to keep in FilterProjectsByUpdateTime or number of copies in FilterProjectsByLastCreatedCopies
   -p PROJECT_PARALLELISM_LEVEL, --ProjectParallelismLevel
                     Project parallelism level
                     Note: This is currently not used in this version of the mend-sca-cleanup-tool. Was kept to prevent breaking existing integrations.
   -y DRY_RUN, --DryRun
@@ -140,15 +140,15 @@
                     default False
   -j SKIP_PROJECT_DELETION, --SkipProjectDeletion
                     Skip project deletion step
                     default False                                        
   -x EXCLUDED_PROJECT_TOKENS, --excludedProjectTokens
                     List of excluded projects
   -n EXCLUDED_PROJECT_NAME_PATTERNS, --excludedProjectNamePatterns
-                    List of excluded project name patterns                 
+                    List of excluded project name patterns (comma seperated list). Case sensitive.            
 ```
 
 ## Available reports
 The following Mend project reports are available through the clean-up tool. These values can be specified with the -t flag to generate specific reports.
 * alerts
 * alerts_rejected_by_policy
 * attribution
```

## Comparing `mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD` & `mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mend_sca_cleanup_tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_sca_cleanup_tool/_version.py,sha256=lO6f6bjBTbV6kyBSXBMNyWNAqxcmEId4bg-H39-5Atw,102
-mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=mKMZ5vjti-vqBlz7FxKnvnxDii831N3dFC0PU4xGpQQ,20930
-mend_sca_cleanup_tool-23.6.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_sca_cleanup_tool-23.6.1.2.dist-info/METADATA,sha256=XX4fm7b3-RbatlQe3awixwNzTKmqPfisj19wVsaafgI,9107
-mend_sca_cleanup_tool-23.6.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_sca_cleanup_tool-23.6.1.2.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
-mend_sca_cleanup_tool-23.6.1.2.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
-mend_sca_cleanup_tool-23.6.1.2.dist-info/RECORD,,
+mend_sca_cleanup_tool/_version.py,sha256=3aTs7mVNzp9xAYZG6VGggngBngkNKFe2sHW64JdIrLU,102
+mend_sca_cleanup_tool/sca_cleanup_tool.py,sha256=Tur515deNQPRmpWjQ9nobRVMDCYwpG-oXw1BA5RkBW4,21666
+mend_sca_cleanup_tool-23.6.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_sca_cleanup_tool-23.6.1.3.dist-info/METADATA,sha256=jPGdsdlauxIq4ReFdSsCyZOz1ePMpzLQn9u4XdsxdWo,9176
+mend_sca_cleanup_tool-23.6.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_sca_cleanup_tool-23.6.1.3.dist-info/entry_points.txt,sha256=yLEwcaHEQGPNm0keG7j_fMa5hTpgY-KD5_6lgtDvBGc,87
+mend_sca_cleanup_tool-23.6.1.3.dist-info/top_level.txt,sha256=mtHqnBzr2AOf1X3bpDd_2SwjqMDn_jS2isoa9Y0sVfA,22
+mend_sca_cleanup_tool-23.6.1.3.dist-info/RECORD,,
```

