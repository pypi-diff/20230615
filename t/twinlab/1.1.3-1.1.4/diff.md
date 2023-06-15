# Comparing `tmp/twinlab-1.1.3.tar.gz` & `tmp/twinlab-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.3.tar", max compression
+gzip compressed data, was "twinlab-1.1.4.tar", max compression
```

## Comparing `twinlab-1.1.3.tar` & `twinlab-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.3/LICENSE
--rw-r--r--   0        0        0     2011 2023-05-25 13:37:52.705700 twinlab-1.1.3/README.md
--rw-r--r--   0        0        0      932 2023-05-25 13:37:55.886193 twinlab-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.3/twinlab/__init__.py
--rw-r--r--   0        0        0     8531 2023-05-25 13:37:55.886468 twinlab-1.1.3/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.3/twinlab/plotting.py
--rw-r--r--   0        0        0      702 2023-05-25 12:10:04.800688 twinlab-1.1.3/twinlab/settings.py
--rw-r--r--   0        0        0     6174 2023-05-25 13:37:55.886723 twinlab-1.1.3/twinlab/utils.py
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 twinlab-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2037 2023-06-15 08:30:01.835810 twinlab-1.1.4/README.md
+-rw-r--r--   0        0        0      932 2023-06-15 08:30:01.841314 twinlab-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      574 2023-06-15 08:30:01.844913 twinlab-1.1.4/twinlab/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-15 08:30:01.845288 twinlab-1.1.4/twinlab/_version.py
+-rw-r--r--   0        0        0    13412 2023-06-15 08:30:01.845725 twinlab-1.1.4/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.4/twinlab/plotting.py
+-rw-r--r--   0        0        0     1322 2023-06-15 08:30:01.846138 twinlab-1.1.4/twinlab/settings.py
+-rw-r--r--   0        0        0     4777 2023-06-15 08:30:01.846448 twinlab-1.1.4/twinlab/utils.py
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 twinlab-1.1.4/PKG-INFO
```

### Comparing `twinlab-1.1.3/LICENSE` & `twinlab-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.3/README.md` & `twinlab-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,25 +54,25 @@
 
 # Train a machine-learning model for the data
 params = {
     'filename': 'test.csv',
     'inputs': ['X'],
     'outputs': ['y'],
 }
-tl.train_campaign(params, campaign='test')
+tl.train_campaign(params, campaign_name='test')
 
 # Evaluate the model on some unseen data
 df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-df_mean, df_std = tl.predict_campaign(df, campaign='test')
+df_mean, df_std = tl.predict_campaign(df, campaign_name='test')
 ```
 
 ## Notebooks
 
 Check out the `notebooks` directory for some additional examples to get started!
 
 ## Documentation
 
 See the live documentation at https://digilab-ai.github.io/twinLab-client/. Or build a copy locally:
 ```shell
 cd docs
-yarn start
+yarn install && yarn start
 ```
```

### Comparing `twinlab-1.1.3/pyproject.toml` & `twinlab-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.3"
+version = "1.1.4"
 description = "Client interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab-client"
 authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
```

### Comparing `twinlab-1.1.3/twinlab/__init__.py` & `twinlab-1.1.4/twinlab/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Version
+from ._version import __version__
+
 # Utility functions
 from .utils import get_command_line_args
 
 # API dataset functions
 from .client import upload_dataset
 from .client import query_dataset
 from .client import list_datasets
```

### Comparing `twinlab-1.1.3/twinlab/utils.py` & `twinlab-1.1.4/twinlab/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 # Third-party imports
 import requests
 import pandas as pd
 
 # Project imports
 from .settings import ENV
 
