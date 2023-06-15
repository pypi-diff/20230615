# Comparing `tmp/gaohn-common-utils-0.0.59.tar.gz` & `tmp/gaohn-common-utils-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.59.tar", last modified: Thu Jun 15 07:25:50 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.60.tar", last modified: Thu Jun 15 07:31:00 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.59.tar` & `gaohn-common-utils-0.0.60.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.548148 gaohn-common-utils-0.0.59/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:25:50.000000 gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:25:33.000000 gaohn-common-utils-0.0.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:25:50.552148 gaohn-common-utils-0.0.59/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.885999 gaohn-common-utils-0.0.60/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:31:00.000000 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:31:00.000000 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:31:00.000000 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:31:00.000000 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:31:00.000000 gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:30:43.000000 gaohn-common-utils-0.0.60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:31:00.889999 gaohn-common-utils-0.0.60/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.59/LICENSE` & `gaohn-common-utils-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/PKG-INFO` & `gaohn-common-utils-0.0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.59
+Version: 0.0.60
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.59/README.md` & `gaohn-common-utils-0.0.60/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.60/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.60/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.60/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/core/base.py` & `gaohn-common-utils-0.0.60/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/core/common.py` & `gaohn-common-utils-0.0.60/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.60/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.60/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/core/logger.py` & `gaohn-common-utils-0.0.60/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.60/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.60/common_utils/versioning/dvc/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self,
         storage: Storage,
         remote_bucket_project_name: str,
         data_dir: str = "./data",
         cache_dir: str = ".cache",
     ) -> None:
         self.storage = storage
-        self.remote_bucket_project_name = remote_bucket_project_name
+        self._remote_bucket_project_name = remote_bucket_project_name
 
         self.data_dir = Path(data_dir)
         self.cache_dir = Path(cache_dir)
 
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
         self.metadata_file: Path
@@ -53,15 +53,15 @@
     @property
     def remote_bucket_name(self) -> str:
         """It is important to know that the Storage object has `bucket_name` as an attribute."""
         return self.storage.bucket_name
 
     @property
     def remote_bucket_project_name(self) -> str:
-        return self.remote_bucket_project_name
+        return self._remote_bucket_project_name
 
     def _get_destination_blob_name(self, md5: str) -> str:
         return f"{self.remote_bucket_project_name}/{self.remote_dvc_dir_name}/{md5}"
 
     def _create_gitignore(self, pattern: str) -> None:
         gitignore_file = self.data_dir / ".gitignore"
         if not gitignore_file.exists():
```

### Comparing `gaohn-common-utils-0.0.59/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.60/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.59
+Version: 0.0.60
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.59/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.60/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.59/pyproject.toml` & `gaohn-common-utils-0.0.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.59"
+version = "0.0.60"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

