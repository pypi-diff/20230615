# Comparing `tmp/lime_trader_sdk-0.2.0.tar.gz` & `tmp/lime_trader_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime_trader_sdk-0.2.0.tar", max compression
+gzip compressed data, was "lime_trader_sdk-0.3.0.tar", max compression
```

## Comparing `lime_trader_sdk-0.2.0.tar` & `lime_trader_sdk-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      815 2023-04-19 18:06:04.914359 lime_trader_sdk-0.2.0/README.md
--rw-r--r--   0        0        0       86 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/__init__.py
--rw-r--r--   0        0        0     7868 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/api_client.py
--rw-r--r--   0        0        0     4552 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/api/authenticated_api_client.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/__init__.py
--rw-r--r--   0        0        0     2104 2023-04-19 18:06:04.915359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_api_client.py
--rw-r--r--   0        0        0     2091 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_authenticated_api_client.py
--rw-r--r--   0        0        0     2282 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/async_client.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/__init__.py
--rw-r--r--   0        0        0     4805 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_account_client.py
--rw-r--r--   0        0        0     4470 2023-04-19 18:06:04.916359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_market_data_client.py
--rw-r--r--   0        0        0     3097 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_trading_client.py
--rw-r--r--   0        0        0     7787 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/client.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/__init__.py
--rw-r--r--   0        0        0     6775 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/account_client.py
--rw-r--r--   0        0        0     4341 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/account_feed_client.py
--rw-r--r--   0        0        0     8195 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/market_data_client.py
--rw-r--r--   0        0        0     2260 2023-04-19 18:06:04.917359 lime_trader_sdk-0.2.0/lime_trader/clients/market_data_feed_client.py
--rw-r--r--   0        0        0     5211 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/clients/trading_client.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/constants/__init__.py
--rw-r--r--   0        0        0     1707 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/constants/urls.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/__init__.py
--rw-r--r--   0        0        0      979 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/abstract_converter.py
--rw-r--r--   0        0        0     2088 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/converters/cattr_converter.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/exceptions/__init__.py
--rw-r--r--   0        0        0      446 2023-04-19 18:06:04.918359 lime_trader_sdk-0.2.0/lime_trader/exceptions/api_error.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/__init__.py
--rw-r--r--   0        0        0     5360 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/account_feed_handler.py
--rw-r--r--   0        0        0     3272 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/handlers/market_data_feed_handler.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/__init__.py
--rw-r--r--   0        0        0     8409 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/accounts.py
--rw-r--r--   0        0        0      294 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/errors.py
--rw-r--r--   0        0        0     6134 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/market.py
--rw-r--r--   0        0        0     2311 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/page.py
--rw-r--r--   0        0        0     3054 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/token_storage.py
--rw-r--r--   0        0        0     5148 2023-04-19 18:06:04.919359 lime_trader_sdk-0.2.0/lime_trader/models/trading.py
--rw-r--r--   0        0        0        0 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/__init__.py
--rw-r--r--   0        0        0     1275 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/date_utils.py
--rw-r--r--   0        0        0     1480 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/logging_utils.py
--rw-r--r--   0        0        0     1405 2023-04-19 18:06:04.920359 lime_trader_sdk-0.2.0/lime_trader/utils/pagination.py
--rw-r--r--   0        0        0      649 2023-04-19 18:06:04.921360 lime_trader_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      815 2023-06-15 18:03:08.022000 lime_trader_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0       86 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/api/__init__.py
+-rw-r--r--   0        0        0     8874 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/api/api_client.py
+-rw-r--r--   0        0        0     4552 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/api/authenticated_api_client.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/api/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/api/async_api_client.py
+-rw-r--r--   0        0        0     2091 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/api/async_authenticated_api_client.py
+-rw-r--r--   0        0        0     2420 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/async_client.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_account_client.py
+-rw-r--r--   0        0        0     4964 2023-06-15 18:03:08.023000 lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_market_data_client.py
+-rw-r--r--   0        0        0     3097 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_trading_client.py
+-rw-r--r--   0        0        0     7947 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/client.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/__init__.py
+-rw-r--r--   0        0        0     6775 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/account_client.py
+-rw-r--r--   0        0        0     4341 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/account_feed_client.py
+-rw-r--r--   0        0        0     8195 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/market_data_client.py
+-rw-r--r--   0        0        0     2260 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/market_data_feed_client.py
+-rw-r--r--   0        0        0     5211 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/clients/trading_client.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/constants/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/constants/config.py
+-rw-r--r--   0        0        0     1707 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/constants/urls.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/converters/__init__.py
+-rw-r--r--   0        0        0      979 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/converters/abstract_converter.py
+-rw-r--r--   0        0        0     2088 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/converters/cattr_converter.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/exceptions/__init__.py
+-rw-r--r--   0        0        0      446 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/exceptions/api_error.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/handlers/__init__.py
+-rw-r--r--   0        0        0     5360 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/handlers/account_feed_handler.py
+-rw-r--r--   0        0        0     3272 2023-06-15 18:03:08.024000 lime_trader_sdk-0.3.0/lime_trader/handlers/market_data_feed_handler.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/__init__.py
+-rw-r--r--   0        0        0     8409 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/accounts.py
+-rw-r--r--   0        0        0      301 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/errors.py
+-rw-r--r--   0        0        0     7798 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/market.py
+-rw-r--r--   0        0        0     2311 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/page.py
+-rw-r--r--   0        0        0     3054 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/token_storage.py
+-rw-r--r--   0        0        0     5148 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/models/trading.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/utils/__init__.py
+-rw-r--r--   0        0        0     1275 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/utils/date_utils.py
+-rw-r--r--   0        0        0     1480 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/utils/logging_utils.py
+-rw-r--r--   0        0        0     1405 2023-06-15 18:03:08.025000 lime_trader_sdk-0.3.0/lime_trader/utils/pagination.py
+-rw-r--r--   0        0        0      649 2023-06-15 18:03:08.026000 lime_trader_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.3.0/PKG-INFO
```

### Comparing `lime_trader_sdk-0.2.0/README.md` & `lime_trader_sdk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/api/api_client.py` & `lime_trader_sdk-0.3.0/lime_trader/api/api_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 
 class ApiClient:
     """
     Used for communication with the API
     """
 
     def __init__(self, base_url: Url, converter: AbstractConverter, use_https: bool, use_wss: bool,
+                 timeout: int,
                  logger: Logger):
         """
         Args:
             base_url: Base url that will be appended to all urls
             converter: Converter to use for transforming response data to Python objects
             use_https: Indicator if https protocol should be used, http is used if False
             use_wss: Indicator if wss protocol should be used, ws is used if False
+            timeout: Request timeout
             logger: Logger to use for logging messages
         """
         self._base_url = base_url
         self._converter = converter
         self._use_https = use_https
         self._use_wss = use_wss
