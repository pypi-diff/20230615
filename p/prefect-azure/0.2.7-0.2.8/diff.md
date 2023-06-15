# Comparing `tmp/prefect-azure-0.2.7.tar.gz` & `tmp/prefect-azure-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-xafqlomh/prefect-azure-0.2.7.tar", last modified: Tue Apr 25 20:23:42 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-bwbm0f6n/prefect-azure-0.2.8.tar", last modified: Thu Jun 15 14:49:58 2023, max compression
```

## Comparing `prefect-azure-0.2.7.tar` & `prefect-azure-0.2.8.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/ml_datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37699 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 20:23:42.000000 prefect-azure-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    37898 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-25 20:21:59.000000 prefect-azure-0.2.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32951 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/ml_datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37898 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/versioneer.py
```

### Comparing `prefect-azure-0.2.7/LICENSE` & `prefect-azure-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/PKG-INFO` & `prefect-azure-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.7
-Summary: Prefect tasks and subflows for interacting with Azure
+Version: 0.2.8
+Summary: Prefect integrations with Microsoft Azure services
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect-azure-0.2.7/README.md` & `prefect-azure-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/prefect_azure/__init__.py` & `prefect-azure-0.2.8/prefect_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/prefect_azure/blob_storage.py` & `prefect-azure-0.2.8/prefect_azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/prefect_azure/container_instance.py` & `prefect-azure-0.2.8/prefect_azure/container_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
             identity="/my/managed/identity/123abc"
         )
     )
     ```
 """
 import datetime
 import json
+import random
+import string
 import sys
 import time
 import uuid
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 import anyio
@@ -94,14 +96,15 @@
     UserAssignedIdentities,
 )
 from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.infrastructure.base import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from pydantic import BaseModel, Field, SecretStr
+from slugify import slugify
 from typing_extensions import Literal
 
 from prefect_azure.credentials import AzureContainerInstanceCredentials
 
 ACI_DEFAULT_CPU = 1.0
 ACI_DEFAULT_MEMORY = 1.0
 ACI_DEFAULT_GPU = 0.0
@@ -466,15 +469,27 @@
             EnvironmentVariable(name=k, secure_value=v)
             if k in ENV_SECRETS
             else EnvironmentVariable(name=k, value=v)
             for (k, v) in self._get_environment().items()
         ]
 
         # all container names in a resource group must be unique
-        container_name = str(uuid.uuid4())
+        if self.name:
+            slugified_name = slugify(
+                self.name,
+                max_length=52,
+                regex_pattern=r"[^a-zA-Z0-9-]+",
+            )
+            random_suffix = "".join(
+                random.choices(string.ascii_lowercase + string.digits, k=10)
+            )
+            container_name = slugified_name + "-" + random_suffix
+        else:
+            container_name = str(uuid.uuid4())
+
         container_resource_requirements = self._configure_container_resources()
 
         # add the entrypoint if provided, because creating an ACI container with a
         # command overrides the container's built-in entrypoint.
         if self.entrypoint:
             self.command.insert(0, self.entrypoint)
```

### Comparing `prefect-azure-0.2.7/prefect_azure/cosmos_db.py` & `prefect-azure-0.2.8/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/prefect_azure/credentials.py` & `prefect-azure-0.2.8/prefect_azure/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Credential classes used to perform authenticated interactions with Azure"""
 
 import functools
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
-from azure.identity import ClientSecretCredential, DefaultAzureCredential
+from azure.identity.aio import ClientSecretCredential, DefaultAzureCredential
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
 from azure.mgmt.resource import ResourceManagementClient
 from pydantic import Field, SecretStr, root_validator
 
 try:
     from azure.cosmos import CosmosClient
 
