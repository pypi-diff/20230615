# Comparing `tmp/prefect-gcp-0.4.2.tar.gz` & `tmp/prefect-gcp-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-b22u9uqx/prefect-gcp-0.4.2.tar", last modified: Thu May 25 19:23:55 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-igqgbo2s/prefect-gcp-0.4.3.tar", last modified: Thu Jun 15 14:42:53 2023, max compression
```

## Comparing `prefect-gcp-0.4.2.tar` & `prefect-gcp-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45746 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/prefect_gcp/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:23:55.000000 prefect-gcp-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-25 19:22:10.000000 prefect-gcp-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/prefect_gcp/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:42:53.000000 prefect-gcp-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:41:08.000000 prefect-gcp-0.4.3/versioneer.py
```

### Comparing `prefect-gcp-0.4.2/LICENSE` & `prefect-gcp-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/PKG-INFO` & `prefect-gcp-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.2
+Version: 0.4.3
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.2 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.3 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.2/README.md` & `prefect-gcp-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/aiplatform.py` & `prefect-gcp-0.4.3/prefect_gcp/aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/bigquery.py` & `prefect-gcp-0.4.3/prefect_gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/cloud_run.py` & `prefect-gcp-0.4.3/prefect_gcp/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/cloud_storage.py` & `prefect-gcp-0.4.3/prefect_gcp/cloud_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,19 +908,17 @@
         """
 
         bucket_path = self._join_bucket_folder()
         self.logger.info(f"Listing folders in bucket {bucket_path}.")
 
         blobs = await self.list_blobs(folder)
         # gets all folders with full path
-        folders = {
-            str(PurePosixPath(blob.name).parent).replace(".", "") for blob in blobs
-        }
+        folders = {str(PurePosixPath(blob.name).parent) for blob in blobs}
 
-        return list(folders)
+        return [folder for folder in folders if folder != "."]
 
     @sync_compatible
     async def download_object_to_path(
         self,
         from_path: str,
         to_path: Optional[Union[str, Path]] = None,
         **download_kwargs: Dict[str, Any],
```

### Comparing `prefect-gcp-0.4.2/prefect_gcp/credentials.py` & `prefect-gcp-0.4.3/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/projects/steps.py` & `prefect-gcp-0.4.3/prefect_gcp/deployments/steps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,99 @@
 """
-Prefect project steps for code storage in and retrieval from Google Cloud Storage.
+Prefect deployment steps for code storage in and retrieval from Google Cloud Storage.
 """
 from pathlib import Path, PurePosixPath
 from typing import Dict, Optional
 
 import google.auth
 from google.cloud.storage import Client as StorageClient
 from google.oauth2.service_account import Credentials
+from prefect._internal.compatibility.deprecated import deprecated_callable
 from prefect.utilities.filesystem import filter_files, relative_path_to_current_platform
 from typing_extensions import TypedDict
 
 
-class PushProjectToGcsOutput(TypedDict):
+class PushToGcsOutput(TypedDict):
     """
-    The output of the `push_project_to_gcs` step.
+    The output of the `push_to_gcs` step.
     """
 
     bucket: str
     folder: str
 
 
-class PullProjectFromGcsOutput(TypedDict):
+@deprecated_callable(start_date="Jun 2023", help="Use `PushToGcsOutput` instead.")
+class PushProjectToGcsOutput(PushToGcsOutput):
+    """Deprecated. Use `PushToGcsOutput` instead."""
+
+
+class PullFromGcsOutput(TypedDict):
     """
