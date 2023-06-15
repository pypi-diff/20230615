# Comparing `tmp/paradigm_client-0.2.tar.gz` & `tmp/paradigm_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm_client-0.2.tar", last modified: Wed May 10 11:11:00 2023, max compression
+gzip compressed data, was "paradigm_client-0.2.1.tar", last modified: Thu Jun 15 09:09:12 2023, max compression
```

## Comparing `paradigm_client-0.2.tar` & `paradigm_client-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 11:10:41.000000 paradigm_client-0.2/.github/workflows/build-test-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-10 11:10:41.000000 paradigm_client-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 11:10:41.000000 paradigm_client-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-10 11:11:00.219883 paradigm_client-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-10 11:10:41.000000 paradigm_client-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-10 11:10:41.000000 paradigm_client-0.2/examples/create_endpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-10 11:10:41.000000 paradigm_client-0.2/examples/create_endpoint_batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-10 11:10:41.000000 paradigm_client-0.2/examples/mini_instruct_sagemaker_model_consumer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-05-10 11:10:41.000000 paradigm_client-0.2/examples/select_endpoint.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/paradigm_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:10:41.000000 paradigm_client-0.2/paradigm_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-10 11:10:41.000000 paradigm_client-0.2/paradigm_client/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-10 11:10:41.000000 paradigm_client-0.2/paradigm_client/remote_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-10 11:10:41.000000 paradigm_client-0.2/paradigm_client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-10 11:10:41.000000 paradigm_client-0.2/paradigm_client/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/paradigm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-10 11:11:00.000000 paradigm_client-0.2/paradigm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 11:11:00.000000 paradigm_client-0.2/paradigm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:11:00.000000 paradigm_client-0.2/paradigm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 11:11:00.000000 paradigm_client-0.2/paradigm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 11:11:00.000000 paradigm_client-0.2/paradigm_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 11:10:41.000000 paradigm_client-0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:11:00.219883 paradigm_client-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 11:10:41.000000 paradigm_client-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:11:00.219883 paradigm_client-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 11:10:41.000000 paradigm_client-0.2/tests/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/.github/workflows/build-test-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.871257 paradigm_client-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/create_endpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/create_endpoint_batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/mini_instruct_sagemaker_model_consumer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/examples/select_endpoint.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/paradigm_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/paradigm_client/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/paradigm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:09:12.000000 paradigm_client-0.2.1/paradigm_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:09:12.875257 paradigm_client-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-15 09:08:52.000000 paradigm_client-0.2.1/tests/example.py
```

### Comparing `paradigm_client-0.2/.github/workflows/build-test-deploy.yaml` & `paradigm_client-0.2.1/.github/workflows/build-test-deploy.yaml`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/.gitignore` & `paradigm_client-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/LICENSE` & `paradigm_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/PKG-INFO` & `paradigm_client-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm_client
-Version: 0.2
+Version: 0.2.1
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -32,29 +32,27 @@
 pip install -U git+https://github.com/lightonai/paradigm-client.git
 ```
 
 Once the package is installed, make sure to define environment variables PARADIGM_API_KEY and HOST to your API key, e.g. by adding the following lines to your .bashrc
 
 ```
 export PARADIGM_API_KEY="<your api key>"
-export HOST="<your host IP>"
 ```
 
 ## Quick Start
 
 Using paradigm-client is pretty simple, here are a code example to show you how you can use it.
 
 ```
 from paradigm_client.remote_model import RemoteModel
 import os
 
-host = os.environ.get('HOST')
-
+host = "https://llm.lighton.ai"
 model = RemoteModel(host, model_name="llm-mini")
 
 print(model.create("Hello, I am").completions[0].output_text)
 ```
 
 ## Access to LightOn Paradigm
 
