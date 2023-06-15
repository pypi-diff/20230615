# Comparing `tmp/oci_mlflow-1.0.1-py3-none-any.whl.zip` & `tmp/oci_mlflow-1.0b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 25021 bytes, number of entries: 17
--rw-r--r--  2.0 unx      938 b- defN 23-Jun-15 21:31 oci_mlflow/__init__.py
--rw-r--r--  2.0 unx    21498 b- defN 23-Jun-15 21:31 oci_mlflow/deployment.py
--rw-r--r--  2.0 unx     7310 b- defN 23-Jun-15 21:31 oci_mlflow/oci_object_storage.py
--rw-r--r--  2.0 unx    26088 b- defN 23-Jun-15 21:31 oci_mlflow/project.py
--rw-r--r--  2.0 unx     4448 b- defN 23-Jun-15 21:31 oci_mlflow/telemetry_logging.py
--rw-r--r--  2.0 unx     9236 b- defN 23-Jun-15 21:31 oci_mlflow/utils.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-15 21:31 oci_mlflow/version.json
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 21:31 oci_mlflow/templates/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Jun-15 21:31 oci_mlflow/templates/project_description.jinja2
--rw-r--r--  2.0 unx      163 b- defN 23-Jun-15 21:31 oci_mlflow/templates/runtime.yaml.jinja2
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-15 21:31 oci_mlflow/templates/score.py.jinja2
--rw-r--r--  2.0 unx     1860 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4228 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      243 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1452 b- defN 23-Jun-15 21:31 oci_mlflow-1.0.1.dist-info/RECORD
-17 files, 79214 bytes uncompressed, 22611 bytes compressed:  71.5%
+Zip file size: 23367 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      938 b- defN 23-May-17 00:36 oci_mlflow/__init__.py
+-rw-r--r--  2.0 unx    21498 b- defN 23-May-17 00:36 oci_mlflow/deployment.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-May-17 00:36 oci_mlflow/oci_object_storage.py
+-rw-r--r--  2.0 unx    26088 b- defN 23-May-17 00:36 oci_mlflow/project.py
+-rw-r--r--  2.0 unx     4448 b- defN 23-May-17 00:36 oci_mlflow/telemetry_logging.py
+-rw-r--r--  2.0 unx     9236 b- defN 23-May-17 00:36 oci_mlflow/utils.py
+-rwxrwxrwx  2.0 unx       25 b- defN 23-May-17 00:36 oci_mlflow/version.json
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 00:36 oci_mlflow/templates/__init__.py
+-rwxrwxrwx  2.0 unx     1200 b- defN 23-May-17 00:36 oci_mlflow/templates/project_description.jinja2
+-rwxrwxrwx  2.0 unx      163 b- defN 23-May-17 00:36 oci_mlflow/templates/runtime.yaml.jinja2
+-rwxrwxrwx  2.0 unx      422 b- defN 23-May-17 00:36 oci_mlflow/templates/score.py.jinja2
+-rwxrwxrwx  2.0 unx     1860 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2156 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      243 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1452 b- defN 23-May-17 00:40 oci_mlflow-1.0b0.dist-info/RECORD
+17 files, 74067 bytes uncompressed, 20957 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: oci_mlflow/templates/runtime.yaml.jinja2
 Comment: 
 
 Filename: oci_mlflow/templates/score.py.jinja2
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/LICENSE.txt
+Filename: oci_mlflow-1.0b0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/METADATA
+Filename: oci_mlflow-1.0b0.dist-info/METADATA
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/WHEEL
+Filename: oci_mlflow-1.0b0.dist-info/WHEEL
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/entry_points.txt
+Filename: oci_mlflow-1.0b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/top_level.txt
+Filename: oci_mlflow-1.0b0.dist-info/top_level.txt
 Comment: 
 
-Filename: oci_mlflow-1.0.1.dist-info/RECORD
+Filename: oci_mlflow-1.0b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oci_mlflow/oci_object_storage.py