-    The output of the `pull_project_from_gcs` step.
+    The output of the `pull_from_gcs` step.
     """
 
     bucket: str
     folder: str
     directory: str
 
 
-def push_project_to_gcs(
+@deprecated_callable(start_date="Jun 2023", help="Use `PullFromGcsOutput` instead.")
+class PullProjectFromGcsOutput(PullFromGcsOutput):
+    """Deprecated. Use `PullFromGcsOutput` instead."""
+
+
+def push_to_gcs(
     bucket: str,
     folder: str,
     project: Optional[str] = None,
     credentials: Optional[Dict] = None,
     ignore_file=".prefectignore",
-) -> PushProjectToGcsOutput:
+) -> PushToGcsOutput:
     """
     Pushes the contents of the current working directory to a GCS bucket,
     excluding files and folders specified in the ignore_file.
 
     Args:
-        bucket: The name of the GCS bucket where the project files will be uploaded.
-        folder: The folder in the GCS bucket where the project files will be uploaded.
+        bucket: The name of the GCS bucket where files will be uploaded.
+        folder: The folder in the GCS bucket where files will be uploaded.
         project: The GCP project the bucket belongs to. If not provided, the project
             will be inferred from the credentials or the local environment.
         credentials: A dictionary containing the service account information and project
             used for authentication. If not provided, the application default
             credentials will be used.
         ignore_file: The name of the file containing ignore patterns.
 
     Returns:
-        A dictionary containing the bucket and folder where the project was uploaded.
+        A dictionary containing the bucket and folder where files were uploaded.
 
     Examples:
-        Push a project to an GCS bucket:
+        Push to a GCS bucket:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.push_project_to_gcs:
+            - prefect_gcp.deployments.steps.push_to_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-project
         ```
 
-        Push a project to an GCS bucket using credentials stored in a block:
+        Push  to a GCS bucket using credentials stored in a block:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.push_project_to_gcs:
+            - prefect_gcp.deployments.steps.push_to_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-folder
                 credentials: "{{ prefect.blocks.gcp-credentials.dev-credentials }}"
         ```
 
-        Push a project to an GCS bucket using credentials stored in a service account
+        Push to a GCS bucket using credentials stored in a service account
         file:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.push_project_to_gcs:
+            - prefect_gcp.deployments.steps.push_to_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-folder
                 credentials:
                     project: my-project
                     service_account_file: /path/to/service_account.json
         ```
@@ -131,60 +142,67 @@
 
     return {
         "bucket": bucket,
         "folder": folder,
     }
 
 
-def pull_project_from_gcs(
+@deprecated_callable(start_date="Jun 2023", help="Use `push_to_gcs` instead.")
+def push_project_to_gcs(*args, **kwargs) -> PushToGcsOutput:
+    """
+    Deprecated. Use `push_to_gcs` instead.
+    """
+    return push_to_gcs(*args, **kwargs)
+
+
+def pull_from_gcs(
     bucket: str,
     folder: str,
     project: Optional[str] = None,
     credentials: Optional[Dict] = None,
 ) -> PullProjectFromGcsOutput:
     """
     Pulls the contents of a project from an GCS bucket to the current working directory.
 
     Args:
-        bucket: The name of the GCS bucket where the project files are stored.
-        folder: The folder in the GCS bucket where the project files are stored.
+        bucket: The name of the GCS bucket where files are stored.
+        folder: The folder in the GCS bucket where files are stored.
         project: The GCP project the bucket belongs to. If not provided, the project will be
             inferred from the credentials or the local environment.
         credentials: A dictionary containing the service account information and project
             used for authentication. If not provided, the application default
             credentials will be used.
 
     Returns:
-        A dictionary containing the bucket, folder, and local directory where the
-            project files were downloaded.
+        A dictionary containing the bucket, folder, and local directory where files were downloaded.
 
     Examples:
-        Pull a project from GCS using the default environment credentials:
+        Pull from GCS using the default environment credentials:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.pull_project_from_gcs:
+            - prefect_gcp.deployments.steps.pull_from_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-folder
         ```
 