-
-PARAMS_COERCION = {  # Convert these names in the params file
+# Convert these names in the params file
+PARAMS_COERCION = {
     "test_train_split": "train_test_split",  # Common mistake
     "num_training_examples": "train_test_split",  #  TODO: Think of something better
-    "dataset": "filename",
+    "filename": "dataset",  # Suppoprt old name
+    "filename_std": "dataset_std",  # Support old name
 }
-TRAIN_CAMPAIGN_DEV_URL = "https://pdersvjxmgrkqojwyeyocqm7le0iwtkx.lambda-url.eu-west-2.on.aws/"
-TRAIN_CAMPAIGN_STAGE_URL = "https://b7vgjlsn73e7n7kci5rwoxjc7e0pkcqn.lambda-url.eu-west-2.on.aws/"
-TRAIN_CAMPAIGN_CLOUD_URL = "https://cma567qwquixu7bbjcnhbjsxjm0yumvu.lambda-url.eu-west-2.on.aws/"
 
 
 ### Utility functions ###
 
 
 # def unwrap_payload(event: dict) -> dict:
 #     """
@@ -64,51 +62,14 @@
         "X-User": ENV.TWINLAB_USERNAME,
         "authorizationToken": ENV.TWINLAB_TOKEN,
         "X-Debug": str(debug).lower(),
     }
     return headers
 
 
-def get_server_url(server: str) -> str:
-    """
-    The URL is the dockerised lambda function that's been set up in cloud by alexander
-    """
-    if server == "local":
-        baseURL = ENV.TWINLAB_LOCAL_SERVER
-    elif server == "dev":
-        baseURL = ENV.TWINLAB_DEV_SERVER
-    elif server == "stage":
-        baseURL = ENV.TWINLAB_STAGE_SERVER
-    elif server == "cloud":
-        baseURL = ENV.TWINLAB_SERVER
-    else:
-        print("Server:", server)
-        raise ValueError(
-            "Server must be either 'local', 'dev', 'stage', or 'cloud'")
-    if baseURL is None:  # Catch if the server URL has not been set
-        raise ValueError("Server URL not set")
-    return baseURL
-
-
-def get_train_campaign_url(server: str) -> str:
-    """
-    Get the URL for the train_campaign lambda function
-    These are different to avoid the AWS Lambda 29s gateway timeout
-    """
-    if server == "dev":
-        url = TRAIN_CAMPAIGN_DEV_URL
-    elif server == "stage":
-        url = TRAIN_CAMPAIGN_STAGE_URL
-    elif server == "cloud":
-        url = TRAIN_CAMPAIGN_CLOUD_URL
-    else:
-        url = get_server_url(server)+"/train_campaign"
-    return url
-
-
 def coerce_params_dict(params: dict) -> dict:
     """
     Relabel parameters to be consistent with twinLab library
     """
     for param in PARAMS_COERCION:
         if param in params:
             params[PARAMS_COERCION[param]] = params.pop(param)
@@ -138,15 +99,15 @@
         else:
             print(f"File upload failed")
             print(f"Status code: {response.status_code}")
             print(f"Reason: {response.text}")
         print()
 
 
-def upload_dataframe_to_presigned_url(dataset_name: str, df: pd.DataFrame, url: str, verbose=False) -> None:
+def upload_dataframe_to_presigned_url(df: pd.DataFrame, url: str, verbose=False) -> None:
     """
     Upload a panads dataframe to the specified pre-signed URL.
     params:
         df: The pandas dataframe to upload
         presigned_url: The pre-signed URL generated for uploading the file.
     """
     headers = {"Content-Type": "application/octet-stream"}
```

### Comparing `twinlab-1.1.3/PKG-INFO` & `twinlab-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.1.3
+Version: 1.1.4
 Summary: Client interface for twinLab machine-learning in the cloud.
 Home-page: https://www.digilab.co.uk/
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: DigiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
@@ -78,26 +78,26 @@
 
 # Train a machine-learning model for the data
 params = {
     'filename': 'test.csv',
     'inputs': ['X'],
     'outputs': ['y'],
 }
-tl.train_campaign(params, campaign='test')
+tl.train_campaign(params, campaign_name='test')
 
 # Evaluate the model on some unseen data
 df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-df_mean, df_std = tl.predict_campaign(df, campaign='test')
+df_mean, df_std = tl.predict_campaign(df, campaign_name='test')
 ```
 
 ## Notebooks
 
 Check out the `notebooks` directory for some additional examples to get started!
 
 ## Documentation
 
 See the live documentation at https://digilab-ai.github.io/twinLab-client/. Or build a copy locally:
 ```shell
 cd docs
-yarn start
+yarn install && yarn start
 ```
```