@@ -68,45 +68,52 @@
         return inner
 
     return outer
 
 
 class AzureBlobStorageCredentials(Block):
     """
-    Block used to manage Blob Storage authentication with Azure.
-    Azure authentication is handled via the `azure` module through
-    a connection string.
+    Stores credentials for authenticating with Azure Blob Storage.
 
     Args:
-        connection_string: Includes the authorization information required.
+        account_url: The URL for your Azure storage account. If provided, the account
+            URL will be used to authenticate with the discovered default Azure
+            credentials.
+        connection_string: The connection string to your Azure storage account. If
+            provided, the connection string will take precedence over the account URL.
 
     Example:
-        Load stored Azure Blob Storage credentials:
+        Load stored Azure Blob Storage credentials and retrieve a blob service client:
         ```python
         from prefect_azure import AzureBlobStorageCredentials
+
         azure_credentials_block = AzureBlobStorageCredentials.load("BLOCK_NAME")
+
+        blob_service_client = azure_credentials_block.get_blob_client()
         ```
     """
 
     _block_type_name = "Azure Blob Storage Credentials"
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/6AiQ6HRIft8TspZH7AfyZg/39fd82bdbb186db85560f688746c8cdd/azure.png?h=250"  # noqa
     _documentation_url = "https://prefecthq.github.io/prefect-azure/credentials/#prefect_azure.credentials.AzureBlobStorageCredentials"  # noqa
 
     connection_string: Optional[SecretStr] = Field(
         default=None,
         description=(
-            "If account_url is not provided, " "the connection string to authenticate."
+            "The connection string to your Azure storage account. If provided, the "
+            "connection string will take precedence over the account URL."
         ),
     )
     account_url: Optional[str] = Field(
         default=None,
+        title="Account URL",
         description=(
-            "If a connection string is not provided, "
-            "the URL to the Blob Storage account; will use "
-            "DefaultAzureCredential to authenticate."
+            "The URL for your Azure storage account. If provided, the account "
+            "URL will be used to authenticate with the discovered default "
+            "Azure credentials."
         ),
     )
 
     @root_validator
     def check_connection_string_or_account_url(
         cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
```

### Comparing `prefect-azure-0.2.7/prefect_azure/ml_datastore.py` & `prefect-azure-0.2.8/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/prefect_azure/workers/container_instance.py` & `prefect-azure-0.2.8/prefect_azure/workers/container_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,14 +511,29 @@
     """
     A Prefect worker that runs flows in an Azure Container Instance.
     """
 
     type = "azure-container-instance"
     job_configuration = AzureContainerJobConfiguration
     job_configuration_variables = AzureContainerVariables
+    _is_beta = True
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/6AiQ6HRIft8TspZH7AfyZg/39fd82bdbb186db85560f688746c8cdd/azure.png?h=250"  # noqa
+    _display_name = "Azure Container Instances"
+    _description = (
+        "Execute flow runs within containers on Azure's Container Instances "
+        "service. Requires an Azure account."
+    )
+    _documentation_url = (
+        "https://prefecthq.github.io/prefect-azure/container_instance_worker/"
+    )
+
+    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/6AiQ6HRIft8TspZH7AfyZg/39fd82bdbb186db85560f688746c8cdd/azure.png?h=250"  # noqa
+    _documentation_url = (
+        "https://prefecthq.github.io/prefect-azure/container_instance_worker/"
+    )
 
     async def run(
         self,
         flow_run: FlowRun,
         configuration: AzureContainerJobConfiguration,
         task_status: Optional[anyio.abc.TaskStatus] = None,
     ):
```

### Comparing `prefect-azure-0.2.7/prefect_azure.egg-info/PKG-INFO` & `prefect-azure-0.2.8/prefect_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.7
-Summary: Prefect tasks and subflows for interacting with Azure
+Version: 0.2.8
+Summary: Prefect integrations with Microsoft Azure services
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect-azure-0.2.7/prefect_azure.egg-info/SOURCES.txt` & `prefect-azure-0.2.8/prefect_azure.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 prefect_azure/ml_datastore.py
 prefect_azure.egg-info/PKG-INFO
 prefect_azure.egg-info/SOURCES.txt
 prefect_azure.egg-info/dependency_links.txt
 prefect_azure.egg-info/entry_points.txt
 prefect_azure.egg-info/requires.txt
 prefect_azure.egg-info/top_level.txt
+prefect_azure/deployments/__init__.py
+prefect_azure/deployments/steps.py
 prefect_azure/workers/__init__.py
 prefect_azure/workers/container_instance.py
 tests/test_aci_infrastructure.py
 tests/test_aci_worker.py
 tests/test_blob_storage.py
 tests/test_block_standards.py
 tests/test_cosmos_db.py
```

### Comparing `prefect-azure-0.2.7/setup.cfg` & `prefect-azure-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/setup.py` & `prefect-azure-0.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 extras_require["all_extras"] = sorted(
     {lib for key in extras_require.values() for lib in key if key != "dev"}
 )
 extras_require["dev"] = dev_requires + extras_require["all_extras"]
 
 setup(
     name="prefect-azure",
-    description="Prefect tasks and subflows for interacting with Azure",
+    description="Prefect integrations with Microsoft Azure services",
     license="Apache License 2.0",
     author="Prefect Technologies, Inc.",
     author_email="help@prefect.io",
     keywords="prefect",
     url="https://github.com/PrefectHQ/prefect-azure",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `prefect-azure-0.2.7/tests/test_aci_infrastructure.py` & `prefect-azure-0.2.8/tests/test_aci_infrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict, List, Tuple, Union
 from unittest.mock import MagicMock, Mock
 
 import dateutil.parser
 import pytest
 from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
-from azure.identity import ClientSecretCredential, DefaultAzureCredential
+from azure.identity.aio import ClientSecretCredential, DefaultAzureCredential
 from azure.mgmt.containerinstance.models import (
     EnvironmentVariable,
     ImageRegistryCredential,
     UserAssignedIdentities,
 )
 from azure.mgmt.resource import ResourceManagementClient
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
```

### Comparing `prefect-azure-0.2.7/tests/test_aci_worker.py` & `prefect-azure-0.2.8/tests/test_aci_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/tests/test_blob_storage.py` & `prefect-azure-0.2.8/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/tests/test_block_standards.py` & `prefect-azure-0.2.8/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/tests/test_cosmos_db.py` & `prefect-azure-0.2.8/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/tests/test_credentials.py` & `prefect-azure-0.2.8/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/tests/test_ml_datastore.py` & `prefect-azure-0.2.8/tests/test_ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.7/versioneer.py` & `prefect-azure-0.2.8/versioneer.py`

 * *Files identical despite different names*