```diff
@@ -1,190 +1,95 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*--
 
 # Copyright (c) 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 import os
-from typing import List
 from urllib.parse import urlparse
 
 import fsspec
-from ads.common.auth import AuthType, default_signer, set_auth
-from ads.common.oci_client import OCIClientFactory
 from mlflow.entities import FileInfo
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.utils.file_utils import relative_path_to_artifact_path
-from oci import object_storage
 from ocifs import OCIFileSystem
 
 from oci_mlflow import logger
 
-OCI_SCHEME = "oci"
-OCI_PREFIX = f"{OCI_SCHEME}://"
+OCI_PREFIX = "oci://"
 
 
-def parse_os_uri(uri: str):
-    """
-    Parse an OCI object storage URI, returning tuple (bucket, namespace, path).
-
-    Parameters
-    ----------
-    uri: str
-        The OCI Object Storage URI.
-
-    Returns
-    -------
-    Tuple
-        The (bucket, ns, type)
-
-    Raise
-    -----
-    Exception
-        If provided URI is not an OCI OS bucket URI.
-    """
-    parsed = urlparse(uri)
-    if parsed.scheme.lower() != OCI_SCHEME:
-        raise Exception("Not an OCI object storage URI: %s" % uri)
-    path = parsed.path
-
-    if path.startswith("/"):
-        path = path[1:]
-
-    bucket, ns = parsed.netloc.split("@")
-
-    return bucket, ns, path
-
-
-class ArtifactUploader:
+class OCIObjectStorageArtifactRepository(ArtifactRepository):
     """
-    The class helper to upload model artifacts.
-
-    Attributes
-    ----------
-    upload_manager: UploadManager
-        The uploadManager simplifies interaction with the Object Storage service.
+    MLFlow Plugin implementation for storing artifacts to OCI Object Storage
     """
 
-    def __init__(self):
-        """Initializes `ArtifactUploader` instance."""
-        auth_type = os.environ.get(
-            "OCI_IAM_TYPE", os.environ.get("OCIFS_IAM_TYPE", AuthType.API_KEY)
-        )
-        logger.debug(f"Using auth {auth_type=}")
-        set_auth(auth_type)
-
-        self.upload_manager = object_storage.UploadManager(
-            OCIClientFactory(**default_signer()).object_storage
-        )
-
-    def upload(self, file_path: str, dst_path: str):
-        """Uploads model artifacts.
-
-        Parameters
-        ----------
-        file_path: str
-            The source file path.
-        dst_path: str
-            The destination path.
-        """
-        bucket_name, namespace_name, object_name = parse_os_uri(dst_path)
-        logger.debug(f"{bucket_name=}, {namespace_name=}, {object_name=}")
-        response = self.upload_manager.upload_file(
-            namespace_name=namespace_name,
-            bucket_name=bucket_name,
-            object_name=object_name,
-            file_path=file_path,
-        )
-        logger.debug(response)
-
-
-class OCIObjectStorageArtifactRepository(ArtifactRepository):
-    """MLFlow Plugin implementation for storing artifacts to OCI Object Storage."""
+    @staticmethod
+    def parse_os_uri(uri):
+        """Parse an OCI object storage URI, returning (bucket, namespace, path)"""
+        parsed = urlparse(uri)
+        if parsed.scheme != "oci":
+            raise Exception("Not an OCI object storage URI: %s" % uri)
+        path = parsed.path
+        if path.startswith("/"):
+            path = path[1:]
+        bucket, ns = parsed.netloc.split("@")
+        return bucket, ns, path
+
+    def _upload_file(self, local_file, dest_path):
+        with open(local_file, "rb") as data:
+            with fsspec.open(dest_path, "wb") as outfile:
+                outfile.write(data.read())
 
     def _download_file(self, remote_file_path, local_path):
         if not remote_file_path.startswith(self.artifact_uri):
             full_path = os.path.join(self.artifact_uri, remote_file_path)
         else:
             full_path = remote_file_path
         fs: OCIFileSystem = self.get_fs()
         logger.info(f"{full_path}, {remote_file_path}")
         fs.download(full_path, local_path)
 
-    def log_artifact(self, local_file: str, artifact_path: str = None):
-        """
-        Logs a local file as an artifact, optionally taking an ``artifact_path`` to place it in
-        within the run's artifacts. Run artifacts can be organized into directories, so you can
-        place the artifact in a directory this way.
-
-        Parameters
-        ----------
-        local_file:str
-            Path to artifact to log.
-        artifact_path:str
-            Directory within the run's artifact directory in which to log the artifact.
-        """
-        dest_path = os.path.join(
-            self.artifact_uri, artifact_path or "", os.path.basename(local_file)
-        )
-        ArtifactUploader().upload(local_file, dest_path)
-
-    def log_artifacts(self, local_dir: str, artifact_path: str = None):
-        """
-        Logs the files in the specified local directory as artifacts, optionally taking
-        an ``artifact_path`` to place them in within the run's artifacts.
+    def log_artifact(self, local_file, artifact_path=None):
+        if artifact_path:
+            dest_path = os.path.join(self.artifact_uri, artifact_path)
+        else:
+            dest_path = self.artifact_uri
+        dest_path = os.path.join(dest_path, os.path.basename(local_file))
+        self._upload_file(local_file, dest_path)
 
-        Parameters
-        ----------
-        local_dir:str
-            Directory of local artifacts to log.
-        artifact_path:str
-            Directory within the run's artifact directory in which to log the artifacts.
-        """
-        artifact_uploader = ArtifactUploader()
-        dest_path = os.path.join(self.artifact_uri, artifact_path or "")
+    def log_artifacts(self, local_dir, artifact_path=None):
+        if artifact_path:
+            dest_path = os.path.join(self.artifact_uri, artifact_path)
+        else:
+            dest_path = artifact_path
         local_dir = os.path.abspath(local_dir)
-
-        for root, _, filenames in os.walk(local_dir):
+        for (root, _, filenames) in os.walk(local_dir):
             upload_path = dest_path
             if root != local_dir:
                 rel_path = os.path.relpath(root, local_dir)
                 rel_path = relative_path_to_artifact_path(rel_path)
                 upload_path = os.path.join(dest_path, rel_path)
             for f in filenames:
-                artifact_uploader.upload(
-                    file_path=os.path.join(root, f),
-                    dst_path=os.path.join(upload_path, f),
+                self._upload_file(
+                    local_file=os.path.join(root, f),
+                    dest_path=os.path.join(upload_path, f),
                 )
 
     def get_fs(self):
         """
-        Gets fssepc filesystem based on the uri scheme.
+        Get fssepc filesystem based on the uri scheme
         """
         self.fs = fsspec.filesystem(
             urlparse(self.artifact_uri).scheme
         )  # FileSystem class corresponding to the URI scheme.
 
         return self.fs
 
-    def list_artifacts(self, path: str = "") -> List[FileInfo]:
-        """
-        Return all the artifacts for this run_id directly under path. If path is a file, returns
-        an empty list. Will error if path is neither a file nor directory.
-
-        Parameters
-        ----------
-        path:str
-            Relative source path that contains desired artifacts
-
-        Returns
-        -------
-        List[FileInfo]
-            List of artifacts as FileInfo listed directly under path.
-        """
+    def list_artifacts(self, path: str = ""):
         result = []
         dest_path = self.artifact_uri
         if path:
             dest_path = os.path.join(dest_path, path)
 
         logger.debug(f"{path=}, {self.artifact_uri=}, {dest_path=}")
 
@@ -202,25 +107,15 @@
             result.append(FileInfo(file, file_isdir, size))
 
         logger.debug(f"{result=}")
 
         result.sort(key=lambda f: f.path)
         return result
 
-    def delete_artifacts(self, artifact_path: str = None):
-        """
-        Delete the artifacts at the specified location.
-        Supports the deletion of a single file or of a directory. Deletion of a directory
-        is recursive.
-
-        Parameters
-        ----------
-        artifact_path: str
-            Path of the artifact to delete.
-        """
+    def delete_artifacts(self, artifact_path=None):
         dest_path = self.artifact_uri
         if artifact_path:
             dest_path = os.path.join(self.artifact_uri, artifact_path)
         fs = self.get_fs()
         files = fs.ls(dest_path, refresh=True)
         for to_delete_obj in files:
             fs.delete(to_delete_obj)
```