-        Pull a project from GCS using credentials stored in a block:
+        Pull from GCS using credentials stored in a block:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.pull_project_from_gcs:
+            - prefect_gcp.deployments.steps.pull_from_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-folder
                 credentials: "{{ prefect.blocks.gcp-credentials.dev-credentials }}"
         ```
 
-        Pull from a project to an GCS bucket using credentials stored in a service account file:
+        Pull from to an GCS bucket using credentials stored in a service account file:
         ```yaml
         build:
-            - prefect_gcp.projects.steps.pull_project_from_gcs:
+            - prefect_gcp.deployments.steps.pull_from_gcs:
                 requires: prefect-gcp
                 bucket: my-bucket
                 folder: my-folder
                 credentials:
                     project: my-project
                     service_account_file: /path/to/service_account.json
         ```
@@ -225,7 +243,15 @@
         blob.download_to_filename(local_blob_download_path)
 
     return {
         "bucket": bucket,
         "folder": folder,
         "directory": str(local_path),
     }
+
+
+@deprecated_callable(start_date="Jun 2023", help="Use `pull_from_gcs` instead.")
+def pull_project_from_gcs(*args, **kwargs) -> PullProjectFromGcsOutput:
+    """
+    Deprecated. Use `pull_from_gcs` instead.
+    """
+    return pull_from_gcs(*args, **kwargs)
```

### Comparing `prefect-gcp-0.4.2/prefect_gcp/secret_manager.py` & `prefect-gcp-0.4.3/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp/worker.py` & `prefect-gcp-0.4.3/prefect_gcp/worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/prefect_gcp.egg-info/PKG-INFO` & `prefect-gcp-0.4.3/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.2
+Version: 0.4.3
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.2 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.3 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.2/prefect_gcp.egg-info/SOURCES.txt` & `prefect-gcp-0.4.3/prefect_gcp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 prefect_gcp/worker.py
 prefect_gcp.egg-info/PKG-INFO
 prefect_gcp.egg-info/SOURCES.txt
 prefect_gcp.egg-info/dependency_links.txt
 prefect_gcp.egg-info/entry_points.txt
 prefect_gcp.egg-info/requires.txt
 prefect_gcp.egg-info/top_level.txt
-prefect_gcp/projects/__init__.py
-prefect_gcp/projects/steps.py
+prefect_gcp/deployments/__init__.py
+prefect_gcp/deployments/steps.py
 tests/test_aiplatform.py
 tests/test_bigquery.py
 tests/test_block_standards.py
 tests/test_cloud_run.py
 tests/test_cloud_storage.py
 tests/test_credentials.py
 tests/test_secret_manager.py
```

### Comparing `prefect-gcp-0.4.2/prefect_gcp.egg-info/requires.txt` & `prefect-gcp-0.4.3/prefect_gcp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/setup.cfg` & `prefect-gcp-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/setup.py` & `prefect-gcp-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_aiplatform.py` & `prefect-gcp-0.4.3/tests/test_aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_bigquery.py` & `prefect-gcp-0.4.3/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_block_standards.py` & `prefect-gcp-0.4.3/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_cloud_run.py` & `prefect-gcp-0.4.3/tests/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_cloud_storage.py` & `prefect-gcp-0.4.3/tests/test_cloud_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
         # check all files exist on returned paths
         for file_path in actual:
             assert os.path.isfile(file_path)
 
         # blob.txt, base_folder/nested_blob.txt, base_folder/sub_folder/nested_blob.txt
         if not prefix:
-            assert len(actual) == 3
+            assert len(actual) == 4
         # base_folder/sub_folder/nested_blob.txt
         elif prefix == "base_folder/sub_folder":
             assert len(actual) == 1
         # base_folder/nested_blob.txt, base_folder/sub_folder/nested_blob.txt
         elif prefix == "base_folder" or prefix == "base_folder/":
             assert len(actual) == 2
         else:
@@ -230,23 +230,37 @@
         return pd.DataFrame.from_dict(
             {
                 "name": ["John Doe", "Jane Doe", "Johny", "Jane"],
                 "username": ["john.doe", "jane.doe", "johny", "jane"],
             }
         )
 