+        self._timeout = timeout
         self._logger = logger
 
     def _map_response(self, data: dict[str, Any] | list[str, Any], t: Type[T]) -> T:
         """
         Does conversion between API response (json converted to dictionary) and Python type
 
         Args:
@@ -110,15 +113,22 @@
 
         Returns:
             Response converted to Python type passed as response_schema parameter
         """
         request_url = self._get_url(url, path_params=path_params)
         dict_params = self._converter.dump_to_dict(params, remove_none=True)
         self._logger.debug(f"Executing GET request {request_url}, params={log_json_data(dict_params)}")
-        response = httpx.get(url=request_url, params=dict_params, headers=headers)
+        try:
+            response = httpx.get(url=request_url, params=dict_params, headers=headers, timeout=self._timeout)
+        except httpx.TransportError as e:
+            raise ApiError(
+                Error(status_code=None,
+                      code="transport_error",
+                      message=f"Transport error: {e.__class__.__name__}.{''.join(e.args)}")
+            )
         return self._handle_response(response=response, response_schema=response_schema)
 
     def _get_url(self, path: Url, path_params: dict[str, Any]) -> str:
         """
         Gets full url by prefixing base url to path
 
         Args:
@@ -151,15 +161,22 @@
 
         Returns:
             Response converted to Python type passed as response_schema parameter
         """
         request_url = self._get_url(url, path_params=path_params)
         dict_data = self._converter.dump_to_dict(data, remove_none=True)
         self._logger.debug(f"Executing POST request {request_url}, data={log_json_data(dict_data)}")
