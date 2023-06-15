# Comparing `tmp/hip_data_ml_utils-1.0.2.tar.gz` & `tmp/hip_data_ml_utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hip_data_ml_utils-1.0.2.tar", max compression
+gzip compressed data, was "hip_data_ml_utils-1.0.3.tar", max compression
```

## Comparing `hip_data_ml_utils-1.0.2.tar` & `hip_data_ml_utils-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1085 2023-06-05 08:19:39.988757 hip_data_ml_utils-1.0.2/LICENSE.txt
--rwxr-xr-x   0        0        0     1548 2023-06-05 08:19:39.988757 hip_data_ml_utils-1.0.2/README.md
--rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/__init__.py
--rwxr-xr-x   0        0        0      642 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/config.py
--rw-r--r--   0        0        0     2158 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/databricks_utils.py
--rw-r--r--   0        0        0     3119 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/pyathena_utils.py
--rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/__init__.py
--rw-r--r--   0        0        0     7529 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
--rw-r--r--   0        0        0     2578 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
--rw-r--r--   0        0        0     6370 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
--rw-r--r--   0        0        0     4470 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
--rwxr-xr-x   0        0        0        0 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/__init__.py
--rw-r--r--   0        0        0     4368 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/client.py
--rw-r--r--   0        0        0     1404 2023-06-05 08:19:39.996757 hip_data_ml_utils-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 03:51:21.389634 hip_data_ml_utils-1.0.3/LICENSE.txt
+-rwxr-xr-x   0        0        0     1580 2023-06-15 03:41:54.867127 hip_data_ml_utils-1.0.3/README.md
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.928557 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/__init__.py
+-rwxr-xr-x   0        0        0      642 2023-05-11 01:34:24.776444 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/config.py
+-rw-r--r--   0        0        0     2158 2023-04-04 23:47:04.268778 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/databricks_utils.py
+-rw-r--r--   0        0        0     3119 2023-04-04 23:47:04.269549 hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/pyathena_utils.py
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.930078 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/__init__.py
+-rw-r--r--   0        0        0     7529 2023-05-11 01:34:24.777536 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
+-rw-r--r--   0        0        0     2578 2023-05-11 01:34:24.778338 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
+-rw-r--r--   0        0        0     6370 2023-05-11 01:34:24.779153 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
+-rw-r--r--   0        0        0     4470 2023-03-30 05:32:20.932267 hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
+-rwxr-xr-x   0        0        0        0 2023-03-30 05:32:20.932369 hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/__init__.py
+-rw-r--r--   0        0        0     4368 2023-03-30 05:32:20.932900 hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/client.py
+-rw-r--r--   0        0        0     1267 2023-06-15 01:55:07.851264 hip_data_ml_utils-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.3/PKG-INFO
```

### Comparing `hip_data_ml_utils-1.0.2/LICENSE.txt` & `hip_data_ml_utils-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/README.md` & `hip_data_ml_utils-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Almost one liner
 ```python
 import os
 from hip_data_ml_utils.pyathena_client.client import PyAthenaClient
 
 os.environ["AWS_ACCESS_KEY_ID"] = "xxx"
 os.environ["AWS_SECRET_ACCESS_KEY"] = "xxx" # pragma: allowlist secret
+os.environ["S3_BUCKET"] = "xxx"
 
 pyathena_client = PyAthenaClient()
 ```
 ![Pyathena client initialisation](docs/_static/initialise_pyathena_client.png)
 
 ### Pyathena query
 Almost one liner
