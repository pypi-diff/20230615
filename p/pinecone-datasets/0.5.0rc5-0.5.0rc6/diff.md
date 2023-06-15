# Comparing `tmp/pinecone_datasets-0.5.0rc5.tar.gz` & `tmp/pinecone_datasets-0.5.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.0rc5.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.0rc6.tar", max compression
```

## Comparing `pinecone_datasets-0.5.0rc5.tar` & `pinecone_datasets-0.5.0rc6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc5/README.md
--rw-r--r--   0        0        0      263 2023-06-11 13:16:57.358883 pinecone_datasets-0.5.0rc5/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc5/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1128 2023-06-06 18:16:41.496757 pinecone_datasets-0.5.0rc5/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    16620 2023-06-11 13:15:00.496257 pinecone_datasets-0.5.0rc5/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc5/pinecone_datasets/ds_utils.py
--rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc5/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc5/pinecone_datasets/public.py
--rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc5/pinecone_datasets/testing.py
--rw-r--r--   0        0        0      815 2023-06-11 13:17:02.737872 pinecone_datasets-0.5.0rc5/pyproject.toml
--rw-r--r--   0        0        0    10066 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc5/setup.py
--rw-r--r--   0        0        0     9871 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc6/README.md
+-rw-r--r--   0        0        0      263 2023-06-15 08:26:33.687548 pinecone_datasets-0.5.0rc6/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc6/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc6/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    20306 2023-06-14 19:42:07.195846 pinecone_datasets-0.5.0rc6/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc6/pinecone_datasets/ds_utils.py
+-rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc6/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc6/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc6/pinecone_datasets/testing.py
+-rw-r--r--   0        0        0      832 2023-06-15 08:26:22.664903 pinecone_datasets-0.5.0rc6/pyproject.toml
+-rw-r--r--   0        0        0    10090 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc6/setup.py
+-rw-r--r--   0        0        0     9909 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc6/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.0rc5/README.md` & `pinecone_datasets-0.5.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/cfg.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/cfg.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 class Storage:
     endpoint: str = "gs://pinecone-datasets-dev"
 
 
 class Schema:
     class Names:
         documents = [
-            ("id", False),
-            ("values", False),
-            ("sparse_values", True),
-            ("metadata", True),
-            ("blob", True),
+            ("id", False, None),
+            ("values", False, None),
+            ("sparse_values", True, None),
+            ("metadata", True, None),
+            ("blob", True, None),
         ]
         queries = [
-            ("vector", False),
-            ("sparse_vector", True),
-            ("filter", True),
-            ("top_k", False),
-            ("blob", True),
+            ("vector", False, None),
+            ("sparse_vector", True, None),
+            ("filter", True, None),
+            ("top_k", False, 5),
+            ("blob", True, None),
         ]
 
     # documents = {
     #     "id": Utf8,
     #     "values": List(Float32),
     #     "sparse_values": Struct(
     #         [Field("indices", List(UInt32)), Field("values", List(Float32))]