-        response = httpx.post(url=request_url, data=dict_data, headers=headers)
+        try:
+            response = httpx.post(url=request_url, data=dict_data, headers=headers, timeout=self._timeout)
+        except httpx.TransportError as e:
+            raise ApiError(
+                Error(status_code=None,
+                      code="transport_error",
+                      message=f"Transport error: {e.__class__.__name__}.{''.join(e.args)}")
+            )
         result = self._handle_response(response=response, response_schema=response_schema)
         return result
 
     def _prepare_json_body(self, json: Any) -> dict[str, Any] | list[dict[str, Any]]:
         if type(json) == list:
             return [self._converter.dump_to_dict(item, remove_none=True) for item in json]
         return self._converter.dump_to_dict(json, remove_none=True)
@@ -178,15 +195,22 @@
 
         Returns:
             Response converted to Python type passed as response_schema parameter
         """
         request_url = self._get_url(url, path_params=path_params)
         dict_data = self._prepare_json_body(json)
         self._logger.debug(f"Executing POST request {request_url}, json={log_json_data(dict_data)}")
-        response = httpx.post(url=request_url, json=dict_data, headers=headers)
+        try:
+            response = httpx.post(url=request_url, json=dict_data, headers=headers, timeout=self._timeout)
+        except httpx.TransportError as e:
+            raise ApiError(
+                Error(status_code=None,
+                      code="transport_error",
+                      message=f"Transport error: {e.__class__.__name__}.{''.join(e.args)}")
+            )
         return self._handle_response(response=response, response_schema=response_schema)
 
     def websocket_connection(self, url: Url, path_params: dict[str, Any], on_message: Callable,
                              on_error: Callable,
                              headers: dict[str, str]) -> websocket.WebSocketApp:
         request_url = self._get_url(url, path_params=path_params)
         self._logger.debug(f"Opening websocket connection {request_url}")
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/api/authenticated_api_client.py` & `lime_trader_sdk-0.3.0/lime_trader/api/authenticated_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/async_trader/api/async_api_client.py` & `lime_trader_sdk-0.3.0/lime_trader/async_trader/api/async_authenticated_api_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from typing import TypeVar, Type, Any
-import httpx
+from typing import TypeVar, Type, Callable, Any
+
 from urllib3.util import Url
+from websocket import WebSocketApp
 
-from lime_trader.api.api_client import ApiClient
-from lime_trader.utils.logging_utils import log_json_data
+from lime_trader.api.authenticated_api_client import AuthenticatedApiClient
 
 T = TypeVar("T")
 
 
-class AsyncApiClient(ApiClient):
+class AsyncAuthenticatedApiClient(AuthenticatedApiClient):
+
+    async def _get_authorization_header(self) -> dict[str, str]:
+        return self._get_authorization_header_for_token(await self._token_storage.get_token())
 
-    async def get(self, url: Url, path_params: dict[str, Any], params: Any, headers: dict[str, str],
-                  response_schema: Type[T]) -> T:
-        request_url = self._get_url(url, path_params=path_params)
-        dict_params = self._converter.dump_to_dict(params, remove_none=True)
-        self._logger.debug(f"Executing GET request {request_url}, params={log_json_data(dict_params)}")
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url=request_url, params=dict_params, headers=headers)
-        return self._handle_response(response=response, response_schema=response_schema)
-
-    async def post_form(self, url: Url, path_params: dict[str, Any], data: Any, headers: dict[str, str],
-                        response_schema: Type[T]) -> T:
-        request_url = self._get_url(url, path_params=path_params)
-        dict_data = self._converter.dump_to_dict(data, remove_none=True)
-        self._logger.debug(f"Executing POST request {request_url}, data={log_json_data(dict_data)}")
-        async with httpx.AsyncClient() as client:
-            response = await client.post(url=request_url, data=dict_data, headers=headers)
-        return self._handle_response(response=response, response_schema=response_schema)
-
-    async def post(self, url: Url, path_params: dict[str, Any], json: Any, headers: dict[str, str],
-                   response_schema: Type[T]) -> T:
-        request_url = self._get_url(url, path_params=path_params)
-        dict_data = self._prepare_json_body(json)
-        self._logger.debug(f"Executing POST request {request_url}, json={log_json_data(dict_data)}")
-        async with httpx.AsyncClient() as client:
-            response = await client.post(url=request_url, json=dict_data, headers=headers)
-        return self._handle_response(response=response, response_schema=response_schema)
+    async def get(self, url: Url, path_params: dict[str, Any], params: Any, response_schema: Type[T]) -> T:
+        return await self._api_client.get(url=url, path_params=path_params, params=params,
+                                          headers=await self._get_authorization_header(),
+                                          response_schema=response_schema)
+
+    async def post_form(self, url: Url, path_params: dict[str, Any], data: Any, response_schema: Type[T]) -> T:
+        return await self._api_client.post_form(url=url, path_params=path_params, data=data,
+                                                headers=await self._get_authorization_header(),
+                                                response_schema=response_schema)
+
+    async def post(self, url: Url, path_params: dict[str, Any], json: Any, response_schema: Type[T]) -> T:
+        return await self._api_client.post(url=url, path_params=path_params, json=json,
+                                           headers=await self._get_authorization_header(),
+                                           response_schema=response_schema)
+
+    async def websocket_connection(self, url: Url, path_params: dict[str, Any], on_message: Callable,
+                                   on_error: Callable,
+                                   ) -> WebSocketApp:
+        return self._api_client.websocket_connection(url=url, path_params=path_params,
+                                                     on_message=on_message, on_error=on_error,
+                                                     headers=await self._get_authorization_header(),
+                                                     )
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/async_trader/async_client.py` & `lime_trader_sdk-0.3.0/lime_trader/async_trader/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import logging
 
 from lime_trader.async_trader.clients.async_account_client import AsyncAccountClient
 from lime_trader.async_trader.clients.async_market_data_client import AsyncMarketDataClient
 from lime_trader.async_trader.clients.async_trading_client import AsyncTradingClient
+from lime_trader.constants.config import DEFAULT_TIMEOUT
 from lime_trader.converters.cattr_converter import CAttrConverter
 
 from lime_trader import LimeClient
 from lime_trader.async_trader.api.async_api_client import AsyncApiClient
 from lime_trader.async_trader.api.async_authenticated_api_client import AsyncAuthenticatedApiClient
 from lime_trader.models.accounts import Credentials
 from lime_trader.models.token_storage import AsyncApiTokenStorage
 
 
 class AsyncLimeClient(LimeClient):
-    def __init__(self, base_url: str, credentials: Credentials, logger: logging.Logger, auth_url: str = None, ):
+    def __init__(self, base_url: str, credentials: Credentials, logger: logging.Logger, auth_url: str = None,
+                 timeout: int = DEFAULT_TIMEOUT):
         super().__init__(base_url=base_url, credentials=credentials, logger=logger, auth_url=auth_url)
         self._converter = CAttrConverter()
         self._api_client = AsyncApiClient(base_url=self._base_url, converter=self._converter,
                                           use_https=self._api_use_https,
-                                          use_wss=self._api_use_wss, logger=self._logger)
+                                          use_wss=self._api_use_wss, logger=self._logger, timeout=timeout)
         self._auth_api_client = AsyncApiClient(base_url=self._auth_url, converter=self._converter,
                                                use_https=self._auth_use_https,
-                                               use_wss=self._auth_use_wss, logger=self._logger)
+                                               use_wss=self._auth_use_wss, logger=self._logger, timeout=timeout)
         self._token_storage = AsyncApiTokenStorage(credentials=credentials, api_client=self._auth_api_client)
         self._authenticated_api_client = AsyncAuthenticatedApiClient(api_client=self._api_client,
                                                                      token_storage=self._token_storage,
                                                                      credentials=self._credentials, logger=self._logger)
 
         # instantiate clients
         self.account = AsyncAccountClient(api_client=self._authenticated_api_client, logger=self._logger)
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_account_client.py` & `lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_market_data_client.py` & `lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_market_data_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import datetime
+from functools import partial
 from logging import Logger
 from typing import Callable
 
 from lime_trader.async_trader.api.async_authenticated_api_client import AsyncAuthenticatedApiClient
 from lime_trader.clients.market_data_client import MarketDataClient
 from lime_trader.clients.market_data_feed_client import MarketDataFeedClient
+from lime_trader.converters.cattr_converter import CAttrConverter
+from lime_trader.handlers.market_data_feed_handler import MarketDataFeedHandler
 from lime_trader.models.market import (Quote, QuoteHistory, Period, Security, SecuritiesPage, Trade, TradesPage,
                                        CurrentSchedule)
 from lime_trader.models.page import Page, PageRequest
 from lime_trader.constants.urls import (MARKET_DATA_GET_CURRENT_QUOTE, MARKET_DATA_GET_QUOTES,
                                         MARKET_DATA_GET_TRADING_SCHEDULE,
                                         MARKET_DATA_LOOKUP_SECURITIES, MARKET_DATA_GET_TIME_AND_SALES,
                                         MARKET_DATA_GET_QUOTES_HISTORY, MARKET_DATA_STREAMING_FEED)
@@ -54,16 +57,21 @@
         response = await self._api_client.get(MARKET_DATA_GET_TIME_AND_SALES, path_params={},
                                               params={"symbol": symbol,
                                                       "limit": page.size,
                                                       "skip": page.get_offset()},
                                               response_schema=TradesPage)
         return Page(data=response.trades, number=page.page, size=page.size, total_elements=response.count)
 
-    async def start_streaming_feed(self, on_message: Callable, on_error: Callable) -> MarketDataFeedClient:
+    async def _start_streaming_feed(self, on_message: Callable, on_error: Callable) -> MarketDataFeedClient:
         websocket_app = await self._api_client.websocket_connection(url=MARKET_DATA_STREAMING_FEED,
                                                                     path_params={}, on_error=on_error,
                                                                     on_message=on_message)
         client = MarketDataFeedClient(websocket_app=websocket_app, logger=self._logger)
         websocket_app.on_open = client.on_market_feed_streaming_feed_open
         websocket_app.on_close = client.on_market_feed_streaming_feed_close
         client.start()
         return client
+
+    async def stream_market_data_feed(self, callback_client: MarketDataFeedHandler) -> MarketDataFeedClient:
+        return await self._start_streaming_feed(
+            on_error=callback_client.on_market_data_feed_client_internal_error,
+            on_message=partial(callback_client.on_message, CAttrConverter()))
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/async_trader/clients/async_trading_client.py` & `lime_trader_sdk-0.3.0/lime_trader/async_trader/clients/async_trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/client.py` & `lime_trader_sdk-0.3.0/lime_trader/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 
 import urllib3.util
 from dotenv import dotenv_values
 
 from lime_trader.clients.account_client import AccountClient
+from lime_trader.constants.config import DEFAULT_TIMEOUT
 from lime_trader.converters.cattr_converter import CAttrConverter
 from lime_trader.models.accounts import Credentials
 from lime_trader.api.api_client import ApiClient
 from lime_trader.api.authenticated_api_client import AuthenticatedApiClient
 from lime_trader.clients.market_data_client import MarketDataClient
 from lime_trader.clients.trading_client import TradingClient
 from lime_trader.models.token_storage import ApiTokenStorage
@@ -23,37 +24,38 @@
     Attributes:
         account: Account client
         market: Market client
         trading: Trading client
     """
 
     def __init__(self, base_url: str, credentials: Credentials, logger: logging.Logger | None = None,
-                 auth_url: str | None = None):
+                 auth_url: str | None = None, timeout: int = DEFAULT_TIMEOUT):
         """
         Args:
             base_url: Base url of the API, this will be prepended to each url
             credentials: Credentials object used for authenticating in the API
             logger: Logger to be used
             auth_url: URL of the authorization server. Only requests related to authentication/authorization
                      will use this url
+            timeout: Request timeout
         """
         self._base_url = urllib3.util.parse_url(base_url)
         self._auth_url = urllib3.util.parse_url(auth_url) if auth_url is not None else self._base_url
         self._api_use_https = self._base_url.url.startswith("https://")
         self._api_use_wss = self._api_use_https
         self._auth_use_https = self._auth_url.url.startswith("https://")
         self._auth_use_wss = self._auth_use_https
         self._credentials = credentials
         self._logger = logger or get_stdout_logger()
         self._converter = CAttrConverter()
         self._api_client = ApiClient(base_url=self._base_url, converter=self._converter, use_https=self._api_use_https,
-                                     use_wss=self._api_use_wss, logger=self._logger)
+                                     use_wss=self._api_use_wss, logger=self._logger, timeout=timeout)
         self._auth_api_client = ApiClient(base_url=self._auth_url, converter=self._converter,
                                           use_https=self._auth_use_https,
-                                          use_wss=self._auth_use_wss, logger=self._logger)
+                                          use_wss=self._auth_use_wss, logger=self._logger, timeout=timeout)
         self._token_storage = ApiTokenStorage(credentials=credentials, api_client=self._auth_api_client)
         self._authenticated_api_client = AuthenticatedApiClient(api_client=self._api_client,
                                                                 token_storage=self._token_storage,
                                                                 credentials=self._credentials, logger=self._logger)
 
         # instantiate clients
         self.account = AccountClient(api_client=self._authenticated_api_client, logger=self._logger)
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/clients/account_client.py` & `lime_trader_sdk-0.3.0/lime_trader/clients/account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/clients/account_feed_client.py` & `lime_trader_sdk-0.3.0/lime_trader/clients/account_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/clients/market_data_client.py` & `lime_trader_sdk-0.3.0/lime_trader/clients/market_data_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/clients/market_data_feed_client.py` & `lime_trader_sdk-0.3.0/lime_trader/clients/market_data_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/clients/trading_client.py` & `lime_trader_sdk-0.3.0/lime_trader/clients/trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/constants/urls.py` & `lime_trader_sdk-0.3.0/lime_trader/constants/urls.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/converters/abstract_converter.py` & `lime_trader_sdk-0.3.0/lime_trader/converters/abstract_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/converters/cattr_converter.py` & `lime_trader_sdk-0.3.0/lime_trader/converters/cattr_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/handlers/account_feed_handler.py` & `lime_trader_sdk-0.3.0/lime_trader/handlers/account_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/handlers/market_data_feed_handler.py` & `lime_trader_sdk-0.3.0/lime_trader/handlers/market_data_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/models/accounts.py` & `lime_trader_sdk-0.3.0/lime_trader/models/accounts.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/models/market.py` & `lime_trader_sdk-0.3.0/lime_trader/models/market.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,32 +38,67 @@
     TRADE = "t"
     AGGREGATE = "a"
     ERROR = "e"
 
 
 @dataclass
 class Quote:
+    """
+    Quote for the specified symbol.
+
+    Attributes:
+        symbol: The security symbol
+        ask: Ask price
+        ask_size: Ask size
+        bid: Bid price
+        bid_size: Bid size
+        last: Last price
+        last_size: Last trade size
+        volume: Today total volume
+        date: Last trade time
+        high: Today's high price
+        low: Today's low price
+        open: Open price
+        close: Yesterday's close price
+        week52_high: 52-week high
+        week52_low: 52-week low
+        change: Today's price change
+        change_pc: Today's percent price change
+        open_interest: Open interest (options)
+        implied_volatility: Implied volatility (options)
+        theoretical_price: Theoretical price (options)
+        delta: Delta value (options)
+        gamma: Gamma value (options)
+        theta: Theta value (options)
+        vega: Vega value (options)
+    """
     symbol: str
     ask: Decimal
     ask_size: Decimal
     bid: Decimal
     bid_size: Decimal
     last: Decimal
     last_size: Decimal
     volume: int
-    date: int
+    date: datetime.datetime
     high: Decimal
     low: Decimal
     open: Decimal
     close: Decimal
     week52_high: Decimal
     week52_low: Decimal
     change: Decimal
     change_pc: Decimal
     open_interest: Decimal
+    implied_volatility: Decimal
+    theoretical_price: Decimal
+    delta: Decimal
+    gamma: Decimal
+    theta: Decimal
+    vega: Decimal
 
 
 @dataclass
 class QuoteHistory:
     timestamp: datetime.datetime
     period: Period
     open: Decimal
