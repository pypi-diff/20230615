# Comparing `tmp/dans-datastation-tools-0.8.0.tar.gz` & `tmp/dans-datastation-tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dans-datastation-tools-0.8.0.tar", max compression
+gzip compressed data, was "dans-datastation-tools-0.9.0.tar", max compression
```

## Comparing `dans-datastation-tools-0.8.0.tar` & `dans-datastation-tools-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,39 @@
--rw-r--r--   0        0        0    11357 2022-09-02 09:16:53.824742 dans-datastation-tools-0.8.0/LICENSE
--rw-r--r--   0        0        0     1824 2022-09-17 09:46:53.313804 dans-datastation-tools-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-02 09:16:53.825993 dans-datastation-tools-0.8.0/src/datastation/__init__.py
--rw-r--r--   0        0        0      945 2022-09-02 09:16:53.826107 dans-datastation-tools-0.8.0/src/datastation/batch_processing.py
--rw-r--r--   0        0        0     1854 2022-09-17 08:23:40.659420 dans-datastation-tools-0.8.0/src/datastation/config.py
--rw-r--r--   0        0        0     1667 2022-09-02 09:16:53.826361 dans-datastation-tools-0.8.0/src/datastation/ds_metadatafile.py
--rw-r--r--   0        0        0      958 2022-09-02 09:16:53.826495 dans-datastation-tools-0.8.0/src/datastation/ds_pidsfile.py
--rw-r--r--   0        0        0     8569 2022-09-02 09:16:53.826622 dans-datastation-tools-0.8.0/src/datastation/dv_api.py
--rw-r--r--   0        0        0     1309 2022-09-02 09:16:53.826736 dans-datastation-tools-0.8.0/src/datastation/dv_search.py
--rw-r--r--   0        0        0     2513 2022-09-02 09:16:53.826855 dans-datastation-tools-0.8.0/src/datastation/dv_storage.py
--rw-r--r--   0        0        0      669 2022-09-17 08:23:40.660584 dans-datastation-tools-0.8.0/src/datastation/example-dans-datastation-tools.yml
--rw-r--r--   0        0        0      338 2022-09-02 09:16:53.827243 dans-datastation-tools-0.8.0/src/datastation/open_csv_file.py
--rw-r--r--   0        0        0        0 2022-09-02 09:16:53.827362 dans-datastation-tools-0.8.0/src/datastation/scripts/__init__.py
--rw-r--r--   0        0        0     2991 2022-09-06 15:03:46.622637 dans-datastation-tools-0.8.0/src/datastation/scripts/add_role_assignments.py
--rw-r--r--   0        0        0     3776 2022-09-07 12:09:31.585068 dans-datastation-tools-0.8.0/src/datastation/scripts/dataset_destroy_migration_placeholder.py
--rw-r--r--   0        0        0     1658 2022-09-02 09:16:53.827612 dans-datastation-tools-0.8.0/src/datastation/scripts/delete_draft_datasets.py
--rw-r--r--   0        0        0     3253 2022-09-02 09:16:53.827718 dans-datastation-tools-0.8.0/src/datastation/scripts/delete_role_assignments.py
--rw-r--r--   0        0        0     2262 2022-09-02 09:16:53.827831 dans-datastation-tools-0.8.0/src/datastation/scripts/find_datasets_with_roleassignment.py
--rw-r--r--   0        0        0     4904 2022-09-02 09:16:53.827951 dans-datastation-tools-0.8.0/src/datastation/scripts/import_user.py
--rw-r--r--   0        0        0     3011 2022-09-02 09:16:53.828079 dans-datastation-tools-0.8.0/src/datastation/scripts/oai_harvest.py
--rw-r--r--   0        0        0     1369 2022-09-02 09:16:53.828269 dans-datastation-tools-0.8.0/src/datastation/scripts/prestage_files.py
--rw-r--r--   0        0        0     1692 2022-09-02 09:16:53.828416 dans-datastation-tools-0.8.0/src/datastation/scripts/publish_datasets.py
--rw-r--r--   0        0        0     1069 2022-09-02 09:16:53.828563 dans-datastation-tools-0.8.0/src/datastation/scripts/reindex_datasets.py
--rw-r--r--   0        0        0     5684 2022-09-02 09:16:53.828709 dans-datastation-tools-0.8.0/src/datastation/scripts/replace_metadata_field_values.py
--rw-r--r--   0        0        0     2195 2022-09-02 09:16:53.828830 dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_metadata.py
--rw-r--r--   0        0        0     1326 2022-09-02 09:16:53.828951 dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_metadata_field.py
--rwxr-xr-x   0        0        0     1409 2022-09-02 09:16:53.829077 dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_pids.py
--rw-r--r--   0        0        0     1633 2022-09-02 09:16:53.829192 dans-datastation-tools-0.8.0/src/datastation/scripts/unlock_datasets.py
--rw-r--r--   0        0        0     1828 2022-09-08 12:14:07.052656 dans-datastation-tools-0.8.0/src/datastation/scripts/update_datacite_records.py
--rw-r--r--   0        0        0     2867 2022-09-17 09:47:11.932727 dans-datastation-tools-0.8.0/setup.py
--rw-r--r--   0        0        0      680 2022-09-17 09:47:11.932995 dans-datastation-tools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-02 09:16:53.824742 dans-datastation-tools-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2375 2022-09-23 14:42:41.881259 dans-datastation-tools-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-02 09:16:53.825993 dans-datastation-tools-0.9.0/src/datastation/__init__.py
+-rw-r--r--   0        0        0      945 2022-09-02 09:16:53.826107 dans-datastation-tools-0.9.0/src/datastation/batch_processing.py
+-rw-r--r--   0        0        0     2005 2022-09-23 14:38:08.784574 dans-datastation-tools-0.9.0/src/datastation/config.py
+-rw-r--r--   0        0        0     1667 2022-09-02 09:16:53.826361 dans-datastation-tools-0.9.0/src/datastation/ds_metadatafile.py
+-rw-r--r--   0        0        0      958 2022-09-02 09:16:53.826495 dans-datastation-tools-0.9.0/src/datastation/ds_pidsfile.py
+-rw-r--r--   0        0        0     8569 2022-09-02 09:16:53.826622 dans-datastation-tools-0.9.0/src/datastation/dv_api.py
+-rw-r--r--   0        0        0     1309 2022-09-02 09:16:53.826736 dans-datastation-tools-0.9.0/src/datastation/dv_search.py
+-rw-r--r--   0        0        0     2513 2022-09-02 09:16:53.826855 dans-datastation-tools-0.9.0/src/datastation/dv_storage.py
+-rw-r--r--   0        0        0     1144 2022-09-23 14:38:08.785234 dans-datastation-tools-0.9.0/src/datastation/example-dans-datastation-tools.yml
+-rwxr-xr-x   0        0        0     2537 2022-09-23 14:38:08.785859 dans-datastation-tools-0.9.0/src/datastation/ingest_flow.py
+-rw-r--r--   0        0        0      338 2022-09-02 09:16:53.827243 dans-datastation-tools-0.9.0/src/datastation/open_csv_file.py
+-rw-r--r--   0        0        0        0 2022-09-02 09:16:53.827362 dans-datastation-tools-0.9.0/src/datastation/scripts/__init__.py
+-rw-r--r--   0        0        0     2991 2022-09-06 15:03:46.622637 dans-datastation-tools-0.9.0/src/datastation/scripts/add_role_assignments.py
+-rw-r--r--   0        0        0     3776 2022-09-07 12:09:31.585068 dans-datastation-tools-0.9.0/src/datastation/scripts/dataset_destroy_migration_placeholder.py
+-rw-r--r--   0        0        0     1658 2022-09-02 09:16:53.827612 dans-datastation-tools-0.9.0/src/datastation/scripts/delete_draft_datasets.py
+-rw-r--r--   0        0        0     3253 2022-09-02 09:16:53.827718 dans-datastation-tools-0.9.0/src/datastation/scripts/delete_role_assignments.py
+-rw-r--r--   0        0        0     2262 2022-09-02 09:16:53.827831 dans-datastation-tools-0.9.0/src/datastation/scripts/find_datasets_with_roleassignment.py
+-rw-r--r--   0        0        0     4904 2022-09-02 09:16:53.827951 dans-datastation-tools-0.9.0/src/datastation/scripts/import_user.py
+-rw-r--r--   0        0        0     1772 2022-09-23 14:38:08.786679 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_copy_batch_to_ingest_area.py
+-rw-r--r--   0        0        0      895 2022-09-23 14:38:08.787347 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_list_events.py
+-rw-r--r--   0        0        0     1701 2022-09-23 14:38:08.787877 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_move_batch_to_ingest_area.py
+-rw-r--r--   0        0        0      435 2022-09-23 14:38:08.788694 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_progress_report.py
+-rw-r--r--   0        0        0      947 2022-09-23 14:38:08.789219 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_start_import.py
+-rw-r--r--   0        0        0     1197 2022-09-23 14:38:08.790032 dans-datastation-tools-0.9.0/src/datastation/scripts/ingest_flow_start_migration.py
+-rw-r--r--   0        0        0     3011 2022-09-02 09:16:53.828079 dans-datastation-tools-0.9.0/src/datastation/scripts/oai_harvest.py
+-rw-r--r--   0        0        0     1369 2022-09-02 09:16:53.828269 dans-datastation-tools-0.9.0/src/datastation/scripts/prestage_files.py
+-rw-r--r--   0        0        0     1692 2022-09-02 09:16:53.828416 dans-datastation-tools-0.9.0/src/datastation/scripts/publish_datasets.py
+-rw-r--r--   0        0        0     1069 2022-09-02 09:16:53.828563 dans-datastation-tools-0.9.0/src/datastation/scripts/reindex_datasets.py
+-rw-r--r--   0        0        0     5684 2022-09-02 09:16:53.828709 dans-datastation-tools-0.9.0/src/datastation/scripts/replace_metadata_field_values.py
+-rw-r--r--   0        0        0     2195 2022-09-02 09:16:53.828830 dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_metadata.py
+-rw-r--r--   0        0        0     1326 2022-09-02 09:16:53.828951 dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_metadata_field.py
+-rwxr-xr-x   0        0        0     1409 2022-09-02 09:16:53.829077 dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_pids.py
+-rw-r--r--   0        0        0     1633 2022-09-02 09:16:53.829192 dans-datastation-tools-0.9.0/src/datastation/scripts/unlock_datasets.py
+-rw-r--r--   0        0        0     1828 2022-09-08 12:14:07.052656 dans-datastation-tools-0.9.0/src/datastation/scripts/update_datacite_records.py
+-rw-r--r--   0        0        0     6130 2022-09-23 14:38:08.790346 dans-datastation-tools-0.9.0/src/datastation/scripts/validate_dans_bag.py
+-rw-r--r--   0        0        0     3770 2022-09-23 14:43:07.605939 dans-datastation-tools-0.9.0/setup.py
+-rw-r--r--   0        0        0      680 2022-09-23 14:43:07.606269 dans-datastation-tools-0.9.0/PKG-INFO
```

### Comparing `dans-datastation-tools-0.8.0/LICENSE` & `dans-datastation-tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/pyproject.toml` & `dans-datastation-tools-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "dans-datastation-tools"
-version = "0.8.0"
+version = "0.9.0"
 description = "Command line utilities for Data Station application management"
 authors = ["DANS-KNAW"]
 packages = [
     { include = "datastation", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 requests = "^2.26.0"
 lxml = "^4.8.0"
 dicttoxml = "^1.7.4"
 pyYAML = "^6.0"
 psycopg = "^3.0.16"
 
-
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
-mkdocs = "==1.3.0"
 psycopg_binary = "^3.0.16"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-dv-dataset-update-datacite-record = "datastation.scripts.update_datacite_records:main"
+dv-dataset-oai-harvest = "datastation.scripts.oai_harvest:main"
+dv-datacite-records-update = "datastation.scripts.update_datacite_records:main"
 dv-dataset-add-role-assignment="datastation.scripts.add_role_assignments:main"
 dv-dataset-delete-draft="datastation.scripts.delete_draft_datasets:main"
 dv-dataset-delete-role-assignment="datastation.scripts.delete_role_assignments:main"
 dv-dataset-destroy-migration-placeholder="datastation.scripts.dataset_destroy_migration_placeholder:main"
 dv-dataset-find-with-role-assignment="datastation.scripts.find_datasets_with_roleassignment:main"
 dv-dataset-publish="datastation.scripts.publish_datasets:main"
 dv-dataset-reindex="datastation.scripts.reindex_datasets:main"
@@ -38,7 +37,15 @@
 dv-dataset-retrieve-metadata="datastation.scripts.retrieve_dataset_metadata:main"
 dv-dataset-retrieve-metadata-field="datastation.scripts.retrieve_dataset_metadata_field:main"
 dv-dataset-unlock = "datastation.scripts.unlock_datasets:main"
 dv-dataverse-oai-harvest = "datastation.scripts.oai_harvest:main"
 dv-dataverse-retrieve-pids="datastation.scripts.retrieve_dataset_pids:main"
 dv-file-prestage="datastation.scripts.prestage_files:main"
 dv-user-import="datastation.scripts.import_user:main"
+
+ingest-flow-copy-batch-to-ingest-area="datastation.scripts.ingest_flow_copy_batch_to_ingest_area:main"
+ingest-flow-move-batch-to-ingest-area="datastation.scripts.ingest_flow_move_batch_to_ingest_area:main"
+ingest-flow-start-migration="datastation.scripts.ingest_flow_start_migration:main"
+ingest-flow-start-import="datastation.scripts.ingest_flow_start_import:main"
+ingest-flow-progress-report="datastation.scripts.ingest_flow_progress_report:main"
+
+dans-bag-validate="datastation.scripts.validate_dans_bag:main"
```

### Comparing `dans-datastation-tools-0.8.0/src/datastation/batch_processing.py` & `dans-datastation-tools-0.9.0/src/datastation/batch_processing.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/config.py` & `dans-datastation-tools-0.9.0/src/datastation/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from os.path import exists
-from shutil import copyfile
 import yaml
 from pkgutil import get_data
 from logging import config as logconfig
 import logging
 
 configuration_file = '.dans-datastation-tools.yml'
 example_configuration_file = 'example-dans-datastation-tools.yml'
@@ -17,14 +16,17 @@
         print("No %s found; instantiating in current directory" % configuration_file)
         with open(configuration_file, 'wb') as f:
             example_cfg = get_data('datastation', example_configuration_file)
             if example_cfg is None:
                 print("WARN: cannot find example-dans-datastation-tools.yml")
             else:
                 f.write(example_cfg)
+                f.flush()
+                logging.debug("Make sure only user can read and write configuration file")
+                os.chmod(path=configuration_file, mode=0o700)
 
 
 def find_config_file():
     return next(filter(lambda p: exists(p), configuration_file_locations), None)
 
 
 def init():
```

### Comparing `dans-datastation-tools-0.8.0/src/datastation/ds_metadatafile.py` & `dans-datastation-tools-0.9.0/src/datastation/ds_metadatafile.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/ds_pidsfile.py` & `dans-datastation-tools-0.9.0/src/datastation/ds_pidsfile.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/dv_api.py` & `dans-datastation-tools-0.9.0/src/datastation/dv_api.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/dv_search.py` & `dans-datastation-tools-0.9.0/src/datastation/dv_search.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/dv_storage.py` & `dans-datastation-tools-0.9.0/src/datastation/dv_storage.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/add_role_assignments.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/add_role_assignments.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/dataset_destroy_migration_placeholder.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/dataset_destroy_migration_placeholder.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/delete_draft_datasets.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/delete_draft_datasets.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/delete_role_assignments.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/delete_role_assignments.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/find_datasets_with_roleassignment.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/find_datasets_with_roleassignment.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/import_user.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/import_user.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/oai_harvest.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/oai_harvest.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/prestage_files.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/prestage_files.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/publish_datasets.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/publish_datasets.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/reindex_datasets.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/reindex_datasets.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/replace_metadata_field_values.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/replace_metadata_field_values.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_metadata.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_metadata_field.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_metadata_field.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/retrieve_dataset_pids.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/retrieve_dataset_pids.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/unlock_datasets.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/unlock_datasets.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/src/datastation/scripts/update_datacite_records.py` & `dans-datastation-tools-0.9.0/src/datastation/scripts/update_datacite_records.py`

 * *Files identical despite different names*

### Comparing `dans-datastation-tools-0.8.0/setup.py` & `dans-datastation-tools-0.9.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,49 +14,63 @@
 ['dicttoxml>=1.7.4,<2.0.0',
  'lxml>=4.8.0,<5.0.0',
  'psycopg>=3.0.16,<4.0.0',
  'pyYAML>=6.0,<7.0',
  'requests>=2.26.0,<3.0.0']
 
 entry_points = \
-{'console_scripts': ['dv-dataset-add-role-assignment = '
+{'console_scripts': ['dans-bag-validate = '
+                     'datastation.scripts.validate_dans_bag:main',
+                     'dv-datacite-records-update = '
+                     'datastation.scripts.update_datacite_records:main',
+                     'dv-dataset-add-role-assignment = '
                      'datastation.scripts.add_role_assignments:main',
                      'dv-dataset-delete-draft = '
                      'datastation.scripts.delete_draft_datasets:main',
                      'dv-dataset-delete-role-assignment = '
                      'datastation.scripts.delete_role_assignments:main',
                      'dv-dataset-destroy-migration-placeholder = '
                      'datastation.scripts.dataset_destroy_migration_placeholder:main',
                      'dv-dataset-find-with-role-assignment = '
                      'datastation.scripts.find_datasets_with_roleassignment:main',
+                     'dv-dataset-oai-harvest = '
+                     'datastation.scripts.oai_harvest:main',
                      'dv-dataset-publish = '
                      'datastation.scripts.publish_datasets:main',
                      'dv-dataset-reindex = '
                      'datastation.scripts.reindex_datasets:main',
                      'dv-dataset-replace-metadata-field-values = '
                      'datastation.scripts.replace_metadata_field_values:main',
                      'dv-dataset-retrieve-metadata = '
                      'datastation.scripts.retrieve_dataset_metadata:main',
                      'dv-dataset-retrieve-metadata-field = '
                      'datastation.scripts.retrieve_dataset_metadata_field:main',
                      'dv-dataset-unlock = '
                      'datastation.scripts.unlock_datasets:main',
-                     'dv-dataset-update-datacite-record = '
-                     'datastation.scripts.update_datacite_records:main',
                      'dv-dataverse-oai-harvest = '
                      'datastation.scripts.oai_harvest:main',
                      'dv-dataverse-retrieve-pids = '
                      'datastation.scripts.retrieve_dataset_pids:main',
                      'dv-file-prestage = '
                      'datastation.scripts.prestage_files:main',
-                     'dv-user-import = datastation.scripts.import_user:main']}
+                     'dv-user-import = datastation.scripts.import_user:main',
+                     'ingest-flow-copy-batch-to-ingest-area = '
+                     'datastation.scripts.ingest_flow_copy_batch_to_ingest_area:main',
+                     'ingest-flow-move-batch-to-ingest-area = '
+                     'datastation.scripts.ingest_flow_move_batch_to_ingest_area:main',
+                     'ingest-flow-progress-report = '
+                     'datastation.scripts.ingest_flow_progress_report:main',
+                     'ingest-flow-start-import = '
+                     'datastation.scripts.ingest_flow_start_import:main',
+                     'ingest-flow-start-migration = '
+                     'datastation.scripts.ingest_flow_start_migration:main']}
 
 setup_kwargs = {
     'name': 'dans-datastation-tools',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Command line utilities for Data Station application management',
     'long_description': None,
     'author': 'DANS-KNAW',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dans-datastation-tools-0.8.0/PKG-INFO` & `dans-datastation-tools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dans-datastation-tools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command line utilities for Data Station application management
 Author: DANS-KNAW
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