```

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import sys
 import glob
 import os
+import itertools
+import time
 import json
 import asyncio
-from functools import cached_property
-from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
 import warnings
+import pytest
 from urllib.parse import urlparse
+from dataclasses import dataclass
+from functools import cached_property
+from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
 
 import gcsfs
-from pydantic import ValidationError
 import s3fs
-
+from pydantic import ValidationError
 import pandas as pd
 import pyarrow.parquet as pq
+from tqdm.auto import tqdm
 
-from pinecone import Client, Index
+from pinecone import Client, Index, PineconeOpError
 
 from pinecone_datasets import cfg
 from pinecone_datasets.catalog import DatasetMetadata
 from pinecone_datasets.fs import get_cloud_fs, LocalFileSystem
 
 
+@dataclass
+class UpsertResponse:
+    upserted_count: int
+
+
 def iter_pandas_dataframe_slices(
     df: pd.DataFrame, batch_size=1
 ) -> Generator[List[Dict[str, Any]], None, None]:
     for i in range(0, len(df), batch_size):
         yield df.iloc[i : i + batch_size].to_dict(orient="records")
 
 
@@ -106,15 +115,17 @@
             queries, queries_column_mapping, cfg.Schema.Names.queries
         )
         clazz.metadata = metadata
         return clazz
 
     @staticmethod
     def _read_pandas_dataframe(
-        df: pd.DataFrame, column_mapping: Dict[str, str], schema: List[Tuple[str, bool]]
+        df: pd.DataFrame,
+        column_mapping: Dict[str, str],
+        schema: List[Tuple[str, bool, Any]],
     ) -> pd.DataFrame:
         """
         Reads a pandas DataFrame and validates it against a schema.
 
         Args:
             df (pd.DataFrame): the pandas DataFrame to read
             column_mapping (Dict[str, str]): a dictionary mapping the columns of the DataFrame to the Pinecone Datasets Schema (col_name, pinecone_name)
@@ -124,22 +135,22 @@
             pd.DataFrame: the validated, renamed DataFrame
         """
         if df is None or df.empty:
             return pd.DataFrame(columns=[column_name for column_name, _ in schema])
         else:
             if column_mapping is not None:
                 df.rename(columns=column_mapping, inplace=True)
-            for column_name, is_nullable in schema:
+            for column_name, is_nullable, null_value in schema:
                 if column_name not in df.columns and not is_nullable:
                     raise ValueError(
                         f"error, file is not matching Pinecone Datasets Schmea: {column_name} not found"
                     )
                 elif column_name not in df.columns and is_nullable:
-                    df[column_name] = None
-            return df[[column_name for column_name, _ in schema]]
+                    df[column_name] = null_value
+            return df[[column_name for column_name, _, _ in schema]]
 
     def __init__(
         self,
         dataset_path: str,
         **kwargs,
     ) -> None:
         """
@@ -164,14 +175,15 @@
             ```
 
         """
         self._config = cfg
         endpoint = urlparse(dataset_path)._replace(path="").geturl()
         self._fs = get_cloud_fs(endpoint, **kwargs)
         self._dataset_path = dataset_path
+        self._pinecone_client = None
 
         if not self._fs.exists(self._dataset_path):
             raise FileNotFoundError(
                 "Dataset does not exist. Please check the path or dataset_id"
             )
 
     def _is_datatype_exists(self, data_type: str) -> bool:
@@ -181,30 +193,30 @@
         read_path_str = os.path.join(self._dataset_path, data_type, "*.parquet")
         read_path = self._fs.glob(read_path_str)
         if self._is_datatype_exists(data_type):
             dataset = pq.ParquetDataset(read_path, filesystem=self._fs)
             dataset_schema_names = dataset.schema.names
             columns_to_null = []
             columns_not_null = []
-            for column_name, is_nullable in getattr(
+            for column_name, is_nullable, null_value in getattr(
                 self._config.Schema.Names, data_type
             ):
                 if column_name not in dataset_schema_names and not is_nullable:
                     raise ValueError(
                         f"error, file is not matching Pinecone Datasets Schmea: {column_name} not found"
                     )
                 elif column_name not in dataset_schema_names and is_nullable:
-                    columns_to_null.append(column_name)
+                    columns_to_null.append((column_name, null_value))
                 else:
                     columns_not_null.append(column_name)
             try:
                 # TODO: use of the columns_not_null and columns_to_null is only a workaround for proper schema validation and versioning
                 df = dataset.read_pandas(columns=columns_not_null).to_pandas()
-                for column_name in columns_to_null:
-                    df[column_name] = None
+                for column_name, null_value in columns_to_null:
+                    df[column_name] = null_value
                 return df
             # TODO: add more specific error handling, explain what is wrong
             except Exception as e:
                 print("error, no exception: {}".format(e), file=sys.stderr)
                 raise (e)
         else:
             warnings.warn(
@@ -257,15 +269,17 @@
 
         Examples:
             for batch in dataset.iter_documents(batch_size=100):
                 index.upsert(batch)
         """
         if isinstance(batch_size, int) and batch_size > 0:
             return iter_pandas_dataframe_slices(
-                self.documents[self._config.Schema.documents_select_columns],
+                self.documents[self._config.Schema.documents_select_columns].dropna(
+                    axis=1, how="all"
+                ),
                 batch_size,
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
     @cached_property
     def queries(self) -> pd.DataFrame:
@@ -343,104 +357,203 @@
             catalog_base_path
             if catalog_base_path
             else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
         )
         dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
         self.to_path(dataset_path, **kwargs)
 