@@ -216,14 +251,20 @@
         v: Volume
         chpc: Change percent
         ls: Last Size, trade quantity
         o: Open price
         h: High
         low: Low price
         d: Date
+        iv: Implied volatility (options)
+        tp: Theoretical price (options)
+        delta: Delta value (options)
+        theta: Theta value (options)
+        gamma: Gamma value (options)
+        vega: Vega value (options)
     """
 
     t: MarketDataFeedType
     s: str
 
     ch: Decimal | None = None
 
@@ -237,14 +278,21 @@
     chpc: Decimal | None = None
     ls: int | None = None
     o: Decimal | None = None
     h: Decimal | None = None
     low: Decimal | None = None
     d: datetime.datetime | None = None
 
+    iv: Decimal | None = None
+    tp: Decimal | None = None
+    delta: Decimal | None = None
+    theta: Decimal | None = None
+    gamma: Decimal | None = None
+    vega: Decimal | None = None
+
     @property
     def type(self) -> MarketDataFeedType:
         return self.t
 
     @property
     def symbol(self) -> str:
         return self.s
@@ -297,14 +345,22 @@
     def change(self) -> Decimal | None:
         return self.ch
 
     @property
     def change_percent(self) -> Decimal | None:
         return self.chpc
 
+    @property
+    def implied_volatility(self) -> Decimal | None:
+        return self.iv
+
+    @property
+    def theoretical_price(self) -> Decimal | None:
+        return self.tp
+
 
 @dataclass
 class MarketDataFeedError:
     """Error during streaming market feed data
 
     Attributes:
         t: Type. Always equal to "e"
```

### Comparing `lime_trader_sdk-0.2.0/lime_trader/models/page.py` & `lime_trader_sdk-0.3.0/lime_trader/models/page.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/models/token_storage.py` & `lime_trader_sdk-0.3.0/lime_trader/models/token_storage.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/models/trading.py` & `lime_trader_sdk-0.3.0/lime_trader/models/trading.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/utils/date_utils.py` & `lime_trader_sdk-0.3.0/lime_trader/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/utils/logging_utils.py` & `lime_trader_sdk-0.3.0/lime_trader/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/lime_trader/utils/pagination.py` & `lime_trader_sdk-0.3.0/lime_trader/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.2.0/PKG-INFO` & `lime_trader_sdk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: lime-trader-sdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python wrapper for Lime Trader REST API (https://docs.lime.co/trader/)
 Author: Lime Financial
 Author-email: support@lime.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: orjson (>=3.8.10,<4.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: orjson (>=3.8.12,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rel (>=0.4.8,<0.5.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Lime-Trader-SDK
 
 Quick example:
```