+    def test_list_folders_root_folder(self, gcs_bucket_no_bucket_folder):
+        folders = gcs_bucket_no_bucket_folder.list_folders()
+        assert len(folders) == 3
+        assert set(folders) == {
+            "base_folder",
+            "base_folder/sub_folder",
+            "dotted.folder",
+        }
+
     def test_list_folders_with_root_only(self, gcs_bucket_with_bucket_folder):
-        blobs = gcs_bucket_with_bucket_folder.list_folders()
-        assert len(blobs) == 2
-        assert set(blobs) == {"base_folder", "base_folder/sub_folder"}
+        folders = gcs_bucket_with_bucket_folder.list_folders()
+        assert len(folders) == 2
+        assert set(folders) == {"base_folder", "base_folder/sub_folder"}
 
     def test_list_folders_with_sub_folders(self, gcs_bucket_with_bucket_folder):
-        blobs = gcs_bucket_with_bucket_folder.list_folders("sub_folder/")
-        assert len(blobs) == 1
-        assert blobs[0] == "base_folder/sub_folder"
+        folders = gcs_bucket_with_bucket_folder.list_folders("sub_folder/")
+        assert len(folders) == 1
+        assert folders[0] == "base_folder/sub_folder"
+
+    def test_list_folders_with_dotted_folders(self, gcs_bucket_no_bucket_folder):
+        folders = gcs_bucket_no_bucket_folder.list_folders("dotted.folder/")
+        assert len(folders) == 1
+        assert folders[0] == "dotted.folder"
 
     def test_list_blobs(self, gcs_bucket_no_bucket_folder):
         blobs = gcs_bucket_no_bucket_folder.list_blobs(folder="base_folder/")
         assert len(blobs) == 2
         assert blobs[0].name == "base_folder/nested_blob.txt"
         assert blobs[1].name == "base_folder/sub_folder/nested_blob.txt"
 
@@ -260,18 +274,19 @@
         # now test with sub_folder
         blobs = gcs_bucket_with_bucket_folder.list_blobs(folder="sub_folder")
         assert len(blobs) == 1
         assert blobs[0].name == "base_folder/sub_folder/nested_blob.txt"
 
     def test_list_blobs_root_folder(self, gcs_bucket_no_bucket_folder):
         blobs = gcs_bucket_no_bucket_folder.list_blobs(folder="")
-        assert len(blobs) == 3
+        assert len(blobs) == 4
         assert blobs[0].name == "blob.txt"
         assert blobs[1].name == "base_folder/nested_blob.txt"
         assert blobs[2].name == "base_folder/sub_folder/nested_blob.txt"
+        assert blobs[3].name == "dotted.folder/nested_blob.txt"
 
     def test_download_object_to_path_default(
         self, gcs_bucket_with_bucket_folder, tmp_path
     ):
         os.chdir(tmp_path)
         from_path = tmp_path / "from_path"
         output_to_path = gcs_bucket_with_bucket_folder.download_object_to_path(
```

### Comparing `prefect-gcp-0.4.2/tests/test_credentials.py` & `prefect-gcp-0.4.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_secret_manager.py` & `prefect-gcp-0.4.3/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.2/tests/test_worker.py` & `prefect-gcp-0.4.3/tests/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             },
         },
     }
 
 
 @pytest.fixture
 def flow_run():
-    return FlowRun(name="my-flow-run-name")
+    return FlowRun(flow_id=uuid.uuid4(), name="my-flow-run-name")
 
 
 @pytest.fixture
 def cloud_run_worker_job_config(service_account_info, jobs_body):
     return CloudRunWorkerJobConfiguration(
         name="my-job-name",
         image="gcr.io//not-a/real-image",
```

### Comparing `prefect-gcp-0.4.2/versioneer.py` & `prefect-gcp-0.4.3/versioneer.py`

 * *Files identical despite different names*