-    async def _async_upsert(self, index: Index, batch_size: int, concurrency: int):
+    async def _async_upsert(self, index_name: str, batch_size: int, concurrency: int):
+        index = self._pinecone_client.get_index(index_name=index_name)
+
         sem = asyncio.Semaphore(concurrency)
 
-        async def send_batch(batch):
+        pinecone_failed_batches: Dict[Int, Any] = {}
+
+        async def send_batch(batch, i):
             async with sem:
-                return await index.upsert(vectors=batch, async_req=True)
+                try:
+                    return await index.upsert(vectors=batch, async_req=True)
+                except PineconeOpError as pe:
+                    if i in pinecone_failed_batches:
+                        raise PineconeOpError("Uploading batch failed twice")
+                    else:
+                        pinecone_failed_batches[i] = batch
+                        print(f"failed batches: {pinecone_failed_batches.keys()}")
+                        return UpsertResponse(upserted_count=0)
+                except Exception as e:
+                    raise e
+
+        tasks = [
+            send_batch(chunk, i)
+            for i, chunk in enumerate(self.iter_documents(batch_size=batch_size))
+        ]
+        failed_tasks_pinecone = []
+
+        pbar = tqdm(total=len(self.documents), desc="Upserting Vectors")
+        total_upserted_count = 0
+        for task in asyncio.as_completed(tasks):
+            res = await task
+            total_upserted_count += res.upserted_count
+            pbar.update(res.upserted_count)
+
+        failed_tasks = [
+            send_batch(chunk, i) for i, chunk in pinecone_failed_batches.items()
+        ]
+
+        for task in asyncio.as_completed(failed_tasks):
+            res = await task
+            total_upserted_count += res.upserted_count
+            pbar.update(res.upserted_count)
+
+        return {"upserted_count": total_upserted_count}
 