-Try our Paradigm LLM at https://www.lighton.ai/fr/paradigm.
-See some Paradigm user cases at https://www.lighton.ai/fr/blog/ai-use-case-5.
+Learn more about Paradigm: https://www.lighton.ai/fr/paradigm.
+For a list of use cases: https://www.lighton.ai/fr/blog/ai-use-case-5.
```

### Comparing `paradigm_client-0.2/README.md` & `paradigm_client-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 pip install -U git+https://github.com/lightonai/paradigm-client.git
 ```
 
 Once the package is installed, make sure to define environment variables PARADIGM_API_KEY and HOST to your API key, e.g. by adding the following lines to your .bashrc
 
 ```
 export PARADIGM_API_KEY="<your api key>"
-export HOST="<your host IP>"
 ```
 
 ## Quick Start
 
 Using paradigm-client is pretty simple, here are a code example to show you how you can use it.
 
 ```
 from paradigm_client.remote_model import RemoteModel
 import os
 
-host = os.environ.get('HOST')
-
+host = "https://llm.lighton.ai"
 model = RemoteModel(host, model_name="llm-mini")
 
 print(model.create("Hello, I am").completions[0].output_text)
 ```
 
 ## Access to LightOn Paradigm
 
-Try our Paradigm LLM at https://www.lighton.ai/fr/paradigm.
-See some Paradigm user cases at https://www.lighton.ai/fr/blog/ai-use-case-5.
+Learn more about Paradigm: https://www.lighton.ai/fr/paradigm.
+For a list of use cases: https://www.lighton.ai/fr/blog/ai-use-case-5.
```

### Comparing `paradigm_client-0.2/examples/create_endpoint.ipynb` & `paradigm_client-0.2.1/examples/create_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/examples/create_endpoint_batching.ipynb` & `paradigm_client-0.2.1/examples/create_endpoint_batching.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/examples/select_endpoint.ipynb` & `paradigm_client-0.2.1/examples/select_endpoint.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/paradigm_client/communicator.py` & `paradigm_client-0.2.1/paradigm_client/communicator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod, ABC
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 import json
-from typing import Any, Generator
+from typing import Any, Generator, Optional, Union
 
 import aiohttp
 import requests
 from tqdm import tqdm
 
 from .request import Endpoint, Progress, Status
 from .response import CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse
@@ -45,23 +45,23 @@
     @abstractmethod
     def is_available(self) -> bool:
         pass
 
 
 class Communicator(AbstractCommunicator):
     def __init__(
-        self, base_address: str, headers: dict[str, str], timeout_s: int | float, raise_for_status: bool = False
+        self, base_address: str, headers: dict[str, str], timeout_s: Union[int, float], raise_for_status: bool = False
     ) -> None:
         self.base_address = base_address
         self.headers = headers
         self.timeout_s = aiohttp.ClientTimeout(total=timeout_s)
         self.model_name: str | None = None
         self.raise_for_status = raise_for_status
 
-    async def _post(self, data: Any, endpoint: Endpoint, session_id: str | None = None):
+    async def _post(self, data: Any, endpoint: Endpoint, session_id: Optional[str] = None):
         request_id = {"request_id": session_id} if session_id else {}
         async with aiohttp.ClientSession(
             base_url=self.base_address,
             headers=self.headers | request_id,
             timeout=self.timeout_s,
             raise_for_status=self.raise_for_status,
         ) as session:
@@ -97,17 +97,15 @@
             timeout=self.timeout_s.total,
             stream=True,
         )
         yield from stream.iter_content(chunk_size=1024, decode_unicode=True)
 
     def __call__(
         self, data: Any, endpoint: Endpoint, stream: bool, **kwargs
-    ) -> list[SelectResponse] | list[AnalyseResponse] | list[CreateResponse] | list[
-        TokenizeResponse
-    ] | ErrorResponse | Generator[str, None, None]:
+    ) -> Union[list[SelectResponse], list[AnalyseResponse], list[CreateResponse], list[TokenizeResponse], ErrorResponse, Generator[str, None, None]]:
 
         if self.model_name is None:
             self.model_name = self.get_model_name()
 
         show_progress = kwargs.get("show_progress", False)
         num_tasks = kwargs.get("num_tasks", 1)
 
