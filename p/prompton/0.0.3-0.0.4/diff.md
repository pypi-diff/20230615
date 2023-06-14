# Comparing `tmp/prompton-0.0.3.tar.gz` & `tmp/prompton-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.3.tar", max compression
+gzip compressed data, was "prompton-0.0.4.tar", max compression
```

## Comparing `prompton-0.0.3.tar` & `prompton-0.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.3/README.md
--rw-r--r--   0        0        0     2408 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      367 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      268 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0     9839 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    14700 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16684 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15826 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13165 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/users/client.py
--rw-r--r--   0        0        0     3055 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1274 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1458 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/db_status.py
--rw-r--r--   0        0        0      843 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0     1556 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_create_by_prompt_id.py
--rw-r--r--   0        0        0     1156 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_create_by_prompt_version_id.py
--rw-r--r--   0        0        0      926 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     2081 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1308 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1051 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0      330 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/new_inference_request.py
--rw-r--r--   0        0        0     1028 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/org_read.py
--rw-r--r--   0        0        0     1184 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      152 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1651 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/token.py
--rw-r--r--   0        0        0     1236 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      450 2023-06-13 19:02:26.478078 prompton-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.4/README.md
+-rw-r--r--   0        0        0     2408 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      367 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      268 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0     9839 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    14702 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16684 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15828 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13165 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     3055 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1274 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1458 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/db_status.py
+-rw-r--r--   0        0        0      843 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0     2205 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_create_by_prompt_id.py
+-rw-r--r--   0        0        0     1805 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_create_by_prompt_version_id.py
+-rw-r--r--   0        0        0      926 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     2730 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1229 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1051 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0      330 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/new_inference_request.py
+-rw-r--r--   0        0        0     1028 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1184 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      152 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1651 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/token.py
+-rw-r--r--   0        0        0     1236 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/user_read.py
+-rw-r--r--   0        0        0      686 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      450 2023-06-14 23:07:02.809554 prompton-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.4/PKG-INFO
```

### Comparing `prompton-0.0.3/prompton/__init__.py` & `prompton-0.0.4/prompton/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/client.py` & `prompton-0.0.4/prompton/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/core/datetime_utils.py` & `prompton-0.0.4/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/core/jsonable_encoder.py` & `prompton-0.0.4/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/resources/authentication/client.py` & `prompton-0.0.4/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/resources/inferences/client.py` & `prompton-0.0.4/prompton/resources/inferences/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/resources/orgs/client.py` & `prompton-0.0.4/prompton/resources/orgs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class OrgsClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_org_list(self) -> typing.List[OrgRead]:
+    def get_orgs_list(self) -> typing.List[OrgRead]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "orgs"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
@@ -154,15 +154,15 @@
 
 
 class AsyncOrgsClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_org_list(self) -> typing.List[OrgRead]:
+    async def get_orgs_list(self) -> typing.List[OrgRead]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "orgs"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
```

### Comparing `prompton-0.0.3/prompton/resources/prompt_versions/client.py` & `prompton-0.0.4/prompton/resources/prompt_versions/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/resources/prompts/client.py` & `prompton-0.0.4/prompton/resources/prompts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class PromptsClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_prompt_list(self) -> typing.List[PromptRead]:
+    def get_prompts_list(self) -> typing.List[PromptRead]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "prompts"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
@@ -170,15 +170,15 @@
 
 
 class AsyncPromptsClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_prompt_list(self) -> typing.List[PromptRead]:
+    async def get_prompts_list(self) -> typing.List[PromptRead]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "prompts"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
```

### Comparing `prompton-0.0.3/prompton/resources/server_status/client.py` & `prompton-0.0.4/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/resources/users/client.py` & `prompton-0.0.4/prompton/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/__init__.py` & `prompton-0.0.4/prompton/types/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/api_status_response.py` & `prompton-0.0.4/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.4/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.4/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_message.py` & `prompton-0.0.4/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_role.py` & `prompton-0.0.4/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.4/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/db_status.py` & `prompton-0.0.4/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/http_validation_error.py` & `prompton-0.0.4/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/inference_create_by_prompt_id.py` & `prompton-0.0.4/prompton/types/prompt_read.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,31 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .prompt_status import PromptStatus
 
 
-class InferenceCreateByPromptId(pydantic.BaseModel):
-    """
-    Create inference by `prompt_id`. It can only be used if there is at least one 'Live' status prompt version for the provided `prompt_id`.
-    If there are multiple prompt versions in Live status it will pick one randomly. Useful for split testing prompt versions.
-    It stores all other `prompt_version_id`s in Live status at the time of the inference in `prompt_version_ids_considered` field.
-    """
-
-    end_user_id: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    source: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    template_args: typing.Optional[typing.Dict[str, str]]
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
-    request_timeout: typing.Optional[float]
-    prompt_id: str
+class PromptRead(pydantic.BaseModel):
+    id: typing.Optional[str] = pydantic.Field(alias="_id")
+    created_at: typing.Optional[str]
+    created_by_user_id: typing.Optional[str]
+    created_by_org_id: typing.Optional[str]
+    status: typing.Optional[PromptStatus]
+    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
+    description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `prompton-0.0.3/prompton/types/inference_create_by_prompt_version_id.py` & `prompton-0.0.4/prompton/types/validation_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class InferenceCreateByPromptVersionId(pydantic.BaseModel):
-    end_user_id: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    source: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    template_args: typing.Optional[typing.Dict[str, str]]
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
-    request_timeout: typing.Optional[float]
-    prompt_version_id: str
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.3/prompton/types/inference_post_response.py` & `prompton-0.0.4/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/inference_read.py` & `prompton-0.0.4/prompton/types/prompt_version_read.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inference_read_response import InferenceReadResponse
-from .inference_request_data import InferenceRequestData
-from .inference_response_status import InferenceResponseStatus
+from .chat_gpt_chat_completition_config import ChatGptChatCompletitionConfig
+from .chat_gpt_message import ChatGptMessage
+from .prompt_version_providers import PromptVersionProviders
+from .prompt_version_status import PromptVersionStatus
 
 
-class InferenceRead(pydantic.BaseModel):
+class PromptVersionRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
-    end_user_id: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    source: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    template_args: typing.Optional[typing.Dict[str, str]]
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
-    request_timeout: typing.Optional[float]
-    prompt_version_id: str
-    prompt_version_ids_considered: typing.Optional[typing.List[str]] = pydantic.Field(
-        description=(
-            "If inference was by prompt_id then a list of all other prompt versions considered for this inference. I.e. all prompt versions in Live status at the time of the inference\n"
-        )
-    )
+    status: typing.Optional[PromptVersionStatus]
+    provider: typing.Optional[PromptVersionProviders]
+    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
+    description: typing.Optional[str]
     prompt_id: str
-    prompt_version_name: typing.Optional[str]
-    status: typing.Optional[InferenceResponseStatus]
-    request: typing.Optional[InferenceRequestData]
-    response: typing.Optional[InferenceReadResponse]
+    template: typing.Optional[typing.List[ChatGptMessage]]
+    model_config: typing.Optional[ChatGptChatCompletitionConfig]
+    template_arg_names: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.3/prompton/types/inference_request_data.py` & `prompton-0.0.4/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/inference_response_data.py` & `prompton-0.0.4/prompton/types/inference_response_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .chat_gpt_chat_completition_response import ChatGptChatCompletitionResponse
-from .chat_gpt_message import ChatGptMessage
 from .chat_gpt_token_usage import ChatGptTokenUsage
 
 
 class InferenceResponseData(pydantic.BaseModel):
     completed_at: typing.Optional[str]
     completition_duration_seconds: typing.Optional[float]
     is_client_connected_at_finish: typing.Optional[bool]
     is_error: typing.Optional[bool] = pydantic.Field(alias="isError")
-    first_message: ChatGptMessage
     token_usage: ChatGptTokenUsage
     raw_response: ChatGptChatCompletitionResponse
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `prompton-0.0.3/prompton/types/inference_response_error.py` & `prompton-0.0.4/prompton/types/inference_response_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/inference_response_status.py` & `prompton-0.0.4/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/org_read.py` & `prompton-0.0.4/prompton/types/org_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/prompt_read.py` & `prompton-0.0.4/prompton/types/user_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_status import PromptStatus
+from .user_roles import UserRoles
 
 
-class PromptRead(pydantic.BaseModel):
+class UserRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
-    status: typing.Optional[PromptStatus]
-    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    description: typing.Optional[str]
+    full_name: typing.Optional[str] = pydantic.Field(
+        description=('<span style="white-space: nowrap">`non-empty`</span>\n')
+    )
+    disabled: typing.Optional[bool]
+    role: typing.Optional[UserRoles]
+    org_id: str
+    email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.3/prompton/types/prompt_version_read.py` & `prompton-0.0.4/prompton/types/inference_create_by_prompt_version_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_gpt_chat_completition_config import ChatGptChatCompletitionConfig
-from .chat_gpt_message import ChatGptMessage
-from .prompt_version_providers import PromptVersionProviders
-from .prompt_version_status import PromptVersionStatus
-
-
-class PromptVersionRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
-    status: typing.Optional[PromptVersionStatus]
-    provider: typing.Optional[PromptVersionProviders]
-    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    description: typing.Optional[str]
-    prompt_id: str
-    template: typing.Optional[typing.List[ChatGptMessage]]
-    model_config: typing.Optional[ChatGptChatCompletitionConfig]
-    template_arg_names: typing.Optional[typing.List[str]]
+
+
+class InferenceCreateByPromptVersionId(pydantic.BaseModel):
+    end_user_id: typing.Optional[str] = pydantic.Field(
+        description=(
+            "The API consumer's internal user reference for metrics. It is also relayed to the provider as part of the request if the provider supports it (eg. OpenAI's user field).\n"
+        )
+    )
+    source: typing.Optional[str] = pydantic.Field(
+        description=("The API consumer's source for metrics (e.g. AndroidApp etc).\n")
+    )
+    client_ref_id: typing.Optional[str] = pydantic.Field(
+        description=("The API consumer's internal reference id to able to link references to their sessions.\n")
+    )
+    template_args: typing.Optional[typing.Dict[str, str]]
+    metadata: typing.Optional[typing.Dict[str, typing.Any]]
+    request_timeout: typing.Optional[float] = pydantic.Field(
+        description=(
+            "Provider request timout in seconds. If not provided, then Prompton API's default timeout for the provider will be used (90sec or `DEFAULT_OPENAI_REQUEST_TIMEOUT_SECONDS` env var if provided).\n"
+        )
+    )
+    prompt_version_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `prompton-0.0.3/prompton/types/prompt_version_status.py` & `prompton-0.0.4/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/token.py` & `prompton-0.0.4/prompton/types/token.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/prompton/types/user_roles.py` & `prompton-0.0.4/prompton/types/user_roles.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.3/PKG-INFO` & `prompton-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompton
-Version: 0.0.3
+Version: 0.0.4
 Summary: Chat prompt template evaluation and inference monitoring
 Author: PromptOn
 Author-email: hello@prompton.ai
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