-        await asyncio.gather(
-            *[send_batch(chunk) for chunk in self.iter_documents(batch_size=batch_size)]
+    def _create_index(
+        self,
+        index_name: str,
+        api_key: Optional[str] = None,
+        environment: Optional[str] = None,
+        **kwargs,
+    ) -> Index:
+        dimension = self.metadata.dense_model.dimension
+        api_key = api_key if api_key else os.environ.get("PINECONE_API_KEY", None)
+        environment = (
+            environment if environment else os.environ.get("PINECONE_ENVIRONMENT", None)
         )
 
-    def to_index(
+        if not (api_key and environment):
+            raise ValueError(
+                "Please set PINECONE_API_KEY and PINECONE_ENVIRONMENT environment variables, \
+                or pass them as arguments to the function"
+            )
+        # create client
+        self._pinecone_client = Client(api_key=api_key, region=environment)
+
+        pinecone_index_list = self._pinecone_client.list_indexes()
+
+        if index_name in pinecone_index_list:
+            raise ValueError(
+                f"index {index_name} already exists, Pinecone Datasets can only be upserted to a new indexe"
+            )
+        else:
+            # create index
+            print("creating index")
+            self._pinecone_client.create_index(
+                name=index_name, dimension=self.metadata.dense_model.dimension, **kwargs
+            )
+            print("index created")
+
+        current_status = self._pinecone_client.describe_index(name=index_name).status
+        if current_status == "Ready":
+            return True
+        return False
+
+    def to_pinecone_index(
         self,
         index_name: str,
         batch_size: int = 100,
         concurrency: int = 10,
-        create_index: bool = False,
+        api_key: Optional[str] = None,
+        environment: Optional[str] = None,
         **kwargs,
     ):
         """
         Saves the dataset to a Pinecone index.
 
         this function will look for two environment variables:
         - PINECONE_API_KEY
-        - PINECONE_ENVIRONMENT / PINECONE_REGION
+        - PINECONE_ENVIRONMENT
 
         Then, it will init a Pinecone Client and will perform an upsert to the index.
         The upsert will be using async batches to increase performance.
 
         Args:
             index_name (str): the name of the index to upsert to
             batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
-            should_create (bool, optional): whether to create the index if it does not exist. Defaults to True.
+            concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
-                if should_create is False, these arguments will be ignored.
-                if should_create is True, and the index already exists, ValueError is thrown.
-                if should_create is True, dimension will be taken from the documents metadata.
-                see
+
+
+        Returns:
+            UpsertResponse: an object containing the upserted_count
+
+        Examples:
+            ```python
+            result = dataset.to_pinecone_index(index_name="my_index")
+            ```
         """
 
-        # make sure the region is set
-        if (
-            "PINECONE_ENVIRONMENT" not in os.environ
-            and "PINECONE_REGION" not in os.environ
-        ):
-            raise ValueError(
-                "PINECONE_ENVIRONMENT or PINECONE_REGION environment variable must be set"
+        loop = asyncio.get_event_loop()
+        if loop.is_running():
+            raise RuntimeError(
+                "You are running inside a Jupyter Notebook or another Asyncio context. "
+                + "Plesae use the function to_pinecone_index_async instead. "
+                + "example: `await dataset.to_pinecone_index_async(index_name)`"
             )
-        elif "PINECONE_ENVIRONMENT" in os.environ:
-            region = os.environ["PINECONE_ENVIRONMENT"]
-        elif "PINECONE_REGION" in os.environ:
-            region = os.environ["PINECONE_REGION"]
-
-        # make sure the api key is set
-        if "PINECONE_API_KEY" not in os.environ:
-            raise ValueError("PINECONE_API_KEY environment variable must be set")
 
-        # create client
-        pinecone = Client(api_key=os.environ["PINECONE_API_KEY"], region=region)
+        if not self._create_index(index_name, **kwargs):
+            raise RuntimeError("index creation failed")
 
-        pinecone_index_list = pinecone.list_indexes()
+        cor = self._async_upsert(
+            index_name=index_name,
+            batch_size=batch_size,
+            concurrency=concurrency,
+        )
+        return asyncio.run(cor)
 
-        if create_index:
-            # make sure the index does not exist
-            if index_name in pinecone_index_list:
-                raise ValueError(
-                    f"index {index_name} already exists. Please delete it or use should_create=False"
-                )
+    @pytest.mark.skip(
+        reason="this functionaility should be tested in notebook environment"
+    )
+    async def to_pinecone_index_async(
+        self,
+        index_name: str,
+        batch_size: int = 100,
+        concurrency: int = 10,
+        api_key: Optional[str] = None,
+        environment: Optional[str] = None,
+        **kwargs,
+    ):
+        """
+        Saves the dataset to a Pinecone index.
 
-            # create index
-            pinecone.create_index(
-                name=index_name, dimension=self.metadata.dense_model.dimension, **kwargs
-            )
-        else:
-            if index_name not in pinecone_index_list:
-                raise ValueError(
-                    f"index {index_name} does not exist. Please create it or use should_create=True"
-                )
+        this function will look for two environment variables:
+        - PINECONE_API_KEY
+        - PINECONE_ENVIRONMENT
 
-        index = pinecone.Index(index_name)
+        Then, it will init a Pinecone Client and will perform an upsert to the index.
+        The upsert will be using async batches to increase performance.
 
-        # upsert
-        try:
-            asyncio.run(
-                self._async_upsert(
-                    index=index, batch_size=batch_size, concurrency=concurrency
-                )
-            )
-            warnings.warn(
-                "asyncio.run call failed, will differ to use _async_upsert directly, this may happen when running in Jupyter Notebook"
-            )
-        except RuntimeError:
-            self._async_upsert(
-                index=index, batch_size=batch_size, concurrency=concurrency
+        Args:
+            index_name (str): the name of the index to upsert to
+            batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
+            concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
+
+        Keyword Args:
+            kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
+
+        Returns:
+            UpsertResponse: an object containing the upserted_count
+
+        Examples:
+            ```python
+            result = await dataset.to_pinecone_index_async(index_name="my_index")
+            ```
+        """
+        loop = asyncio.get_event_loop()
+        if not loop.is_running():
+            raise RuntimeError(
+                "You are running inside a Jupyter Notebook or another Asyncio context. \
+                Plesae use the function to_pinecone_index instead. \
+                example: `dataset.to_pinecone_index(index_name)`"
             )
+
+        if not self._create_index(index_name, **kwargs):
+            raise RuntimeError("index creation failed")
+
+        res = await self._async_upsert(
+            index_name=index_name,
+            batch_size=batch_size,
+            concurrency=concurrency,
+        )
+
+        return res
```

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/ds_utils.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/ds_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc5/pinecone_datasets/public.py` & `pinecone_datasets-0.5.0rc6/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc5/pyproject.toml` & `pinecone_datasets-0.5.0rc6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.0-rc.5"
+version = "0.5.0-rc.6"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
@@ -16,14 +16,15 @@
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
 protobuf = ">=3.19.3,<3.20.0"
 pandas = "^2.0.0"
 pinecone-client = "3.0.0rc2"
+tqdm = "^4.65.0"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
```

### Comparing `pinecone_datasets-0.5.0rc5/setup.py` & `pinecone_datasets-0.5.0rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,20 @@
  'gcsfs>=2023.1.0,<2024.0.0',
  'pandas>=2.0.0,<3.0.0',
  'pinecone-client==3.0.0rc2',
  'polars>=0.16.4,<0.17.0',
  'protobuf>=3.19.3,<3.20.0',
  'pyarrow>=12.0.0,<13.0.0',
  'pydantic>=1.10.5,<2.0.0',
- 's3fs>=2023.1.0,<2024.0.0']
+ 's3fs>=2023.1.0,<2024.0.0',
+ 'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pinecone-datasets',
-    'version': '0.5.0rc5',
+    'version': '0.5.0rc6',
     'description': 'Pinecone Datasets lets you easily load datasets into your Pinecone index.',
     'long_description': '# Pinecone Datasets\n\n## install\n\n```bash\npip install pinecone-datasets\n```\n\n##  Usage - Loading\n\nYou can use Pinecone Datasets to load our public datasets or with your own datasets. Datasets library can be used in 2 main ways: ad-hoc loading of datasets from a path or as a catalog loader for datasets. \n\n### Loading Pinecone Public Datasets (catalog)\n\nPinecone hosts a public datasets catalog, you can load a dataset by name using `list_datasets` and `load_dataset` functions. This will use the default catalog endpoint (currently GCS) to list and load datasets.\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n# ["quora_all-MiniLM-L6-bm25", ... ]\n\ndataset = load_dataset("quora_all-MiniLM-L6-bm25")\n\ndataset.head()\n\n# Prints\n# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐\n# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │\n# │     ┆                           ┆                                     ┆                   ┆      │\n# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │\n# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡\n# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │\n# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │\n# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘\n```\n\n### Expected dataset structure\n\npinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)\n\n we expect data to be uploaded to the following directory structure:\n\n    ├── my-subdir                     # path to where all datasets\n    │   ├── my-dataset                # name of dataset\n    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)\n    │   │   ├── documents             # datasets documents\n    │   │   │   ├── file1.parquet      \n    │   │   │   └── file2.parquet      \n    │   │   ├── queries               # dataset queries\n    │   │   │   ├── file1.parquet  \n    │   │   │   └── file2.parquet   \n    └── ...\n\nThe data schema is expected to be as follows:\n\n- `documents` directory contains parquet files with the following schema:\n    - Mandatory: `id: str, values: list[float]`\n    - Optional: `sparse_values: Dict: indices: List[int], values: List[float]`, `metadata: Dict`, `blob: dict`\n        - note: blob is a dict that can contain any data, it is not returned when iterating over the dataset and is inteded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. In future version this may become a first class citizen in the dataset schema.\n- `queries` directory contains parquet files with the following schema:\n    - Mandatory: `vector: list[float], top_k: int`\n    - Optional: `sparse_vector: Dict: indices: List[int], values: List[float]`, `filter: Dict`\n        - note: filter is a dict that contain pinecone filters, for more information see [here](https://docs.pinecone.io/docs/metadata-filtering)\n\nin addition, a metadata file is expected to be in the dataset directory, for example: `s3://my-bucket/my-dataset/metadata.json`\n\n```python\nfrom pinecone_datasets.catalog import DatasetMetadata\n\nmeta = DatasetMetadata(\n    name="test_dataset",\n    created_at="2023-02-17 14:17:01.481785",\n    documents=2,\n    queries=2,\n    source="manual",\n    bucket="LOCAL",\n    task="unittests",\n    dense_model={"name": "bert", "dimension": 3},\n    sparse_model={"name": "bm25"},\n)\n```\n\nfull metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`\n\n### Loading your own dataset from catalog\n\nTo set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```bash\nexport DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"\n```\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n\n# ["my-dataset", ... ]\n\ndataset = load_dataset("my-dataset")\n```\n\n### Loading your own dataset from path\n\nYou can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```python\nfrom pinecone_datasets import Dataset\n\ndataset = Dataset("s3://my-bucket/my-subdir/my-dataset")\n```\n\n### Loading from a pandas dataframe\n\nPinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.\nThe minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.\n\n```python\nimport pandas as pd\n\ndf = pd.read_parquet("my-dataset.parquet")\n\ndataset = Dataset.from_pandas(df)\n```\n\nPlease check the documentation for more information on the expected dataframe schema. There\'s also a column mapping variable that can be used to map the dataframe columns to the expected schema.\n\n\n## Usage - Accessing data\n\nPinecone Datasets is build on top of pandas. This means that you can use all the pandas API to access the data. In addition, we provide some helper functions to access the data in a more convenient way. \n\n### Accessing documents and queries dataframes\n\naccessing the documents and queries dataframes is done using the `documents` and `queries` properties. These properties are lazy and will only load the data when accessed. \n\n```python\ndocument_df: pd.DataFrame = dataset.documents\n\nquery_df: pd.DataFrame = dataset.queries\n```\n\n\n## Usage - Iterating\n\nOne of the main use cases for Pinecone Datasets is iterating over a dataset. This is useful for upserting a dataset to an index, or for benchmarking. It is also useful for iterating over large datasets - as of today, datasets are not yet lazy, however we are working on it.\n\n\n```python\n\n# List Iterator, where every list of size N Dicts with ("id", "values", "sparse_values", "metadata")\ndataset.iter_documents(batch_size=n) \n\n# Dict Iterator, where every dict has ("vector", "sparse_vector", "filter", "top_k")\ndataset.iter_queries()\n\n```\n\n### The \'blob\' column\n\nPinecone dataset ship with a blob column which is inteneded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. We added a utility function to move data from the blob column to the metadata column. This is useful for example when upserting a dataset to an index and want to use the metadata to store text data.\n\n```python\nfrom pinecone_datasets import import_documents_keys_from_blob_to_metadata\n\nnew_dataset = import_documents_keys_from_blob_to_metadata(dataset, keys=["text"])\n```\n\n\n### upserting to Index\n\nWhen upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. \n\n```python\nds = load_dataset("dataset_name")\n\n# If index exists\nds.to_index("index_name")\n\n# If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.\nds.to_index("index_name", create_index=True)\n\n```\n\nthe `to_index` function also accepts additional parameters\n\n* `batch_size` and `concurrency` - for controlling the upserting process\n* `kwargs` - for passing additional parameters to the index creation process\n\n\n## For developers\n\nThis project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:\n\n```bash\npoetry install --with dev\n```\n\nTo run test locally run \n\n```bash\npoetry run pytest --cov pinecone_datasets\n```',
     'author': 'Pinecone',
     'author_email': 'None',
     'maintainer': 'Roy Miara',
     'maintainer_email': 'miararoy@gmail.com',
     'url': 'None',
```

### Comparing `pinecone_datasets-0.5.0rc5/PKG-INFO` & `pinecone_datasets-0.5.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.5.0rc5
+Version: 0.5.0rc6
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,14 +16,15 @@
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pinecone-client (==3.0.0rc2)
 Requires-Dist: polars (>=0.16.4,<0.17.0)
 Requires-Dist: protobuf (>=3.19.3,<3.20.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Pinecone Datasets
 
 ## install
 
 ```bash
```