@@ -143,27 +141,27 @@
         self.endpoint_name = endpoint_name
         assert IS_BOTO3_AVAILABLE, "boto3 is required to use the Sagemaker client"
         self._runtime_sm_client = boto3.client("sagemaker-runtime")
         self._sm_client = boto3.client("sagemaker")
 
         self.model_name: str | None = None
 
-    def _invoke_endpoint(self, endpoint: str, session_id: str | None = None, data: dict | None = None):
+    def _invoke_endpoint(self, endpoint: str, session_id: Optional[str] = None, data: Optional[dict] = None):
         request_id = {"request_id": session_id} if session_id else {}
         data = {"data": data} if data else {}
 
         response = self._runtime_sm_client.invoke_endpoint(
             EndpointName=self.endpoint_name,
             ContentType="application/json",
             Body=json.dumps({"endpoint": endpoint} | request_id | data),
         )
 
         return response["Body"].read().decode("utf8")
 
-    async def _post(self, data: Any, endpoint: Endpoint, session_id: str | None = None):
+    async def _post(self, data: Any, endpoint: Endpoint, session_id: Optional[str] = None):
         return json.loads(self._invoke_endpoint(f"llm/{endpoint.value}", session_id, data))
 
     async def _get_progress_task(self, session_id: str, num_tasks: int, endpoint: Endpoint):
         num_completed_tasks = 0
         with tqdm(total=num_tasks) as pbar:
             while True:
                 resp = self._invoke_endpoint(f"/progress/{session_id}")
@@ -186,17 +184,15 @@
         while not done:
             stream_tokens = _safe_run_tasks([self._post({}, Endpoint.stream_tokens, session_id=session_id)])[0]
             yield ''.join(stream_tokens.get('tokens'))
             done = stream_tokens.get('done')
 
     def __call__(
         self, data: Any, endpoint: Endpoint, stream: bool, **kwargs
-    ) -> list[SelectResponse] | list[AnalyseResponse] | list[CreateResponse] | list[
-        TokenizeResponse
-    ] | ErrorResponse | Generator[str, None, None]:
+    ) -> Union[list[SelectResponse], list[AnalyseResponse], list[CreateResponse], list[TokenizeResponse], ErrorResponse, Generator[str, None, None]]:
         if self.model_name is None:
             self.model_name = self.get_model_name()
 
         show_progress = kwargs.get("show_progress", False)
         num_tasks = kwargs.get("num_tasks", 1)
 
         if not stream:
```

### Comparing `paradigm_client-0.2/paradigm_client/remote_model.py` & `paradigm_client-0.2.1/paradigm_client/remote_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from typing import Any, Generator
+from typing import Any, Generator, Optional, Union
 
 from pydantic import BaseModel, validate_arguments
 
 from .request import (
     CreateRequest,
     CreateParameters,
     AnalyseRequest,
@@ -12,29 +12,29 @@
     TokenizeRequest,
     Endpoint,
 )
 from .response import CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse
 from .communicator import Communicator
 
 
-def print_logs(msg, end: str | None = None, verbose: bool = False):
+def print_logs(msg, end: Optional[str] = None, verbose: bool = False):
     if verbose:
         print(msg, end=end, flush=True)
 
 
 class RemoteModel:
     def __init__(
         self,
-        base_address: str | None = None,
-        headers: dict[str, str] | None = None,
+        base_address: Optional[str] = None,
+        headers: Optional[dict[str, str]] = None,
         timeout_s: int = 180,
         verbose: bool = False,
         comm=None,
         raise_for_status: bool = False,
-        model_name: str | None = None,
+        model_name: Optional[str] = None,
     ) -> None:
         self.verbose = verbose
         assert base_address is not None or comm is not None, "You must provide base_address or comm"
         base_headers = {"Content-Type": "application/json", "Accept": "application/json"} | {
             "X-API-KEY": os.environ.get("PARADIGM_API_KEY", str(None)),
             "X-Model": str(model_name),
         }