## oci_mlflow/version.json

### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'version'": "'1.0b0'"}*

```diff
@@ -1,3 +1,3 @@
 {
-    "version": "1.0.1"
+    "version": "1.0b0"
 }
```

## Comparing `oci_mlflow-1.0.1.dist-info/LICENSE.txt` & `oci_mlflow-1.0b0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `oci_mlflow-1.0.1.dist-info/RECORD` & `oci_mlflow-1.0b0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 oci_mlflow/__init__.py,sha256=fObIqoSRHDbkSEBxLxH8j52vTOR5B4qzGJXpwhw2KNo,938
 oci_mlflow/deployment.py,sha256=XKxQU5hzefmMsKHL7D90sM0FMB-qQW3m27bIlHyb59o,21498
-oci_mlflow/oci_object_storage.py,sha256=434EhlyS0MJ1AnfbzuNbhqUCIJI90mImcvqz8fZ6OiA,7310
+oci_mlflow/oci_object_storage.py,sha256=T2WGInAx0MloieknoveVk8vOGQQ5lJM-cC6fXZ4dxh4,4235
 oci_mlflow/project.py,sha256=feqiOBTyCP6HQBenzjfwT90u_wiBNyw3bUniuievkHo,26088
 oci_mlflow/telemetry_logging.py,sha256=NWufc4Y7sFvSG9npPXRVudxO6gB1k5azCCZ9Yi_jbME,4448
 oci_mlflow/utils.py,sha256=Yc0mqf0-j_5VZuEWFKAPqlde9gSJLetODqCJX1mbtIQ,9236
