# Comparing `tmp/gaohn-common-utils-0.0.57.tar.gz` & `tmp/gaohn-common-utils-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.57.tar", last modified: Wed Jun 14 13:48:09 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.58.tar", last modified: Thu Jun 15 07:00:18 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.57.tar` & `gaohn-common-utils-0.0.58.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.681422 gaohn-common-utils-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 13:48:09.681422 gaohn-common-utils-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.673421 gaohn-common-utils-0.0.57/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.673421 gaohn-common-utils-0.0.57/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.669422 gaohn-common-utils-0.0.57/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.673421 gaohn-common-utils-0.0.57/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.673421 gaohn-common-utils-0.0.57/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.677421 gaohn-common-utils-0.0.57/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.677421 gaohn-common-utils-0.0.57/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.677421 gaohn-common-utils-0.0.57/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.669422 gaohn-common-utils-0.0.57/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.677421 gaohn-common-utils-0.0.57/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.677421 gaohn-common-utils-0.0.57/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:48:09.681422 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 13:48:09.000000 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 13:48:09.000000 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:48:09.000000 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 13:48:09.000000 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 13:48:09.000000 gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 13:47:50.000000 gaohn-common-utils-0.0.57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:48:09.681422 gaohn-common-utils-0.0.57/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.586228 gaohn-common-utils-0.0.58/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:00:18.000000 gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:00:00.000000 gaohn-common-utils-0.0.58/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:00:18.590228 gaohn-common-utils-0.0.58/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.57/LICENSE` & `gaohn-common-utils-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/PKG-INFO` & `gaohn-common-utils-0.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.57
+Version: 0.0.58
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.57/README.md` & `gaohn-common-utils-0.0.58/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.58/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.58/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.58/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/core/base.py` & `gaohn-common-utils-0.0.58/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/core/common.py` & `gaohn-common-utils-0.0.58/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.58/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.58/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/core/logger.py` & `gaohn-common-utils-0.0.58/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.58/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.58/common_utils/versioning/dvc/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,33 +41,58 @@
 
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
         self.metadata_file: Path
 
     @property
     def remote_dvc_dir(self) -> str:
-        """Always fixed to gaohn-dvc."""
+        """Always fixed to gaohn-dvc. Immutable just like how dvc always uses .dvc."""
         return "gaohn-dvc"
 
+    @property
+    def remote_project_name(self) -> str:
+        return self.storage.bucket_name
+
     def _create_gitignore(self, pattern: str) -> None:
         gitignore_file = self.data_dir / ".gitignore"
         if not gitignore_file.exists():
             with open(gitignore_file, "w", encoding="utf-8") as file:
                 file.write(pattern)
         else:
             with open(gitignore_file, "a+", encoding="utf-8") as file:
                 file.seek(0)
                 if pattern not in file.read():
                     file.write("\n" + pattern)
 
     def _get_cache_file_path(self, filename: str) -> Path:
         return self.cache_dir / filename
 
+    def _get_metadata_file_path(self, filename: str) -> Path:
+        """
+        Constructs a Path object for a metadata file in the data directory.
+
+        Args:
+            filename (str): Name of the file.
+
+        Returns:
+            Path: Path object for the metadata file in the data directory.
+        """
+        return self.data_dir / f"{filename}.json"
+
     def _load_metadata(self, filename: str) -> Dict[str, str]:
-        metadata_file = self.data_dir / f"{filename}.json"
+        """
+        Loads the metadata for a file from its metadata JSON file.
+
+        Args:
+            filename (str): Name of the file.
+
+        Returns:
+            Dict[str, str]: Metadata dictionary for the file.
+        """
+        metadata_file = self._get_metadata_file_path(filename)
         with metadata_file.open("r") as file:
             return json.load(file)
 
     def _calculate_md5(self, filepath: str) -> str:
         hash_md5 = hashlib.md5()
         with open(filepath, "rb") as file:
             for chunk in iter(lambda: file.read(4096), b""):
@@ -84,14 +109,15 @@
 
         shutil.copy(filepath, cache_filepath)
 
         metadata = {
             "filename": filename,
             "filepath": str(cache_filepath),
             "extension": extension,
+            "remote_project_name": self.remote_project_name,
             "md5": md5,
         }
         self.metadata_file = self.data_dir / f"{filename}.json"
 
         with self.metadata_file.open("w") as file:
             json.dump(metadata, file, indent=4)
```

### Comparing `gaohn-common-utils-0.0.57/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.58/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.57
+Version: 0.0.58
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.57/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.58/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.57/pyproject.toml` & `gaohn-common-utils-0.0.58/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.57"
+version = "0.0.58"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