@@ -44,28 +44,27 @@
             timeout_s,
             raise_for_status=raise_for_status,
         )
         self._wait_for_model_server()
 
     def _post(
         self, data: Any, endpoint: Endpoint, num_tasks: int, show_progress: bool = True
-    ) -> list[SelectResponse] | list[AnalyseResponse] | list[CreateResponse] | list[TokenizeResponse] | ErrorResponse:
+    ) -> Union[list[SelectResponse], list[AnalyseResponse], list[CreateResponse], list[TokenizeResponse], ErrorResponse]:
 
         response = self.comm(data, endpoint, stream=False, **{"num_tasks": num_tasks, "show_progress": show_progress})
 
         def convert_output(response):
-            match endpoint:
-                case Endpoint.select:
-                    return SelectResponse(**response)
-                case Endpoint.analyse:
-                    return AnalyseResponse(**response)
-                case Endpoint.create:
-                    return CreateResponse(**response)
-                case Endpoint.tokenize:
-                    return TokenizeResponse(**response)
+            if endpoint == Endpoint.select:
+                return SelectResponse(**response)
+            elif endpoint == Endpoint.analyse:
+                return AnalyseResponse(**response)
+            elif endpoint == Endpoint.create:
+                return CreateResponse(**response)
+            elif endpoint == Endpoint.tokenize:
+                return TokenizeResponse(**response)
 
         if "responses" not in response:
             if "detail" in response:
                 return ErrorResponse(
                     request_id="", error_msg=response.get("detail"), status_code=response.get("status_code")
                 )
             return ErrorResponse(**response)
@@ -74,86 +73,85 @@
 
         return outputs
 
     def _post_stream(self, data: Any) -> Generator[str, None, None]:
         yield from self.comm(data, Endpoint.stream_create, stream=True)
 
     def _post_objects(
-        self, objects: BaseModel | list[BaseModel], endpoint: Endpoint, show_progress: bool = False
-    ) -> list[SelectResponse] | list[AnalyseResponse] | list[CreateResponse] | list[TokenizeResponse] | ErrorResponse:
+        self, objects: Union[BaseModel, list[BaseModel]], endpoint: Endpoint, show_progress: bool = False
+    ) -> Union[list[SelectResponse], list[AnalyseResponse], list[CreateResponse], list[TokenizeResponse], ErrorResponse]:
         def compute_num_tasks(obj) -> int:
-            match endpoint:
-                case Endpoint.create:
-                    return obj.params.n_completions
-                case Endpoint.select:
-                    return len(obj.candidates)
-                case _:
-                    return 1
+            if endpoint == Endpoint.create:
+                return obj.params.n_completions
+            elif endpoint == Endpoint.select:
+                return len(obj.candidates)
+            else:
+                return 1
 
         if isinstance(objects, list):
             num_tasks = sum([compute_num_tasks(obj) for obj in objects])
             data = [obj.dict() for obj in objects]
         else:
             num_tasks = compute_num_tasks(objects)
             data = objects.dict()
         return self._post(data, endpoint, num_tasks=num_tasks, show_progress=show_progress)
 
