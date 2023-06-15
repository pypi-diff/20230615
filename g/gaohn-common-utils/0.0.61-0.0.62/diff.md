# Comparing `tmp/gaohn-common-utils-0.0.61.tar.gz` & `tmp/gaohn-common-utils-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.61.tar", last modified: Thu Jun 15 07:32:58 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.62.tar", last modified: Thu Jun 15 11:03:48 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.61.tar` & `gaohn-common-utils-0.0.62.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.672674 gaohn-common-utils-0.0.61/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:32:58.672674 gaohn-common-utils-0.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.668674 gaohn-common-utils-0.0.61/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.668674 gaohn-common-utils-0.0.61/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.668674 gaohn-common-utils-0.0.61/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.664674 gaohn-common-utils-0.0.61/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.668674 gaohn-common-utils-0.0.61/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.668674 gaohn-common-utils-0.0.61/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:32:58.672674 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 07:32:58.000000 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 07:32:58.000000 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:32:58.000000 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 07:32:58.000000 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 07:32:58.000000 gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 07:32:37.000000 gaohn-common-utils-0.0.61/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:32:58.672674 gaohn-common-utils-0.0.61/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.657107 gaohn-common-utils-0.0.62/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.657107 gaohn-common-utils-0.0.62/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.657107 gaohn-common-utils-0.0.62/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.657107 gaohn-common-utils-0.0.62/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:03:48.000000 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 11:03:48.000000 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:03:48.000000 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:03:48.000000 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 11:03:48.000000 gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 11:03:16.000000 gaohn-common-utils-0.0.62/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:03:48.661107 gaohn-common-utils-0.0.62/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.61/LICENSE` & `gaohn-common-utils-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/PKG-INFO` & `gaohn-common-utils-0.0.62/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.61
+Version: 0.0.62
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.61/README.md` & `gaohn-common-utils-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.62/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.62/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.62/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/core/base.py` & `gaohn-common-utils-0.0.62/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/core/common.py` & `gaohn-common-utils-0.0.62/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.62/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.62/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/core/logger.py` & `gaohn-common-utils-0.0.62/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.62/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.62/common_utils/versioning/dvc/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     def _calculate_md5(self, filepath: str) -> str:
         hash_md5 = hashlib.md5()
         with open(filepath, "rb") as file:
             for chunk in iter(lambda: file.read(4096), b""):
                 hash_md5.update(chunk)
         return hash_md5.hexdigest()
 
-    def add(self, filepath: str) -> Dict[str, str]:
+    def add(self, filepath: str, save_metadata: bool = True) -> Dict[str, str]:
         filepath = Path(filepath)
         filename = filepath.name
         extension = filepath.suffix
 
         md5 = self._calculate_md5(str(filepath))
         cache_filepath = self.cache_dir / md5
 
@@ -125,18 +125,18 @@
             "extension": extension,
             "remote_bucket_name": self.remote_bucket_name,
             "remote_bucket_project_name": self.remote_bucket_project_name,
             "remote_dvc_dir_name": self.remote_dvc_dir_name,
             "md5": md5,
         }
 
-        self.metadata_file = self.data_dir / f"{filename}.json"
-
-        with self.metadata_file.open("w") as file:
-            json.dump(metadata, file, indent=4)
+        if save_metadata:
+            self.metadata_file = self.data_dir / f"{filename}.json"
+            with self.metadata_file.open("w") as file:
+                json.dump(metadata, file, indent=4)
 
         self._create_gitignore(filename)
 
         return metadata
 
     def push(self, filepath: str) -> None:
         filepath = Path(filepath)
```

### Comparing `gaohn-common-utils-0.0.61/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.62/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.61
+Version: 0.0.62
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.61/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.62/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.61/pyproject.toml` & `gaohn-common-utils-0.0.62/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.61"
+version = "0.0.62"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

