# Comparing `tmp/prefect-aws-0.3.3.tar.gz` & `tmp/prefect-aws-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-1ip9v5mt/prefect-aws-0.3.3.tar", last modified: Tue Jun 13 17:03:32 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-8kaz6hzb/prefect-aws-0.3.4.tar", last modified: Thu Jun 15 14:30:23 2023, max compression
```

## Comparing `prefect-aws-0.3.3.tar` & `prefect-aws-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/ecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56907 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:32.000000 prefect-aws-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-06-13 17:01:37.000000 prefect-aws-0.3.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35068 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56907 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:23.000000 prefect-aws-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-06-15 14:28:43.000000 prefect-aws-0.3.4/versioneer.py
```

### Comparing `prefect-aws-0.3.3/LICENSE` & `prefect-aws-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/PKG-INFO` & `prefect-aws-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.3
+Version: 0.3.4
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.3 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.4 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.3/README.md` & `prefect-aws-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/batch.py` & `prefect-aws-0.3.4/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/client_parameters.py` & `prefect-aws-0.3.4/prefect_aws/client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/client_waiter.py` & `prefect-aws-0.3.4/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/credentials.py` & `prefect-aws-0.3.4/prefect_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/ecs.py` & `prefect-aws-0.3.4/prefect_aws/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/s3.py` & `prefect-aws-0.3.4/prefect_aws/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import uuid
 from pathlib import Path
 from typing import Any, BinaryIO, Dict, List, Optional, Union
 
 import boto3
 from botocore.paginate import PageIterator
+from botocore.response import StreamingBody
 from prefect import get_run_logger, task
 from prefect.blocks.abstract import ObjectStorageBlock
 from prefect.filesystems import WritableDeploymentStorage, WritableFileSystem
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.filesystem import filter_files
 from pydantic import Field
 
@@ -783,14 +784,78 @@
                 )
             )
         await asyncio.gather(*async_coros)
 
         return Path(to_folder)
 
     @sync_compatible
+    async def stream_from(
+        self,
+        bucket: "S3Bucket",
+        from_path: str,
+        to_path: Optional[str] = None,
+        **upload_kwargs: Dict[str, Any],
+    ) -> str:
+        """Streams an object from another bucket to this bucket.
+
+        Args:
+            bucket: The bucket to stream from.
+            from_path: The path of the object to stream.
+            to_path: The path to stream the object to. Defaults to the object's name.
+            **upload_kwargs: Additional keyword arguments to pass to
+                `Client.upload_fileobj`.
+
+        Returns:
+            The path that the object was uploaded to.
+
+        Examples:
+            Stream notes.txt from your-bucket/notes.txt to my-bucket/landed/notes.txt.
+
+            ```python
+            from prefect_aws.s3 import S3Bucket
+
+            your_s3_bucket = S3Bucket.load("your-bucket")
+            my_s3_bucket = S3Bucket.load("my-bucket")
+
+            my_s3_bucket.stream_from(
+                your_s3_bucket,
+                "notes.txt",
+                to_path="landed/notes.txt"
+            )
+            ```
+
+        """
+        if to_path is None:
+            to_path = Path(from_path).name
+
+        # Get the source object's StreamingBody
+        from_path: str = self._join_bucket_folder(from_path)
+        from_client = bucket.credentials.get_s3_client()
+        obj = await run_sync_in_worker_thread(
+            from_client.get_object, Bucket=bucket.bucket_name, Key=from_path
+        )
+        body: StreamingBody = obj["Body"]
+
+        # Upload the StreamingBody to this bucket
+        bucket_path = str(self._join_bucket_folder(to_path))
+        to_client = self.credentials.get_s3_client()
+        await run_sync_in_worker_thread(
+            to_client.upload_fileobj,
+            Fileobj=body,
+            Bucket=self.bucket_name,
+            Key=bucket_path,
+            **upload_kwargs,
+        )
+        self.logger.info(
+            f"Streamed s3://{bucket.bucket_name}/{from_path} to the bucket "
+            f"{self.bucket_name!r} path {bucket_path!r}."
+        )
+        return bucket_path
+
+    @sync_compatible
     async def upload_from_path(
         self,
         from_path: Union[str, Path],
         to_path: Optional[str] = None,
         **upload_kwargs: Dict[str, Any],
     ) -> str:
         """
```

### Comparing `prefect-aws-0.3.3/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.4/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.3.4/prefect_aws/workers/ecs_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.4/prefect_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.3
+Version: 0.3.4
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.3 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.4 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.3/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.4/prefect_aws.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 prefect_aws/secrets_manager.py
 prefect_aws.egg-info/PKG-INFO
 prefect_aws.egg-info/SOURCES.txt
 prefect_aws.egg-info/dependency_links.txt
 prefect_aws.egg-info/entry_points.txt
 prefect_aws.egg-info/requires.txt
 prefect_aws.egg-info/top_level.txt
-prefect_aws/projects/__init__.py
-prefect_aws/projects/steps.py
+prefect_aws/deployments/__init__.py
+prefect_aws/deployments/steps.py
 prefect_aws/workers/__init__.py
 prefect_aws/workers/ecs_worker.py
 tests/test_batch.py
 tests/test_block_standards.py
 tests/test_client_parameters.py
 tests/test_client_waiter.py
 tests/test_credentials.py
```

### Comparing `prefect-aws-0.3.3/setup.cfg` & `prefect-aws-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/setup.py` & `prefect-aws-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_batch.py` & `prefect-aws-0.3.4/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_block_standards.py` & `prefect-aws-0.3.4/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_client_parameters.py` & `prefect-aws-0.3.4/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_client_waiter.py` & `prefect-aws-0.3.4/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_credentials.py` & `prefect-aws-0.3.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_ecs.py` & `prefect-aws-0.3.4/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/tests/test_s3.py` & `prefect-aws-0.3.4/tests/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,14 +711,27 @@
         os.chdir(tmp_path)
         s3_bucket_with_objects.download_folder_to_path("folder", to_path)
         if to_path is None:
             to_path = ""
         to_path = Path(to_path)
         assert (to_path / "object").read_text() == "TEST OBJECT IN FOLDER"
 
+    @pytest.mark.parametrize("to_path", ["to_path", None])
+    @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
+    def test_stream_from(
+        self,
+        s3_bucket_with_object: S3Bucket,
+        s3_bucket_empty: S3Bucket,
+        client_parameters,
+        to_path,
+    ):
+        path = s3_bucket_empty.stream_from(s3_bucket_with_object, "object", to_path)
+        data: bytes = s3_bucket_empty.read_path(path)
+        assert data == b"TEST"
+
     @pytest.mark.parametrize("to_path", ["new_object", None])
     @pytest.mark.parametrize("client_parameters", aws_clients[-1:], indirect=True)
     def test_upload_from_path(
         self, s3_bucket_empty: S3Bucket, client_parameters, tmp_path, to_path
     ):
         from_path = tmp_path / "new_object"
         from_path.write_text("NEW OBJECT")
```

### Comparing `prefect-aws-0.3.3/tests/test_secrets_manager.py` & `prefect-aws-0.3.4/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.3/versioneer.py` & `prefect-aws-0.3.4/versioneer.py`

 * *Files identical despite different names*

