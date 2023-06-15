# Comparing `tmp/pinecone_datasets-0.5.0rc6.tar.gz` & `tmp/pinecone_datasets-0.5.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.0rc6.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.0rc7.tar", max compression
```

## Comparing `pinecone_datasets-0.5.0rc6.tar` & `pinecone_datasets-0.5.0rc7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc6/README.md
--rw-r--r--   0        0        0      263 2023-06-15 08:26:33.687548 pinecone_datasets-0.5.0rc6/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc6/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc6/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    20306 2023-06-14 19:42:07.195846 pinecone_datasets-0.5.0rc6/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc6/pinecone_datasets/ds_utils.py
--rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc6/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc6/pinecone_datasets/public.py
--rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc6/pinecone_datasets/testing.py
--rw-r--r--   0        0        0      832 2023-06-15 08:26:22.664903 pinecone_datasets-0.5.0rc6/pyproject.toml
--rw-r--r--   0        0        0    10090 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc6/setup.py
--rw-r--r--   0        0        0     9909 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc7/README.md
+-rw-r--r--   0        0        0      263 2023-06-15 08:51:37.997122 pinecone_datasets-0.5.0rc7/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc7/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc7/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    20186 2023-06-15 08:42:45.599902 pinecone_datasets-0.5.0rc7/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc7/pinecone_datasets/ds_utils.py
+-rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc7/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc7/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc7/pinecone_datasets/testing.py
+-rw-r--r--   0        0        0      832 2023-06-15 08:51:46.177765 pinecone_datasets-0.5.0rc7/pyproject.toml
+-rw-r--r--   0        0        0    10090 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc7/setup.py
+-rw-r--r--   0        0        0     9909 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc7/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.0rc6/README.md` & `pinecone_datasets-0.5.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/cfg.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import glob
 import os
 import itertools
 import time
 import json
 import asyncio
 import warnings
-import pytest
 from urllib.parse import urlparse
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
 
 import gcsfs
 import s3fs
@@ -497,17 +496,15 @@
         cor = self._async_upsert(
             index_name=index_name,
             batch_size=batch_size,
             concurrency=concurrency,
         )
         return asyncio.run(cor)
 