-oci_mlflow/version.json,sha256=QCR1S9jw5FNM8TYfxn-1dpxB4Hb1fGEoKrKmnKauiO0,25
+oci_mlflow/version.json,sha256=dIF7j8Kscg63L06DLzFI5t0nH4LWJOH1Byf99ECohNY,25
 oci_mlflow/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oci_mlflow/templates/project_description.jinja2,sha256=WPUhBUA8xs0AFpxs5aSCK7Rvd1YPIyjegxp_W1rMlxk,1200
 oci_mlflow/templates/runtime.yaml.jinja2,sha256=cBhdxsurzIw2kEZ0-HNpepytsQdGRugfyi50KUSvVdE,163
 oci_mlflow/templates/score.py.jinja2,sha256=-yynJDrIYTJD4-zCYaxRoQ0oPdVKhB1b1wjDzvoADCk,422
-oci_mlflow-1.0.1.dist-info/LICENSE.txt,sha256=0ggOnaxgPaQEBstfywBdLBJ-kO9cJ4shpvZplaXiSDo,1860
-oci_mlflow-1.0.1.dist-info/METADATA,sha256=bq8edsqL4yVjQQceT5AahQM3_k9rpbZKRAH2Xb6SNVA,4228
-oci_mlflow-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oci_mlflow-1.0.1.dist-info/entry_points.txt,sha256=o3F_Wjg0uvEgMbYAAKC8dEmQJLd750Y1u14raQN77Uk,243
-oci_mlflow-1.0.1.dist-info/top_level.txt,sha256=_4zSAoTy-jMuG5boO5gwRB9cI9WuD5x4ReALJaKH9Q0,11
-oci_mlflow-1.0.1.dist-info/RECORD,,
+oci_mlflow-1.0b0.dist-info/LICENSE.txt,sha256=0ggOnaxgPaQEBstfywBdLBJ-kO9cJ4shpvZplaXiSDo,1860
+oci_mlflow-1.0b0.dist-info/METADATA,sha256=XcTltXCpt_X2Wwi-G1pA2twilqLeVagosQWNbGvHXgA,2156
+oci_mlflow-1.0b0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+oci_mlflow-1.0b0.dist-info/entry_points.txt,sha256=o3F_Wjg0uvEgMbYAAKC8dEmQJLd750Y1u14raQN77Uk,243
+oci_mlflow-1.0b0.dist-info/top_level.txt,sha256=_4zSAoTy-jMuG5boO5gwRB9cI9WuD5x4ReALJaKH9Q0,11
+oci_mlflow-1.0b0.dist-info/RECORD,,
```