-    def _get_params(self, params: CreateParameters | None = None, **kwargs) -> dict[str, Any]:
+    def _get_params(self, params: Optional[CreateParameters] = None, **kwargs) -> dict[str, Any]:
         if params is None:
             params = CreateParameters()
         if kwargs:
             params = params.copy(update=kwargs)
         return params.dict()
 
     def _format_single_request_output(
         self,
-        response: list[CreateResponse]
-        | list[AnalyseResponse]
-        | list[SelectResponse]
-        | list[TokenizeResponse]
-        | ErrorResponse,
-    ) -> CreateResponse | AnalyseResponse | SelectResponse | TokenizeResponse | ErrorResponse:
+        response: Union[list[CreateResponse],
+        list[AnalyseResponse],
+        list[SelectResponse],
+        list[TokenizeResponse],
+        ErrorResponse],
+    ) -> Union[CreateResponse, AnalyseResponse, SelectResponse, TokenizeResponse, ErrorResponse]:
         return response if isinstance(response, ErrorResponse) else response[0]
 
     @validate_arguments
     def create(
-        self, prompt: str, params: CreateParameters | None = None, show_progress: bool = False, **kwargs: Any
-    ) -> CreateResponse | ErrorResponse:
+        self, prompt: str, params: Optional[CreateParameters] = None, show_progress: bool = False, **kwargs: Any
+    ) -> Union[CreateResponse, ErrorResponse]:
         params = self._get_params(params, **kwargs)
         response = self._post(
             {"text": prompt, "params": params},
             Endpoint.create,
             num_tasks=params.get("n_completions", 1),
             show_progress=show_progress,
         )
         return self._format_single_request_output(response)
 
     @validate_arguments
     def stream_create(
-        self, prompt: str, params: CreateParameters | None = None, **kwargs: Any
+        self, prompt: str, params: Optional[CreateParameters] = None, **kwargs: Any
     ) -> Generator[str, None, None]:
         params = self._get_params(params, **kwargs)
         return self._post_stream({"text": prompt, "params": params})
 
     @validate_arguments
-    def analyse(self, text: str, show_progress: bool = False) -> AnalyseResponse | ErrorResponse:
+    def analyse(self, text: str, show_progress: bool = False) -> Union[AnalyseResponse , ErrorResponse]:
         response = self._post({"text": text}, Endpoint.analyse, num_tasks=1, show_progress=show_progress)
         return self._format_single_request_output(response)
 
     @validate_arguments
     def select(
         self,
         reference: str,
         candidates: list[str],
-        conjunction: str | None = None,
+        conjunction: Optional[str] = None,
         evaluate_reference: bool = False,
         return_is_greedy_generation: bool = False,
         return_log_probs: bool = False,
         show_progress: bool = False,
-    ) -> SelectResponse | ErrorResponse:
+    ) -> Union[SelectResponse, ErrorResponse]:
         response = self._post(
             {
                 "reference": reference,
                 "candidates": candidates,
                 "conjunction": conjunction,
                 "evaluate_reference": evaluate_reference,
                 "return_is_greedy_generation": return_is_greedy_generation,
@@ -162,50 +160,50 @@
             Endpoint.select,
             num_tasks=len(candidates),
             show_progress=show_progress,
         )
         return self._format_single_request_output(response)
 
     @validate_arguments
-    def tokenize(self, text: str, show_progress: bool = False) -> TokenizeResponse | ErrorResponse:
+    def tokenize(self, text: str, show_progress: bool = False) -> Union[TokenizeResponse, ErrorResponse]:
         response = self._post({"text": text}, Endpoint.tokenize, num_tasks=1, show_progress=show_progress)
         return self._format_single_request_output(response)
 
     @validate_arguments
     def create_from_objects(
-        self, create_obj: CreateRequest | list[CreateRequest], show_progress: bool = False
-    ) -> list[CreateResponse] | ErrorResponse:
+        self, create_obj: Union[CreateRequest, list[CreateRequest]], show_progress: bool = False
+    ) -> Union[list[CreateResponse], ErrorResponse]:
         return self._post_objects(create_obj, Endpoint.create, show_progress=show_progress)
 
     @validate_arguments
     def analyse_from_objects(
-        self, analyse_obj: AnalyseRequest | list[AnalyseRequest], show_progress: bool = False
-    ) -> list[AnalyseResponse] | ErrorResponse:
+        self, analyse_obj: Union[AnalyseRequest, list[AnalyseRequest]], show_progress: bool = False
+    ) -> Union[list[AnalyseResponse], ErrorResponse]:
         return self._post_objects(analyse_obj, Endpoint.analyse, show_progress=show_progress)
 
     @validate_arguments
     def select_from_objects(
-        self, select_obj: SelectRequest | list[SelectRequest], show_progress: bool = False
-    ) -> list[SelectResponse] | ErrorResponse:
+        self, select_obj: Union[SelectRequest, list[SelectRequest]], show_progress: bool = False
+    ) -> Union[list[SelectResponse], ErrorResponse]:
         return self._post_objects(select_obj, Endpoint.select, show_progress=show_progress)
 
     @validate_arguments
     def tokenize_from_objects(
-        self, tokenize_obj: TokenizeRequest | list[TokenizeRequest], show_progress: bool = False
-    ) -> list[TokenizeResponse] | ErrorResponse:
+        self, tokenize_obj: Union[TokenizeRequest, list[TokenizeRequest]], show_progress: bool = False
+    ) -> Union[list[TokenizeResponse], ErrorResponse]:
         return self._post_objects(tokenize_obj, Endpoint.tokenize, show_progress=show_progress)
 
     def _wait_for_model_server(self):
         print_logs(f"Waiting for the ModelServer to be ready", end="", verbose=self.verbose)
         counter = 0
         while not self.comm.is_available():
             print_logs(f".", end="", verbose=self.verbose)
             time.sleep(10.0)
             counter += 1