-    @pytest.mark.skip(
-        reason="this functionaility should be tested in notebook environment"
-    )
+
     async def to_pinecone_index_async(
         self,
         index_name: str,
         batch_size: int = 100,
         concurrency: int = 10,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
```

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/ds_utils.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/ds_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pinecone_datasets/public.py` & `pinecone_datasets-0.5.0rc7/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc6/pyproject.toml` & `pinecone_datasets-0.5.0rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.0-rc.6"
+version = "0.5.0-rc.7"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `pinecone_datasets-0.5.0rc6/setup.py` & `pinecone_datasets-0.5.0rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pyarrow>=12.0.0,<13.0.0',
  'pydantic>=1.10.5,<2.0.0',
  's3fs>=2023.1.0,<2024.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pinecone-datasets',
-    'version': '0.5.0rc6',
+    'version': '0.5.0rc7',
     'description': 'Pinecone Datasets lets you easily load datasets into your Pinecone index.',
     'long_description': '# Pinecone Datasets\n\n## install\n\n```bash\npip install pinecone-datasets\n```\n\n##  Usage - Loading\n\nYou can use Pinecone Datasets to load our public datasets or with your own datasets. Datasets library can be used in 2 main ways: ad-hoc loading of datasets from a path or as a catalog loader for datasets. \n\n### Loading Pinecone Public Datasets (catalog)\n\nPinecone hosts a public datasets catalog, you can load a dataset by name using `list_datasets` and `load_dataset` functions. This will use the default catalog endpoint (currently GCS) to list and load datasets.\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n# ["quora_all-MiniLM-L6-bm25", ... ]\n\ndataset = load_dataset("quora_all-MiniLM-L6-bm25")\n\ndataset.head()\n\n# Prints\n# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐\n# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │\n# │     ┆                           ┆                                     ┆                   ┆      │\n# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │\n# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡\n# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │\n# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │\n# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘\n```\n\n### Expected dataset structure\n\npinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)\n\n we expect data to be uploaded to the following directory structure:\n\n    ├── my-subdir                     # path to where all datasets\n    │   ├── my-dataset                # name of dataset\n    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)\n    │   │   ├── documents             # datasets documents\n    │   │   │   ├── file1.parquet      \n    │   │   │   └── file2.parquet      \n    │   │   ├── queries               # dataset queries\n    │   │   │   ├── file1.parquet  \n    │   │   │   └── file2.parquet   \n    └── ...\n\nThe data schema is expected to be as follows:\n\n- `documents` directory contains parquet files with the following schema:\n    - Mandatory: `id: str, values: list[float]`\n    - Optional: `sparse_values: Dict: indices: List[int], values: List[float]`, `metadata: Dict`, `blob: dict`\n        - note: blob is a dict that can contain any data, it is not returned when iterating over the dataset and is inteded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. In future version this may become a first class citizen in the dataset schema.\n- `queries` directory contains parquet files with the following schema:\n    - Mandatory: `vector: list[float], top_k: int`\n    - Optional: `sparse_vector: Dict: indices: List[int], values: List[float]`, `filter: Dict`\n        - note: filter is a dict that contain pinecone filters, for more information see [here](https://docs.pinecone.io/docs/metadata-filtering)\n\nin addition, a metadata file is expected to be in the dataset directory, for example: `s3://my-bucket/my-dataset/metadata.json`\n\n```python\nfrom pinecone_datasets.catalog import DatasetMetadata\n\nmeta = DatasetMetadata(\n    name="test_dataset",\n    created_at="2023-02-17 14:17:01.481785",\n    documents=2,\n    queries=2,\n    source="manual",\n    bucket="LOCAL",\n    task="unittests",\n    dense_model={"name": "bert", "dimension": 3},\n    sparse_model={"name": "bm25"},\n)\n```\n\nfull metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`\n\n### Loading your own dataset from catalog\n\nTo set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```bash\nexport DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"\n```\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n\n# ["my-dataset", ... ]\n\ndataset = load_dataset("my-dataset")\n```\n\n### Loading your own dataset from path\n\nYou can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```python\nfrom pinecone_datasets import Dataset\n\ndataset = Dataset("s3://my-bucket/my-subdir/my-dataset")\n```\n\n### Loading from a pandas dataframe\n\nPinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.\nThe minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.\n\n```python\nimport pandas as pd\n\ndf = pd.read_parquet("my-dataset.parquet")\n\ndataset = Dataset.from_pandas(df)\n```\n\nPlease check the documentation for more information on the expected dataframe schema. There\'s also a column mapping variable that can be used to map the dataframe columns to the expected schema.\n\n\n## Usage - Accessing data\n\nPinecone Datasets is build on top of pandas. This means that you can use all the pandas API to access the data. In addition, we provide some helper functions to access the data in a more convenient way. \n\n### Accessing documents and queries dataframes\n\naccessing the documents and queries dataframes is done using the `documents` and `queries` properties. These properties are lazy and will only load the data when accessed. \n\n```python\ndocument_df: pd.DataFrame = dataset.documents\n\nquery_df: pd.DataFrame = dataset.queries\n```\n\n\n## Usage - Iterating\n\nOne of the main use cases for Pinecone Datasets is iterating over a dataset. This is useful for upserting a dataset to an index, or for benchmarking. It is also useful for iterating over large datasets - as of today, datasets are not yet lazy, however we are working on it.\n\n\n```python\n\n# List Iterator, where every list of size N Dicts with ("id", "values", "sparse_values", "metadata")\ndataset.iter_documents(batch_size=n) \n\n# Dict Iterator, where every dict has ("vector", "sparse_vector", "filter", "top_k")\ndataset.iter_queries()\n\n```\n\n### The \'blob\' column\n\nPinecone dataset ship with a blob column which is inteneded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. We added a utility function to move data from the blob column to the metadata column. This is useful for example when upserting a dataset to an index and want to use the metadata to store text data.\n\n```python\nfrom pinecone_datasets import import_documents_keys_from_blob_to_metadata\n\nnew_dataset = import_documents_keys_from_blob_to_metadata(dataset, keys=["text"])\n```\n\n\n### upserting to Index\n\nWhen upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. \n\n```python\nds = load_dataset("dataset_name")\n\n# If index exists\nds.to_index("index_name")\n\n# If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.\nds.to_index("index_name", create_index=True)\n\n```\n\nthe `to_index` function also accepts additional parameters\n\n* `batch_size` and `concurrency` - for controlling the upserting process\n* `kwargs` - for passing additional parameters to the index creation process\n\n\n## For developers\n\nThis project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:\n\n```bash\npoetry install --with dev\n```\n\nTo run test locally run \n\n```bash\npoetry run pytest --cov pinecone_datasets\n```',
     'author': 'Pinecone',
     'author_email': 'None',
     'maintainer': 'Roy Miara',
     'maintainer_email': 'miararoy@gmail.com',
     'url': 'None',
```

### Comparing `pinecone_datasets-0.5.0rc6/PKG-INFO` & `pinecone_datasets-0.5.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.5.0rc6
+Version: 0.5.0rc7
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