```

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/config.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/config.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/databricks_utils.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/core/pyathena_utils.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/core/pyathena_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/hip_data_ml_utils/pyathena_client/client.py` & `hip_data_ml_utils-1.0.3/hip_data_ml_utils/pyathena_client/client.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-1.0.2/pyproject.toml` & `hip_data_ml_utils-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 [tool.poetry]
 name = "hip_data_ml_utils"
-version = "1.0.2"
+version = "1.0.3"
 description = "Common Python tools and utilities for Hipages ML work"
 authors = ["Hipages Data Team <datascience@hipagesgroup.com.au>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 aiobotocore = "2.4.2"
 appdirs = "1.4.4"
 attrs = "22.1.0"
 black = "^22.6.0"
-boto3 = "1.24.28"
+boto3 = "1.24.59"
 botocore = "1.27.59"
 certifi = "2022.12.7"
 cfgv = "3.2.0"
 coverage = "5.4"
 distlib = "0.3.6"
 filelock = "3.6.0"
 flake8 = "^4.0.1"
 identify = "1.5.13"
 iniconfig = "1.1.1"
 isort = "^5.10.1"
 joblib= "1.2.0"
 mccabe = "0.6.1"
+mlflow = "2.3.1"
 mock = "^4.0.3"
 moto = "^3.1.5"
 mypy-extensions = "0.4.3"
 nodeenv = "1.5.0"
-numpy = "1.21.5"
+numpy = "1.22.4"
 packaging = "^23.1"
 pandas = "1.4.4"
 pluggy = "1.0.0"
 polling = "0.3.2"
 pre-commit = "2.10.0"
 py = "1.10.0"
 pyarrow = "8.0.0"
-pyathena = "^2.13.0"
+pyathena = "^2.17.0"
 pydantic = "^1.9.0"
 pyparsing = "2.4.7"
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 pytest-custom-exit-code = "0.3.0"
 PyYAML = "6.0"
 regex = "2022.7.9"
-requests = "2.28.1"
+requests = "2.28.2"
 responses = "0.23.1"
 s3fs = "^2023.3.0"
 six = "1.15.0"
 toml = "0.10.2"
 typed-ast = "^1.5.3"
-virtualenv = "20.16.3"
 typing-extensions = "^4.2.0"
-mlflow-skinny = "^2.3.2"
-urllib3 = "1.26.11"
-pytz = "2022.1"
-charset-normalizer = "2.0.4"
-chardet = "4.0.0"
-platformdirs = "2.5.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hip_data_ml_utils-1.0.2/PKG-INFO` & `hip_data_ml_utils-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hip-data-ml-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Common Python tools and utilities for Hipages ML work
 License: MIT
 Author: Hipages Data Team
 Author-email: datascience@hipagesgroup.com.au
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,60 +12,54 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: aiobotocore (==2.4.2)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: attrs (==22.1.0)
 Requires-Dist: black (>=22.6.0,<23.0.0)
-Requires-Dist: boto3 (==1.24.28)
+Requires-Dist: boto3 (==1.24.59)
 Requires-Dist: botocore (==1.27.59)
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: cfgv (==3.2.0)
-Requires-Dist: chardet (==4.0.0)
-Requires-Dist: charset-normalizer (==2.0.4)
 Requires-Dist: coverage (==5.4)
 Requires-Dist: distlib (==0.3.6)
 Requires-Dist: filelock (==3.6.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: identify (==1.5.13)
 Requires-Dist: iniconfig (==1.1.1)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
 Requires-Dist: joblib (==1.2.0)
 Requires-Dist: mccabe (==0.6.1)
-Requires-Dist: mlflow-skinny (>=2.3.2,<3.0.0)
+Requires-Dist: mlflow (==2.3.1)
 Requires-Dist: mock (>=4.0.3,<5.0.0)
 Requires-Dist: moto (>=3.1.5,<4.0.0)
 Requires-Dist: mypy-extensions (==0.4.3)
 Requires-Dist: nodeenv (==1.5.0)
-Requires-Dist: numpy (==1.21.5)
+Requires-Dist: numpy (==1.22.4)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pandas (==1.4.4)
-Requires-Dist: platformdirs (==2.5.2)
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: polling (==0.3.2)
 Requires-Dist: pre-commit (==2.10.0)
 Requires-Dist: py (==1.10.0)
 Requires-Dist: pyarrow (==8.0.0)
-Requires-Dist: pyathena (>=2.13.0,<3.0.0)
+Requires-Dist: pyathena (>=2.17.0,<3.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: pyparsing (==2.4.7)
 Requires-Dist: pytest (>=7.1.1,<8.0.0)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
 Requires-Dist: pytest-custom-exit-code (==0.3.0)
-Requires-Dist: pytz (==2022.1)
 Requires-Dist: regex (==2022.7.9)
-Requires-Dist: requests (==2.28.1)
+Requires-Dist: requests (==2.28.2)
 Requires-Dist: responses (==0.23.1)
 Requires-Dist: s3fs (>=2023.3.0,<2024.0.0)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: toml (==0.10.2)
 Requires-Dist: typed-ast (>=1.5.3,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
-Requires-Dist: urllib3 (==1.26.11)
-Requires-Dist: virtualenv (==20.16.3)
 Description-Content-Type: text/markdown
 
 # data-ml-utils
 A utility python package that covers the common libraries we use.
 
 ## Installation
 This is an open source library hosted on pypi. Run the following command to install the library
@@ -81,14 +75,15 @@
 Almost one liner
 ```python
 import os
 from hip_data_ml_utils.pyathena_client.client import PyAthenaClient
 
 os.environ["AWS_ACCESS_KEY_ID"] = "xxx"
 os.environ["AWS_SECRET_ACCESS_KEY"] = "xxx" # pragma: allowlist secret
+os.environ["S3_BUCKET"] = "xxx"
 
 pyathena_client = PyAthenaClient()
 ```
 ![Pyathena client initialisation](docs/_static/initialise_pyathena_client.png)
 
 ### Pyathena query
 Almost one liner
```

