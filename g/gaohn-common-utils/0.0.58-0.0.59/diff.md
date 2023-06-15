# Comparing `tmp/gaohn-common-utils-0.0.58.tar.gz` & `tmp/gaohn-common-utils-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.58.tar", last modified: Thu Jun 15 07:00:18 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.59.tar", last modified: Thu Jun 15 07:25:50 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.58.tar` & `gaohn-common-utils-0.0.59.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.58/LICENSE` & `gaohn-common-utils-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/PKG-INFO` & `gaohn-common-utils-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.58
+Version: 0.0.59
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.58/README.md` & `gaohn-common-utils-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.59/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/core/base.py` & `gaohn-common-utils-0.0.59/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/core/common.py` & `gaohn-common-utils-0.0.59/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.59/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.59/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/core/logger.py` & `gaohn-common-utils-0.0.59/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.59/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.59/common_utils/versioning/dvc/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,45 +17,55 @@
     ├── interim
     ├── processed
     └── raw
         ├── filtered_movies_incremental.csv             # filename
         └── filtered_movies_incremental.csv.json        # metadata for filename
 
     REMOTE DVC TREE
-    gaohn/                                              # bucket
-    └── imdb                                            # remote project name
-        └── gaohn-dvc                                   # remote dvc name
+    gaohn/                                              # remote_bucket_name
+    └── imdb                                            # remote_bucket_project_name
+        └── gaohn-dvc                                   # remote_dvc_dir_name
             ├── 1234567890                              # md5 hash for raw/filtered_movies_incremental.csv
             └── filtered_movies_incremental.csv.json
     """
 
     def __init__(
         self,
         storage: Storage,
+        remote_bucket_project_name: str,
         data_dir: str = "./data",
         cache_dir: str = ".cache",
     ) -> None:
         self.storage = storage
+        self.remote_bucket_project_name = remote_bucket_project_name
 
         self.data_dir = Path(data_dir)
         self.cache_dir = Path(cache_dir)
 
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
         self.metadata_file: Path
 
     @property
-    def remote_dvc_dir(self) -> str:
+    def remote_dvc_dir_name(self) -> str:
         """Always fixed to gaohn-dvc. Immutable just like how dvc always uses .dvc."""
         return "gaohn-dvc"
 
     @property
-    def remote_project_name(self) -> str:
+    def remote_bucket_name(self) -> str:
+        """It is important to know that the Storage object has `bucket_name` as an attribute."""
         return self.storage.bucket_name
 
+    @property
+    def remote_bucket_project_name(self) -> str:
+        return self.remote_bucket_project_name
+
+    def _get_destination_blob_name(self, md5: str) -> str:
+        return f"{self.remote_bucket_project_name}/{self.remote_dvc_dir_name}/{md5}"
+
     def _create_gitignore(self, pattern: str) -> None:
         gitignore_file = self.data_dir / ".gitignore"
         if not gitignore_file.exists():
             with open(gitignore_file, "w", encoding="utf-8") as file:
                 file.write(pattern)
         else:
             with open(gitignore_file, "a+", encoding="utf-8") as file:
@@ -109,41 +119,45 @@
 
         shutil.copy(filepath, cache_filepath)
 
         metadata = {
             "filename": filename,
             "filepath": str(cache_filepath),
             "extension": extension,
-            "remote_project_name": self.remote_project_name,
+            "remote_bucket_name": self.remote_project_name,
             "md5": md5,
         }
         self.metadata_file = self.data_dir / f"{filename}.json"
 
         with self.metadata_file.open("w") as file:
             json.dump(metadata, file, indent=4)
 
         self._create_gitignore(filename)
 
         return metadata
 
-    def push(self, filepath: str, destination_blob_name: str) -> None:
+    def push(self, filepath: str) -> None:
         filepath = Path(filepath)
         filename = filepath.name
         metadata = self._load_metadata(filename)
         cache_filepath = metadata["filepath"]
 
-        # this effectively uploads the cached file to the remote storage
+        md5 = metadata["md5"]
+
+        destination_blob_name = self._get_destination_blob_name(md5)
+
+        # This effectively uploads the cached file to the remote storage
         self.storage.upload_blob(
             source_file_name=cache_filepath, destination_blob_name=destination_blob_name
         )
 
-    def pull(self, filename: str, remote_project_name: str) -> None:
+    def pull(self, filename: str, remote_bucket_project_name: str) -> None:
         metadata = self._load_metadata(filename)
         source_blob_name = (
-            f"{remote_project_name}/{self.remote_dvc_dir}/{metadata['md5']}"
+            f"{remote_bucket_project_name}/{self.remote_dvc_dir_name}/{metadata['md5']}"
         )
         self.storage.download_blob(source_blob_name, self.data_dir / filename)
 
     def checkout(self, filename: str) -> None:
         metadata = self._load_metadata(filename)
         if metadata["filename"] == filename:
             shutil.copy(metadata["filepath"], str(self.data_dir / filename))
```

### Comparing `gaohn-common-utils-0.0.58/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.59/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.58
+Version: 0.0.59
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.58/pyproject.toml` & `gaohn-common-utils-0.0.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.58"
+version = "0.0.59"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