-            if counter > 60:
+            if counter > 4:
                 break
         if self.comm.is_available():
             print_logs(" ModelServer is ready!", verbose=self.verbose)
         else:
-            print(
+            raise ConnectionError(
                 "We're sorry, but the ModelServer is currently unavailable. Please try again later. If you continue to experience issues, please contact our support team for further assistance. Thank you."
             )
```

### Comparing `paradigm_client-0.2/paradigm_client/request.py` & `paradigm_client-0.2.1/paradigm_client/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from enum import Enum
 from re import Pattern
+from typing import Optional, Union
 
 from pydantic import BaseModel, validator, Field
 
 
 MAX_SEQ_LEN = 2048
 
 
@@ -21,22 +22,22 @@
     waiting = "waiting"
     in_progress = "in_progress"
     done = "done"
 
 
 class CreateParameters(BaseModel):
     n_tokens: int = 20  # number of tokens to generate
-    temperature: float = 1.0  # temperature to apply to the logits
+    temperature: float = 0.7  # temperature to apply to the logits
     top_p: float = 0.9  # p parameter for nucleus sampling
     n_completions: int = 1  # number of generated samples per input
     generate_stop: bool = True
-    seed: int | None = None  # set the seed for the sampling phase
+    seed: Optional[int] = None  # set the seed for the sampling phase
     show_special_tokens: bool = False
     biases: dict[int, float] = Field(default_factory=dict)
-    stop_regex: Pattern | None = None
+    stop_regex: Optional[Pattern] = None
     prettify: bool = True
     return_log_probs: bool = False
     echo: bool = False
 
     class Config:
         extra: str = "forbid"
         allow_population_by_field_name: bool = True
@@ -90,15 +91,15 @@
         return d
 
 
 def is_empty_text(txt: str) -> bool:
     return not txt
 
 
-def check_text(text: str | list[str]) -> str | list[str]:
+def check_text(text: Union[str, list[str]]) -> Union[str, list[str]]:
     def validate(t: str):
         if is_empty_text(t):
             raise ValueError(f"Receive empty text. Abort")
 
     if isinstance(text, str):
         validate(text)
     else:
@@ -111,15 +112,15 @@
 class Progress:
     status: Status
     completed_task: int
 
 
 class CreateRequest(BaseModel):
     text: str
-    params: CreateParameters | None = None
+    params: Optional[CreateParameters] = None
     _validate_text = validator("text", allow_reuse=True)(check_text)
 
     @validator("params", always=True, pre=True)
     def check_params(cls, params, values) -> CreateParameters:
         if params is None:
             return CreateParameters()
         return params
@@ -156,15 +157,15 @@
     class Config:
         extra: str = "forbid"
 
 
 class SelectRequest(BaseModel):
     reference: str
     candidates: list[str]
-    conjunction: str | None = None
+    conjunction: Optional[str] = None
     evaluate_reference: bool = False
     return_is_greedy_generation: bool = False
     return_log_probs: bool = False
     _validate_reference = validator("reference", allow_reuse=True)(check_text)
 
     class Config:
         extra: str = "forbid"
```

### Comparing `paradigm_client-0.2/paradigm_client/response.py` & `paradigm_client-0.2.1/paradigm_client/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,42 +11,44 @@
     stop_regex = "stop_regex"
     stop_word = "stop_word"  # TODO: remove when server up-to-date
 
 
 class LogProbs(BaseModel):
     log_prob: float
     normalized_log_prob: float
-    token_log_probs: list[dict[str, float]] | None
+    token_log_probs: Optional[list[dict[str, float]]]
 
 
 class CreateCandidatesOutput(BaseModel):
     output_text: str
-    log_probs: LogProbs | None
+    log_probs: Optional[LogProbs]
     finish_reason: FinishReason
+    completion_id: Optional[str] = None
 
 
 class CreateResponse(BaseModel):
+    response_id: Optional[str] = None
     input_text: str
     completions: list[CreateCandidatesOutput]
 
 
 class AnalyseResponse(BaseModel):
     text: str
     log_probs: LogProbs
 
 
 class Rankings(BaseModel):
     text: str
     log_probs: LogProbs
-    is_greedy_generation: list[bool] | None = None
+    is_greedy_generation: Optional[list[bool]] = None
 
 
 class SelectResponse(BaseModel):
     reference: str
-    rankings: list[Rankings] | None
+    rankings: Optional[list[Rankings]]
     best: str
 
 
 class TokenizeResponse(BaseModel):
     text: str
     n_tokens: int
     tokens: list[dict[str, int]]
```

### Comparing `paradigm_client-0.2/paradigm_client.egg-info/PKG-INFO` & `paradigm_client-0.2.1/paradigm_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-client
-Version: 0.2
+Version: 0.2.1
 Summary: Python client for LightOn Paradigm
 Home-page: https://github.com/lightonai/paradigm-client
 Author: LightOn AI
 Author-email: support@lighton.ai
 Keywords: NLP,API,AI,LLM
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -32,29 +32,27 @@
 pip install -U git+https://github.com/lightonai/paradigm-client.git
 ```
 
 Once the package is installed, make sure to define environment variables PARADIGM_API_KEY and HOST to your API key, e.g. by adding the following lines to your .bashrc
 
 ```
 export PARADIGM_API_KEY="<your api key>"
-export HOST="<your host IP>"
 ```
 
 ## Quick Start
 
 Using paradigm-client is pretty simple, here are a code example to show you how you can use it.
 
 ```
 from paradigm_client.remote_model import RemoteModel
 import os
 
-host = os.environ.get('HOST')
-
+host = "https://llm.lighton.ai"
 model = RemoteModel(host, model_name="llm-mini")
 
 print(model.create("Hello, I am").completions[0].output_text)
 ```
 
 ## Access to LightOn Paradigm
 
-Try our Paradigm LLM at https://www.lighton.ai/fr/paradigm.
-See some Paradigm user cases at https://www.lighton.ai/fr/blog/ai-use-case-5.
+Learn more about Paradigm: https://www.lighton.ai/fr/paradigm.
+For a list of use cases: https://www.lighton.ai/fr/blog/ai-use-case-5.
```

### Comparing `paradigm_client-0.2/paradigm_client.egg-info/SOURCES.txt` & `paradigm_client-0.2.1/paradigm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradigm_client-0.2/setup.py` & `paradigm_client-0.2.1/setup.py`

 * *Files identical despite different names*

